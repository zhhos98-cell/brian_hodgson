# Archive research wave 27 — visual diagnostic schemas, local access, corpus abstraction, and recipient buffering

Date: 2026-08-31

Status: focused deep pass on the long life of Hodgson's Buddhist visual materials. This wave extends Wave 26's `DIAGNOSTIC_ABSTRACTION` mechanism backward to 1827 and forward to the Yule-mediated publication of 1872.

## Executive result

The visual-material corpus now supports a long, source-visible sequence:

`restricted local access -> diagnostic feature schema -> transmitted drawings/images -> extracted comparative symbols -> abandoned/reopened corpus -> later sketch + interpretation -> recipient buffering -> delayed journal publication`

This is important because it shows that a `visual archive` is not one stable collection. The same representational system passes through multiple states and different actors control different transitions.

Three mechanisms are now especially clear:

1. **diagnostic feature schema**: images are made comparable by selecting a finite set of meaningful differences;
2. **access-dependent evidence production**: the schema depends on uneven access to books, ritual specialists, painters and restricted images;
3. **recipient buffering**: a recipient can delay a transmitted item while waiting for a better publication context, then later lower the threshold for release.

---

## 1. August 1827: collecting and transmitting materials is already framed as an infrastructure problem

### Source

Uploaded `书籍 2025年3月28日(OCR)`, reprinting Hodgson's `Sketch of Buddhism, Derived from the Bauddha Scriptures of Nepaul` and extracts of letters to Nathaniel Wallich.

A letter is headed:

`Nepaul, 11th of August, 1827.`

Hodgson says that soon after arriving in Nepal, six years earlier, he began to devise means of procuring accurate information about Buddhism. Formal investigation was outside his official pursuits, but he used his residence in a Buddhist country to **collect and transmit to Calcutta the materials for such investigation**.

### Mechanism

Code:

`MATERIALS_FOR_DISTANT_INVESTIGATION`

The stated goal is not simply personal mastery of Buddhism. Hodgson explicitly constructs a supply of materials that can be investigated elsewhere.

This is a foundational form of the repo's central logic:

`local access -> selected material -> transmission -> distant investigation`

---

## 2. October 1827: local access is staged and socially differentiated

### Source

Same uploaded printed reprint, extract of Hodgson to Wallich dated `Nepaul, 17th October, 1827`.

### Direct evidence

Hodgson rejects a published claim that Jaina statues are naked and Buddhist statues clothed, using newly sent pictures as counter-evidence.

He then describes restricted access to Buddhist esoteric dogmas and symbols. After years of enquiry:

- an old `Vajra Acharya` friend only recently gave him a view of esoteric doctrines;
- his `Chitrakár`, explicitly identified as Buddhist, had only within the preceding twelve months brought him some esoteric pictures;
- a `Bhótiya` had put into his hands a picture containing one of the naked saints;
- his own limited ability to examine Buddhist books helped make this access possible.

### Mechanism

Code:

`ACCESS_DEPENDENT_EVIDENCE_PRODUCTION`

The visual archive is not produced by one collector extracting neutral information from an open field. It depends on differentiated permissions, expertise and trust.

Operational chain:

`restricted doctrine/image -> local specialist/intermediary -> partial disclosure -> Hodgson comparison -> transmitted picture/evidence`

### Source-control consequence

The persons should not be flattened into generic `informants`. Their functions differ:

- ritual/learned access (`Vajra Acharya`);
- visual production/access (`Chitrakár`);
- object/image transfer (`Bhótiya`);
- textual cross-check (Hodgson's book access).

This is a better basis for later collaborator analysis than a broad claim about hidden local labour.

---

## 3. 1827: a finite diagnostic feature schema is explicit

### Source

Extract of a letter from Hodgson to Nathaniel Wallich in the same reprinted corpus.

### Direct statement

Hodgson says that he cannot then describe the significance of all details of the sculptures sent, but that **every part of each image is significant**.

He says the differences among five images are marked by four classes of feature:

1. different positions of the hands, called `mudrá`;
2. different supporters;
3. different cognizances placed between the supporters;
4. where painting/colour is used, different colours.

He then assigns colours to Vairochana, Akshobhya, Ratna-Sambhava, Amitabha and Amogha-Siddha.

### Mechanism

Code:

`DIAGNOSTIC_FEATURE_SCHEMA`

This is stronger and earlier than the Wave 26 code `DIAGNOSTIC_ABSTRACTION`.

The image is converted into a structured comparison object:

`whole image -> hand position + supporter + cognizance + colour -> identity`

### HPS significance

This is a nineteenth-century field-level account of what might now be called feature selection. The historical point is not the modern analogy; it is that Hodgson explicitly reduces the visual comparison problem to a finite diagnostic set while insisting that the full object remains semantically dense.

The source therefore preserves a tension:

- `every part` is meaningful;
- identity can nevertheless be operationalized by selected differences.

That tension should remain visible in the analysis.

---

## 4. The 1827 feature schema is used to correct existing identifications

### Evidence

The October letter uses pictures to reject the naked-Jaina/clothed-Buddhist distinction.

Elsewhere in the reprinted material Hodgson corrects identifications of figures that had been taken for Siva, pointing to Buddhist diagnostic markers such as the small image of Amitabha associated with Padma Pani.

### Mechanism

Code:

`DIAGNOSTIC_REIDENTIFICATION`

The representation is not merely illustrative. It can adjudicate between competing names.

Operationally:

`received/published image -> inspect diagnostic accessory -> compare with schema/text/local report -> reidentify figure`

This anticipates later museum-type and manuscript-catalogue reidentification problems elsewhere in the repo.

---

## 5. 1860: diagnostic features are detached into a portable comparative corpus

### Source

Uploaded `Adobe Scan 2025年3月28日 (3) (1)`, `Notice on Buddhist Symbols`, dated 26 September 1860.

### Operation

The earlier image-level diagnostic logic is expanded into a symbol corpus.

Hodgson describes bringing together:

- symbols from coins;
- symbols from temples;
- statues;
- pictures;
- illuminated manuscripts.

The original purpose was to obtain explanations from learned Saugatas. The explanatory programme was interrupted and apparently never completed.

### Mechanism

Retain:

`DIAGNOSTIC_ABSTRACTION`

with historical genealogy:

`1827 structured feature comparison -> 1860 detached symbol corpus`

The 1860 sheets make diagnostic elements physically portable apart from their source monuments/images.

### Important distinction

`DIAGNOSTIC_FEATURE_SCHEMA` and `DIAGNOSTIC_ABSTRACTION` are related but not identical:

- schema = which features count as differences;
- abstraction = those features are represented separately from the original whole.

---

## 6. 1860–63: the visual corpus acquires an institutional afterlife in France

### Retrospective evidence in uploaded printed material

A later report describes Buddhist drawings made for Hodgson in Nepal, 1824–1843, and presented to the Institute of France in 1860.

The collection is said to have two parts:

1. drawings copied from monuments of sculpture and architecture;
2. original images Hodgson obtained from the hands of believers.

A letter from Professor Weber, Berlin, 24 April 1860, anticipates scholarly use of the pictorial, sculptural and architectural illustrations in Paris.

### Mechanism

Code:

`VISUAL_CORPUS_INSTITUTIONAL_REHOSTING`

The same visual evidence changes operating environment:

`Nepalese production/access -> Hodgson holding -> Institute of France -> external specialist visit/use`

### Source-control note

Exact dates and the distinction between `presented in 1860` and other retrospective donation dates in the larger Hodgson literature should be reconciled separately. The uploaded printed witness is retained as one state, not automatically normalized against other catalogues.

---

## 7. 1870: Hodgson delegates publication discretion with the object

### Source

Uploaded `Adobe Scan 2025年3月28日 (3) (1)`, later printed as `Northern Buddhism`, note by Colonel H. Yule.

Yule states that Hodgson had written to him about two years earlier concerning Yule's paper on the Senbyú Pagoda in Burma and had put into his hands:

- a letter;
- the original sketch;
- authorization to `make what use of them seemed best`.

The excerpt identifies the Hodgson letter as written in 1870 and begins with a sketch of a mutilated figure from Surakarta, identified by Hodgson as Padma Pani.

### Mechanism

Code:

`DELEGATED_PUBLICATION_DISCRETION`

A transmitted knowledge object carries not only content but decision rights.

`author -> sketch + interpretation + permission -> recipient controls next publication state`

This is a different form of circulation from sending a finished article directly to a journal.

---

## 8. 1870–72: Yule deliberately buffers the transmitted item

### Direct evidence

Yule says the letter and sketch had been kept by him since receiving them, in the hope of an opportunity to communicate them to the Society in a **less isolated manner**.

No such opportunity occurred. By 13 September 1872 he judged it desirable not to delay longer and submitted the material, hoping the Society would authorize publication of the drawing with extracts from Hodgson's letter.

### Mechanism

Code:

`RECIPIENT_BUFFERING`

The recipient actively controls time-to-publication according to perceived contextual adequacy.

Sequence:

`receive object -> retain privately -> wait for contextual fit -> contextual fit fails to appear -> delay threshold exceeded -> submit isolated item -> Society decides publication`

### Why this matters

Circulation latency is not reducible to transport time.

An object can arrive safely and remain epistemically dormant because a recipient with publication authority judges the context insufficient.

This is a strong new counterpart to `institutional legibility`:

- legible object may still be withheld;
- the bottleneck can be editorial/contextual rather than linguistic, taxonomic or physical.

---

## 9. Recipient buffering and intermediate-state fixation

Wave 26 showed an author-side failure:

`temporary correction hints -> hurried press transmission -> intermediate state accidentally fixed in print`

Wave 27 adds a recipient-side control:

`finished-enough sketch/argument -> deliberate withholding -> later release`

Together they show that publication timing is governed by multiple control points.

### Proposed broader mechanism

`PUBLICATION_GATEKEEPING_STATE`

Possible states:

- author holds back for deeper investigation;
- author releases because departure makes further delay costly;
- recipient holds back for contextual integration;
- recipient releases because further delay becomes undesirable;
- Society may still authorize or refuse image publication.

This is much more precise than saying communication was `delayed`.

---

## 10. Long visual-knowledge chronology

### 1827

- Hodgson explicitly aims to collect and transmit materials for investigation.
- local access to esoteric images/documents is staged through different people.
- image identity is operationalized via hand positions, supporters, cognizances and colours.

### 1827–1843

- drawings and images accumulate through copying from monuments and acquisition from believers.

### 1860

- visual diagnostics are aggregated into symbol sheets / comparative publication.
- an earlier explanatory project is acknowledged as unfinished.
- larger visual collection enters a French institutional setting.

### 1863 retrospective report

- collection is differentiated by production/provenance class: copied monumental drawings vs original images obtained from believers.

### 1870

- Hodgson sends Yule a sketch and interpretive letter with delegated use permission.

### 1872

- Yule publishes only after a two-year contextual waiting period fails to yield a better integration opportunity.

### Core claim

**The visual archive is a sequence of re-formattings and gatekeeping events, not a stable store of illustrations.**

---

## 11. Implications for the article

The visual case can now perform more than a supporting Buddhist comparison. It supplies mechanisms unavailable in exactly the same form elsewhere:

- differentiated local access;
- feature-schema construction;
- correction by diagnostic accessories;
- detachment of features into comparative sheets;
- provenance-sensitive distinction between copied and acquired images;
- delegated publication rights;
- deliberate recipient-side buffering.

The strongest cross-domain comparison is therefore not `image = specimen` or `image = manuscript`.

It is:

**all domains depend on intermediate surfaces, but each medium generates different control points for what can be selected, compared, transmitted, withheld and reidentified.**

---

## 12. New codes

- `MATERIALS_FOR_DISTANT_INVESTIGATION`
- `ACCESS_DEPENDENT_EVIDENCE_PRODUCTION`
- `DIAGNOSTIC_FEATURE_SCHEMA`
- `DIAGNOSTIC_REIDENTIFICATION`
- `VISUAL_CORPUS_INSTITUTIONAL_REHOSTING`
- `DELEGATED_PUBLICATION_DISCRETION`
- `RECIPIENT_BUFFERING`
- `PUBLICATION_GATEKEEPING_STATE`

Existing codes retained:

- `DIAGNOSTIC_ABSTRACTION`
- `ABANDONED_CORPUS_REACTIVATION`
- `INTERMEDIATE_STATE_FIXATION`

---

## 13. Next falsification targets

1. date and identify the exact Wallich letter containing the four-feature diagnostic schema if the printed sequence does not itself preserve a heading on the same page;
2. map the individual artists/copyists and the surviving drawings to the two 1863 provenance classes;
3. compare the 1860 corrected autograph to the Journal publication and symbol sheets;
4. identify the original 1870 Hodgson-Yule letter/sketch witness, if extant, and compare it with Yule's 1872 extracts;
5. determine whether Yule omitted passages from Hodgson's letter and whether the published drawing reproduces the original sketch directly or through redrawing;
6. test whether publication rights or permission language recurs elsewhere in Hodgson's correspondence;
7. add collaborator roles as operational categories rather than one generic `local collaborator` field.

## Bottom line

The visual corpus now provides one of the repo's clearest long-duration histories of **how a comparison system is built and governed**. The diagnostic categories are explicit by 1827; access to the evidence is socially mediated; the diagnostic marks are later detached into a portable corpus; the corpus is rehosted institutionally; and later individual sketches can be held, contextualized, or released by recipients exercising delegated publication discretion. This is a concrete history of visual knowledge infrastructure rather than a thematic history of Buddhist iconography.