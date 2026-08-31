# Web research 2026-09-01 — Wave 42
## Exact historical addresses: Box 2 / Item 12 and the old-container graph

Date: 2026-09-01

Status: follow-up to Waves 40–41. This wave distinguishes explicit numeric historical addresses from merely surviving-but-unread shipment identifiers and seeds a graph whose nodes are historical addresses rather than modern volume numbers, support classes or languages.

## Executive result

Cambridge `MSS EUR HODGSON/6` preserves the first exact **two-level** old archival address recovered in the current pass:

`original Box 2 / Item 12`.

The address survives in the Nepali title layer of a modern volume whose documents are overwhelmingly English machine-paper copies and most of which were published.

This strengthens two conclusions.

First:

`historical custody identity != support identity != language identity`.

Second:

historical addressing could apply not only to local-source manuscripts but to a copy/report family consisting of machine-paper English documents.

Together with the already secure `Sack 8` and `Box 3` nodes, this makes a genuine old-address graph possible.

Mechanisms:

- `HISTORICAL_ADDRESS_SURVIVES_AS_EXACT_TWO_LEVEL_KEY`
- `OLD_CONTAINER_ADDRESS_ON_MACHINE_PAPER_COPY_VOLUME`
- `PAPER_AS_ADDRESSABLE_RELATIONAL_SURFACE`
- `NUMERIC_ADDRESS_REQUIRES_INVENTORY_GENERATION_CONTROL`.

---

## 1. MSS EUR HODGSON/6 = original Box 2 / Item 12

Cambridge describes `MSS EUR HODGSON/6` as a volume concerning:

- ethnic groups;
- law/legal practice;
- judicial system and police;
- towns, villages and households of the Kathmandu Valley;
- army;
- military-road measurement;
- commerce;
- Nepali papermaking.

Its English title is:

`Tribes of people, judicial system, trade, army, topography`.

Its Nepali title is given as:

`thar-tharko, adālatko, phaujako vayān`.

Crucially, Cambridge says that in this Nepali title layer there is mention of:

`the original box and Item number (2 and 12 respectively)`.

Source:
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol006.html

Thus the recoverable historical address is:

`Box 2 -> Item 12`.

This is more precise than a generic statement that the object once had a shipment number.

It is an address composed of at least two nested fields.

Mechanism:

`HISTORICAL_ADDRESS_SURVIVES_AS_EXACT_TWO_LEVEL_KEY`.

---

## 2. The address is attached to a machine-paper English copy family

The material context matters.

Cambridge states that **all manuscripts in vol.6 are copies and most were published**.

The individual items are overwhelmingly on machine-made paper, including:

- military-tribe classification;
- law/legal practice;
- Kathmandu household list;
- military-road measurement;
- Nepal commerce report;
- Hodgson's paper-making letter;
- judicial-system/police working;
- army survey.

Some are described as fine writing in excellent or very fine condition; Hodgson's pencil addenda survive on some pieces.

The historical address therefore belongs to a materially worked copy/report corpus rather than a single untouched local source.

This falsifies any assumption that old box/sack/item metadata belongs primarily to vernacular handmade-paper originals.

The current object form is:

`English analytical/copy family`
+ `machine-made support`
+ `Nepali title/address layer`
+ `historical Box 2 / Item 12 identity`
+ `modern MSS EUR HODGSON/6 identity`.

Mechanism:

`MULTIAXIAL_DOCUMENT_IDENTITY`.

---

## 3. The old address may describe a packet/family rather than one modern inventory item

Cambridge places the `Box 2 / Item 12` information at **volume level**, not under one modern item description.

That is analytically important.

Possible historical scopes include:

1. one old packet that contained several modern item states;
2. an old numbered cover or wrapper now functioning as the title layer for the modern volume;
3. a copied dossier later expanded or rearranged before 1921;
4. another custody relation not recoverable from online description alone.

Therefore do not write:

`old Item 12 = modern vol.6 item 12`.

There is no such equivalence.

The numbering systems belong to different archival ontologies.

Mechanism:

`OLD_ITEM_NUMBER_NOT_MODERN_ITEM_NUMBER`.

---

## 4. Exact-address graph now has three secure numeric nodes

### Node A — Sack 8

Modern evidence:

- `vol.58/18 f.65`: contents of manuscripts from sack No.8;
- `vol.85/4`: member manuscript explicitly carrying original sack number 8.

This is already a direct old-container → multiple-modern-volume relation.

### Node B — Box 3

Modern evidence:

- `vol.55/20 f.129v`: contents page of Box No.3 of original shipment.

Member mapping remains unresolved.

### Node C — Box 2 / Item 12

Modern evidence:

- `vol.6` title/address layer.

This is the first exact nested address.

The graph therefore begins with different node granularities:

`sack`

`box`

`box/item`.

This implies that Hodgson's historical archival addresses were hierarchical rather than a flat serial-number system.

Mechanism:

`HIERARCHICAL_HISTORICAL_ADDRESSING`.

---

## 5. RAS BHH/11/1 cannot yet be joined to Box 2 or Box 3

RAS `BHH/11/1` is the 1837–1844 list:

`List of Buddha Books & drawings, & of Statistics of Nepaul left in Residency in five Boxes`.

The RAS online description confirms:

- five boxes;
- each box individually listed;
- a sixth package;
- later notes;
- an additional heading recording that the boxes were repackaged in 1844 to take home.

Source:
https://royalasiaticarchives.org/

However, the online description does **not** transcribe the contents of Box 2 or Box 3.

Therefore the following equations are forbidden at present:

`vol.6 old Box 2 = BHH/11/1 1837 Box 2`

or

`vol.55 old Box 3 = BHH/11/1 1837 Box 3`.

Why?

The archive has documented repacking events in 1844 and later trunk/store states. Container numbers could have been retained, replaced or reused.

Numerical coincidence is a candidate relation, not identity evidence.

Mechanism:

`NUMERIC_ADDRESS_REQUIRES_INVENTORY_GENERATION_CONTROL`.

---

## 6. Evidence classes for the address graph

The reconstruction should now distinguish at least three evidence states.

### A. EXACT_TWO_LEVEL_NUMERIC_ADDRESS

Example:

`vol.6 = Box 2 / Item 12`.

### B. EXACT_NUMERIC

Examples:

`Sack 8`, `Box 3`.

### C. IDENTIFIER_PRESENT_VALUE_UNREAD

Examples:

- `vol.1/8`: original box and sack numbers exist but values omitted online;
- vol.4 notebook covers: original shipment numbers exist but values omitted;
- vol.5 covers: original shipment/sack numbers exist but values omitted;
- `vol.94/7`: old bundle numbers exist but are not transcribed.

The graph must not silently upgrade C to A/B.

Mechanism:

`IDENTIFIER_EVIDENCE_CLASS_CONTROLS_GRAPH_EDGE`.

---

## 7. Paper now has a third historically specific role

The article already treats paper as:

1. **manufactured material** — process-retentive sheet;
2. **working surface** — translation, tabulation, correction and documentary versioning.

The address evidence adds a third role:

3. **addressable custody surface**.

A paper object can carry a structured historical location such as:

`Box 2 / Item 12`.

This address can outlive:

- the box;
- the old item arrangement;
- repacking;
- institutional transfer;
- 1921 rebinding.

The modern archive may destroy physical adjacency while the old address remains legible on a title or cover surface.

Thus:

`paper stores content + operations + address`.

Mechanism:

`PAPER_AS_ADDRESSABLE_RELATIONAL_SURFACE`.

---

## 8. Strong article-facing formulation

**The old Hodgson archive was not merely a set of manuscripts later placed into boxes. Its paper objects could carry hierarchical archival addresses. A modern volume of English machine-paper copies still bears a Nepali indication that it belonged to Box 2, Item 12; other surviving sheets name Sack 8 or Box 3. These addresses are materially distinct from the texts they locate and from the modern shelfmarks that later replaced them. When twentieth-century rebinding separated earlier relations, the old address layer remained available on paper as a latent map of the archive's former topology.**

---

## 9. Immediate falsification target

The decisive next archival comparison is now sharply defined.

Read RAS `BHH/11/1` directly and transcribe:

- Box 2 contents;
- Box 3 contents;
- internal item numbering, if present;
- later 1844 annotations.

Then test:

### Test A

Does 1837 Box 2 contain a cluster resembling vol.6:

`tribes + law + trade + army + topography + paper-making`?

If yes, continuity becomes plausible and can be tested at item 12.

If no, Box numbering was likely revised between inventory generations.

### Test B

Does 1837 Box 3 match the surviving vol.55 f.129v Box 3 contents page?

If yes, Box 3 continuity can be established.

If no, number reuse/repacking is demonstrated.

Both outcomes are historically useful.

---

## Source-control rules

1. `old Item 12` is not modern `item 12`.
2. Numerical identity across inventory dates is not proof of container identity.
3. Repacking documented in 1844 makes numbering continuity an empirical question.
4. The volume-level old address in vol.6 may apply to a historical wrapper or dossier rather than every modern item equally; inspect the title/cover surface.
5. Machine-made is a support/formation description, not secure maker or national origin.
6. Do not infer unread old numbers on vol.1/4/5/94 from thematic similarity.

## Bottom line

The Hodgson paper archive now yields an exact nested historical address: `Box 2 / Item 12`, preserved on the Nepali title layer of a modern volume of English machine-paper copies. Alongside Sack 8 and Box 3, this establishes historical custody identity as a separately recoverable dimension of the paper object. The next step is no longer generic provenance research: it is a controlled comparison of exact old addresses against successive 1837–1864 inventory generations to determine which archival relations persisted through repacking and which were renumbered.