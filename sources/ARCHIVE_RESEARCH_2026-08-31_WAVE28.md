# Archive research wave 28 — household testimonial labour, anonymous self-publication, and recursive career re-segmentation

Date: 2026-08-31

Status: source-control correction and deep reconstruction of the Hodgson testimonial / `Notes of the Services` sequence. This wave supersedes the overly simple Wave 25–26 label `SELF_CURATED_REPUTATION_DOSSIER` wherever it implied that Brian Houghton Hodgson personally assembled the 1868 testimonial notebook from the outset.

## Executive result

The reputation archive is more complex and more historically interesting than a single act of self-curation.

The evidence now supports at least three distinct operations:

1. **household testimonial compilation**: Anne/Annie Hodgson collected handwritten copies and newspaper cuttings of testimonials concerning Brian Hodgson's work;
2. **posthumous household recovery and re-inscription**: Brian found the notebook in Anne's desk and dated/identified the discovery on 12 March 1868;
3. **recursive anonymous self-publication**: a printed pamphlet, `Notes of the Services of B. H. Hodgson ... Collected by a Friend`, was repeatedly corrected, expanded and reprinted/renewed, with strong evidence that Hodgson himself was the author and active reviser.

The result is not merely `self-archive`. It is a **household-to-print evidence pipeline** in which reputation is gathered, inherited within the household, reclassified by career domain, privately circulated, annotated, and re-issued in new documentary states.

This is one of the clearest cases in the repo of `INTERMEDIATE_STATE_FIXATION` becoming recursive across decades.

---

## 1. Source-control correction: the 1868 notebook was collected by Anne/Annie Hodgson

### Uploaded witness

`Adobe Scan 2025年3月28日 (5)` contains the testimonial notebook and an OCR-imperfect version of its title inscription.

The uploaded OCR had been read provisionally as if Hodgson himself had gathered the volume.

### External archival control

The Royal Asiatic Society catalogue identifies the item as:

`GB 891 BHH-BHH/10-BHH/10/2 — Testimonials to the value of my labours in literature, education & science`.

The RAS description gives the full inscription:

`Testimonials to the value of my labours in literature, education & science collected by my darling Annie and found in her desk Mar 12 1868.`

The catalogue identifies **Hodgson Annie** as creator and describes the object as a notebook containing handwritten copies and newspaper cuttings of testimonials concerning Hodgson's work, ranging from 1849–1863, with two further inserts dated across 1849–1868.

The larger `BHH/10 — Books of Testimonials` series is described as **two books of testimonials compiled to bring together all the accolades and achievements of Hodgson**, with both Brian Houghton Hodgson and Annie Hodgson associated as creators.

### Corrected mechanism

Replace the narrow code:

`SELF_CURATED_REPUTATION_DOSSIER`

with a layered sequence:

- `HOUSEHOLD_TESTIMONIAL_COMPILATION`
- `POSTHUMOUS_HOUSEHOLD_RECOVERY`
- `REPUTATION_ARCHIVE_CO_PRODUCTION`

### Operational sequence

`external testimonial -> Anne selects/copies/cuts -> household notebook -> Anne's death / notebook remains in desk -> Brian finds notebook -> Brian inscribes discovery and retains object`

### Why this is stronger

The testimonial archive is not reducible to Hodgson managing his own image. The evidential labour is distributed within the household.

The archive therefore contains an otherwise easily erased form of scholarly/reputational labour: **spousal collection, copying, clipping, preservation and arrangement**.

---

## 2. The discovery inscription converts Anne's compilation into Brian's inherited evidence object

The phrase `found in her desk Mar 12 1868` records a custody transition.

Before discovery, the notebook was Anne's compilation.

After discovery, Brian knows of, identifies and preserves it as evidence of `the value of my labours`.

### Mechanism

Code:

`HOUSEHOLD_CUSTODY_TRANSITION`

This is a small but precise archival event:

`compiler's desk -> discovery by subject of compilation -> retained personal archive`

The meaning of the same physical notebook changes because the custodian and the relationship to its contents change.

This should be distinguished from assuming that every item later present in Hodgson's papers was produced by Hodgson.

---

## 3. The testimonial books constitute a series, not a single isolated scrapbook

The RAS archive describes `BHH/10` as **Books of Testimonials**, plural, consisting of two books.

This matters because the 1868 notebook should not be treated as the entire reputation archive.

### Mechanism

Code:

`SERIAL_REPUTATION_ARCHIVE`

Research consequence:

The order, overlap and division of labour between the two testimonial books must be mapped before claims are made about the architecture of Hodgson's reputation archive as a whole.

The current uploaded notebook gives one object-state, not the full series.

---

## 4. Identify the later printed source: `Notes of the Services of B. H. Hodgson ... Collected by a Friend`

### Uploaded source

The large uploaded `Adobe Scan 2025年3月28日` contains:

- political/official service testimonials in the early pages;
- `APPENDIX B. PART II.` beginning at printed p. 34;
- seven disciplinary/career sections;
- later appendices including manuscript gift material;
- `APPENDIX D. CATALOGUES OF HODGSON COLLECTION. (Copies distributed.)` beginning at printed p. 78.

The title has now been externally identified as:

`Notes of the services of B. H. Hodgson, Esq., late British minister at the court of Nepal, collected by a friend.`

Google Books records multiple states/editions, including 1868/1869 and 1883.

### Version-scale difference

Google Play/Books describes the 1869 state as about **30 pages**, while the 1883 state is **104 pages**.

The 1883 Google Books contents show nine major sections beginning on pp. 3, 12, 33, 46, 47, 52, 65, 74 and 78 — a pagination pattern consistent with the uploaded source's Appendix B Part II at p. 34 and Appendix D at p. 78.

### Source-control conclusion

The uploaded source is consistent with the expanded **1883 documentary state** of `Notes of the Services`, but the exact surviving exemplar/copy should remain unidentified until its cover/title-page annotations are matched against known copies.

Code:

`NOTES_OF_SERVICES_1883_STATE_PROVISIONAL_MATCH`

---

## 5. Authorship: `Collected by a Friend` is a pseudonymous/anonymous self-presentation problem

### Historiographical conflict

Some cataloguing traditions attributed the unnamed `friend` to W. W. Hunter.

Harihar Raj Joshi reports that the India Office/British Library catalogue made this identification on acquisition, but argues that it is wrong.

David Waterhouse, citing a Bodleian letter, states that **Hodgson himself was the author of `Notes of the Services`**.

### Source-control rule

Do not write `compiled by W. W. Hunter` for `Notes of the Services` merely because Hunter later compiled the Sanskrit manuscript catalogue included/attached to later Hodgson material.

The strongest present working attribution is:

`anonymous/"friend" voice; authorial responsibility attributed to Hodgson by Waterhouse on Bodleian evidence; Hunter attribution disputed`.

### Mechanism

Code:

`ANONYMOUS_SELF_ADVOCACY`

The rhetorical form matters. Hodgson does not simply publish `my services`; the pamphlet presents an apparently external collector/advocate.

This creates a documentary distance between:

- the person whose value is being demonstrated;
- the textual voice that assembles the proof.

Yet Hodgson's own authorship and revision activity collapse that distance at the production level.

---

## 6. Joshi's copy census: `Notes of the Services` was repeatedly corrected and renewed

### Secondary bibliographical control

Joshi describes several physical copies of the privately printed pamphlet and concludes that at least two, probably more, editions/impressions existed.

He stresses that the pamphlet was marked **NOT PUBLISHED** but was physically printed for private distribution among friends, relatives, acquaintances and well-wishers.

He describes three useful copy states:

### A. `Tushar` state

- no printed or handwritten year;
- 75 pages;
- Hodgson writes `Private / Own Corrected / and list added` on cover;
- `Collected` and `Friend` are crossed out;
- Hunter's catalogue is present;
- additional Hodgson annotations.

### B. `Calvin` state

- 51 pages;
- `1883` added by Hodgson in manuscript;
- `Collected By A Friend` remains uncancelled;
- Hodgson writes `Own copy corrected`, then `Imperfect`, with a direction equivalent to `See renewed COPY`;
- annotations across multiple pages.

### C. `Indu` state

- 104 pages including four-page index;
- `1883` printed;
- Hodgson writes `Own Copy` and refers to another copy for Hunter's list of MSS;
- substantial additions occur on pp. 34, 47–49, 57 and covers.

### Mechanism

Codes:

- `PRIVATE_PRINT_VERSION_CHAIN`
- `OWN_COPY_CORRECTION`
- `RENEWED_COPY_PROPAGATION`
- `RECURSIVE_REPUTATION_EDITING`

### Why this is exceptional

The object whose purpose is to stabilize Hodgson's reputation is itself unstable and versioned.

`career proof -> private print -> author annotation -> recognition of imperfection -> renewed copy -> further additions -> new printed state`

The reputation archive is therefore governed by the same revision logic as the scientific catalogues and comparative vocabularies.

---

## 7. 1869 to 1883: the career object expands materially

The external bibliographic record gives a striking scale change:

- 1869 version: approximately 30 pages;
- 1883 version: 104 pages.

Even without a full page-by-page collation, the expansion demonstrates that `Notes of the Services` is not one frozen biography/testimonial pamphlet.

### Mechanism

Code:

`CAREER_OBJECT_ACCUMULATION`

The document grows as later evidence, catalogues, institutional recognitions, corrections and classificatory structures are incorporated.

This is a reputational analogue of collection growth:

`new evidence -> new section/appendix -> revised totality`

### Falsification requirement

A proper stemma must still compare 1868/1869, undated, manuscript-1883 and printed-1883 copies directly. Page count alone does not establish which passages were added at which exact revision.

---

## 8. Appendix B Part II: heterogeneous achievements are re-segmented into seven career domains

The uploaded 1883-state source has a clear Part II taxonomy.

### Section I

`VERNACULAR EDUCATION`

### Section II

`HINDU LAW AND LEGAL ADMINISTRATION`

### Section III

`PHYSICAL GEOGRAPHY OF HIMALAYA AND TIBET`

### Section IV

`ETHNOLOGY`

### Section V

`SETTLEMENT OF EUROPEANS IN INDIA, AND TRANS-HIMALAYAN COMMERCE`

### Section VI

`BUDDHISM`

### Section VII

`ZOOLOGY`

These headings collect quotations from reports, reviews, dedications, learned-society speeches, books and correspondence under domain labels.

### Mechanism

Code:

`CAREER_RESEGMENTATION`

The operation is:

`heterogeneous external judgments -> assign disciplinary/policy domain -> arrange as comparable evidential series -> construct a classified career`

### Important distinction

This taxonomy belongs to the printed `Notes of the Services` state, not automatically to Anne's 1868 notebook.

A page-level collation is required before any claim that Anne's notebook already used the same seven-part classification.

---

## 9. Part I and Part II encode a political/scholarly split, but Part I title remains source-controlled

The uploaded source before Appendix B Part II contains a sustained block of official and political evidence, especially around:

- Nepal Residency;
- the 1838–42 diplomatic crisis;
- negotiations with the Durbar;
- Governor-General / Government commendation;
- border/security and related official service.

The exact printed heading of `Part I` has not yet been securely recovered in the OCR/search pass.

### Safe formulation

Use:

`political/official-service block preceding Appendix B Part II`

rather than inventing an exact Part I title.

### Analytical implication

The 1883 state nevertheless creates a high-level division between official/political proof and Part II's subdivided literature/science/education proof.

This produces a two-stage normalization:

`state service evidence` versus `scholarly/public-policy evidence`

and then:

`scholarly/public-policy evidence -> seven classified domains`.

---

## 10. The 1883 pamphlet explicitly totalizes Hodgson's writings before classifying their value

A passage immediately before Appendix D says Hodgson's writings are too numerous and various to specify singly and therefore enumerates their topics.

It lists fields including:

- National Education for India;
- Military Tribes and Military System of Nepal;
- Routes, Topography and Physical Geography;
- Settlement of Europeans in the Himalaya;
- trans-Himalayan commerce;
- antiquities;
- Northern Buddhist literature and religion;
- ethnology and comparative vocabularies;
- zoology.

It then asks how these writings were appreciated by competent judges and points the reader to the testimonial apparatus.

### Mechanism

Code:

`CAREER_TOTALIZATION_BEFORE_EVALUATION`

This closely parallels the 1838 zoological catalogue:

`piecemeal descriptions -> orderly complete enumeration -> comparative judgment`

In the career archive:

`scattered papers/services -> topic enumeration -> testimonial classification -> aggregate reputation`

This is a striking recursive reuse of catalogue logic on the self.

---

## 11. Hunter's manuscript catalogue becomes one appended proof-object, not necessarily the authorial frame

The uploaded source reaches `APPENDIX D. CATALOGUES OF HODGSON COLLECTION. (Copies distributed.)` at printed p. 78.

The standalone `Catalogue of Sanskrit Manuscripts collected in Nepal ...` was compiled by W. W. Hunter and includes assistance from Max Müller, Cowell, Bendall and Bunyiu Nanjio.

Joshi's copy census explicitly notes Hunter's catalogue within some `Notes of the Services` copies.

### Mechanism

Code:

`EXTERNAL_CATALOGUE_AS_SELF_EVIDENCE`

A catalogue produced through external scholarly labour can be inserted into Hodgson's private reputation pamphlet as documentary proof of:

- scale of collecting;
- distribution;
- institutional uptake;
- continuing scholarly usability.

This is not the same operation as Hunter authoring the reputation pamphlet.

---

## 12. The household notebook and the printed pamphlet are distinct but connected archival regimes

### Anne's notebook

Primary operation:

`collect testimonial traces`.

Media:

- handwritten copies;
- newspaper cuttings;
- inserts.

Unit of value:

`testimony / accolade`.

### Brian's `Notes of the Services`

Primary operations:

- classify;
- totalize;
- quote;
- append;
- privately circulate;
- correct;
- renew.

Media:

- privately printed pamphlet;
- handwritten annotations/cancellations;
- appended catalogues/lists.

Unit of value:

`career domain + supporting external judgment/document`.

### Mechanism

Code umbrella:

`HOUSEHOLD_TO_PRINT_REPUTATION_PIPELINE`

The relationship should be tested by direct collation rather than assumed item-for-item, but the two objects clearly belong to a broader household/personal practice of assembling proofs of Hodgson's work.

---

## 13. Strong cross-domain comparison: reputation itself becomes a catalogue problem

The archive now supports a structural comparison across knowledge domains.

### Zoology

`species observations -> scattered descriptions -> classified catalogue -> later correction/distribution tables`

### Ethnography

`language samples -> provisional arrangement -> working corrections -> print state -> later explanatory correction`

### Manuscripts

`physical copies -> lists/catalogues -> institutional re-segmentation -> later catalogue correction`

### Reputation

`external judgments -> household collection -> anonymous/self-authored private print -> career-domain segmentation -> appended external catalogues -> own-copy corrections -> renewed copies`

### General mechanism

`CLASSIFICATION_AS_RECURSIVE_SELF_INFRASTRUCTURE`

Hodgson applies or participates in analogous documentary operations not only to animals, peoples, texts and images, but eventually to **his own career as an evidential object**.

This is a stronger and more source-specific formulation than the earlier generic phrase `self as archive`.

---

## 14. New source-state hierarchy for reputation evidence

Every reputation claim should now record at least:

- `testimonial_original_event_date`
- `testimonial_original_document_type`
- `original_speaker/institution`
- `Anne_notebook_present?`
- `Notes_of_Services_version_present?`
- `career_section_assigned`
- `quotation_full_or_extract`
- `Brian_annotation_present?`
- `private_print_state`
- `later_biographical_reuse` (e.g. Hunter 1896)

This prevents a quotation copied in 1883 from being mistaken for an 1883 judgment.

---

## 15. Corrections to earlier repo language

The following earlier formulations should be treated as superseded:

### Superseded

`1868 Testimonials = Hodgson independently self-curated external praise into a bound dossier.`

### Replace with

`Anne/Annie Hodgson compiled at least one testimonial notebook from handwritten copies and clippings; Brian found it in her desk in March 1868 and retained/re-inscribed it within the Hodgson archive.`

### Superseded

`later Appendix B taxonomy = an unidentified later editor's career classification.`

### Replace with

`Appendix B Part II belongs to the versioned, privately printed Notes of the Services. Strong secondary evidence attributes authorship of Notes to Hodgson himself, while the historic Hunter attribution to the unnamed “friend” is disputed. The pamphlet was repeatedly corrected and renewed by Hodgson.`

---

## 16. Revised article claim

A high-value concluding mechanism can now be stated as:

**Hodgson's later archive did not merely preserve earlier achievements. Reputation was itself produced through documentary labour. Anne converted dispersed public judgments into household evidence; Brian inherited that evidence, then repeatedly transformed the career into a classified private print whose own copies were corrected, expanded and renewed. The same practices that made species, manuscripts and linguistic comparisons revisable and auditable were eventually turned onto the person of the investigator.**

This should remain an operational comparison, not a claim that zoological taxonomy and biography are semantically identical.

---

## 17. New mechanism codes

- `HOUSEHOLD_TESTIMONIAL_COMPILATION`
- `POSTHUMOUS_HOUSEHOLD_RECOVERY`
- `REPUTATION_ARCHIVE_CO_PRODUCTION`
- `HOUSEHOLD_CUSTODY_TRANSITION`
- `SERIAL_REPUTATION_ARCHIVE`
- `ANONYMOUS_SELF_ADVOCACY`
- `PRIVATE_PRINT_VERSION_CHAIN`
- `OWN_COPY_CORRECTION`
- `RENEWED_COPY_PROPAGATION`
- `RECURSIVE_REPUTATION_EDITING`
- `CAREER_OBJECT_ACCUMULATION`
- `CAREER_RESEGMENTATION`
- `CAREER_TOTALIZATION_BEFORE_EVALUATION`
- `EXTERNAL_CATALOGUE_AS_SELF_EVIDENCE`
- `HOUSEHOLD_TO_PRINT_REPUTATION_PIPELINE`
- `CLASSIFICATION_AS_RECURSIVE_SELF_INFRASTRUCTURE`

---

## 18. Immediate falsification targets

1. Digitally/physically inspect both RAS `BHH/10` testimonial books and construct a page-level source map.
2. Compare Anne's notebook contents with the 1868/1869 and 1883 `Notes of the Services` to test actual reuse rather than infer a pipeline from proximity.
3. Obtain or inspect the 1868 and 1869 Google Books states page-by-page and construct a version stemma against undated / manuscript-1883 / printed-1883 copies described by Joshi.
4. Recover the exact Part I heading in the expanded pamphlet.
5. Identify the uploaded scan's exact exemplar by cover inscriptions, page count, index and marginalia.
6. Compare Hodgson's handwritten additions on pp. 34, 47–49 and 57 against the next printed/renewed state.
7. Locate the Bodleian letter cited by Waterhouse that establishes Hodgson's authorship.
8. Reconstruct the historical origin of the erroneous Hunter attribution and keep Hunter's actual contribution — the manuscript catalogue — separate.
9. Compare the private pamphlet to Hunter's 1896 `Life` to measure which categories and testimonial selections migrated into formal biography.
10. Add `household_actor` and `documentary_labour_role` fields to the broader provenance schema.

## Bottom line

The reputation archive is now a major primary case, not a decorative epilogue. Its history runs from Anne's household collection of praise to Brian's recovery, anonymous self-advocacy, classified private printing, own-copy correction and renewed editions. In this corpus, a life becomes an object that is repeatedly catalogued — and the surviving versions preserve the same mixture of operational usefulness, correction, incompleteness and state change that the repo has already found in Hodgson's scientific and manuscript infrastructures.