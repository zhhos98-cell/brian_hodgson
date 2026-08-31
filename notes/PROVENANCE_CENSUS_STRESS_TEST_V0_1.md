# Provenance census stress test v0.1

Date: 2026-08-31

Purpose: manually encode five structurally different Hodgson cases before committing the project to CSV/JSON/SQLite. This is not yet the database. It tests whether the schema can represent the archive without collapsing object chronology, container chronology, identifier history, and institutional handling.

## Result at a glance

The current schema survives all five cases, but the test exposes four additions that should be retained in implementation:

1. one `shipment` may contain multiple nested containers and heterogeneous object classes;
2. `receipt` must be separated from `inventory reconciliation`;
3. identifiers need their own history because a wrapper title, drawing number, catalogue number, or foliation can be correct at one level and wrong at another;
4. relations themselves require temporal states (`attached`, `separated`, `reunited`, `superseded`) rather than being treated as timeless edges.

---

# Case 1 — 1837 Société Asiatique manuscript shipment

## Source state

RAS correspondence records:

- 15 July 1837, Eugène Burnouf acknowledges the **safe arrival of three cases of manuscripts** at the Société Asiatique;
- 29 July 1837, Jules Mohl separately reports the arrival of the **three crates**;
- later Burnouf correspondence asks Hodgson to use a safer address for further manuscript transmission.

Public-web evidence is summarised in Waves 9–10.

## Provisional entities

### Shipment event

`HOD-EVT-TEMP-1837-SA-DISPATCH`

- `event_type`: dispatch
- `object_class`: multiple manuscript copies
- `container_count`: 3
- `container_type`: case/crate
- `destination`: Société Asiatique, Paris
- `claim_status`: direct for arrival; dispatch details still incomplete

### Receipt event 1

`HOD-EVT-TEMP-1837-07-15-SA-RECEIPT`

- `event_type`: safe_arrival_acknowledged
- `agent_to`: Eugène Burnouf / Société Asiatique
- `receipt_container_count_reported`: 3
- `granularity_verified`: containers only

### Receipt event 2

`HOD-EVT-TEMP-1837-07-29-SA-RECEIPT2`

- `event_type`: receive / redundant acknowledgement
- `agent_to`: Jules Mohl
- `receipt_container_count_reported`: 3

## What this tests

The same custody transition has two documentary acknowledgements. The schema therefore needs multiple source/events without treating them as duplicate noise.

`safe arrival` verifies **three transport units**, not every manuscript inside. Item-level reconciliation remains unknown.

## Schema verdict

Pass.

Need field in implementation:

- `verification_granularity`: container / item / list / condition / identifier / complete_inventory.

---

# Case 2 — 1844–47 British Museum zoological reconciliation loop

## Source state

This case is reconstructed in Wave 11 from ZSL correspondence.

Key events:

1. British Museum agrees to receive specimens/drawings and distribute duplicates with specimen lists.
2. Gray sorts received materials.
3. Inventory exceptions appear:
   - Tibetan pheasant omitted from list because at the stuffer;
   - Ganges Pelican represented only by a head;
   - some specimens too defective for useful distribution;
   - fifty drawings found at ZSL;
   - other drawings remain dispersed or detained.
4. Gray reports copied names wrong although numbers were correct in one list, and fears number collisions where two differing kinds share one number.
5. Whole collection must be sorted before new/old species can be compared.
6. corrected catalogue produced and distributed with duplicate sets.
7. 1847 Hodgson receives twelve catalogue copies and promises `fresh and superior samples` for specimens/drawings still defective or missing.
8. later Hodgson marks catalogue disagreements and calls attention to Gray's deviations in allocation of new types.

## Provisional event chain

`HOD-EVT-TEMP-1844-BM-RECEIVE`
→ `HOD-EVT-TEMP-1845-BM-UNPACK-SORT`
→ `HOD-EVT-TEMP-1845-BM-RECONCILE`
→ multiple exception events
→ identifier/name correction events
→ duplicate partition events
→ catalogue compilation/printing
→ catalogue distribution with duplicate sets
→ remote receipt by Hodgson
→ replacement/supplementation promise
→ later catalogue annotation/version disagreement.

## Example exception entities

### Tibetan pheasant

- expected in list: yes
- physical state: temporarily at stuffer
- list state: omitted
- event: `exception_detected`
- mechanism: object temporarily outside list-making workspace

### Ganges Pelican

- expected entity: full specimen(s)
- received state: head only
- failure tag: `partial_object_only`
- catalogue implication: full taxonomic witness unavailable in expected material form

### duplicate number collision

- identifier type: specimen/drawing number
- status: collision
- evidence: Gray fears two very different kinds share same number
- repair status: unresolved in the cited letter

## What this tests

This case requires the database to represent **recursion**. A catalogue is simultaneously:

- output of reconciliation;
- metadata distributed with physical duplicate sets;
- diagnostic device defining what remains missing/defective;
- input to later replacement collecting;
- versioned object subject to taxonomic disagreement.

A simple linear provenance table would fail here.

## Schema verdict

Pass, but implementation should allow `event_parent_id` or `workflow_id` so related repair events can be queried as one audit loop.

Add:

- `workflow_id`
- `event_parent_id`
- `exception_status`: open / repaired / partially_repaired / unresolved.

---

# Case 3 — 1858 Institut de France waterproof shipment and later container-chronology error

## Source state

Wave 9–10 reconstructs:

- Hodgson's boxes initially in a clearing agent's hands;
- Mitchell consults Jules Mohl;
- a roll is placed into a purpose-built waterproof box;
- waterproof box plus another box entrusted to Molini, bookseller/Institut agent;
- British Embassy route rejected after prior non-arrival/delay;
- later two parcels acknowledged at the Académie;
- the knowledge package included paintings/drawings, explanatory Sanskrit texts, Hodgson notes;
- later collection state separated paintings/drawings from some explanatory manuscripts into different cases;
- Foucher apparently read a note found in a case as indicating shipment in 1866;
- Saint-Hilaire had already discussed the collection in 1863, so the inferred 1866 acquisition chronology cannot stand.

## Provisional container nesting

`HOD-CNT-TEMP-1858-ROLL`
→ contained in `HOD-CNT-TEMP-1858-WATERPROOF-BOX`

plus

`HOD-CNT-TEMP-1858-OTHER-BOX`

both participate in one routing workflow.

## Event chain

clearing-agent custody
→ route redesign
→ waterproofing/repacking
→ Molini custody
→ dispatch/forward
→ two-parcel receipt
→ institutional storage/rearrangement
→ later separation of explanatory material
→ later case-note interpretation
→ catalogue chronology error
→ twentieth-century correction/reconstruction.

## Identifier/chronology issue

The `1866` date belongs first to an **inscription/note associated with a later container state**. It should not be copied directly into `object acquisition date`.

Required relation:

`container_note_date` → interpreted_as → `packing/repacking/storage event?`

with separate independent chronological evidence:

`Saint-Hilaire 1863 discussion` → contradicts → `first-arrival-in-1866 hypothesis`.

## What this tests

Container chronology and object chronology need independent fields and contradiction edges.

The case also tests **relational preservation**: separating explanatory texts from images changes what later scholars can infer from the case structure.

## Schema verdict

Pass.

Implementation needs:

- `chronology_role`: production / copy / pack / repack / dispatch / receipt / storage / catalogue / unknown;
- `chronology_conflict_id` or ordinary `contradicts` relation.

---

# Case 4 — 1870 `big deal box` and four ornithological portfolios

## Source state

Hodgson's 11 February 1870 letter to G. F. L. Marshall describes a `big deal box` containing four portfolios and a mixed research apparatus. The memorandum counts **1,104 drawing sheets** and lists:

- Hodgson's manuscript bird list;
- native painter's Hindi list including Sikkim;
- one red-bound volume of bird manners written from viva voce statements of shikaris;
- additional Darjeeling volumes of similar material;
- Hodgson's 1846 Tarai memoranda;
- printed catalogue copies/reprints;
- sundry printed papers.

Hodgson asks to hear of the `safe arrival of the box`.

## Provisional nesting

`big deal box`
→ four portfolios
→ 1,104 drawing sheets

and the same outer box also contains:

- manuscript list(s)
- Hindi list
- behavioural notebooks
- field memoranda
- printed catalogues/reprints.

## Relation graph

shikari testimony
→ written by Hodgson's writer
→ behavioural notebook

native painter
→ Hindi list

bird specimens/observations
↔ drawings
↔ Hodgson manuscript list
↔ printed catalogue.

## What this tests

A transport unit can contain heterogeneous media and multiple levels of nested containers. `Container = discipline` fails completely.

It also demonstrates that one shipment can deliberately **reassemble an evidence system that had been distributed across production stages and media**.

## Schema verdict

Pass.

Implementation should not store `contains_entity_ids` as one denormalized text field in final database. Use relation rows (`contained_in`) so nesting can be arbitrarily deep.

---

# Case 5 — RAS Hodgson MS 67, wrapper title and century-long textual misidentification

## Source state

Wave 7 records the Royal Asiatic Society case.

Cowell and Eggeling catalogued RAS Hodgson MS 67, a palm-leaf codex, as `Anumânakhaṇḍam`, apparently following a provisional title on the **wrapper**. A 2016 re-examination determined that the codex actually contains two incomplete works:

- beginning of Ratnakīrti's *Sthirasiddhidūṣaṇa*;
- substantial portion of Arcaṭa's *Hetubinduṭīkā*.

The wrapper/paracontent therefore stabilized a wrong institutional identity for more than a century.

## Provisional entities

### Object

`HOD-OBJ-TEMP-RAS-MS67`

- `object_class`: manuscript_coding_unit
- `support_material`: palm leaf
- `condition`: incomplete
- `current_repository`: RAS

### Identifier 1

`HOD-ID-TEMP-MS67-WRAPPER`

- `identifier_type`: wrapper_title
- `identifier_value_as_written`: `Anumânakhaṇḍam` (historical catalogue rendering)
- `status`: superseded / incorrect as codex-level identity
- `attached_to`: wrapper/container

### Identifier 2

modern re-identification of *Sthirasiddhidūṣaṇa* portion

### Identifier 3

modern re-identification of *Hetubinduṭīkā* portion

## Event chain

manuscript production
→ wrapper/title supplied at unknown stage
→ wrapper and codex travel together
→ nineteenth-century catalogue adopts wrapper title
→ institutional identity stabilizes
→ 2016 folio/textual re-examination
→ codex split analytically into two incomplete textual units
→ older title superseded.

## What this tests

An identifier can be physically authentic to the archival object yet textually misleading. `Original label` and `correct identity` are not equivalent categories.

The database therefore needs to preserve the wrapper title as a historical object rather than overwrite it with the modern identification.

## Schema verdict

Pass.

This is the manuscript analogue of zoological number/name failure.

---

# Cross-case findings

## 1. Auditability is an eventful property

Objects do not simply `have provenance`. Their auditability rises and falls through events:

- packing can preserve relations;
- transit can destroy material;
- receipt can verify only container-level arrival;
- sorting can expose errors;
- cataloguing can synchronize distributed sets;
- cataloguing can also propagate wrong identities;
- replacement can repair missing/defective states;
- relabelling/rebinding can erase earlier relations;
- later re-examination can restore them.

## 2. Identifiers must be historical objects

Across the five cases:

- case count verifies shipment only coarsely;
- specimen numbers collide;
- copied names diverge from numbers;
- catalogue versions alter names/synonymies;
- wrapper title misidentifies a codex;
- later case date misdates a collection.

No identifier should be silently normalized away.

## 3. `Complete collection` is a negotiated state

The British Museum case is particularly clear. `complete` emerges from repeated reconciliation, replacement and catalogue work. It is not a natural property of the shipment.

Recommended field:

- `completeness_claim`
- `completeness_basis`
- `completeness_date`
- `completeness_scope`

## 4. Relationship history is as important as object history

The same object can remain physically unchanged while its evidential relation changes:

- image separated from explanatory text;
- specimen stripped of original label;
- drawing separated from specimen set;
- wrapper title retained while textual identity is revised;
- catalogue distributed with duplicate specimens and later locally renumbered.

Final structured implementation should therefore use a relation/event model rather than a single flat object table.

---

# Schema v0.1 decision

The stress test is successful enough to freeze a **provisional relational model**, with these additions before implementation:

- `verification_granularity`
- `workflow_id`
- `event_parent_id`
- `exception_status`
- `chronology_role`
- `completeness_claim`
- `completeness_basis`
- `completeness_date`
- `completeness_scope`

Next implementation step should be a small structured dataset containing only these five cases, not an attempt to ingest the whole Hodgson archive at once. Once the five-case dataset survives querying and contradiction tracking, expand domain by domain.
