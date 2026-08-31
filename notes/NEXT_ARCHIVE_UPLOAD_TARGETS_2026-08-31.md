# Next archive upload targets — after public Waves 17–24

Date: 2026-08-31

Status: active ingestion priority note.

## Decision

The repo has reached a high-value archival-upload threshold.

Public-source work now provides independently reconstructed comparison regimes for:

- manuscript production/procurement/accounting;
- manuscript institutional metadata and catalogue labour;
- manuscript counting/segmentation failures;
- zoological specimen/drawing/list relations;
- duplicate/reference-series construction and distribution;
- paper manufacture, treatment and affordance failure;
- transport, receipt and custody checks;
- **reconciliation surfaces**: lists/tables/catalogues used to compare expected, received, retained, distributed, missing or corrected collection states;
- **copy-state counting failure**: numerical conflicts can occur inside retained copies and should not automatically be projected back onto sent originals;
- **destination subset marking**: a global catalogue can encode the physical subset sent to one recipient by crosses/ticks or related marks.

The next archival batch can therefore be read against explicit tests rather than broad themes.

## Priority 0 — reconciliation surfaces

Wave 24 makes these the highest-value objects if available.

Prioritize any sheet/list/table/catalogue containing:

- expected count vs observed count;
- received / retained / distributed columns or subtotals;
- grand totals or recalculations;
- crosses, ticks, underlining, destination initials or other subset markers;
- marginal comments such as missing, omitted, inaccurate, corrected;
- evidence that a fair/corrected copy was requested;
- several copy states of the same list or letter;
- numbered catalogues used to infer missing or expected objects.

Key tests:

1. what historical state does the document claim to represent?
2. what other state was it compared against?
3. does arithmetic close internally?
4. is the witness an original, sent letter, retained copy, draft, fair copy, printed version or later transcript?
5. does a graphical mark identify the physical subset sent to a particular destination?
6. was a corrected version propagated after an error was found?

Model public case: `NZSL/HOD/5/4/9`, whose surviving **copy** gives a tabulated 85 drawings but later prose says 81; its stated grand total closes only with 81. Do not normalize comparable archival discrepancies prematurely.

## Priority 1 — highest information gain

### A. Original specimen lists / distribution tables

Especially valuable if they contain any combination of:

- Hodgson/Gray numbers;
- names;
- sex/age;
- locality;
- date;
- preparation state;
- condition;
- destination;
- duplicate status;
- later corrections.

Key tests:

- can the mutable list states described by Gray in February 1845 be reconstructed?
- were distributions written back onto the same list?
- can specimen numbers be linked to drawings or surviving institutional accessions?
- do received, retained and distributed totals occupy distinct list states?

### B. Original labels or label transcriptions

Highest value if they preserve:

- local name;
- locality;
- date;
- red drawing number;
- later Museum labels alongside old labels.

Key test:

- what relational information was lost or transformed by later relabelling?

### C. Numbered zoological drawings

Prioritize sheets with:

- Hodgson number;
- local/Sanskrit/Nepali/Tibetan name;
- Latin/European taxonomic name;
- sex/age annotations;
- measurements;
- specimen references;
- paper/watermark evidence;
- corrections by Hodgson or later zoologists.

Key test:

- does drawing number function as a stable cross-media key in the actual archive?

## Priority 2 — manuscript production and incorporation

### D. Working manuscript lists

Especially lists recording:

- title;
- leaves;
- slokas/stanzas;
- price;
- bundle/box number;
- copy/original status;
- support;
- condition;
- owner/source;
- corrections/addenda.

Top known targets remain BL Hodgson/12 ff. 179–182 and related lists if private copies/photos exist.

Key test:

- how were work, volume, bundle and price converted into one another operationally?

### E. Bills / accounts

Prioritize bills joining at least two of:

- paper purchase;
- scribal labour;
- binding;
- carpentry;
- packaging;
- wax cloth/thread/twine;
- porters;
- freight/shipment;
- reimbursement.

Key test:

- reconstruct manuscript production as a costed material supply chain.

### F. Catalogue proofs / abstracts / correction sheets

Especially:

- Pandit abstracts;
- Mitra/Hodgson corrections;
- proof sheets;
- title corrections;
- cross-references to original MSS;
- translation stages.

Key test:

- measure derivation depth and verification depth between manuscript and printed catalogue.

## Priority 3 — container and custody relations

### G. Packing lists tied to boxes/bundles

High value fields:

- box/bundle number;
- contents count;
- internal list;
- packing/repacking date;
- destination;
- receipt annotation;
- missing/extra items;
- later container reuse.

Key test:

- separate transport identity from later catalogue identity and container chronology.

### H. Receipts and reconciliation documents

Especially documents that distinguish:

- cases/boxes received;
- internal items checked;
- missing/partial/damaged objects;
- later inventory correction;
- safe arrival vs actual incorporation.

## Priority 4 — paper census material

### I. Full recto/verso images with scale

For any Hodgson sheet, record if visible:

- dimensions;
- edges;
- folds;
- laid/wove/cloth-frame appearance;
- watermark/countermark;
- thickness variation;
- colour;
- surface treatment;
- mounting/pasting;
- verso reuse;
- seals/labels/adhesives.

Do not need transmitted light for first-pass upload. Ordinary full-sheet images are enough to triage which cases justify better imaging.

## Upload does not need archival completeness

A useful batch can be small and heterogeneous.

Preferred first batch size:

- roughly 10–30 high-information objects/images/documents;
- preserve file names or shelfmarks where known;
- include recto/verso together where possible;
- do not spend time normalizing or renaming before upload if that delays access.

The repo can reconstruct relations after ingestion.

## Ingestion questions to apply to every item

1. What historical unit is being counted?
2. Is the count `expected`, `observed`, `received`, `retained`, `distributed`, `missing`, or `corrected`?
3. Does the arithmetic close internally?
4. What physical object or document state is visible?
5. Is this an original, sent copy, retained copy, draft, fair copy, proof, printed version or later transcript?
6. What metadata fields are actually present?
7. Are there graphical subset markers: cross, tick, underline, destination initial, cancellation?
8. Which relations are physically carried by the sheet/label/list?
9. What downstream operation was this object meant to enable?
10. Is this a first record, updated state, receipt, reconciliation, correction or propagated corrected copy?
11. What is semantically addressable?
12. What is physically addressable?
13. What is relationally addressable?
14. Does the surviving identifier prove only species/object relation, or a stronger specific historical event relation?
15. Is there an explicit failure/reconciliation/correction event?
16. Can the object be joined to a public printed/catalogue state already in the repo?
17. What paper/material observations can be made without over-inference?

## Bottom line

Upload next rather than waiting for a complete archival sorting pass. Waves 17–24 have moved the public-source scaffold from thematic reconstruction to object-level tests of counts, copy states, subset markers, cross-media identifiers and reconciliation. Even scattered archival records can now falsify, refine or materially strengthen the article's central claim about reconstructibility after movement.
