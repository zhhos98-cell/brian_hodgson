# Web research wave 21 — zoological catalogue versions, additions filters, annotation, and publication timing

Date: 2026-08-31

Status: version-history reconstruction from ZSL archival descriptions, the 1847/1863 British Museum catalogues, and Dickinson/Walters 2006 publication-history analysis.

## 1. Working lists existed before the printed catalogue

ZSL preserves `NZSL/HOD/1/2`, formal copies of lists of skins, skeletons and skulls sent to the British Museum, described as probably compiled by J. E. Gray and G. R. Gray before their printed catalogue. The archival description reports large class counts and explicit origins, but one count label in the online summary appears internally ambiguous and should be checked against the digitized object before use.

This archival survival is important even without the unresolved count:

**working list -> printed catalogue** is demonstrably a version sequence, not an inferred one.

The 1845 Gray correspondence independently shows the bird and mammal lists being physically returned, corrected and extended as distributions occurred.

### Rule

Treat the pre-publication list as a versioned operational object with its own date, completeness and correction state.

---

## 2. The first British Museum catalogue has an imprint/publication-date split

The first *Catalogue of the specimens and drawings of Mammalia and Birds of Nepal and Thibet* bears an 1846 imprint.

Dickinson & Walters reconstruct that it was not actually available as a published work until January 1847. British Museum Standing Committee minutes of 9 January 1847 record that the catalogue had been completed and received from the printer.

### Mechanism

`imprint_date` and `actual_availability_date` are separate metadata fields.

This matters because zoological names and priority depend on when a printed catalogue became publicly available, not merely the year printed on its title page.

### Schema consequence

For catalogues/publications store:

- `imprint_date`;
- `printer_completion_date`;
- `institutional_receipt_from_printer`;
- `public_availability_date_if_known`;
- `priority_relevance`.

The publication object itself has a custody/availability biography.

---

## 3. Authorship is also a version-history problem

The first catalogue has often been attributed to John Edward Gray alone or to Hodgson. Dickinson & Walters argue that both John Edward and George Robert Gray should be credited, particularly for the ornithological portion; Hodgson's role remains that of collection-maker, donor, source of names/descriptions and author of associated material rather than straightforward sole catalogue authorship.

### Importance

A printed catalogue is produced from distributed intellectual labour:

- Hodgson's specimens/drawings/numbers/names;
- Gray brothers' museum comparison and catalogue compilation;
- printers;
- British Museum institutional authorization.

This parallels the manuscript catalogue labour economy without assuming identical professional structure.

---

## 4. 1863 is a second catalogue state, not a complete restatement of the 1847 collection

The 1863 *Catalogue of the Specimens and Drawings of Mammals, Birds, Reptiles, and Fishes of Nepal and Tibet* is explicitly a **Second Edition**, xii + 90 pages, and includes Hodgson's own “Account of the collection.”

But its operational scope is better understood as an **additions/update layer**.

Later reconstruction shows:

- Hodgson resumed collecting after moving to Darjeeling/Sikkim;
- while packing in Darjeeling in December 1857 he counted **2,986 skins**;
- only **eight** were judged still to require description, associated with drawing numbers 908, 953, 956, 977, 979, 980, 981 and 982;
- the British Museum later selected **598** specimens from subsequent material;
- only about **90** are actually represented in the 1863 report because most of the remainder were additional specimens of species already present from the 1843–45 donations, including duplicates potentially useful for exchange.

### Consequence

A catalogue's apparent absence of a received specimen can reflect a **version-purpose filter**, not loss or oversight.

Add controlled reason:

- `EXCLUDED_AS_ALREADY_REPRESENTED_TAXON`;
- `DUPLICATE_NOT_RELISTED`;
- `VERSION_SCOPE_ADDITIONS_ONLY`.

This is essential when reconstructing object counts from printed catalogues.

---

## 5. Catalogue entry count != specimen receipt count

The 1863 case makes the distinction quantitative:

**598 selected specimens -> ~90 catalogue-listed additions.**

This is not a direct conversion ratio and should never be generalized. It proves that the catalogue is performing a different counting operation.

The receiving institution asks not simply “how many objects arrived?” but:

- which taxa are already represented?
- which specimens add descriptive novelty?
- which are duplicates?
- which are useful for exchange?
- which require new description?

### Counting ontology extension

Add zoological units:

- `received_specimen_count`;
- `selected_specimen_count`;
- `reference_specimen_count`;
- `duplicate_specimen_count`;
- `taxon_addition_count`;
- `catalogue_entry_count`;
- `new_description_required_count`.

Do not reconcile these by subtraction without the historical sorting rule.

---

## 6. Hodgson retained and annotated institutional catalogues

ZSL `NZSL/HOD/1/4` preserves:

- British Museum mammal list, 1843 — Hodgson-signed, not annotated;
- British Museum bird list, Accipitres, 1844 — Hodgson-signed, not annotated;
- British Museum mammal catalogue, `Ungulata furcipeda`, 1852 — annotated by Hodgson;
- **three copies** of the 1863 second edition — annotated by Hodgson.

ZSL `NZSL/HOD/1/5` also preserves **two Hodgson-annotated copies** of Thomas Horsfield's catalogue of the mammal collection presented to the East India Company.

### Mechanism: returned catalogue

The institutional catalogue moves back to the donor/collector and becomes a working correction surface:

**collection/list -> receiving institution -> printed catalogue -> copy returns to Hodgson -> annotation/correction -> later archival survival.**

This creates a recursive metadata loop rather than a one-way publication endpoint.

### Archive priority

The annotated copies are high-value because they can identify:

- name disagreements;
- missing taxa/objects;
- additions;
- priority claims;
- corrections to locality or number;
- dissatisfaction with institutional classification;
- self-archival revision.

Their annotations should be transcribed layer by layer rather than summarized thematically.

---

## 7. Different receiving institutions generated different metadata afterlives

The British Museum removed many original Hodgson labels, while Frederic Moore at the East India Company Museum preserved them, a practice later praised by Sharpe.

The two institutions therefore received overlapping Hodgson material but produced different later capacities for audit:

- British Museum: powerful cataloguing/comparison infrastructure, but destructive intervention in original labels;
- East India Company Museum: stronger survival of original Hodgson labels, enabling later historical reconstruction.

### Comparative claim

Institutional sophistication cannot be ranked on one scale. One practice may increase taxonomic legibility while reducing provenance legibility.

This is a direct analogue to manuscript cataloguing that increases textual access while rebinding or reclassification may destroy older relational structure.

---

## 8. Version-specific correction should replace the notion of “the Hodgson catalogue”

The zoological source chain now includes at least:

1. Hodgson working drawing/specimen numbers;
2. Hodgson lists;
3. Gray working receipt/distribution lists;
4. 1844 Hodgson bird catalogue/list;
5. 1847 British Museum printed catalogue (1846 imprint);
6. East India Company/Horsfield-Moore catalogue states;
7. Hodgson annotations on institutional catalogues;
8. 1863 British Museum second edition;
9. Hodgson annotations on three 1863 copies;
10. later museum type catalogues and re-identifications.

Each state can change:

- object inclusion;
- taxonomic name;
- synonymy;
- drawing-number relation;
- institutional location;
- publication/priority status;
- provenance recoverability.

### Rule

Never cite “Gray's Hodgson catalogue” without specifying edition/state where the distinction matters.

---

## 9. Cross-domain comparison with Hunter/Mitra

The manuscript chain:

**working/list state -> Hunter printed catalogue -> Mitra diagnosis of errors -> deeper reanalysis -> new catalogue identity.**

The zoological chain:

**working/specimen/distribution lists -> Gray printed catalogue -> Hodgson annotations + new collections -> 1863 additions edition -> later type re-identification.**

The structural similarity is strong enough to support a cross-domain claim:

**catalogues are versioned instruments for reconciling changing object populations with changing classification systems.**

But the primary error mechanisms differ:

- manuscripts: segmentation, aliasing, shallow codex inspection;
- zoology: label loss, name/number divergence, specimen duplication, priority and event-history uncertainty.

---

## 10. New article-level mechanism: version-purpose filtering

### Definition

**Version-purpose filtering** = the selection rule by which a new list/catalogue state represents only those objects or relations relevant to its current institutional purpose.

Examples:

- distribution list records who received duplicates rather than every descriptive trait;
- 1863 catalogue emphasizes additions/new representation rather than every later specimen received;
- type catalogue later selects specimens relevant to nomenclatural history;
- Hodgson annotations select errors/disagreements important to him.

### Why it matters

An omission from a later catalogue cannot be treated immediately as evidence of physical absence.

One must ask:

**what was this version trying to make visible?**

---

## 11. Immediate archive checks

Highest-value next objects:

1. `NZSL/HOD/1/4` — compare the three annotated 1863 copies: identical annotations or distinct working copies?
2. `NZSL/HOD/1/5` — compare Hodgson's two annotated Horsfield copies.
3. `NZSL/HOD/1/2` — inspect pre-publication formal lists and resolve the ambiguous online count labels.
4. Hodgson bird-description notebooks numbered by drawings (`NZSL/HOD` notebooks covering 1–169, 340–488, 755–855).
5. identify whether Hodgson annotations were incorporated into any later catalogue/reprint or remained private recursive archive.

## Bottom line

Wave 21 turns zoological catalogue history into a version graph. The first British Museum catalogue has an 1846 imprint but a January 1847 availability history; the 1863 second edition is an additions-oriented state in which hundreds of received/selected specimens need not reappear as catalogue entries because most belonged to already represented taxa. Hodgson's multiple annotated institutional catalogues then show metadata returning to the collector as a correction surface. Catalogue omission, annotation and republication must therefore be interpreted through version purpose, not as transparent reflections of the physical collection.
