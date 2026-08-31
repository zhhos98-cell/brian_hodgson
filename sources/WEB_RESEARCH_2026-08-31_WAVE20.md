# Web research wave 20 — zoological distribution matrix, relational addressability, and type-proof limits

Date: 2026-08-31

Status: direct archival-description reconstruction from ZSL/RAS catalogues plus modern type-history controls. The distribution counts and 1845 correspondence are from archival transcriptions; label-system reconstruction is supported by Dickinson 2006, who explicitly cites Gray & Gray 1847 and surviving Hodgson labels.

## 1. Formal delivery to the British Museum, 3 January 1845

Hodgson's copy letter to the Trustees of the British Museum records a large continuation of his Nepal/Tibet zoological donation:

- animal drawings: 15;
- bird drawings: 70;
- drawings total: 85;
- mammal skins: 402;
- bird skins: 4,444;
- skins total: 4,846;
- osteological specimens of mammals: 406;
- osteological specimens of birds: 663;
- osteological total: 1,069;
- grand total: **5,996** items according to the detailed lists delivered to Edward Gerrard.

The osteological material was added after suggestion by the Keeper of the Zoological Department following inspection. Hodgson explicitly connected the bones with determining the nature/limits of species and natural classification.

### Mechanism

The receiving institution did not simply accept a pre-fixed object class. Inspection changed the desired evidential package:

**skins + drawings -> institutional inspection -> osteological series added -> expanded comparative object system.**

This is an important form of receiving-side co-production.

Primary archival transcription:
ZSL `NZSL/HOD/5/4/9`, 3 Jan 1845.

---

## 2. February 1845 distribution matrix

A Hodgson memo of the zoological collections records how the enlarged British Museum holdings were redistributed after incorporation. It separates at least four material classes:

- bird skins;
- mammal skins;
- bird bones;
- mammal bones/horns.

Named recipient nodes include:

- British Museum;
- India House;
- Leyden;
- Paris;
- Berlin;
- Frankfurt;
- Edinburgh;
- Dublin;
- Newcastle;
- Canterbury;
- Manchester;
- Earl of Derby;
- H. Strickland;
- Royal College of Surgeons;
- Haslar College/Hospital.

The surviving transcription gives, for example:

| Destination | Bird skins | Mammal skins | Bird bones | Mammal bones/horns |
|---|---:|---:|---:|---:|
| British Museum | 1,753 | 170 | 337 | 195 |
| India House | 655 | 102 | 79 | 45 horns |
| Leyden | 536 | 78 | 40 | — |
| Paris | 462 | 48 | 52 | — |
| Berlin | 411 | 37 | — | — |
| Frankfurt | 352 | 7 | — | — |
| Edinburgh | 321 | — | — | — |
| Dublin | 290 | — | — | — |
| Newcastle | 259 | — | — | — |
| Canterbury | 237 | 2 | — | — |
| Manchester | 213 | — | — | — |
| Earl Derby | 205 | — | — | — |
| H. Strickland | 169 | — | — | — |
| Royal College of Surgeons | 140 | — | — | 58 |
| Haslar College/Hospital | 1 | — | 79 | — |

The memo's surviving transcription also records column totals at least for bird skins and mammal skins/bones; these should be checked against the digital object before publication-level use because the archival HTML formatting is partly degraded.

Primary archival transcription:
ZSL `NZSL/HOD/5/4/16`, Feb 1845.

### Analytical point

This is a genuine **distribution matrix**, not merely a donation list. Duplicate-making was an institutional operation that converted one received collection into multiple geographically separated comparison sets.

The matrix creates three different object states:

1. retained reference series;
2. distributed duplicate series;
3. residual/problem specimens excluded from useful distribution.

The act of distribution therefore changes the future verification architecture of the collection.

---

## 3. Gray's 6 February letter: list reconciliation after receipt

J. E. Gray tells Hodgson that while looking over the bird list he found an omission: a Tibetan pheasant had not been marked because it was at the stuffer when the list was prepared. The Ganges Pelican was represented only by a head rather than full specimens. He also says many specimens were in such poor condition that they were useless for distribution.

Gray states that the catalogue then being prepared would contain a detailed list of **every specimen received from Hodgson between 1840 and 1845**. He sends a mammal/bone distribution list and asks Hodgson to return the bird list temporarily so later distributions can be added to it.

Primary archival transcription:
ZSL `NZSL/HOD/5/2/15`, 6 Feb 1845.

### Mechanism

The list is a **mutable operational ledger**, not a frozen catalogue precursor:

**receipt -> physical inspection -> exception detection -> distribution -> list returned/updated -> catalogue compilation.**

The stuffer case is especially valuable because it shows how temporary physical location produces metadata omission even when the specimen has not been lost.

---

## 4. Gray's 13 February letter: sorting creates usefulness classes

After boxes of birds were examined, Gray divided them into four series:

- British Museum: 352 specimens;
- Collection no. 1: 140;
- Collection no. 2: 79;
- Collection no. 3: 40;
- additional 52 birds judged comparatively little use because they were unnamed or problematic in naming.

He also retained a complete reference series of mammalian skulls/horns and bird bones while setting aside obvious duplicates.

Primary archival transcription:
ZSL `NZSL/HOD/5/2/16`, 13 Feb 1845.

### Mechanism

This gives a clean receiving-institution pipeline:

**box contents -> examination -> identification/naming -> condition/usefulness judgment -> reference-series retention -> duplicate selection -> numbered distribution series.**

A duplicate is therefore not simply a pre-existing second specimen. It becomes a `duplicate for distribution` through institutional comparison and selection.

---

## 5. Hodgson's original specimen identity was relational

Modern reconstruction of Hodgson's bird collections, based on Gray & Gray 1847 and surviving labels, describes a two-label system:

- one label recorded collection date, locality and a local name;
- another carried the corresponding Hodgson drawing number, often in red ink.

Hodgson used the drawing number to relate specimens to his retained/master drawings. By 1837 he had assigned hundreds of such numbers, and the same number could be applied to more than one comparable specimen.

British Museum practice later removed many original Hodgson labels. Some drawing-number labels survive in specimens that passed through other institutional routes, and some Hodgson information was copied onto later museum labels.

Control source:
Edward C. Dickinson, 2006, “An introduction to the bird collections of Brian Houghton Hodgson (1801–1894),” *Zoologische Mededelingen* 80.

### Relational addressability

A zoological specimen's historical identity can therefore depend on a graph:

**specimen <-> local/date/locality label <-> drawing-number label <-> master drawing <-> manuscript list/catalogue <-> institutional accession record.**

Removing one node or edge can preserve the physical skin while degrading the capacity to reconstruct collection event, representation, or taxonomic history.

---

## 6. Three strengths of addressability

Wave 20 sharpens the repo's `addressability` concept into three levels.

### A. Physical addressability

Can the institution locate the object?

Examples:
- accession number;
- box/series location;
- current shelf/storage unit.

### B. Relational addressability

Can the object be connected to its distributed representations and historical metadata?

Examples:
- Hodgson drawing number;
- original label;
- drawing;
- distribution list;
- Hodgson bird/mammal list.

### C. Event-proof addressability

Can surviving identifiers prove that this particular object participated in a specific historical event?

Example:
- was this exact specimen available to Hodgson or Blyth when a taxon was described?

The third level is substantially stronger than the first two.

---

## 7. Type identification demonstrates the limit of surviving identifiers

Later type research explicitly warns that an original Hodgson label plus drawing number can strongly improve historical reconstruction but may still be insufficient to prove type status.

A surviving Hodgson number may establish:

- relation to a master drawing;
- compatibility with the taxon represented;
- continuity with Hodgson's numbering system.

A British Museum accession number may establish:

- museum incorporation year or approximate receipt event.

But the same drawing number could be used on several comparable specimens, and collection dates are frequently absent. Therefore one cannot automatically prove that a particular skin was physically before the author at the moment of description.

### Rule

**identifier match != event participation proof.**

The census should distinguish:

- `IDENTIFIED_OBJECT`;
- `RELATIONALLY_LINKED_OBJECT`;
- `EVENT_PARTICIPATION_PROBABLE`;
- `EVENT_PARTICIPATION_PROVED`.

This is directly comparable to manuscript work-identification problems while remaining materially distinct.

---

## 8. 1870 Marshall loan shows Hodgson preserving a composite verification apparatus

A memorandum for G. F. L. Marshall records a loan in **four portfolios** containing:

1. 1,104 sheets of ornithological drawings;
2. Hodgson's own manuscript list of Nepal birds;
3. his native painter's Hindi list of the whole collection including Sikkim material;
4. a red-bound volume on bird manners produced by Hodgson's writer from viva voce statements of shikaris;
5. manuscript memos made by Hodgson in the Sikkim Tarai in 1846;
6. two copies of his own London-printed catalogue;
7. six copies of the Calcutta reprint;
8. author copies of various printed papers.

Primary archival transcription:
ZSL, Marshall memorandum, Feb 1870.

### Analytical importance

This is not simply a drawing archive. It is a **composite verification apparatus** in which visual, numerical, vernacular, behavioural, manuscript and printed representations travel together.

The four portfolios preserve relations among media that later institutional dispersal could sever.

---

## 9. Cross-domain comparison with manuscript cataloguing

The manuscript and zoological systems now share several mechanisms:

| Mechanism | Manuscripts | Zoology |
|---|---|---|
| transport unit | bundle/box | box/crate/series |
| physical object | codex/leaf | skin/bone/drawing |
| operational identifier | shelfmark/title/list number | drawing number/specimen number/accession |
| receiving operation | identify/segment/catalogue | identify/compare/sort/distribute |
| major failure | false lump/split | label loss/number collision/misnaming |
| institutional output | catalogue entry/work identity | reference series/distribution series/catalogue |
| deeper proof problem | is this one work or several? | is this exact specimen historically the type/witness? |

### Critical distinction

Do not force the two systems into one ontology.

Manuscript failure often concerns **segmentation**: how many textual works inhabit a material codex?

Zoological failure often concerns **relation and event identity**: which representation, collection event, name, and description belong to this physical specimen?

The shared problem is not `classification` in the abstract. It is **maintaining auditable relations through movement and institutional transformation**.

---

## 10. New article-level formulation

A stronger cross-domain claim is now available:

> Hodgson's collections became institutionally usable only when receiving institutions could address objects at several levels at once: physically locate them, reconnect them to lists and representations, and sometimes prove their participation in earlier acts of observation or description. Manuscript cataloguing created textual units by inspecting internal boundaries; zoological cataloguing instead had to preserve links among skins, drawings, labels, names and collection histories. In both domains, material survival could coexist with loss of historical auditability.

---

## 11. Archive-upload implications

This wave further raises the value of the following archive materials:

1. Hodgson's original bird/mammal distribution lists;
2. lists with corrections after Gray/British Museum sorting;
3. surviving paired labels or label transcriptions;
4. numbered drawings with verso/locality/date annotations;
5. accession/register extracts showing institutional replacement of Hodgson identifiers;
6. packing/crate lists whose item counts can be joined to the 1845 distribution matrix;
7. 1870 portfolio/list apparatus or later copies derived from it.

If any of these appear in the next uploaded batch, ingest them before generic correspondence.

## Bottom line

Wave 20 converts Hodgson's zoological circulation from a narrative of donation into an object-level distribution and verification system. The 5,996-item 1845 delivery was reworked by inspection into reference and duplicate series distributed across multiple institutions. Lists were repeatedly corrected as physical inspection exposed missing, partial, badly preserved or unnamed objects. Hodgson's paired labels and drawing numbers made specimens relationally addressable, but later label removal demonstrates that physical survival need not preserve evidential relations. Type-history work adds the final limit: even a surviving identifier may locate and link an object without proving its participation in a specific historical description event.
