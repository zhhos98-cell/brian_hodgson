# Archive research wave 41 — container fossils: original bundle covers, shipment numbers, box content pages, and the archaeology of pre-1921 paper order

Date: 2026-08-31

Status: paper-centred reconstruction from the British Library Hodgson inventory. This wave asks whether the pre-1921 physical organization of Hodgson's papers can be partially reconstructed from surviving cover pages, title folios, bundle numbers and box-content sheets that were incorporated as folios when the India Office Library rebound the papers in 1921.

## Executive result

The British Library inventory preserves repeated remnants of Hodgson's earlier paper grouping system:

- cover pages of original bundles;
- title folios from shipment groups;
- content pages of numbered boxes;
- original shipment numbers written on notebook covers;
- Nepali title descriptions on covers;
- covers of posted letters with postal stamps.

These remnants survive **inside later bound volumes** even when the original bundle/box/notebook relationships have been rearranged.

The core mechanism is:

`CONTAINER_FOSSIL_AS_PROVENANCE_SURFACE`.

A later archive can destroy or alter an earlier physical grouping while preserving fragments of the old grouping's paper boundary and metadata system.

The result is an archival archaeology:

`old bundle/box/notebook -> cover/title/content surface -> 1921 rebinding -> displaced folio -> modern catalogue -> partial reconstruction of prior order`.

---

## 1. 1921 binding created a new physical order

The Hodgson collection introduction states that the India Office Library bound the papers into 95 volumes in 1921, partly according to physical dimensions.

Consequences explicitly recorded by the catalogue:

- intellectually related documents could be separated;
- original manuscripts and translations/copies could be bound in different places because their paper sizes differed;
- some modern volumes contain heterogeneous subject matter.

### Mechanism

`ARCHIVE_GENERATED_SIZE_ORDER`.

Wave 41 adds the inverse question:

**what traces of the old order survived the creation of the new one?**

---

## 2. MSS EUR HODGSON/55 preserves several original bundle covers as folios

`MSS EUR HODGSON/55`, item 20, ff.114–172, is a mixed corpus of original/copy royal orders, official notes and letters, mostly on Nepali hand-made paper with some machine-made paper.

The catalogue identifies:

- `ff.126–128: Cover pages of different original bundles`;
- `f.129 verso: Content page of box No. 3 of original shipment`;
- `f.172: Cover of a letter addressed to Hodgson in Darjeeling with Darjeeling Post Office stamp dated 1856`.

Earlier in the same volume:

- `f.72` is identified as a cover-page of another manuscript group relating to Bhaktapur/Patan revenue.

### Mechanisms

- `ORIGINAL_BUNDLE_COVER_SURVIVAL`
- `ORIGINAL_BOX_CONTENT_PAGE_SURVIVAL`
- `POSTAL_COVER_SURVIVAL`
- `DISPLACED_BOUNDARY_SURFACE`.

### Strong point

The later volume contains paper objects whose **historical function was to delimit or describe a different grouping**.

They are not ordinary content folios.

---

## 3. A box content page is a nested metadata surface

`f.129 verso` records the contents of `box No. 3 of original shipment`.

### Mechanism

`BOX_CONTENT_METADATA_SURFACE`.

### Operational hierarchy

Potentially:

`shipment -> numbered box -> content page -> bundles/items`.

The paper page sits inside a container hierarchy but makes that hierarchy portable after the box itself disappears.

### Research value

If its entries can be joined to surviving folios/items, the content page can reconstruct:

- original co-packaging;
- shipment sequence;
- category labels;
- perhaps missing or displaced items.

This is a direct paper-based route to provenance reconstruction.

---

## 4. MSS EUR HODGSON/56 independently preserves original group covers

`MSS EUR HODGSON/56`, item 1, ff.1–20:

- Nepali hand-made paper;
- mixed notes on Tibetan animals, family names, payments, letters and other material;
- catalogue explicitly says `ff.1–2 are cover pages of two different original groups of manuscripts`.

Item 15, ff.53–58:

- contains `a cover page from the original bundle` related to Tibetan and Nepali/Vajrayana Buddhist traditions.

Item 20, ff.98–116:

- miscellaneous inserted material includes a `cover page with content of original bundles of manuscript`.

### Mechanisms

- `MULTIPLE_ORIGINAL_GROUP_COVER_SURVIVAL`
- `COVER_CONTENT_METADATA_SURFACE`
- `OLD_GROUPING_TRACE_INSIDE_NEW_VOLUME`.

### Significance

The repeated wording across multiple items confirms that original cover pages were not one accidental survival.

They form a recurrent class of archival object.

---

## 5. MSS EUR HODGSON/94 preserves original shipment numbering and categories

`MSS EUR HODGSON/94`, item 7, ff.40–44:

- separated leaves;
- Nepali hand-made paper;
- title folio of a set of manuscripts;
- list of contents of an original shipment of Hodgson's Nepali manuscripts;
- details include **bundle number and categories**.

### Mechanisms

- `ORIGINAL_SHIPMENT_TITLE_FOLIO`
- `BUNDLE_NUMBER_AS_PROVENANCE_KEY`
- `CATEGORY_ON_SHIPMENT_SURFACE`.

### Strong paper-history point

Shipment identity was externalized on paper before later institutional cataloguing.

`bundle number` is therefore not merely a modern archival identifier; it belongs to an earlier transport/grouping system.

---

## 6. Pre-bound notebooks preserve original shipment numbers on covers

The inventory gives particularly explicit statements for several volumes.

### MSS EUR HODGSON/4

Four pre-bound notebooks; in most cases the cover pages carry:

- Nepali title;
- original shipment number in Nepali language/script.

### MSS EUR HODGSON/5

Six pre-bound notebooks; again, cover pages normally bear:

- Nepali title;
- original shipment number in Nepali language/script.

### Mechanisms

- `NOTEBOOK_COVER_AS_SHIPMENT_IDENTITY_SURFACE`
- `LOCAL_SCRIPT_PROVENANCE_METADATA`
- `COVER_TITLE_PLUS_TRANSPORT_NUMBER`.

### Importance

The cover combines at least two identity systems:

- semantic title;
- transport/shipment number.

That makes it a join surface between intellectual content and logistics.

---

## 7. Covers are not merely protective paper

Across the corpus, covers can carry:

- title;
- original shipment number;
- contents;
- addressee;
- postal stamp;
- provenance grouping;
- later English/Nepali title descriptions.

### Mechanism

`COVER_AS_RELATIONAL_METADATA_LAYER`.

### Core operation

`physical boundary -> semantic/logistical identity surface`.

The loss of the cover can therefore destroy relations even if inner text survives.

This directly reinforces Wave 39's Cowell–Eggeling case where a manuscript title survives on the wrapper only.

---

## 8. Container fossils permit pre-archive reconstruction

A `container fossil` is defined here as:

**a surviving paper surface whose earlier function was to delimit, title, number, index or route a physical grouping that no longer survives intact in that form.**

Examples:

- bundle cover now bound as a folio;
- box contents page without original box;
- shipment title folio separated from original leaves;
- notebook cover embedded within later volume;
- postal cover preserved without original envelope configuration.

### Mechanism

`CONTAINER_FOSSIL_AS_PROVENANCE_SURFACE`.

### Caution

The term is analytical, not a historical archival category. Every use must be tied to a catalogue-described original container/boundary operation.

---

## 9. Old and new archival orders coexist materially

After 1921:

- modern volume number locates the folio;
- old bundle/box/shipment number may still appear on its surface.

### Mechanism

`SUPERIMPOSED_ARCHIVAL_ADDRESS_SYSTEMS`.

Potential identity tuple:

`modern BL volume/folio`

+ `historical notebook title`

+ `historical shipment number`

+ `historical bundle/box number`

+ `later catalogue item`.

### HPS significance

A paper object can carry several non-coincident systems of order produced at different moments.

This is a material version history of archival addressability.

---

## 10. Original covers can expose lost historical classification

Because cover/title pages name or summarize original groups, they can reveal categories that later volume titles obscure.

Example problem:

A modern volume may be called `Ethnography, topography, history`, yet its original cover surfaces may encode narrower or differently organized groupings.

### Mechanism

`ORIGINAL_COVER_CATEGORY_VS_LATER_VOLUME_CATEGORY`.

### Research question

How often does a historical group name differ from the 1921 volume-level subject heading?

This can test whether later archival classification merely rearranged physical order or also changed conceptual grouping.

---

## 11. Volume 4 shows reuse inside pre-bound notebook paper before 1921

`MSS EUR HODGSON/4` contains a striking internal relation:

- Item 2, a notebook on Newars;
- Item 3, `Buddha Scriptures of Nepal`, written on the **back pages of the same folios**.

### Mechanism

`NOTEBOOK_REVERSE_SIDE_REUSE`.

### Importance

The historical notebook itself already contains cross-subject reuse before later archival binding.

This warns against treating 1921 as the sole producer of mixed subject adjacency.

There are at least two layers:

1. Hodgson-era reuse/composition;
2. India Office size-based rebinding.

---

## 12. A very long folded paper is another pre-binding form state

`MSS EUR HODGSON/60`, item 7, f.59:

- 32 answers on the judicial system collected by Bicari Shankar;
- a single folio described as `a very long folded paper`.

### Mechanism

`LONG_FOLDED_SINGLE_DOCUMENT_STATE`.

### Significance

The fold is part of the document's physical form, not automatically a postal/storage crease.

Direct inspection should test:

- whether folding regulates reading sequence;
- whether writing crosses fold panels;
- whether the current folio numbering flattens a longer original sheet.

This extends Wave 39's distinction between production/form fold and later archival fold.

---

## 13. Original packet/bundle order may be partly recoverable computationally

Potential join fields:

- modern shelfmark;
- modern folio;
- original shipment number;
- bundle number;
- box number;
- historical title on cover;
- language/script of title;
- cover/content relation;
- cross-reference to translation/copy;
- date;
- paper type;
- dimensions where recorded.

### Mechanism

`PRE_1921_ORDER_RECONSTRUCTION_GRAPH`.

### Method

Do not infer adjacency from matching topics alone.

Require one or more historical relation keys:

- same shipment number;
- explicit bundle membership;
- box content list;
- cover text;
- original sequence notation;
- colophon/title relation.

---

## 14. Container fossils reveal archive loss and archive survival simultaneously

The original container relation may be gone:

`bundle physically dismantled`.

Yet metadata survives:

`cover page retained`.

### Mechanism

`RELATION_LOST_METADATA_SURVIVES`.

This parallels other Hodgson mechanisms:

- specimen lost / drawing-number relation survives;
- manuscript segmentation wrong / physical codex survives;
- original paper grouping lost / bundle cover survives.

### Paper-centred formulation

The surviving paper fragment becomes evidence of a relation whose physical embodiment has disappeared.

---

## 15. Archival rebinding creates affordance reversal for cover paper

Before rebinding, a cover page's value is positional:

`it surrounds/precedes a group`.

After rebinding as an internal folio:

- protection/boundary affordance disappears;
- metadata/provenance value can remain or increase for historians.

### Mechanism

`ARCHIVAL_AFFORDANCE_REVERSAL_OF_COVER`.

The same paper shifts from:

`active container boundary`

to

`inactive boundary fossil / provenance evidence`.

This is a particularly clean extension of the project's affordance-reversal argument beyond paper manufacture.

---

## 16. Shipment numbers are historically layered identifiers

The original shipment number on notebook covers has at least two functions:

- route/group objects during transfer;
- later help identify historical grouping after institutional rearrangement.

### Mechanism

`TRANSPORT_IDENTIFIER_TO_PROVENANCE_IDENTIFIER`.

The identifier's function changes over time while the mark remains materially stable.

---

## 17. Article-level claim

**The later archive did not erase Hodgson's earlier paper order completely. When the India Office Library rebound the collection in 1921, original bundles and boxes were dismantled or redistributed, yet their covers, title folios, content pages and shipment numbers often survived as ordinary folios inside new volumes. These displaced boundary sheets are container fossils: paper objects whose protective or grouping function has vanished but whose titles, bundle numbers and content lists still permit the older order to be reconstructed. Archival preservation thus simultaneously destroyed one paper topology and preserved the metadata needed to recover parts of it.**

---

## 18. New mechanism codes

- `CONTAINER_FOSSIL_AS_PROVENANCE_SURFACE`
- `ARCHIVE_GENERATED_SIZE_ORDER`
- `ORIGINAL_BUNDLE_COVER_SURVIVAL`
- `ORIGINAL_BOX_CONTENT_PAGE_SURVIVAL`
- `POSTAL_COVER_SURVIVAL`
- `DISPLACED_BOUNDARY_SURFACE`
- `BOX_CONTENT_METADATA_SURFACE`
- `MULTIPLE_ORIGINAL_GROUP_COVER_SURVIVAL`
- `COVER_CONTENT_METADATA_SURFACE`
- `OLD_GROUPING_TRACE_INSIDE_NEW_VOLUME`
- `ORIGINAL_SHIPMENT_TITLE_FOLIO`
- `BUNDLE_NUMBER_AS_PROVENANCE_KEY`
- `CATEGORY_ON_SHIPMENT_SURFACE`
- `NOTEBOOK_COVER_AS_SHIPMENT_IDENTITY_SURFACE`
- `LOCAL_SCRIPT_PROVENANCE_METADATA`
- `COVER_TITLE_PLUS_TRANSPORT_NUMBER`
- `COVER_AS_RELATIONAL_METADATA_LAYER`
- `SUPERIMPOSED_ARCHIVAL_ADDRESS_SYSTEMS`
- `ORIGINAL_COVER_CATEGORY_VS_LATER_VOLUME_CATEGORY`
- `NOTEBOOK_REVERSE_SIDE_REUSE`
- `LONG_FOLDED_SINGLE_DOCUMENT_STATE`
- `PRE_1921_ORDER_RECONSTRUCTION_GRAPH`
- `RELATION_LOST_METADATA_SURVIVES`
- `ARCHIVAL_AFFORDANCE_REVERSAL_OF_COVER`
- `TRANSPORT_IDENTIFIER_TO_PROVENANCE_IDENTIFIER`

---

## 19. Immediate next tasks

1. Build census of all BL entries described as `cover page`, `title folio`, `original bundle`, `shipment number`, `box content`, `original shipment`.
2. Transcribe visible original shipment numbers from cover images where digitally accessible.
3. Reconstruct box No.3 using f.129v and join its listed contents to present BL folios.
4. Test whether ff.126–128 bundle covers in vol.55 can be matched to present groups through title/category text.
5. Compare original cover categories to 1921 volume subject headings.
6. Record script/language of cover metadata; test whether transport metadata was systematically local-language while later archival metadata became English.
7. Directly inspect the long folded f.59 in vol.60 for fold-reading relation.
8. Separate Hodgson-era/pre-bound notebook reuse from 1921 archive-generated adjacency.
9. Add `historical_container_id` and `container_fossil_type` to paper surface schema.
10. Treat modern folio adjacency as secondary unless historical grouping markers confirm it.

## Bottom line

Wave 41 makes pre-1921 paper order partially reconstructible. The later British Library volumes contain remnants of the containers they replaced: original bundle covers, box-content pages, title folios and notebook covers marked with shipment numbers. These papers no longer perform their original boundary function, yet their metadata makes the earlier grouping visible. Paper therefore survives archival transformation not only as text-bearing content but as the fossilized infrastructure of older containers and routes.