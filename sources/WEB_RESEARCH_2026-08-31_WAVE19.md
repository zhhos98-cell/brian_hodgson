# Web research wave 19 — zoological metadata, distributed specimen identity, and list maintenance, 1843–1846

Date: 2026-08-31

Status: cross-domain calibration wave. Core evidence comes from the ZSL Hodgson correspondence catalogue/transcriptions, the 1846 British Museum catalogue, and later reconstruction of Hodgson's original paired-label system. This wave asks whether manuscript `operational metadata` has a genuinely comparable zoological counterpart.

## 1. Yes: zoological incorporation is also a metadata pipeline, but its fields and failures differ

The British Museum processing of Hodgson's collection in 1845 exposes a sequence:

**box receipt → unpack/examine → identify/name → assess completeness/condition → retain representative series → separate duplicates → allocate distribution sets → update lists → compile detailed catalogue.**

This is structurally comparable to manuscript institutionalization without assuming that manuscripts and specimens are the same kind of object.

Primary institutional witness:
ZSL Hodgson archive, especially `NZSL/HOD/5/2/15` and `/16`.

Catalogue/transcription search pages:
https://zsl-archive.maxarchiveservices.co.uk/index.php/informationobject/browse?media=print&names=8774&places=61164&showAdvanced=1&sort=referenceCode&sortDir=asc&topLod=0

---

## 2. 6 February 1845: list inspection reveals state-dependent invisibility

J. E. Gray tells Hodgson that while looking over the bird list he noticed a Tibetan pheasant had not been marked because it was **at the stuffer's when the list was being prepared**, and therefore escaped the list.

He also says they had not received full specimens of the Ganges Pelican, only a head.

### Mechanism

The catalogue/list is generated from an institutionally available object state.

An object can be physically within the broader institutional workflow yet absent from the list because it is temporarily:

- at the taxidermist/stuffer;
- elsewhere for preparation;
- represented only by a partial body;
- not yet reconciled with the incoming list.

This is the zoological analogue of `receipt ≠ item-level incorporation`.

### New failure mode

`PROCESS_STAGE_VISIBILITY_FAILURE`:

**object temporarily in another processing node → omitted from current inventory/list.**

Do not infer historical non-arrival from absence in one catalogue state.

---

## 3. Partial object changes what counts as a specimen

Gray says the Ganges Pelican was represented only by a head.

This creates a counting/identity problem distinct from manuscript segmentation:

- taxon/species identity may be represented;
- a complete specimen is absent;
- a body part remains an evidential object;
- collection count can depend on whether head/skull/skin/skeleton is counted as specimen, osteological unit or partial object.

### Schema consequence

For zoological records distinguish:

- `organism_instance`;
- `prepared_specimen_unit`;
- `body_part_unit`;
- `skin`;
- `skull`;
- `skeleton`;
- `horn`;
- `drawing_representation`.

Do not collapse these under one `specimen` count when reconstructing historical totals.

---

## 4. Condition determines institutional usability

Gray reports numerous bird specimens in such poor condition that they were not useful to anyone and asks Hodgson what should be done with them.

The 13 February letter similarly says a group of 52 birds were apparently misnamed/unnamed and therefore of comparatively little use.

### Analytical point

Possession is not enough. Zoological usefulness depends jointly on:

- physical condition;
- adequate naming/identification;
- comparison readiness;
- relation to lists/drawings;
- intended recipient/use.

This is a close cross-domain parallel to the manuscript distinction between physical custody and semantic addressability.

### Two independent axes

A specimen can fail institutionally because:

1. **material failure** — damaged, partial, imperfect;
2. **metadata failure** — unnamed, misnamed, detached from identifying relations.

These should be coded separately.

---

## 5. Detailed catalogue = retrospective incorporation of a temporal accession stream

On 6 February Gray says the catalogue being prepared would contain a **detailed list of every specimen received from Hodgson between 1840 and the present**.

This means the 1846 catalogue is not simply a snapshot of one shipment. It is a retrospective attempt to consolidate multiple accession/transfer events into one published descriptive state.

### Version rule

For every catalogue entry distinguish:

- specimen collection date if known;
- dispatch/shipment date;
- receipt/accession date;
- preparation/identification date;
- catalogue compilation date;
- publication date.

A catalogue dated 1846 can describe specimens received across several preceding years.

---

## 6. Distribution metadata is written back into lists

Gray sends Hodgson a mammal list showing how mammals and bones had been distributed. He asks to borrow the bird list for a day so that **later distributions could be added to it**.

This is crucial.

The list is not a static descriptive inventory. It is a mutable operational ledger whose fields change after redistribution.

### Mechanism

**specimen identity + distribution destination + current institutional state** are synchronized by list maintenance.

The same type of document can therefore function sequentially as:

- receipt/inventory list;
- reconciliation device;
- distribution ledger;
- source for printed catalogue.

### New relation

`LIST_STATE_UPDATED_BY_EVENT`.

Catalogue/list versions need event dates rather than one timeless `list` entity.

---

## 7. 13 February 1845: unpacking becomes set construction

Gray reports that boxes of birds had been examined and divided into four collections:

- British Museum — 352 specimens;
- Collection No. 1 — 140;
- Collection No. 2 — 79;
- Collection No. 3 — 40;
- plus 52 problematic unnamed/misnamed birds.

He asks Hodgson to specify the recipients of Series 1, 2 and 3.

### Analytical importance

The Museum does not simply receive a collection and then give away leftovers. It **manufactures duplicate/distribution sets** after examination.

This requires decisions about:

- which specimen constitutes the Museum's reference series;
- what counts as duplicate;
- quality/condition;
- completeness;
- recipient priority;
- metadata sufficient for the duplicate to remain useful elsewhere.

### Count ontology

`incoming boxes` → `examined specimens` → `retained reference series` + `distribution series` + `problematic residuals`.

These are different count states generated by institutional processing.

---

## 8. Reference-series construction privileges completeness across anatomical forms

Gray says he kept a complete series of skulls and horns of Mammalia and bones of birds for the Museum, while more or less imperfect mammal skeletons were not yet dealt with.

This shows that `complete series` is not simply taxonomic representation by skin. Institutional completeness can be distributed across anatomical preparations:

- skins;
- skulls;
- horns;
- bones;
- skeletons.

### Mechanism

The Museum constructs an evidentiary collection by selecting **complementary material states**.

This is comparable to Hodgson's distributed text-image systems but should not be treated as identical. The important common mechanism is relational assembly:

**one taxonomic claim may depend on several physically separate representation/preparation forms.**

---

## 9. Hodgson's original label system was explicitly relational

Modern historical reconstruction drawing on Gray & Gray and surviving evidence describes Hodgson specimens as originally carrying paired labels:

1. one label with collection date, locality and local name;
2. a second label with the corresponding drawing number, written in red ink.

The drawing number related specimen to Hodgson's numbered visual series.

Secondary synthesis:
Dickinson, `An introduction to the bird collections of Brian Houghton Hodgson`, *Zoologische Mededelingen* 80 (2006).

Public searchable version:
https://www.researchgate.net/publication/228490048_Systematic_notes_on_Asian_birds_52_An_introduction_to_the_bird_collections_of_Brian_Houghton_Hodgson_1801-1894

### Metadata architecture

The original specimen identity system distributed information across two labels:

**label A:** date + locality + vernacular/local name;

**label B:** drawing number;

and a separate drawing/notebook system supplied additional representation/description.

This is not one self-contained label. It is a relational metadata package.

---

## 10. Label removal is therefore relational data loss, not cosmetic relabelling

Later British Museum practice removed Hodgson's original labels. Because those labels carried date/locality/local name and drawing-number relations, removal can destroy more than provenance wording.

Potential losses include:

- collection date;
- exact locality;
- local/collector name;
- specimen ↔ drawing linkage;
- ability to reconstruct Hodgson's original numbering context.

### Important distinction

The specimen can remain physically preserved while its **relational resolution** decreases.

This strengthens the repo's existing distinction:

**physical preservation ≠ relational preservation.**

---

## 11. Drawing numbers are interoperability keys

Hodgson's numbering system linked:

- specimens;
- drawings;
- notebooks/descriptions;
- later printed names/catalogues.

Modern type research notes that Hodgson's 1844 catalogue contained names linked by numbers to unpublished drawings and specimens.

### Mechanism

The number acts like a cross-media foreign key.

But Wave 11 already shows that such numbers can collide or diverge from copied names. Therefore code number performance empirically:

- unique/stable;
- reused;
- copied incorrectly;
- label detached;
- drawing missing;
- name-number divergence;
- reconstructed from secondary evidence.

The existence of a number does not guarantee auditability; auditability depends on whether the relation survives.

---

## 12. 1846 catalogue as a transformation, not merely publication

The British Museum's *Catalogue of the Specimens and Drawings of Mammalia and Birds of Nepal and Thibet* was printed by order of the Trustees in 1846.

Public bibliographic/full-text controls:
- Biodiversity Heritage Library: https://www.biodiversitylibrary.org/item/77056
- Google digitization / public-domain copies also survive.

Its later appearance as a recognized British Museum catalogue helps stabilize Hodgson's collection in institutional/taxonomic form.

But the letters show the process behind the finished volume:

- recover material from different locations;
- inspect boxes;
- note omissions;
- identify problematic specimens;
- compare specimens;
- divide duplicates;
- update distribution lists;
- recover drawings;
- compile specimens received across years.

The printed catalogue is therefore the end-state of an extended reconciliation workflow.

---

## 13. Direct cross-domain comparison with the manuscript metadata regime

### Manuscript survey, 1868–71

Operational fields include:

- number;
- original-script title;
- Roman title;
- subject/author;
- pages;
- lines/page;
- substance/support;
- script;
- location/owner;
- accuracy/peculiarities.

### Hodgson zoological system / British Museum incorporation

Operational fields/relations include:

- specimen/drawing number;
- taxonomic or local name;
- collection locality;
- collection date;
- anatomical/preparation state;
- physical condition/completeness;
- drawing relation;
- retained vs duplicate status;
- distribution destination;
- current list/catalogue state.

### Shared mechanism

Both regimes make physically distant objects actionable by preserving selected relations.

### Non-equivalence

Manuscript cataloguing must solve textual segmentation and title/copy identity.

Zoological cataloguing must solve organism/specimen/preparation identity, anatomical completeness, taxonomic naming and duplicate-set construction.

The comparison works precisely because the failure modes differ while the infrastructural problem — **maintaining identity across separation** — is shared.

---

## 14. New cross-domain variable: addressability vector

Instead of one binary `catalogued/not catalogued`, record several addressability dimensions.

### Manuscript

- physical location addressable?
- title addressable?
- script/transliteration addressable?
- textual boundaries addressable?
- support/copy state addressable?
- owner/provenance addressable?

### Zoological specimen

- physical storage addressable?
- taxonomic identity addressable?
- locality/date addressable?
- drawing number addressable?
- preparation/body-part relation addressable?
- duplicate/distribution history addressable?

This permits historically specific comparison without flattening the domains.

---

## 15. New failure taxonomy from the cross-domain comparison

Add:

- `PROCESS_STAGE_VISIBILITY_FAILURE` — object omitted because temporarily at another preparation/processing node;
- `PARTIAL_OBJECT_STATE` — only head/skull/skin/etc. survives or was received;
- `MATERIAL_USABILITY_FAILURE` — physical condition makes object unsuitable for distribution/comparison;
- `METADATA_USABILITY_FAILURE` — unnamed/misnamed/detached identifier makes object of limited use;
- `DISTRIBUTION_LEDGER_DRIFT` — physical redistribution occurs without synchronized list update;
- `RELATIONAL_LABEL_LOSS` — original label removal destroys cross-object/media relations;
- `DUPLICATE_SET_CONSTRUCTION` — institutional event creating new collection subsets from incoming material;
- `REFERENCE_SERIES_SELECTION` — retained institutional series is actively constructed rather than simply equal to first receipt.

These complement manuscript-specific `FALSE_LUMP`, `FALSE_SPLIT` and `UNDERDESCRIBED_COMPOSITE`.

---

## 16. This is now a good archive-upload threshold

After Waves 17–19, the public-source structure is sufficiently mature to guide archival ingestion.

The next archival upload should be read against explicit tests rather than general themes.

### Highest-value archival object types

1. original specimen lists / distribution tables;
2. labels or label transcriptions;
3. drawings bearing Hodgson numbers;
4. manuscript lists with leaves/verses/price/support fields;
5. working catalogue forms / proofs / corrections;
6. packing lists tied to boxes/bundles;
7. bills joining paper, labour and transport;
8. correspondence explicitly correcting a number/name/location or reporting a missing/partial object.

### Questions we can now ask immediately of every uploaded item

- what historical unit is being counted?
- what metadata fields are present/absent?
- what downstream operation is the record intended to enable?
- which object relations are carried on the sheet/label/list and which are external?
- what version/state of the collection does it describe?
- does it expose a failure or reconciliation event?
- can it link transport identity to later institutional identity?

This is a much higher-yield archival reading protocol than thematic extraction.

---

## Bottom line

The zoological evidence confirms the cross-domain hypothesis at mechanism level. Gray's 1845 letters show specimen incorporation as a mutable data workflow: list inspection reveals a pheasant omitted because it was at the stuffer; partial specimens and poor condition complicate counts; unnamed/misnamed objects have reduced institutional usefulness; unpacked boxes are actively divided into Museum and duplicate series; distribution events are written back into lists; a retrospective catalogue consolidates specimens received across several years. Hodgson's paired labels and drawing numbers then add a relational identity architecture linking specimen, date, locality, local name and visual witness. Manuscripts and zoological specimens require different metadata, but both become institutionally usable only when selected relations remain addressable after movement.
