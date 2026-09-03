# Web/archive research 2026-09-03 — Wave 85
## Archival closure: register-date correction, controlled 1842 London derivative, and bounded unresolved status of the 1841 bleaching file

Date: 2026-09-03

Status: final archival-recovery wave for the current Hodgson paper-history run. Follow-up to Waves 82–84. This wave deliberately stops broadening the search. It corrects one retrieval shortcut introduced in Wave 84, fixes the strongest currently recoverable documentary chain for Campbell's 1842 paper experiment, and defines what remains genuinely unresolved after the public-web and catalogue pass.

## Executive result

Wave 84 established from the British Library's own `IOR/F/4` series description that Political Board's Collections are subject extractions from Indian Proceedings and form a virtually complete duplicate of Indian Political Proceedings `IOR/P`. It also established that the physical arrangement of `IOR/F/4` follows the numbers and dates of associated London draft despatches in `IOR/E/4`, not the dates of the underlying Indian source papers.

That last point requires an explicit correction.

The source date of O'Shaughnessy's bleaching report is controlled through:

`Political Consultation, 29 Nov 1841, No.147`.

But that date does **not** prove that the relevant Board's Collection was registered in `IOR/Z/F/4/7`, whose catalogue range ends in 1841. British Library warns that Board's Collections can postdate their source documents because they were organised around later associated London draft despatches. A November 1841 Indian consultation could therefore appear in a Board's Collection registered in 1842 or later.

Correct rule:

`INDIAN_SOURCE_DATE != F4_COLLECTION_REGISTER_YEAR != ASSOCIATED_DESPATCH_DATE`.

Therefore:

`IOR/Z/F/4/7 = POSSIBLE REGISTER TARGET FOR NO147 DERIVATIVE`

but

`IOR/Z/F/4/8 = ALSO POSSIBLE / MUST NOT BE EXCLUDED`.

Wave 84's wording that `/7` is the first or corresponding 1841 register should be read as superseded by this broader two-register search rule.

For Campbell 1842, the documentary chain is substantially stronger. British Library directly catalogues:

`IOR/F/4/2006/89528`

as Darjeeling proceedings whose scope explicitly includes:

`report by Dr Campbell of the result of his experiment in making paper from the bark of the paper tree`.

British Library also directly states that Political Board's Collections are extracted from Indian Political Proceedings and are virtually complete duplicates of `IOR/P`. Thus `89528` is securely a London Board-of-Control derivative of Indian Political proceedings concerning the same Darjeeling paper experiment.

The exact item-level equation remains deliberately unmade:

`IOR/F/4/2006/89528 = Political Consultation 11 May 1842 No.70`

is **not yet proven** without the consultation/register crosswalk.

The highest-value remaining archival checks are now narrow and physical/finding-aid based rather than conceptual:

1. inspect `IOR/P/196/12`, 11 May 1842, No.70 and adjacent items;
2. inspect `IOR/Z/F/4/8` for the Board's Collection entry corresponding to `89528` and its associated draft/despatch;
3. inspect `IOR/Z/F/3` and `IOR/Z/E/4/16` for the resulting E/4 crosswalk;
4. inspect the 29 Nov 1841 Political Consultation No.147 and its adjacent items in NAI/IOR/P;
5. search **both** `IOR/Z/F/4/7` and `/8` for the 1841 bleaching business, because Board's Collection registration can postdate the Indian consultation.

No public source recovered in this wave supplies a defensible exact `IOR/P` shelfmark or exact F/4 collection number for No.147. That is now a bounded archival gap rather than an open-ended web-search problem.

---

## 1. Correction: source year cannot select the Board's Collection register automatically

British Library `IOR/F/4` states:

- Board's Collections consist of papers extracted from Indian Proceedings;
- they were assembled in London for review of draft despatches;
- their physical arrangement follows draft numbers and dates of associated `IOR/E/4` despatches;
- there is normally a time gap between source documents and the associated despatch, historically ranging from months to years.

British Library series record:

https://searcharchives.bl.uk/catalog/036-000736052

Therefore the following shortcut is unsafe:

`SOURCE_DOCUMENT_1841 -> REGISTER_VOLUME_ENDING_1841`.

For O'Shaughnessy:

`29 Nov 1841 Political Consultation No.147`

may have entered a Board's Collection associated with an 1842 draft/despatch.

Correct retrieval set:

- `IOR/Z/F/4/7`, Nos.498 (1839)–942 (1841);
- `IOR/Z/F/4/8`, Nos.1 (1842)–302 (1844).

British Library register hierarchy:

https://searcharchives.bl.uk/catalog/037-004319122

Encode:

`NO147_F4_REGISTER_TARGET = Z_F_4_7_OR_Z_F_4_8_PENDING_DIRECT_CROSSWALK`.

---

## 2. 1842 Campbell Board's Collection is direct catalogue evidence

British Library:

`IOR/F/4/2006/89528`.

Date range:

`Mar 1842–Nov 1842`.

Scope includes:

- Darjeeling boundary-mark administration;
- Birch Hill road;
- public works;
- `report by Dr Campbell of the result of his experiment in making paper from the bark of the paper tree`.

Catalogue:

https://searcharchives.bl.uk/catalog/041-000786077

This is direct evidence that Campbell's paper experiment became a London Board's Collection object.

Encode:

`CAMPBELL_DARJEELING_PAPER_EXPERIMENT -> IOR_F_4_2006_89528 = DIRECT_BL_CATALOGUE`.

This is already sufficient for a paper-history claim about documentary reclassification and London administrative circulation.

---

## 3. Why `89528` is more than a thematically similar file

The `IOR/F/4` series description directly states that Board's Collections are copied/extracted from Indian Proceedings and that Political Collections are a virtually complete duplicate of `IOR/P` Political Proceedings.

Thus the correct evidential statement is:

`89528` belongs to a documentary class **derived from the Indian Political Proceedings system** in which Campbell's paper business was processed.

That is stronger than:

`89528 happens to mention the same experiment`.

But it remains weaker than:

`89528 is a verbatim copy of Consultation No.70`.

Encode:

`F4_89528 = DIRECT_PROCEEDINGS_DERIVATIVE_CLASS`;

`F4_89528_EXACTLY_CROSSWALKS_NO70 = PENDING`.

This distinction should be preserved in prose.

---

## 4. Controlled 1842 multi-state chain

Current strongest reconstruction:

`material/manufacturing experiment at Darjeeling`
-> `Campbell report / letter, including 21 Apr 1842 Campbell -> G. A. Bushby`
-> `Political Original Consultation, 11 May 1842, No.70`
-> `[IOR/P consultation/proceedings witness; IOR/P/196/12 high-confidence target volume from published citation evidence]`
-> `subject papers extracted/recompiled for Board of Control`
-> `IOR/F/4/2006/89528`
-> `[associated draft despatch identified through Z/F/4 + Z/F/3]`
-> `IOR/E/4 draft/despatch`
-> `[possible later policy response]`.

Evidence states:

- Campbell experiment: direct through BL F/4 catalogue + Abdul Ali secondary detail;
- 21 Apr letter date: direct through Abdul Ali's recovered 1944 article;
- 11 May No.70: direct through Abdul Ali's archival citation;
- `IOR/P/196/12`: high-confidence volume target from independent published India Political Consultation citation on 11 May 1842;
- `IOR/F/4/2006/89528`: direct BL catalogue;
- exact `No.70 -> 89528` crosswalk: pending;
- exact associated E/4 draft: pending.

This is now stable enough for a dissertation/paper narrative as long as each evidential level is labelled correctly.

---

## 5. Board's Collection 89528 demonstrates documentary recomposition

The file does not isolate paper manufacture. The same Board's Collection groups Campbell's paper experiment with other Darjeeling business such as public works, roads and boundary administration.

Thus the London transformation is not simply copying.

It performs:

`INDIAN PROCEEDINGS ITEMS`
-> `LONDON SUBJECT/ADMINISTRATIVE COLLECTION`
-> `DRAFT-DESPATCH REVIEW PACKET`.

Consequences:

- context can change without document content disappearing;
- material experimentation can be administratively grouped with territorial/public-works business;
- the history of paper is visible through changing documentary neighbours as well as changing material states.

Mechanisms:

- `DOCUMENTARY_RECOMPOSITION_CHANGES_NEIGHBOURHOOD`;
- `ADMINISTRATIVE_RECLASSIFICATION_IS_PART_OF_MATERIAL_HISTORY`;
- `DERIVATIVE_COPY_IS_NOT_NEUTRAL_DUPLICATION`.

---

## 6. 1841 No.147 remains exact at consultation level but unresolved at London shelfmark level

Controlled identity:

`Political Consultation, 29 Nov 1841, No.147`.

1937 Imperial Record Department / Indian Historical Records Commission exhibition description:

`Report on the method of bleaching paper manufactured at Darjeeling` by W. B. O'Shaughnessy.

This is enough to establish:

- consultation date;
- consultation number;
- author;
- report genre;
- subject;
- continued archival existence/identifiability in 1937.

Current unresolved London fields:

- exact `IOR/P` volume;
- exact F/4 Board's Collection number;
- exact associated draft/despatch;
- exact E/4 shelfmark.

Repeated public catalogue and full-web searches during Waves 81–85 did not produce a defensible exact shelfmark for these fields.

Encode:

`NO147_ARCHIVAL_ADDRESS_INDIA_SIDE = SECURE`;

`NO147_EXACT_LONDON_DERIVATIVE_SHELFMARK = BOUNDED_UNRESOLVED`.

Do not spend further general web-search effort unless a new digitised finding aid becomes available.

---

## 7. What the 1937 exhibition evidence does and does not prove

It proves that the Imperial Record Department could identify and exhibit:

- `Pol. Con. 13 Jan 1832, Nos.18–20` on Himalayan/Nepal indigenous paper manufacture;
- `Pol. Con. 29 Nov 1841, No.147`, O'Shaughnessy's Darjeeling bleaching report.

It strongly supports a provenance line from the nineteenth-century consultation archive into Abdul Ali's later historical work.

It does not prove:

- that Abdul Ali's 1944 article was written directly from exhibition notes;
- that every quotation in 1944 reproduces the complete original document;
- that the documents survive today in the same physical arrangement as in 1937.

Use:

`1937_EXHIBITION = ARCHIVAL_EXISTENCE_AND_CURATORIAL_SELECTION_EVIDENCE`.

---

## 8. The 1832 cluster is a proven multi-item transaction

The exhibition lists:

`Pol. Con. 13 Jan 1832, Nos.18–20`.

Abdul Ali's 1944 article cites No.19 in connection with Hodgson's 8 Dec 1831 paper-specimen communication.

Therefore adjacent-number analysis is no longer merely a methodological hypothesis.

At least one early Nepal-paper transaction occupies a **multi-number consultation cluster**.

Encode:

`ADJACENT_CONSULTATION_ITEMS_FORM_PAPER_TRANSACTION = DIRECT_1832_CONTROL`.

This strengthens the instruction to retrieve No.70 and No.147 with neighbouring items rather than in isolation.

---

## 9. Final archive request set

### A. 1842 Darjeeling paper business

Request/inspect:

1. `IOR/P/196/12` — India Political Consultations / Proceedings, 11 May 1842; No.70 plus adjacent items;
2. `IOR/F/4/2006/89528` — Board's Collection containing Campbell paper experiment report;
3. `IOR/Z/F/4/8` — Board's Collections register, 1842–44;
4. relevant `IOR/Z/F/3` draft register entry once the F/4 register supplies draft information;
5. `IOR/Z/E/4/16` — Index to India and Bengal Despatches, 1839–42;
6. exact `IOR/E/4` original draft/despatch identified from those registers.

### B. 1841 bleaching business

Request/inspect:

1. NAI / IOR/P Political Consultation, 29 Nov 1841, No.147 plus adjacent items;
2. search both `IOR/Z/F/4/7` **and** `/8` for the resulting Political Board's Collection;
3. follow register entry into `IOR/Z/F/3` and `IOR/E/4`;
4. search by exact historical title: `Report on the method of bleaching paper manufactured at Darjeeling`;
5. verify whether the O'Shaughnessy report itself, a copy, or only an abstract survives in London.

### C. 1832 calibration cluster

Request/inspect:

`Political Consultation, 13 Jan 1832, Nos.18–20`.

Goal:

reconstruct original letter + specimens + orders/reply structure and calibrate consultation packet form.

---

## 10. Stop condition for the current web run

The remaining questions require one of the following:

- direct image access to the relevant IOR/P consultation volume;
- direct image/reading-room access to `IOR/Z/F/4/7-8`;
- direct access to `IOR/F/4/2006/89528` contents;
- NAI/Abhilekh Patal consultation images/indexes;
- a newly digitised official finding aid with item-level crosswalks.

General web search has reached diminishing returns.

Therefore encode:

`PUBLIC_WEB_RECOVERY_PASS_2026_09_03 = CLOSED_AT_WAVE85`.

This is not a claim of archival exhaustion. It is a methodological boundary between what can now be responsibly reconstructed from accessible catalogues/publications and what requires object-level archive control.

---

## Source-control rules

1. Do not assign the 1841 bleaching derivative to `IOR/Z/F/4/7` solely because the source consultation is dated 1841.
2. Search both `/7` and `/8` because F/4 is organised around later associated draft despatches.
3. `IOR/F/4/2006/89528` directly contains Campbell's Darjeeling paper-experiment report according to BL catalogue.
4. Treat `89528` as a Political-Proceedings-derived London documentary class, not yet a proven one-to-one copy of No.70.
5. Retain `IOR/P/196/12` as high-confidence target volume for 11 May 1842, pending direct No.70 inspection.
6. No.147 is secure at India-side consultation/date/number/title level but exact London shelfmark remains unresolved.
7. Adjacent consultation-number retrieval is directly justified by the 1832 Nos.18–20 paper cluster.
8. Preserve separate dates for underlying letter, consultation, Board's Collection source span, London draft despatch and final despatch.
9. Do not continue generic web searching for the exact 1841 shelfmark without a new finding-aid source.
10. Treat unresolved item-level crosswalks as archive requests, not narrative defects to be filled by interpolation.

## Bottom line

The final public-web archival pass leaves the project in a much stronger and cleaner position than the initial hunt for `Political O.C.`. The abbreviation is now understood as `Original Consultation`; Abdul Ali's citations have professional archival provenance; the consultation date/number system is decoded; the 1832 paper business is known to occupy Nos.18–20; O'Shaughnessy's 1841 bleaching report is securely identified as Political Consultation 29 Nov 1841 No.147 and as a surviving/exhibitable Imperial Record Department object in 1937; Campbell's 1842 paper experiment is securely represented in the London Board's Collection `IOR/F/4/2006/89528`; and British Library directly defines Political Board's Collections as a virtually complete duplicate/derivative of Indian Political Proceedings. What remains is no longer interpretive fog. It is a finite object-level crosswalk problem: inspect No.70 and No.147 with adjacent consultation items, inspect the F/4 registers and the Campbell Board's Collection, and follow the associated draft numbers into E/4. The archive gap is now bounded enough to write around accurately rather than speculate through.