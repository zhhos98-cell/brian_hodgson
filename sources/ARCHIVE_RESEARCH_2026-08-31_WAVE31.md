# Archive research wave 31 — catalogue-distribution coevolution and the production of divergent institutional states

Date: 2026-08-31

Status: reconstruction from ZSL transcriptions of British Museum/Hodgson correspondence, especially J. E. Gray letters of early 1845. Builds on Waves 20, 24, 29 and 30.

## Executive result

The 1845 British Museum processing sequence cannot be represented as a clean linear pipeline:

`receive -> identify -> catalogue -> distribute`.

The correspondence instead shows several operations occurring recursively and partly in parallel:

`receive / unpack -> preliminary sort -> construct duplicate sets -> record distribution -> continue naming -> find omissions/exceptions -> update list -> continue distribution -> build catalogue -> send catalogue with distributed sets`.

This matters because destination collections could begin to separate physically **before descriptive metadata had stabilized**. Later divergence between British Museum, Leiden, Paris, Berlin and other holdings can therefore be generated at the initial distribution event, rather than requiring later curatorial corruption.

The key mechanism is:

`CATALOGUE_DISTRIBUTION_COEVOLUTION`.

---

## 1. Gray's 1844 pledge imagines catalogue and duplicate set as paired outputs

A British Museum/Gray memorandum records promises made in relation to Hodgson's collection:

- describe new species within about a month;
- make a catalogue within three or four months;
- exert himself regarding publication of the drawings;
- **distribute the catalogue with each set of duplicates** forwarded to institutions including Paris, Leiden, India House, Canterbury, Newcastle, Plymouth, Manchester, Liverpool, Edinburgh and Dublin.

### Mechanism

Code:

`CATALOGUE_AS_DISTRIBUTED_REFERENCE_LAYER`

The duplicate specimen set was not intended to circulate as a self-sufficient physical collection.

The catalogue would give each destination access to a wider descriptive/reference universe.

This strengthens Wave 24's `global catalogue + local subset marker` model.

---

## 2. By 6 February 1845 distribution is already occurring while the catalogue is still being prepared

### Source

`NZSL/HOD/5/2/15`, J. E. Gray to Hodgson, 6 Feb. 1845.

Gray states that:

- one Tibetan pheasant had not been marked because it was at the **stuffer's** when the list was prepared and therefore escaped;
- some birds had already been **distributed according to the list**;
- numerous poor-condition specimens remained;
- `The catalogue we are preparing` would contain a detailed list of every specimen received from Hodgson between 1840 and the present;
- Gray sends a Mammalia list showing how mammals/bones **have been distributed**;
- he asks Hodgson to lend him the bird list for a day so that **subsequent distribution could be added to it**.

### Mechanisms

- `DISTRIBUTION_BEFORE_CATALOGUE_COMPLETION`
- `LIST_AS_MUTABLE_DISTRIBUTION_LEDGER`
- `PROCESS_EXCEPTION_AT_STUFFER`

### Key sequence

`list prepared -> specimen temporarily elsewhere at stuffer -> specimen omitted/unmarked -> distribution proceeds -> further distributions occur -> list borrowed back -> distribution state written into list -> catalogue still under construction`.

The list is a live stateful object rather than a final inventory.

---

## 3. The stuffer creates a temporary blind spot in the metadata surface

Gray's Tibetan pheasant example is unusually revealing.

The bird did not vanish from the collection. It was physically in another work stage — `at the stuffers` — when the list was made, and therefore escaped marking.

### Mechanism

Code:

`PROCESS_STAGE_VISIBILITY_GAP`

A collection census can be incomplete because one object is temporarily located at a different production/processing node.

This is neither ordinary loss nor catalogue negligence in the abstract.

It is a synchronization problem:

`inventory time != all-object co-presence time`.

### Wider implication

Preparation, repair, stuffing, imaging, conservation or expert examination can all move an object outside the surface being inventoried.

The catalogue state therefore depends on the timing of observation.

---

## 4. By 13 February another group is already divided into institutional sets despite naming deficits

### Source

`NZSL/HOD/5/2/16`, Gray to Hodgson, 13 Feb. 1845.

Gray reports boxes of birds examined and divided into four collections:

- British Museum: 352 specimens;
- Collection No. 1: 140;
- Collection No. 2: 79;
- Collection No. 3: 40.

He also records another 52 specimens that were apparently badly named or not named at all and therefore of comparatively little use.

He asks Hodgson to decide the destination of Series 1, 2 and 3.

### Mechanisms

- `SET_CONSTRUCTION_BEFORE_DESTINATION_ASSIGNMENT`
- `NAMING_DEFICIT_AS_USE_CONSTRAINT`
- `PHYSICAL_SORTING_AHEAD_OF_SEMANTIC_STABILIZATION`

### Important distinction

A specimen can be physically sortable into a duplicate/reference series before it is sufficiently named to be useful as an informational object.

This gives a direct example of:

`physical addressability > semantic addressability`.

---

## 5. Naming and distribution operate on different clocks

Wave 30 showed Gray simultaneously reporting corrupted names and numbering collisions.

Wave 31 adds the temporal relation:

- physical distribution decisions can be made early;
- names can still be under completion/correction;
- catalogue can still be in preparation;
- destination metadata can be written back after a set has been constructed.

### Mechanism

Code:

`ASYNCHRONOUS_METADATA_AND_OBJECT_CLOCKS`

The collection has several clocks:

1. physical receipt/unpacking;
2. sorting/set construction;
3. preparation/stuffing;
4. naming/identification;
5. destination assignment;
6. physical despatch;
7. catalogue completion;
8. catalogue propagation.

These clocks do not close simultaneously.

---

## 6. Destination identity may be assigned after a physical set exists

Gray's 13 Feb. wording asks Hodgson who is to receive `Series 1.2.3` after those sets have already been physically assembled.

### Mechanism

Code:

`SET_IDENTITY_BEFORE_DESTINATION_IDENTITY`

The temporary collection identity is:

`Collection No. 1 / No. 2 / No. 3`

before it becomes:

`Leiden / Paris / Berlin / etc.`

### Data implication

Separate fields:

- `set_number`
- `set_construction_date`
- `destination_assignment_date`
- `despatch_date`
- `receipt_date`

Do not encode destination as if it were inherent from the moment the specimens were sorted.

---

## 7. Catalogue fields are partly retrospective records of distribution

Gray's request to borrow the bird list in order to add distributions that had occurred `since` is decisive.

### Mechanism

Code:

`POST_HOC_DISTRIBUTION_WRITEBACK`

The catalogue/list does not merely instruct distribution.

Distribution also changes the catalogue.

Bidirectional relation:

`catalogue/list -> guides set handling`

and

`physical distribution event -> updates catalogue/list`.

This is why `catalogue = checksum` is historically dynamic rather than static.

---

## 8. Catalogue-distribution coevolution

### Core mechanism

`CATALOGUE_DISTRIBUTION_COEVOLUTION`

The sequence can be represented as a feedback loop:

`preliminary list`

`-> physical sorting`

`-> duplicate set`

`-> destination decision`

`-> distribution/despatch`

`-> distribution annotation on list`

`-> further naming/correction`

`-> catalogue version`

`-> catalogue distributed with set`

`-> later institutional comparison/correction`.

No single point in the loop is necessarily the final authoritative state.

---

## 9. Metadata instability can be exported geographically

If a set leaves while:

- names are incomplete;
- numbers contain collisions;
- a list contains copier errors;
- distribution annotations are still being added;

then the destination may receive a materially coherent set coupled to an intermediate metadata state.

### Mechanism

Code:

`EXPORTED_METADATA_INTERMEDIATE_STATE`

### Consequence

Later differences between institutions need not imply that one institution corrupted a once-unified master record.

They may inherit different states from the beginning.

This is a crucial change in causal framing.

---

## 10. Physical condition creates another branch in the sorting ontology

Gray repeatedly distinguishes specimens too poor in condition to be useful for distribution.

On 6 Feb. he reports numerous birds in very bad state; on 13 Feb. he separately describes unnamed/poorly named specimens as low-use.

### Mechanism

Code:

`CONDITION_AND_METADATA_DUAL_USE_FILTER`

Institutional utility is constrained by at least two independent dimensions:

- physical condition;
- semantic/descriptive condition.

A well-named ruined specimen and an intact unnamed specimen can fail for different reasons.

### Dataset implication

Keep:

- `physical_condition`
- `metadata_condition`
- `institutional_use_status`

as separate fields.

---

## 11. Distribution list, catalogue and specimen series are distinct witnesses

The archive now contains several surface types that should never be silently merged:

- list prepared before distribution;
- mutable list with distribution writeback;
- destination-specific catalogue with subset crosses;
- British Museum tabular distribution statement;
- later published catalogue;
- Hodgson-corrected catalogue copies;
- recipient acknowledgements.

### Mechanism

Code:

`MULTI_SURFACE_DISTRIBUTION_VERSIONING`

Each surface answers a different question:

- what was planned?
- what was physically sorted?
- what destination was assigned?
- what was sent?
- what was received?
- what was retained?
- what was catalogued later?

---

## 12. March 1845 correction loop is the downstream consequence of February asynchrony

Wave 24 established that Hodgson later described the British Museum distribution statement as `full of omissions and inaccuracies` and requested a corrected copy.

Wave 31 supplies a plausible operational context without reducing all errors to one cause:

- lists were mutable;
- some objects were elsewhere during list preparation;
- distribution continued while catalogue work was unfinished;
- names and numbers contained separate error channels;
- set destination and catalogue propagation occurred at different times.

### Mechanism

Code:

`RECONCILIATION_AFTER_ASYNCHRONOUS_PROCESSING`

The later correction demand is not surprising once the process is reconstructed at operation level.

### Caution

Do not claim that every March omission was caused by the February stuffer/list timing. The sources show a structural vulnerability, not a one-to-one causal attribution for each error.

---

## 13. Receipt acknowledgements later close only selected edges

Later 1845 records show acknowledgements from institutions such as Dublin, Strickland and Haslar for specimens received.

These receipts can verify destination-level physical arrival but cannot retrospectively establish that:

- destination set exactly matched preliminary set number;
- every intended specimen travelled;
- catalogue version matched object version;
- names/numbers had been corrected before despatch.

### Mechanism

Code:

`DESTINATION_RECEIPT_PARTIAL_CLOSURE`

Receipt closes the transport edge, not the entire metadata graph.

---

## 14. The reference-series model is produced before the catalogue is final

The Museum retains its own complete/reference series while duplicate sets are being constructed.

This means `reference collection` is initially a **physical sorting decision**, later reinforced by catalogue description.

### Mechanism

Code:

`PHYSICAL_REFERENCE_SERIES_PRECEDES_FINAL_METADATA`

The authority of the central series does not arise only from a finished published catalogue.

It is materially constituted during sorting.

---

## 15. Distributed identity is generated at the sorting table

A specimen's institutional future can be decided through the act of set construction:

`British Museum reference`

versus

`duplicate set 1 / 2 / 3 ...`.

Names, destinations and catalogues may stabilize later.

### Mechanism

Code:

`SORTING_TABLE_AS_DISTRIBUTED_IDENTITY_GENERATOR`

This is a particularly strong history-of-science point: the distributed network is not merely the downstream result of shipping. It begins in the museum's sorting practice.

---

## 16. Cross-domain comparison

### Manuscript catalogue incorporation

A manuscript can be physically received while textual identity remains unresolved.

### Zoological duplicate distribution

A specimen can be physically sorted into a destination series while naming/catalogue identity remains unresolved.

### Shared structure

`physical operation can precede semantic closure`.

The common mechanism is:

`MATERIAL_STATE_AHEAD_OF_DESCRIPTIVE_STATE`.

This is more precise than generic `institutional legibility`.

---

## 17. New mechanism codes

- `CATALOGUE_AS_DISTRIBUTED_REFERENCE_LAYER`
- `DISTRIBUTION_BEFORE_CATALOGUE_COMPLETION`
- `LIST_AS_MUTABLE_DISTRIBUTION_LEDGER`
- `PROCESS_EXCEPTION_AT_STUFFER`
- `PROCESS_STAGE_VISIBILITY_GAP`
- `SET_CONSTRUCTION_BEFORE_DESTINATION_ASSIGNMENT`
- `NAMING_DEFICIT_AS_USE_CONSTRAINT`
- `PHYSICAL_SORTING_AHEAD_OF_SEMANTIC_STABILIZATION`
- `ASYNCHRONOUS_METADATA_AND_OBJECT_CLOCKS`
- `SET_IDENTITY_BEFORE_DESTINATION_IDENTITY`
- `POST_HOC_DISTRIBUTION_WRITEBACK`
- `CATALOGUE_DISTRIBUTION_COEVOLUTION`
- `EXPORTED_METADATA_INTERMEDIATE_STATE`
- `CONDITION_AND_METADATA_DUAL_USE_FILTER`
- `MULTI_SURFACE_DISTRIBUTION_VERSIONING`
- `RECONCILIATION_AFTER_ASYNCHRONOUS_PROCESSING`
- `DESTINATION_RECEIPT_PARTIAL_CLOSURE`
- `PHYSICAL_REFERENCE_SERIES_PRECEDES_FINAL_METADATA`
- `SORTING_TABLE_AS_DISTRIBUTED_IDENTITY_GENERATOR`
- `MATERIAL_STATE_AHEAD_OF_DESCRIPTIVE_STATE`

---

## 18. Immediate falsification targets

1. Reconstruct a day-by-day January–March 1845 operation chronology from HOD/5/2 and HOD/5/4.
2. Determine whether the unnamed/poorly named 52 birds were later named and assigned to destination sets.
3. Track Collection Nos. 1–3 from 13 Feb. to named institutional destinations.
4. Compare preliminary bird list, distribution writebacks, destination catalogues and final published catalogue at item/number level.
5. Identify specimens known to have been at the stuffer during list preparation and see whether their later catalogue entries retain anomalies.
6. Compare catalogue version actually received at Leiden/Paris/Berlin, if surviving, to the British Museum/Hodgson working list.
7. Separate physical condition exclusions from naming/metadata exclusions quantitatively.
8. Test whether early-exported metadata errors can be found independently in recipient catalogues/labels.
9. Build `set_number -> destination -> receipt -> local accession` joins for the major duplicate series.
10. Treat March Hodgson corrections as a distinct reconciliation state rather than replacing February records.

## Bottom line

The British Museum did not first complete the intellectual identity of Hodgson's collection and then distribute it. Physical set-making, naming, catalogue preparation and distribution advanced on different clocks and continuously wrote back into one another. A bird could be absent from a list because it was at the stuffer; a duplicate series could exist before its destination was chosen; distribution could already have occurred while the catalogue was still being prepared; and the list itself could be borrowed back to record what had happened after its first preparation. The distributed Hodgson collection was therefore born versioned. Later institutional divergences may preserve different states of an originally asynchronous processing system rather than merely later corruption.