# Archive research wave 29 — shikaree observation, drawing-number addressability, and transfer reconciliation failures

Date: 2026-08-31

Status: deep reconstruction from ZSL archive descriptions/transcriptions, with secondary bibliographical control from Dickinson (2006). Claims are kept at source-state level. Where ZSL public transcriptions disagree, the disagreement is preserved rather than silently normalized.

## Executive result

This wave reconstructs a particularly dense zoological knowledge chain:

`field observation by shikarees -> viva voce statement -> writer translation -> behavioural memorandum -> numbered drawing -> specimen label -> catalogue/list -> container manifest -> institutional receipt`

The same archive also preserves two distinct failure modes:

1. **1837 routing/custody failure**: Hodgson's dispatch claims and the Royal Asiatic Society's receipt state do not match; the RAS recorded that none of the expected sheets/boxes had been received.
2. **1870 sender/receiver manifest mismatch**: Hodgson's sender-side inventory explicitly includes eight unbound Darjeeling volumes of bird-manner notes, but Marshall's attached receipt memorandum omits them.

These cases materially strengthen the repo's central claim that reconstructibility depends on relations being externalized across multiple surfaces, and that each transfer surface can preserve a different state.

---

## 1. The shikaree notebooks are linked to a pre-existing drawing-number namespace

### ZSL archival file

`NZSL/HOD/1/3`

Title:

`Memoranda of manners and habits of birds of my Collection (according to the numbers attached to the drawings). Done by my native sportsmen or Shikarees and translated by my writer`

Date range: 1846–1857.

The ZSL catalogue identifies surviving notebook ranges as:

- No.1 / Vol.1: drawing nos. 1–169;
- No.3 / Vol.3: drawing nos. 340–488;
- No.6 / Vol.6: drawing nos. 755–855.

### Mechanism

Code:

`BEHAVIOURAL_MEMORANDUM_DRAWING_KEY`

The bird's behaviour is not merely written as an independent species account. It is addressable through the **number already attached to the drawing**.

Operational relation:

`drawing number -> bird identity -> behavioural memorandum`

This is a relational key across media.

### Critical point

The title assigns production roles explicitly:

- `native sportsmen or Shikarees`: source of behavioural observations;
- `writer`: translator / textual mediator;
- numbered drawing system: object-keying infrastructure;
- Hodgson collection: receiving/organizing system.

Do not collapse these roles into `Hodgson observed bird behaviour`.

---

## 2. Numbered drawings predate the 1846–57 manners notebooks

### ZSL archival file

`NZSL/HOD/1/6 — Lists of drawings and specimens`, 1835–1838.

The archive description says these contain:

- lists of drawings with **numbers and names of species**;
- `Illustrations of Nepalese zoology`;
- lists of specimens sent home.

### Secondary control

Dickinson (2006) reconstructs that by 1837 Hodgson had assigned **721 numbers** to drawings and specimens.

### Mechanism

Code:

`PREEXISTING_NUMBER_NAMESPACE`

The later manners notebooks therefore do not create a new bird identity system. Behavioural knowledge is inserted into an already existing number namespace.

Sequence:

`numbered drawing/specimen system (at least by 1835–37) -> later shikaree behavioural text keyed to same number`

This temporal ordering matters.

---

## 3. Drawing numbers link specimens to images through paired labels

Dickinson's reconstruction, based on Gray & Gray and surviving specimens, states that Hodgson's specimens originally carried a pair of labels:

1. one label with collection date, locality, and local name;
2. a second label carrying the **drawing number**, normally in red ink.

The same drawing number therefore linked a specimen to a particular visual reference.

### Mechanism

Code:

`CROSS_MEDIA_DRAWING_KEY`

Relation:

`specimen -> drawing-number label -> master/associated drawing`

Together with HOD/1/3:

`specimen <-> numbered drawing <-> translated shikaree manners note`

This is a stronger relation than simple co-occurrence in one collection.

### Caution

A drawing number may identify a species-series relation without proving that the physical specimen and drawing depict the same biological individual.

---

## 4. The number namespace was initially systematic, then became historically accretive

Dickinson argues from Hodgson's sequence that numbering was not simply chronological from the first specimen onward.

A plausible historical sequence is:

- a substantial collection already existed;
- Hodgson imposed a systematic family/genus sequence;
- gaps were filled as new material came in;
- after the initial systematic architecture became saturated, later newly encountered taxa were appended in a more chronological manner.

By late 1843 the count approached 890.

### Mechanism

Code:

`SYSTEMATIC_TO_ACCRETIVE_IDENTIFIER_SHIFT`

An identifier system can change semantics over time while retaining the same visible form.

Early number:

`position within planned classificatory order`

Later number:

`new addition after classificatory sequence has broken down / filled`

This warns against treating numerical order as a single invariant chronology.

---

## 5. 1844: original drawings serve as the master state from which transmission copies were made

### Source

`NZSL/HOD/5/4/8` — Hodgson to J. E. Gray, 27 Dec. 1844.

Hodgson states that, when checking the drawings presented to the British Museum, he referred to:

`my own original drawings from which those ... were copied for transmission to England`.

He then reconstructs the original drawing totals by class.

### Mechanism

Code:

`MASTER_DRAWING_TRANSMISSION_COPY`

The relation is explicit:

`Hodgson master original -> fair/transmission copy -> England`

The drawing collection therefore has copy states analogous to manuscript witnesses.

### Consequence

When a transmitted drawing goes missing, the relation may remain reconstructible because Hodgson retained the original master and numbered catalogues/lists.

This is exactly the redundancy architecture highlighted in Waves 23–24.

---

## 6. Drawing copies were transmitted in regular numerical order

The same 27 Dec. 1844 letter says that a nearly complete series was transmitted to England in **regular numerical order** on the smaller scale of about 20 x 12 inches, with an earlier, ruder, larger-scale series also partly transmitted.

### Mechanisms

Codes:

- `NUMERIC_TRANSMISSION_ORDER`
- `MULTIPLE_DRAWING_SERIES_STATE`

The existence of at least two visual series means that a drawing number, sheet count, physical scale and copy-state must be kept distinct.

A later institution can possess:

- original vs copy;
- old vs new series;
- large vs smaller transmission format;
- present vs missing number.

Do not flatten these into one `drawing collection` state.

---

## 7. 1835: publication planning already treats drawings, specimens and descriptions as one transferable package

### Source

`NZSL/HOD/5/2/1` contains the 23 May 1835 Swainson agreement.

Key operational terms include:

- Swainson may request `Drawings. Specimens, or Descriptions` for an intended atlas;
- duplicate specimens may be given to Swainson;
- original drawings and specimens are to be returned when no longer required;
- Hodgson's names for new species are to be retained;
- nomenclatural errors may be rectified by Swainson;
- each party pays its own postage/parcels.

### Mechanism

Code:

`PUBLICATION_PACKAGE_CUSTODY_CONTRACT`

The publication object is constructed from a **temporary custody bundle** of heterogeneous evidence.

`drawings + specimens + descriptions -> temporary publisher custody -> plate/publication production -> return of originals`

This predates the later British Museum distribution regime and shows that custody and publication were coupled from early in the project.

---

## 8. 1837: Royal Asiatic Society records a routing failure

### Source

`NZSL/HOD/5/2/24 — Extracts from the Minutes of the Committee Correspondence of the Royal Asiatic Society`.

Minute of 7 Nov. 1837 reports Hodgson's statement that he had:

- dispatched to the care of RAS **26 sheets of mammals and birds**;
- intended to continue sending sheets until the series was complete;
- dispatched boxes in January via **Captain Robinson**;
- instructed Robinson to deposit the boxes with RAS **if Hodgson's prior stores had been removed from the keeping of ZSL**.

The RAS minute concludes that **none of the above articles had been received** and the matter was to lie over.

### Mechanism

Code:

`CONDITIONAL_ROUTING_RECEIPT_FAILURE`

The intended route was conditional rather than linear:

`Captain Robinson -> check/assume state of prior ZSL custody -> RAS deposit if condition met`

This makes the custody gap harder to localize after the fact.

### Important source-state conflict

ZSL public transcriptions are inconsistent about the box count:

- some surfaces read **5 boxes**;
- others read **8 boxes**.

Do not choose one until the digital master page is inspected.

Code:

`PUBLIC_TRANSCRIPTION_BOX_COUNT_CONFLICT_5_VS_8`

This is a transcription-state conflict, not yet evidence that Hodgson himself supplied two box totals.

---

## 9. The 1837 failure does not end institutional support for the publication

The same RAS minutes later record:

- 15 Mar. 1838: James Prinsep's communication regarding the Mammalia of Nepal and Bengal Society support; Sir William Jardine expressed willingness to cooperate;
- 19 Apr. 1839: another Prinsep letter recommended seeking support from the Court of Directors;
- 5 Mar. 1842: RAS Council agreed to subscribe to the Mammalia of Nepal publication.

### Mechanism

Code:

`MATERIAL_RECEIPT_FAILURE_WITH_INSTITUTIONAL_SUPPORT_CONTINUITY`

Failure to receive the physical sheets/boxes did not terminate the social/institutional publication network.

This separates:

- object custody;
- publication sponsorship;
- reputation/support.

---

## 10. 1842–43: a second disappearance complaint shows receipt and onward transmission are distinct states

### Source

`NZSL/HOD/5/2/4` — Hodgson to H. Torrens, 12 Jan. 1843.

Hodgson says that on 13 May 1842 he transmitted **31 large sheets of drawings** to Torrens/RAS:

- for Society inspection;
- then for onward transmission to England if deemed proper.

He complains of their **alleged disappearance** despite their **known arrival** with the Society.

### Mechanism

Code:

`RECEIVED_BUT_DOWNSTREAM_STATE_UNKNOWN`

This is a different failure from 1837.

1837:

`sender claims dispatch -> recipient says not received`

1842–43:

`recipient arrival acknowledged/known -> later location/onward movement unexplained`

The two must not be combined into one generic `lost drawings` category.

### List structure

The associated list totals 31 sheets and mixes ethnographic and zoological drawings, showing that one transmission package could cross later disciplinary boundaries.

---

## 11. 1845: some missing drawing sets became effectively unrecoverable

The ZSL HOD/5/4 file sequence records Hodgson asking the British Museum in Feb. 1845 for help recovering a set of mammal drawings from Mr Howard.

The British Museum reply of 4 Mar. 1845 reportedly judged that there was **no realistic chance of recovery from Mr Howard's receiver**.

### Mechanism

Code:

`CUSTODY_CHAIN_TERMINATION`

A numbered master catalogue/drawing system can preserve knowledge that something should exist without guaranteeing the physical recovery of the transmitted copy.

This is a key distinction:

`epistemically reconstructible != physically recoverable`

---

## 12. 1870: Hodgson reconstructs the entire ornithological evidence package for Marshall/Hume

### Source

`NZSL/HOD/5/3/9` — Hodgson to G. F. L. Marshall, 11 Feb. 1870.

Hodgson plans to send a `big deal box` containing four portfolios of drawings and associated evidence for possible use in Hume's projected Indian ornithology.

Sender-side contents include:

1. four portfolios / **1,104 sheets of drawings**;
2. Hodgson's own manuscript list of Nepal birds;
3. his **native painter's Hindi list** of the whole collection including Sikkim;
4. one red-bound volume of manners of birds, made in Nepal by Hodgson's writer from **viva voce statements of his Shikaris**;
5. **eight unbound volumes** of the same type, made at Darjeeling;
6. Hodgson's own manuscript memoranda from the Sikkim Tarai in 1846;
7. London and Calcutta printed catalogues/reprints;
8. other authorial printed papers.

### Mechanism

Code:

`MULTI_LAYER_ORNITHOLOGICAL_EVIDENCE_PACKAGE`

This is unusually explicit division of epistemic labour:

- shikaris: oral behavioural observation;
- writer: textual translation/recording;
- native painter: Hindi collection list;
- artists: drawings;
- Hodgson: manuscript list, Tarai memos, classification/publication layer;
- printed catalogues: prior institutional/public states.

The `big deal box` is therefore not merely transporting images. It carries a **portable relational database in heterogeneous media**.

---

## 13. 1870: sender manifest and receiver memorandum do not close

Immediately after Hodgson's letter, the archive preserves a Marshall memorandum acknowledging receipt.

The memorandum lists:

- 1,104 drawing sheets;
- Hodgson's manuscript list;
- native painter's Hindi list;
- one red-bound Nepal manners volume;
- Hodgson's Sikkim Tarai memos;
- London catalogue copies;
- Calcutta reprints;
- other printed papers.

But the sender letter's **eight unbound Darjeeling manners volumes are absent from the receiver memorandum**.

### Mechanism

Code:

`SENDER_RECEIPT_MANIFEST_MISMATCH`

Do not infer physical loss yet.

Possible states include:

- omitted from Marshall's receipt description;
- incorporated under another item without explicit wording;
- not sent despite being intended;
- sent separately;
- physically absent.

The archive presently supports only the mismatch.

### High HPS value

This is a direct same-transfer comparison between:

`intended sender state` and `acknowledged receiver state`.

It is therefore one of the strongest reconciliation surfaces in the whole Hodgson corpus.

---

## 14. The 1870 package preserves several competing list authorities

The transfer simultaneously contains:

- Hodgson's own Nepal bird list;
- native painter's Hindi whole-collection list;
- shikaree-derived manners texts;
- Hodgson's field memos;
- printed catalogues.

### Mechanism

Code:

`PARALLEL_METADATA_AUTHORITIES`

There is no single master textual representation of the bird collection.

Different surfaces encode different relations:

- taxonomic/collection identity;
- vernacular/Hindi naming;
- behaviour;
- field observations;
- printed nomenclature;
- visual morphology.

The collection is operable because these surfaces can be related, not because one replaces all others.

---

## 15. Drawing number is the infrastructural join, not necessarily the taxon name

The evidence now suggests a major reframing for the natural-history section.

Scientific names could change, Hodgson himself could revise classifications, and British Museum catalogues could lump species in ways he disputed.

The more stable operational relation was often the Hodgson drawing number.

### Join graph

`local observation / shikari statement`

`-> writer translation`

`-> manners memorandum`

`-> Hodgson drawing number`

`<-> drawing`

`<-> specimen label`

`<-> species/local-name/locality metadata`

`<-> catalogues and distribution lists`

### Mechanism

Code:

`RELATIONAL_IDENTIFIER_OVER_NAME_STABILITY`

The identifier can preserve relations across nomenclatural change.

### Limit

Dickinson also notes that Hodgson sometimes reused the same drawing number across multiple taxa/specimens. The key is powerful but not infallible.

---

## 16. New general claim: local behavioural knowledge was made transportable through addressability

A narrow collaborator-history reading would say that shikarees supplied knowledge later credited to Hodgson.

The material archive supports a more operational claim:

**viva voce field knowledge became institutionally movable when translated into a written memorandum and keyed to a numbered visual/specimen system.**

The important conversions are:

`oral -> written`

`vernacular/field -> translated textual record`

`behaviour -> numbered species/object relation`

`local notebook -> portable box/portfolio package`

`working archive -> prospective external publication`

This does not erase the asymmetry of authorship/credit. It specifies the mechanism through which local knowledge could enter the distributed collection.

---

## 17. Cross-wave synthesis

Wave 29 makes several earlier mechanisms more precise.

### Error-control redundancy

The master original, transmission copy, specimen label, numbered list and manners notebook preserve overlapping relations.

### Reconciliation surface

1837 RAS minutes and 1870 Marshall receipt compare expected/intended vs acknowledged states.

### Intermediate-state fixation

A receipt can omit an intended component; the resulting incomplete metadata may become the surviving institutional state.

### Future-operation reserve

The 1870 box was assembled specifically so another ornithological project could reuse the materials.

### Institutional legibility

Shikaree observation became legible to later users because it had been translated, written, numbered and packaged with cross-reference objects.

### Relational addressability

The Hodgson number links multiple media despite physical separation.

---

## 18. New mechanism codes

- `BEHAVIOURAL_MEMORANDUM_DRAWING_KEY`
- `PREEXISTING_NUMBER_NAMESPACE`
- `CROSS_MEDIA_DRAWING_KEY`
- `SYSTEMATIC_TO_ACCRETIVE_IDENTIFIER_SHIFT`
- `MASTER_DRAWING_TRANSMISSION_COPY`
- `NUMERIC_TRANSMISSION_ORDER`
- `MULTIPLE_DRAWING_SERIES_STATE`
- `PUBLICATION_PACKAGE_CUSTODY_CONTRACT`
- `CONDITIONAL_ROUTING_RECEIPT_FAILURE`
- `PUBLIC_TRANSCRIPTION_BOX_COUNT_CONFLICT_5_VS_8`
- `MATERIAL_RECEIPT_FAILURE_WITH_INSTITUTIONAL_SUPPORT_CONTINUITY`
- `RECEIVED_BUT_DOWNSTREAM_STATE_UNKNOWN`
- `CUSTODY_CHAIN_TERMINATION`
- `MULTI_LAYER_ORNITHOLOGICAL_EVIDENCE_PACKAGE`
- `SENDER_RECEIPT_MANIFEST_MISMATCH`
- `PARALLEL_METADATA_AUTHORITIES`
- `RELATIONAL_IDENTIFIER_OVER_NAME_STABILITY`

---

## 19. Immediate falsification / archive targets

1. Inspect the digital master of `NZSL/HOD/5/2/24` to resolve whether the original minute says 5 or 8 boxes.
2. Inspect all surviving `NZSL/HOD/1/3` notebook pages to determine the actual field structure of the shikaree/writer memoranda: whether each entry carries drawing number, species name, locality, season, sex, nesting, food, voice, etc.
3. Recover Vols. 2, 4, 5 and the eight unbound Darjeeling volumes if they survive under another arrangement/shelfmark.
4. Compare Marshall's 1870 sender and receiver lists at image level to exclude catalogue-transcription omission.
5. Search later Hume/Marshall correspondence for explicit mention or return of the eight Darjeeling volumes.
6. Reconstruct the 1835–38 `HOD/1/6` numbered drawing lists and test continuity with the later HOD/1/3 number ranges.
7. Map surviving original specimen labels at Cambridge / other institutions against ZSL drawing numbers.
8. Distinguish Hodgson master original, fair/transmission copy, British Museum drawing number and later institutional accession number.
9. Build a network of 1837 conditional routing: Hodgson -> Captain Robinson -> ZSL/RAS conditional custody -> later known holdings.
10. Separate the 1837 `not received` event from the 1842–43 `arrived then disappeared` event in all future narrative.

## Bottom line

Wave 29 exposes the natural-history archive as a deliberately cross-keyed evidence system. Behavioural knowledge supplied orally by shikarees was translated by a writer and attached to the same number namespace that linked drawings, specimen labels and catalogues. The master drawings generated transmission copies; lists and manifests attempted to preserve relations during movement. The surviving failures are correspondingly precise: a conditional routing chain could terminate in `not received`; a received set could later become unlocatable; and a sender's 1870 manifest could preserve eight volumes that the receiver's acknowledgment does not name. These are not peripheral archival accidents. They are direct evidence of how Hodgson's distributed zoological knowledge was made usable, and of where that usability could fail.