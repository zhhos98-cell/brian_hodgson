# Hodgson paper-history mainline — 2026-09-03, through Wave 84

Status: **current active guardrail**. Supersedes `PAPER_HISTORY_MAINLINE_STATUS_2026-09-03_WAVE83.md`. Wave 84 upgrades the relation between India Political Proceedings and London Board's Collections from a project inference to direct British Library series architecture.

## Current strongest documentary architecture

British Library directly defines `IOR/F/4 Board's Collections` as subject papers extracted from Indian Government Proceedings and previous overseas correspondence, assembled for Board of Control review of East India Company draft despatches. It further states that almost all Political Collections survive and may be treated as a **virtually complete duplicate of the Indian Political Proceedings `IOR/P`**.

Current chain:

`UNDERLYING INDIA LETTER / REPORT`
-> `POLITICAL ORIGINAL CONSULTATION`
-> `POLITICAL PROCEEDINGS / IOR/P`
-> `SUBJECT EXTRACTION / REPACKAGING`
-> `IOR/F/4 POLITICAL BOARD'S COLLECTION`
-> `BOARD OF CONTROL REVIEW OF ASSOCIATED DRAFT`
-> `IOR/E/4 ORIGINAL DRAFT DESPATCH`
-> `[sent despatch / later London documentary states]`.

For Campbell's 1842 experiment the controlled nodes are now:

`21 Apr 1842 Campbell -> G. A. Bushby`
-> `11 May 1842 Political Original Consultation No.70`
-> `IOR/P/196/12 = high-confidence consultation-volume target`
-> `[exact extraction/copy relation pending]`
-> `IOR/F/4/2006/89528 = direct Board's Collection file containing Campbell's result report on making paper from paper-tree bark`
-> `[associated draft number/date pending]`
-> `IOR/E/4/740-855 original-draft series`.

The architecture is direct; the exact item-to-item arrows remain to be proven.

---

## 1. Political O.C. control retained

`Political O.C. = Political Original Consultation`.

Consultation date is not underlying-letter date.

Calibration:

`8 Dec 1831 Hodgson letter`
-> `Pol. Con. 13 Jan 1832, Nos.18–20`.

Target A:

`Pol. Con. 29 Nov 1841, No.147`
=
O'Shaughnessy's report on bleaching paper manufactured at Darjeeling, directly attested by the 1937 IRD exhibition list.

Target B:

`21 Apr 1842 Campbell -> Bushby`
-> `Pol. Con. 11 May 1842, No.70`.

Adjacent consultation numbers remain mandatory retrieval units.

---

## 2. Abdul Ali provenance retained

A. F. M. Abdul Ali's archival addresses carry unusually high finding-aid value because:

- he was Keeper of Records / head of the Imperial Record Department;
- he guided the 1925 pre-Mutiny records handbook;
- he signed/organized the 1937 IHRC historical exhibition listing the 1832 and 1841 Nepal/Darjeeling paper consultation objects;
- his 1944 `The Daphne Paper of Nepal` reuses the same consultation addresses.

Treat:

`ABDUL_ALI_ARCHIVAL_ADDRESS = HIGH_CONFIDENCE_REPOSITORY_NATIVE_TRACE`.

Do not upgrade his paraphrases into primary evidence until original files are controlled.

---

## 3. Board's Collections are a direct Proceedings derivative class

British Library `IOR/F/4` states:

- papers are extracted by subject from Indian Government Proceedings;
- previous overseas correspondence may be added;
- Collections were used by the Board of Control during review of draft overseas despatches;
- their physical arrangement follows associated draft despatch numbers/dates in `IOR/E/4`;
- almost all Political Collections survive and can be considered a virtually complete duplicate of `IOR/P` Political Proceedings.

Therefore encode:

`F4_POLITICAL_COLLECTIONS_DERIVE_FROM_IOR_P_PROCEEDINGS = DIRECT_BL_SERIES_LEVEL`.

But retain:

`ONE_F4_FILE = ONE_IOR_P_ITEM = NOT_AUTOMATIC`.

The Board's Collection can combine several proceedings items, prior correspondence and documents of different dates.

---

## 4. Campbell 1842 now has a formally constrained multi-state documentary family

### State A — underlying correspondence/report

`Campbell -> G. A. Bushby, 21 Apr 1842`.

### State B — India consultation

`Political Original Consultation, 11 May 1842, No.70`.

High-confidence London consultation target:

`IOR/P/196/12`.

### State C — London subject extraction

`IOR/F/4/2006/89528`.

Direct BL scope:

Campbell's report on the result of his experiment in making paper from the bark of the paper tree.

### State D — associated London draft despatch

Expected in:

`IOR/E/4/740-855 — Despatches to India and Bengal, Original Drafts`.

Exact draft/despatch remains unresolved.

Encode:

`CAMPBELL_1842_DOCUMENT_FAMILY = DIRECT_AT_SERIES_AND_SUBJECT_LEVEL`.

Retain:

`F4_89528 = OC_NO70 = PENDING_ITEM_LEVEL_CROSSWALK`.

---

## 5. Board's Collection date cannot be collapsed into consultation or despatch date

British Library explicitly notes a time gap between Collection document dates and associated despatch dates; in the later period this was often about a year or less.

Therefore separate:

- underlying report/letter date;
- consultation date;
- source-document range in F/4 Collection;
- Collection/draft-use date;
- associated draft despatch date;
- transmission date.

For `89528`, `Mar 1842-Nov 1842` is the file's document date range, not proof of the associated London despatch date.

Mechanism:

`DOCUMENTARY_REPACKAGING_GENERATES_A_NEW_CHRONOLOGY`.

---

## 6. `IOR/Z/F/4/8` is now the primary 1842 London register target

British Library:

`IOR/Z/F/4 — Registers of Board's Collections`.

Relevant volume:

`IOR/Z/F/4/8`

Scope:

`Nos. 1 (1842) - 302 (1844)`.

Date range:

`1842-1844`.

Immediate target:

find the register entry corresponding to `IOR/F/4/2006/89528` or the Darjeeling/Campbell paper subject.

Desired fields:

- Board's Collection register number;
- subject/title;
- associated draft number;
- draft/despatch date;
- department;
- any India proceedings reference.

Do not assume all these fields exist until the page is inspected.

Critical rule:

`Z/F/4 REGISTER NUMBER != 89528 != POLITICAL CONSULTATION NO70` unless the source itself maps them.

---

## 7. `IOR/Z/F/4/7` is the parallel 1841 register target

British Library:

`IOR/Z/F/4/7`

Scope:

`Nos. 498 (1839) - 942 (1841)`.

Date range:

`1839-1841`.

Use to search the exact O'Shaughnessy object:

`Report on the method of bleaching paper manufactured at Darjeeling`

associated with:

`Political Consultation 29 Nov 1841, No.147`.

This creates a London-first route that may solve the still-unresolved exact IOR/P volume for No.147.

---

## 8. `IOR/Z/F/3` and `IOR/Z/E/4/16` complete the finding-aid chain

### Draft register

`IOR/Z/F/3 — Registers of Drafts`.

First sequence:

`1-988 (1836-1844)`.

Use after a Board's Collection register entry gives an associated draft number/date.

### Despatch index

`IOR/Z/E/4/16 — Index to India and Bengal Despatches, 1839-1842`.

Use as an independent alphabetical/subject cross-check.

Search:

`Campbell`, `Darjeeling`, `Darjiling`, `paper`, `paper tree`, `manufacture`, `experiment`.

Current search-engine indexing has not exposed the target entry; absence is not inferred.

---

## 9. `IOR/E/4` becomes a controlled endpoint rather than a generic duplicate branch

Relevant British Library range:

`IOR/E/4/740-855`
=
`Despatches to India and Bengal (Original Drafts)`.

This is now the expected endpoint after resolving the associated draft through F/4 registers.

Do not guess exact E/4 volume from chronology.

`IOR/E/4/148-288` remains the Letters Received branch for India/Bengal and may contain the incoming London correspondence side where applicable.

Enclosures can remain outside E/4 and survive in F/4 or IOR/P.

---

## 10. Retrieval is now explicitly bidirectional

### India-first

`No.70`
-> `IOR/P/196/12`
-> identify surrounding transaction
-> locate copied/extracted papers in F/4
-> resolve associated draft/despatch.

### London-first

`IOR/F/4/2006/89528`
-> `IOR/Z/F/4/8`
-> associated draft number/date
-> `IOR/Z/F/3`
-> exact `IOR/E/4` draft
-> map references back to `IOR/P/196/12 / No.70`.

For 1841:

`O'Shaughnessy report title`
-> `IOR/Z/F/4/7 / F4 subject file`
-> associated draft/despatch
-> back-resolve the exact IOR/P volume for 29 Nov 1841 No.147.

Mechanism:

`BIDIRECTIONAL_DOCUMENT_CROSSWALK = ACTIVE_RETRIEVAL_METHOD`.

---

## 11. F/4 transformation changes archival neighbourhood

`89528` groups Campbell's paper report with Darjeeling road, boundary and public-works business.

At the Indian consultation level, the same report may have appeared among a different set of Political items on 11 May.

Therefore:

`ARCHIVAL_NEIGHBOURHOOD_IS_STATE_DEPENDENT`.

Do not infer common funding, common administrative department or material causation merely because records are grouped in one F/4 file.

The grouping does show how technological evidence became legible in London under a broader locality/despatch packet.

---

## 12. Material-paper line remains separate from documentary closure

Direct material anchor:

`25 Mar 1842 Hodgson -> 24 packages Nepalese paper pulp -> Champaran/Woodcock -> Patna by land OR Govind Gang by water -> Calcutta`.

Still missing:

- Halliday directive;
- Woodcock route choice/bill;
- intermediate receipt;
- Calcutta receipt;
- final experimental destination.

Even if No.70 ↔ F/4/89528 is proven, that would establish documentary identity of Campbell's experiment, not material identity of Hodgson's 24 packages with Campbell's feedstock.

Keep:

`HODGSON_24_PACKAGES -> CAMPBELL_EXPERIMENT = UNPROVEN`.

---

## Immediate research order

1. Inspect/request `IOR/Z/F/4/8` for the `89528` / Darjeeling Campbell paper entry.
2. Extract its associated draft number/date.
3. Follow that through `IOR/Z/F/3`.
4. Resolve the exact `IOR/E/4` original draft despatch.
5. Cross-check in `IOR/Z/E/4/16`.
6. Compare the resulting references with `IOR/P/196/12`, 11 May 1842 No.70 ± adjacent items.
7. Inspect/request `IOR/Z/F/4/7` for O'Shaughnessy's 1841 Darjeeling bleaching report.
8. Use any resulting draft/despatch reference to identify its F/4 subject file and exact IOR/P volume.
9. Search the nominal/subject index to Board's Collections through season 1842 for Campbell, Darjeeling, O'Shaughnessy and paper.
10. Continue Halliday/Woodcock/Champaran logistics independently.

---

## Guardrails

1. `Political O.C. = Political Original Consultation`.
2. Political Board's Collections are directly documented as a virtually complete duplicate of `IOR/P` at series level.
3. Series-level duplicate != item-level identity.
4. `IOR/F/4/2006/89528` directly contains Campbell's paper-experiment report.
5. `F4/89528 = No.70` remains unproven pending register/content control.
6. `IOR/P/196/12` remains the high-confidence 11 May 1842 consultation-volume target.
7. Exact IOR/P volume for 29 Nov 1841 No.147 remains unresolved.
8. Use `IOR/Z/F/4/8` for 1842 and `/7` for 1841.
9. Do not equate Z/F/4 register numbering with consultation or F/4 item numbering without direct evidence.
10. Use `IOR/Z/F/3` to resolve draft numbers and `IOR/Z/E/4/16` as independent despatch index.
11. `IOR/E/4/740-855` is the controlled draft-despatch series range; exact volume unresolved.
12. Source-document date, consultation date and London despatch date remain distinct.
13. F/4 archival co-location does not establish shared budget or causal connection.
14. Hodgson's 24 pulp packages remain materially unlinked to Campbell's experiment.
15. 1831–42 remains recurrent programme continuity, not proven uninterrupted formal programme.

## Current strongest proposition

**Campbell's 1842 Darjeeling paper experiment is now situated inside a formally documented India-to-London archival transformation. The India-side business was processed as Political Original Consultation No.70 on 11 May, with `IOR/P/196/12` as the high-confidence London consultation witness. British Library separately identifies `IOR/F/4/2006/89528` as containing Campbell's result report, and its own series description explains that Political Board's Collections were assembled from Indian Political Proceedings and survive as a virtually complete duplicate of `IOR/P`, reorganised around the draft despatches being reviewed by the Board of Control. The problem is therefore no longer whether these repositories preserve related material. It is an exact crosswalk problem: identify the `89528` entry in `IOR/Z/F/4/8`, follow its associated draft through `IOR/Z/F/3` to `IOR/E/4`, and use that London chain to test against No.70 in `IOR/P/196/12`. The same method, using `IOR/Z/F/4/7`, may finally resolve the exact London volume containing O'Shaughnessy's 29 November 1841 bleaching consultation No.147.**