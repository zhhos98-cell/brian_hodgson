# Archive research wave 30 — distributed zoological production, working/finished drawing states, and independent metadata failure channels

Date: 2026-08-31

Status: synthesis from ZSL archival transcriptions/descriptions, Hodgson's 1835 production protocol as quoted from the Johnstone correspondence in later scholarship, ZSL modern collection descriptions, and source-controlled secondary reconstruction. Actor attributions are separated by confidence level.

## Executive result

Wave 29 reconstructed the relation graph linking shikaree observation, writer translation, numbered drawings, specimen labels, catalogues and transfer surfaces. Wave 30 asks how the underlying zoological evidence was actually produced.

The answer is a distributed, parallel workflow rather than a single-author sequence:

`fresh/live specimen`

`-> artist visual measurement / repeated correction / anatomical delineation`

`-> Hodgson anatomical, dietary and classificatory notes`

`-> shikaree field observation where direct observation was impossible or insufficient`

`-> writer translation / memorandum`

`-> drawing number and local-name metadata`

`-> rough/master drawing state`

`-> finished/transmission drawing state`

`-> institutional catalogue / distribution / publication`

Two further findings substantially sharpen the repo's error model:

1. **working and finished visual states were historically explicit**: Hodgson distinguished original rough drawings and notes, needed to continue research, from a finished series intended for institutional custody;
2. **names and numbers fail independently**: J. E. Gray could report a list whose numbers were correct while names were corrupted by a copier, while simultaneously fearing that bird specimens themselves carried erroneous/reused numbers.

The resilience of the system therefore lies in overlapping metadata surfaces, not in any single uniquely trustworthy identifier.

---

## 1. 1833–35: zoological drawing was continuous skilled labour, not occasional illustration

### 1833 household letter

Hodgson wrote to his sister Fanny that he had **three native artists always employed in drawing from nature** and that his drawings already numbered about two thousand.

This is retrospective/published through Hunter and Waterhouse rather than an archival original currently inspected in this wave, so it is used as a labour-scale witness rather than verbatim production metadata.

### 1835 Johnstone correspondence

A later transcription/quotation of Hodgson's letter to Sir Alexander Johnstone gives a much more detailed production protocol.

Hodgson describes:

- a series of drawings, birds at natural size;
- **two native artists**;
- training in the strict observance/delineation of `significant parts`;
- several hundred drawings;
- almost every subject repeatedly corrected from **fresh specimens**;
- mature colour and figure;
- sexual differences;
- differences caused by nonage;
- characteristic external and internal structures separately delineated;
- use of a camera/camera lucida for rigid accuracy in some cases;
- repeated supervisory recall to relevant characters where the optical device was not used.

### Mechanisms

- `CONTINUOUS_ARTIST_LABOUR`
- `SPECIMEN_CORRECTED_VISUAL_STATE`
- `DIAGNOSTIC_FEATURE_TRAINING`
- `SEX_AGE_VARIANT_CAPTURE`
- `OPTICAL_ACCURACY_ASSIST`

### Important analytical point

The image is an accumulated corrected state, not one observational event.

`fresh specimen A -> drawing state 1`

`fresh specimen B -> correction`

`additional age/sex specimen -> further correction`

`anatomical structure -> additional figure`

The resulting sheet can therefore aggregate several biological individuals and observational moments.

Do not infer `one drawing = one specimen`.

---

## 2. The same specimen source was processed in parallel by artists and Hodgson

The 1835 production account states that while fresh specimens were being used by the painters, Hodgson himself drew from the same source notes on:

- stomach/intestine structure;
- food as indicated by stomach contents;
- habits;
- manners;
- location;
- economy;
- observation or report.

### Mechanism

Code:

`PARALLEL_SPECIMEN_PROCESSING`

The workflow is not:

`Hodgson studies specimen -> artist illustrates Hodgson's result`.

It is closer to:

`fresh specimen -> parallel visual and textual extraction streams`.

The streams can later be joined by species identity / drawing number.

### Why this matters

The scientific object is assembled from distinct labour streams that can be separated physically:

- image;
- anatomical figure;
- measurement;
- stomach/anatomy memo;
- field-behaviour account;
- vernacular name;
- specimen.

This explains why later loss of one component need not destroy the entire informational relation.

---

## 3. Campbell supplied another anatomical expertise layer

Waterhouse's reconstruction notes that Archibald Campbell, Residency surgeon and later Superintendent at Darjeeling, assisted in the study and description of specimen anatomy.

### Mechanism

Code:

`MEDICAL_ANATOMICAL_COLLABORATION`

This should be kept separate from:

- artist anatomical drawing;
- Hodgson's stomach/intestine notes;
- shikaree behavioural reports.

The zoological knowledge system had multiple expert roles even before institutional experts in Britain entered the chain.

---

## 4. ZSL surviving drawings are composite metadata surfaces

ZSL's current collection descriptions report that a typical Hodgson drawing includes:

- Hodgson's unique species/reference number;
- scientific name;
- common/local names;
- locality;
- sometimes Devanagari text;
- multiple anatomical figures;
- notes on recto/verso;
- measurement and weight tables.

### Mechanism

Code:

`DRAWING_AS_COMPOSITE_METADATA_SURFACE`

The drawing sheet is not merely a pictorial representation. It can combine:

`image + identifier + naming + locality + vernacular/script layer + anatomical decomposition + quantitative measurement`.

This makes the sheet itself a relational hub.

### Source-control limit

ZSL's modern description does not by itself identify which historical actor entered every field.

Do not attribute all Devanagari, measurements or local names automatically to the painter or automatically to Hodgson.

Actor-level palaeographic comparison remains required.

---

## 5. Probable artist measurement layer — high-value but not yet primary-proven

A later close-reading of plates reports tables of measurements on the backs of sheets and argues that these were made by the artist to construct scale; English equivalents appear to be a separate translation/transcription layer.

This interpretation is plausible and consistent with the 1835 production protocol, but has not yet been established by a signed, actor-explicit primary sheet in the current research pass.

### Code

`PROBABLE_ARTIST_MEASUREMENT_LAYER`

### Confidence

`MEDIUM_HIGH_SECONDARY_INFERENCE`

### Research rule

Use the stronger claim only after locating:

- a signed Rajman/Tursmoney drawing;
- non-English measurement table;
- identifiable handwriting relation between table and artist signature/drawing hand;
- English translation in a distinct hand.

Until then, write:

`measurements were integrated into the drawing-production surface; some scholarship attributes the original measurement layer to the artists`.

---

## 6. Rajman Singh and Tursmoney Chittakar are secure named artist nodes, but most production remains anonymous

ZSL identifies:

- **Rajman Singh** as a major artist in the mammal volumes who also accompanied Hodgson to Darjeeling;
- **Tursmoney Chittakar** as another named artist, attested by at least one signed watercolour.

ZSL also notes that most artist names have been lost.

### Mechanisms

- `NAMED_ARTIST_NODE`
- `ANONYMOUS_ARTIST_MAJORITY`

### Source-control rule

Do **not** identify the 1870 `native painter's Hindi list` as Rajman Singh merely because Rajman was Hodgson's best-documented painter and worked at Darjeeling.

Current evidence supports:

`native painter's Hindi list -> artist-role node`

not:

`native painter's Hindi list -> Rajman Singh`.

The same caution applies to `my writer` and individual shikarees in the 1846–57 manners notebooks.

---

## 7. Fieldworkers were sometimes explicitly substitutes for Hodgson's direct observation

ZSL's current interpretation of the Bengal florican material states that Hodgson paid fieldworkers to observe birds on his behalf because restrictions on his movement prevented him from observing these birds directly in the wild.

### Mechanism

Code:

`DELEGATED_FIELD_OBSERVATION`

This is stronger than a generic claim that local hunters supplied specimens.

The fieldworker's operation can be:

`observe living animal behaviour unavailable to Hodgson -> report -> enter translated/numbered knowledge system`.

This fits the HOD/1/3 title assigning manners/habits to shikarees.

---

## 8. Artist and shikaree roles should remain analytically distinct

Some later commentary has suggested that habitat/general behaviour on plates might reflect intimate knowledge of artist or hunter. Other specialist commentary explicitly distinguishes artist and hunter as different people/roles.

The primary archive already supports a differentiated model:

- artist: visual representation / repeated specimen correction;
- shikaree: manners/habits oral knowledge;
- writer: translation/textual record;
- Hodgson: parallel anatomy/food/classification/field notes and supervisory/organizational work.

### Mechanism

Code:

`ROLE_DIFFERENTIATION_BEFORE_ATTRIBUTION`

Do not use visual-sheet metadata alone to merge these functions.

---

## 9. A Newar `Chitrakar` can function as a knowledge intermediary beyond drawing

The Cambridge Hodgson-paper inventory notes a Newar customs manuscript beginning with the phrase `mārphat Citrakāra`, literally `through a Chitrakar`, and observes that Hodgson's official painter was Rajman Singh, though the specific mediator is not proven to be Rajman.

### Mechanism

Code:

`CHITRAKAR_AS_MEDIATION_ROLE`

This is useful comparatively because it shows that the occupational/caste role `Chitrakar` can appear in the documentary archive not only as visual executor but as an intermediary through whom ethnographic knowledge is obtained.

### Caution

Do not transfer this identity automatically to zoological Hindi-list authorship.

It establishes role permeability, not a specific actor join.

---

## 10. 1844 explicitly separates original/working drawings from finished/institutional drawings

### Source

`NZSL/HOD/5/4/3`, Hodgson to Trustees of the British Museum, 15 Dec. 1844.

Hodgson says that because his immediate return to India had been decided, he wanted to:

- **carry back his original Drawings**;
- carry back his **Notes and Memoranda**;
- leave only his **finished series of drawings**;
- leave the specimens with the Museum for appropriation/distribution.

He explains that the originals and notes were required so that he could resume and complete research rapidly in India.

### Mechanism

Codes:

- `WORKING_ORIGINAL_VS_FINISHED_SERIES`
- `GENERATIVE_STATE_RETENTION`
- `INSTITUTIONAL_FINISHED_STATE`

### Operational distinction

`original rough drawing + notes = generative research state`

`finished drawing = transferable/institutional use state`

The same visual subject can therefore have distinct documentary functions by copy state.

---

## 11. British Museum was asked to complete the finished series from Hodgson's rough originals

Another version/proposal in the same 1844 negotiation states:

- the finished series was not quite complete;
- the Museum should appoint an artist;
- that artist should complete the finished series from Hodgson's **original rough drawings**;
- the existing finished series had itself been copied from those originals.

### Mechanism

Code:

`INSTITUTIONAL_COPY_COMPLETION_FROM_MASTER`

The copy relation is not merely:

`master -> one fair copy`.

It is potentially:

`rough/master state -> existing finished copy series -> institutional artist fills missing finished states from master`.

This resembles a manuscript exemplar used to generate replacement/fair copies.

---

## 12. 1844–45 master retention explains how missing transmission states could be audited

Hodgson's later December 1844 comparison of his originals against material transmitted to England now reads differently.

Because the original rough/master drawings remained available as a generative reference state, he could reconstruct:

- how many drawings should have existed;
- which series had been transmitted;
- what copy series was incomplete;
- what had failed to reach or remain at institutions.

### Mechanism

Code:

`MASTER_STATE_AS_AUDIT_REFERENCE`

This is the visual equivalent of the numbered catalogue as checksum.

---

## 13. Names and numbers have independent failure channels

### Source

`NZSL/HOD/5/2/27`, J. E. Gray to Hodgson, undated.

Gray states that a list sent to Hodgson was:

- **correct in the numbers**;
- names `ludicrously wrong`;
- name corruption attributed to the `ignorance of the copyer`;
- expected to be corrected after Hodgson returned the list.

In the same letter, Gray separately says he fears **many errors in the numbering of the birds**, noting that two very different kinds have the same number.

### Mechanisms

- `COPIER_NAME_CORRUPTION_WITH_NUMBER_PRESERVATION`
- `SPECIMEN_NUMBER_COLLISION`
- `INDEPENDENT_METADATA_FAILURE_CHANNELS`

### High-value implication

The archive directly prevents a simplistic hierarchy:

`number > name`.

Instead:

- copy event may preserve number and corrupt name;
- specimen/label event may corrupt/reuse number;
- taxonomic revision may alter scientific name while leaving local/drawing relations intact.

Reliability comes from **cross-checking independent fields and surfaces**.

---

## 14. Sorting is required before names can stabilize

In the same Gray letter, new species could not be described until the entire collection had been sorted so that old and new could be compared.

### Mechanism

Code:

`SORTING_BEFORE_NOMENCLATURAL_STABILIZATION`

Scientific naming is downstream of collection-level comparison, not simply attached at point of capture.

Operational order:

`received collection -> unpack/sort -> compare old/new -> stabilize identification/name -> distribute duplicates`.

This reinforces the repo's claim that institutional handling is an epistemic stage.

---

## 15. Distribution began while metadata was still unstable

Gray's letter simultaneously discusses:

- sorting specimens into British Museum and multiple duplicate collections;
- names still being finished;
- wrong names from a copier;
- feared numbering collisions.

### Mechanism

Code:

`DISTRIBUTION_DURING_METADATA_INSTABILITY`

Objects could become geographically distributed before their descriptive metadata had stabilized.

This creates a historical mechanism for later cross-institutional divergence:

`same source collection -> different destination -> local copy/list/label state -> later inconsistent identity`.

---

## 16. Working drawings and institutional drawings encode different epistemic affordances

The archive now permits a precise distinction.

### Original/rough/master state

Affordances:

- revision from new specimens;
- continued research;
- generating new finished copies;
- reconstructing expected transmission states;
- retaining working annotations.

### Finished/institutional state

Affordances:

- stable viewing/comparison;
- museum use;
- distribution/reference;
- publication preparation;
- preservation away from ongoing field revision.

### Mechanism

Code:

`COPY_STATE_AFFORDANCE_DIFFERENTIATION`

A fair/finished copy is not simply a better version of a rough original. It performs a different historical operation.

---

## 17. The 1870 reuse package reunites layers separated in 1844

In 1844 Hodgson conceptually separates:

`working originals + notes` from `finished institutional series + specimens`.

By 1870, the Marshall/Hume package again assembles a multi-layer package:

- drawings;
- Hodgson manuscript list;
- artist Hindi list;
- shikaree/writer manners volumes;
- Hodgson field memos;
- printed catalogues/reprints.

### Mechanism

Code:

`RECOMPOSITION_FOR_SECONDARY_RESEARCH_USE`

The archive can be decomposed for custody and later recomposed for a new research project.

This is a strong example of **relational portability across decades**.

---

## 18. New error model: redundancy, not identifier purity

Wave 29 proposed `RELATIONAL_IDENTIFIER_OVER_NAME_STABILITY`.

Wave 30 requires a refinement.

### Revised model

`RELATIONAL_REDUNDANCY_OVER_SINGLE_FIELD_STABILITY`

A robust reconstruction may compare:

- drawing number;
- scientific name;
- local name;
- specimen morphology;
- bill/beak or other anatomical character;
- locality;
- measurement;
- drawing image;
- behavioural memorandum;
- catalogue version;
- destination list.

No one field is universally privileged.

### Reason

Gray's letter shows:

- correct number + corrupted name;
- duplicated/wrong number + morphologically distinguishable bird.

The relation survives because other fields remain available for diagnosis.

---

## 19. Actor-level provenance matrix

### High confidence

- Rajman Singh: named Hodgson artist, many mammal drawings, Darjeeling association.
- Tursmoney Chittakar: named artist, signed watercolour.
- shikarees: explicitly responsible for manners/habits statements in HOD/1/3 / 1870 red volume.
- writer: explicitly translates/records shikaree viva voce statements.
- Hodgson: classification, supervision, anatomy/food/location notes, master-state control, lists.
- Archibald Campbell: anatomical/scientific collaboration.
- J. E. Gray/British Museum: sorting, comparison, naming, distribution, correction.

### Medium / unresolved

- 1870 `native painter` who produced the Hindi list: unnamed; Rajman hypothesis unproven.
- individual shikarees: unnamed in current catalogue-level evidence.
- `my writer`: unnamed in current catalogue-level evidence.
- original measurement-table author on specific sheets: probable artist layer, requires palaeographic/object proof.

### Rule

Prefer role-level provenance to speculative name assignment.

---

## 20. Cross-domain significance

The zoological production chain now closely parallels mechanisms found elsewhere without collapsing domain differences.

### Lepcha manuscript copies

`local text -> copyist -> translation-ready page architecture -> later translator`

### Buddhist images

`local religious specialists / Chitrakar -> diagnostic depiction -> Hodgson text/control -> comparative symbol corpus`

### Zoology

`specimen / shikaree field observation -> artist/writer -> drawing/memorandum -> Hodgson number/list -> museum sorter/copyist -> catalogue/distribution`

### Reputation

`external testimony -> Anne compilation -> Brian recovery -> private-print classification/correction`

### General mechanism

`DISTRIBUTED_DOCUMENTARY_LABOUR -> RELATIONAL SURFACE -> VERSIONED INSTITUTIONAL STATE`

---

## 21. New mechanism codes

- `CONTINUOUS_ARTIST_LABOUR`
- `SPECIMEN_CORRECTED_VISUAL_STATE`
- `DIAGNOSTIC_FEATURE_TRAINING`
- `SEX_AGE_VARIANT_CAPTURE`
- `OPTICAL_ACCURACY_ASSIST`
- `PARALLEL_SPECIMEN_PROCESSING`
- `MEDICAL_ANATOMICAL_COLLABORATION`
- `DRAWING_AS_COMPOSITE_METADATA_SURFACE`
- `PROBABLE_ARTIST_MEASUREMENT_LAYER`
- `NAMED_ARTIST_NODE`
- `ANONYMOUS_ARTIST_MAJORITY`
- `DELEGATED_FIELD_OBSERVATION`
- `ROLE_DIFFERENTIATION_BEFORE_ATTRIBUTION`
- `CHITRAKAR_AS_MEDIATION_ROLE`
- `WORKING_ORIGINAL_VS_FINISHED_SERIES`
- `GENERATIVE_STATE_RETENTION`
- `INSTITUTIONAL_FINISHED_STATE`
- `INSTITUTIONAL_COPY_COMPLETION_FROM_MASTER`
- `MASTER_STATE_AS_AUDIT_REFERENCE`
- `COPIER_NAME_CORRUPTION_WITH_NUMBER_PRESERVATION`
- `SPECIMEN_NUMBER_COLLISION`
- `INDEPENDENT_METADATA_FAILURE_CHANNELS`
- `SORTING_BEFORE_NOMENCLATURAL_STABILIZATION`
- `DISTRIBUTION_DURING_METADATA_INSTABILITY`
- `COPY_STATE_AFFORDANCE_DIFFERENTIATION`
- `RECOMPOSITION_FOR_SECONDARY_RESEARCH_USE`
- `RELATIONAL_REDUNDANCY_OVER_SINGLE_FIELD_STABILITY`

---

## 22. Immediate archive/falsification targets

1. Locate the 1835 Johnstone letter in its original/printed first state and verify the production-protocol wording directly.
2. Select 10–20 signed/attributable ZSL sheets and create palaeographic layers for artist hand, Hodgson hand, Devanagari hand, later institutional hand.
3. Test whether measurement tables consistently share an artist hand and whether English values are a second hand/translation layer.
4. Compare Rajman-signed and Tursmoney-signed sheets for metadata-field consistency.
5. Search HOD/1/3 for personal names of individual shikarees or writer in headings, marginalia, covers or colophons.
6. Identify the 1870 native painter Hindi list physically and test handwriting/signature against Rajman materials.
7. Reconstruct all number collisions noted by Gray and determine whether morphology/image/locality fields resolve them.
8. Compare copied names in the erroneous list with Hodgson's originals to identify the copier's transformation/error pattern.
9. Reconstruct when original rough drawings became institutional holdings and whether they remained distinct from finished/fair copies in later ZSL arrangement.
10. Update the article spine from `drawing as representation` to `drawing as composite, versioned metadata surface`.

## Bottom line

Hodgson's zoological drawings were not illustrations appended to completed science. They were versioned working surfaces produced through skilled Nepali artistic labour, repeatedly corrected against fresh specimens and integrated with anatomy, measurements, local names and reference numbers. Behavioural knowledge entered through shikarees and a writer; Hodgson maintained parallel anatomical, classificatory and organizational notes; British Museum staff later sorted, renamed, copied and distributed the collection. The system's strength came from the fact that these streams overlapped. Gray's simultaneous report of correct numbers with absurdly copied names and of separate numbering collisions demonstrates the crucial point: no single identifier was intrinsically reliable. Reconstructibility emerged from redundant relations among multiple imperfect surfaces.