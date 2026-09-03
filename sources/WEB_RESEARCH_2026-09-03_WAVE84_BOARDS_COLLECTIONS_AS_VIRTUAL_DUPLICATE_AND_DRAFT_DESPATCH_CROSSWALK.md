# Web/archive research 2026-09-03 — Wave 84
## Political Board's Collections as a virtually complete duplicate of Indian Political Proceedings, and the `IOR/P -> F/4 -> E/4` draft-despatch crosswalk

Date: 2026-09-03

Status: active paper-history mainline. Follow-up to Wave 83. This wave upgrades the archival relation between India Political Proceedings and London Board's Collections from a project-level inference to a direct British Library series-level statement. It still does **not** prove that `IOR/F/4/2006/89528` is exactly the London derivative of Political Consultation 11 May 1842 No.70. The next missing step is a register/document crosswalk.

## Executive result

British Library's own `IOR/F/4` series description states that Board's Collections consist of copies of papers on a given subject **extracted from the Proceedings of the Indian Governments**, together with copies of previous overseas correspondence. They were assembled for the Board of Control in London while it reviewed East India Company draft overseas despatches. Their physical arrangement follows the numbers and dates of the associated draft despatches in `IOR/E/4`.

Most importantly, the catalogue states that **almost all Political Collections survive and may be considered a virtually complete duplicate of the Indian Political Proceedings `IOR/P`**.

British Library series record:

https://searcharchives.bl.uk/catalog/036-000736052

This produces a controlled documentary architecture:

`INDIAN POLITICAL BUSINESS`
-> `Original Consultation / Political Proceedings in India`
-> `IOR/P Political Proceedings / consultation witness`
-> `subject papers extracted into Board's Collection`
-> `IOR/F/4 Political Collection`
-> `used to review associated draft despatch`
-> `IOR/E/4 original draft despatch`
-> `[despatch sent to India]`.

For Campbell's 1842 Darjeeling paper experiment, Wave 83 already identified the exact subject file:

`IOR/F/4/2006/89528`

whose catalogue scope explicitly includes Campbell's report on the result of making paper from the bark of the paper tree.

Wave 84 therefore upgrades its status from merely `SAME_PROGRAMME_LONDON_DERIVATIVE` to:

`DIRECT_F4_POLITICAL_PROCEEDINGS_DERIVATIVE_CLASS`.

But retain:

`F4_89528 = POLITICAL_CONSULTATION_11_MAY_1842_NO70` = `UNPROVEN_AT_ITEM_LEVEL`.

The exact crosswalk should now be recoverable through contemporary Board's Collection and draft registers:

- `IOR/Z/F/4/8`, Register of Board's Collections, 1842–1844;
- `IOR/Z/F/3`, Registers of Drafts, including a sequence covering 1836–1844;
- `IOR/Z/E/4/16`, Index to India and Bengal Despatches, 1839–1842;
- `IOR/E/4/740-855`, Despatches to India and Bengal, Original Drafts.

For the 1841 O'Shaughnessy bleaching report, the corresponding Board's Collection register is:

- `IOR/Z/F/4/7`, Register of Board's Collections, 1839–1841.

The numbered ranges in `IOR/Z/F/4/7-8` are register-series numbers and must **not** be equated with either Political Consultation numbers or the global Board's Collection item number `89528` without direct image control.

Core mechanisms:

- `F4_POLITICAL_COLLECTIONS_ARE_IOR_P_DERIVATIVE_DUPLICATES`
- `PROCEEDINGS_ARE_REPACKAGED_BY_SUBJECT_FOR_LONDON_REVIEW`
- `BOARDS_COLLECTIONS_ARE_ORGANISED_AROUND_ASSOCIATED_DRAFT_DESPATCHES`
- `DOCUMENTARY_DERIVATION_REORDERS_ARCHIVAL_CONTEXT`
- `COLLECTION_DATE_AND_DESPATCH_DATE_CAN_DIFFER_STRUCTURALLY`
- `REGISTER_CAN_CROSSWALK_COLLECTION_TO_DRAFT`
- `TWO_DIRECTIONAL_RETRIEVAL_CAN_JOIN_INDIA_AND_LONDON_STATES`.

---

## 1. British Library directly defines Board's Collections as extracts from Indian Proceedings

British Library `IOR/F/4` scope:

Board's Collections consist of copies of papers on a given subject extracted from the Proceedings of Indian governments and other East India Company administrations, together with copies of previous overseas correspondence.

This means a Board's Collection is not an unrelated London thematic dossier assembled arbitrarily after the fact. Its normal documentary source is the proceedings business of the Indian administrations.

Encode:

`INDIAN_PROCEEDINGS -> F4_SUBJECT_COLLECTION = DIRECT_BL_SERIES_ARCHITECTURE`.

For the paper project this matters because the Political Consultation / Proceedings layer and the Board's Collection layer now have a formally documented derivational relation.

---

## 2. Political Board's Collections are a virtually complete duplicate of `IOR/P`

British Library explicitly says that almost all Political Collections have been preserved and may therefore be considered a **virtually complete duplicate** of Indian Political Proceedings `IOR/P`.

This is the strongest series-level statement yet recovered for the London duplication architecture.

Correct use:

`F4_POLITICAL_COLLECTIONS ~ VIRTUALLY_COMPLETE_DUPLICATE_OF_IOR_P = DIRECT_SERIES_LEVEL`.

Incorrect use:

`ANY_ONE_F4_ITEM = ANY_ONE_IOR_P_CONSULTATION_ITEM`.

The Board's Collections are subject extractions/recompilations. One F/4 file may contain copies of several proceedings items, prior correspondence and material spanning a period longer than one consultation. Therefore exact item equivalence requires content/register control.

Mechanism:

`SERIES_LEVEL_DUPLICATION_DOES_NOT_ERASE_PACKET_TRANSFORMATION`.

---

## 3. `IOR/F/4/2006/89528` now sits inside a directly controlled derivation class

Wave 83 established:

`IOR/F/4/2006/89528`

Date range:

`Mar 1842-Nov 1842`.

Catalogue scope includes:

- Darjeeling boundary-mark business;
- Birch Hill road;
- public works;
- Campbell's report on the result of his experiment in making paper from paper-tree bark.

Wave 84 can now say more precisely:

because `89528` is a Political Board's Collection item, its documentary class is one whose papers were normally extracted from Indian Political Proceedings and used in London to review a draft Political despatch.

Thus encode:

`F4_89528 = DIRECT_LONDON_POLITICAL_PROCEEDINGS_DERIVATIVE_CLASS`.

Retain:

`F4_89528_CONTAINS_OC_NO70_OR_COPY = HIGH_PRIORITY_TEST / NOT_YET_PROVEN`.

The new evidence raises the probability of a direct No.70 relation but does not substitute for inspection.

---

## 4. Board's Collections were reorganised around associated `IOR/E/4` draft despatches

British Library states that the physical arrangement of Board's Collections follows the **draft numbers and dates of the associated despatches in `IOR/E/4`**.

This changes the retrieval logic. The Board's Collection is not necessarily arranged by the original Indian consultation date.

Expected transformation:

`INDIA CONSULTATION DATE / NUMBER`
-> `PROCEEDINGS SUBJECT PAPERS`
-> `LONDON SUBJECT COLLECTION`
-> `ASSOCIATED DRAFT DESPATCH NUMBER / DATE`.

Therefore the fact that `89528` covers Mar–Nov 1842 does not imply that the associated London despatch was dated inside that range. BL explicitly warns that there is normally a time gap between Collection document dates and the associated despatch date; in the later period this was often about a year or less.

Encode:

`SOURCE_DOCUMENT_DATE != BOARDS_COLLECTION_USE_DATE != ASSOCIATED_DESPATCH_DATE`.

This extends the multi-date documentary model built in Waves 79–80.

---

## 5. `IOR/E/4` supplies the draft-despatch endpoint

British Library `IOR/E/4` describes the general India correspondence system and includes:

- `IOR/E/4/148-288` — Letters received from India and Bengal, 1834–1858;
- `IOR/E/4/740-855` — Despatches to India and Bengal, Original Drafts.

The catalogue also states that Political correspondence is regularly included, while enclosures are generally not bound with letters received and may instead survive in `IOR/F/4`, `IOR/P`, and other departmental series.

British Library:

https://searcharchives.bl.uk/catalog/036-001036642

For Campbell 1842, the target endpoint is therefore not yet an exact E/4 volume but the controlled series range:

`ASSOCIATED_DRAFT_DESPATCH -> IOR/E/4/740-855 = SERIES-LEVEL TARGET`.

Do not interpolate an exact E/4 volume from date sequence.

---

## 6. Contemporary Board's Collection registers provide the next exact crosswalk

British Library finding aid statement for `IOR/F/4` names contemporary registers:

`IOR/Z/F/4/1-18`, seasons 1794/95–1858.

Subseries:

`IOR/Z/F/4 — Registers of Board's Collections`.

British Library:

https://searcharchives.bl.uk/catalog/037-004319122

Two volumes are immediately relevant.

### 1841

`IOR/Z/F/4/7`

Title:

`Register of Board's Collections`.

Scope:

`Nos. 498 (1839) - 942 (1841)`.

Date range:

`1839-1841`.

This is the first register target for the O'Shaughnessy bleaching report associated with Political Consultation 29 Nov 1841 No.147.

### 1842

`IOR/Z/F/4/8`

Title:

`Register of Board's Collections`.

Scope:

`Nos. 1 (1842) - 302 (1844)`.

Date range:

`1842-1844`.

This is the first register target for `IOR/F/4/2006/89528` and Campbell's 1842 paper report.

Critical numbering guardrail:

The catalogue's `Nos. 1–302` and `Nos. 498–942` describe the register sequence. Their relation to the later global Board's Collection item number `89528`, consultation No.70, or No.147 is **not yet controlled**.

Do not encode:

`REGISTER_NO = 89528`

or

`REGISTER_NO = CONSULTATION_NO`.

---

## 7. Draft registers provide the next link after the Board's Collection register

British Library:

`IOR/Z/F/3 — Registers of Drafts`.

Date range:

`1836-1858`.

Its first sequence covers:

`1-988 (1836-1844)`.

British Library:

https://searcharchives.bl.uk/catalog/037-004319109

This gives a plausible finding-aid chain:

`F4 COLLECTION ENTRY`
-> `associated draft number/date`
-> `IOR/Z/F/3 draft register`
-> `IOR/E/4 original draft despatch`.

The precise information fields in the relevant register pages remain to be inspected; do not assert in advance that every F/4 register entry directly prints the E/4 shelfmark.

Encode:

`IOR_Z_F_3 = HIGH_PRIORITY_DRAFT_CROSSWALK`.

---

## 8. `IOR/Z/E/4/16` gives an independent India/Bengal despatch index route

British Library:

`IOR/Z/E/4/16`

Title:

`Index to India and Bengal Despatches`.

Date range:

`1839-1842`.

British Library:

https://searcharchives.bl.uk/catalog/040-001081702

The volume has thousands of alphabetically arranged entries and is digitised through the East India Company archive platform.

It should be searched under:

- Campbell;
- Darjeeling / Darjiling;
- Paper;
- Paper tree;
- Manufacture(s);
- Experiment(s);
- station/locality headings.

Current web indexing has not exposed a controlled Campbell/Darjeeling paper entry.

Use:

`IOR_Z_E_4_16 = INDEPENDENT_DESPATCH_INDEX_CROSSCHECK`.

Do not interpret search-engine silence as archival absence.

---

## 9. Two-directional crosswalk for Campbell 1842

The archive can now be attacked from both ends.

### India-first route

`Campbell -> Bushby, 21 Apr 1842`
-> `Political Original Consultation 11 May 1842 No.70`
-> `IOR/P/196/12`
-> identify subject papers / adjacent numbers
-> locate corresponding F/4 Political Collection
-> identify associated draft/despatch.

### London-first route

`IOR/F/4/2006/89528`
-> `IOR/Z/F/4/8`
-> identify associated draft number/date
-> `IOR/Z/F/3`
-> `IOR/E/4 original draft despatch`
-> use subject/date references to map back to `IOR/P/196/12` and No.70.

This is now the preferred method because either side can compensate for an inaccessible or poorly indexed witness.

Mechanism:

`BIDIRECTIONAL_ARCHIVAL_CROSSWALK_REDUCES_DEPENDENCE_ON_ONE_SURVIVING_PACKET`.

---

## 10. The same London-first method can solve the 1841 bleaching file

Controlled India-side identity:

`Political Consultation 29 Nov 1841, No.147`
=
O'Shaughnessy's report on the method of bleaching paper manufactured at Darjeeling.

The exact IOR/P volume remains unresolved.

Wave 84 adds a second route:

`exact report title / O'Shaughnessy / Darjeeling bleaching`
-> search 1841 Political Board's Collections and subject indexes
-> `IOR/Z/F/4/7`
-> identify F/4 Collection + associated draft/despatch
-> use the London references to back-resolve the corresponding IOR/P volume.

This may be easier than continuing to infer the IOR/P volume from chronology.

Search vocabulary:

`O'Shaughnessy`, `Oshaughnessy`, `Darjeeling`, `Darjiling`, `paper`, `bleaching`, `manufacture`, `chemical examiner`, `red lead`, `manganese`.

---

## 11. Board's Collection transformation changes context as well as location

Campbell's paper report appears in `89528` beside roads, public works and boundary administration. At consultation level, the same paper business may have sat beside entirely different Political items numbered on 11 May.

The Board's Collection process therefore performs at least two archival transformations:

1. **selection by subject/administrative usefulness** from Indian Proceedings;
2. **reordering around a London draft despatch**.

This creates a documentary history in which the same report can acquire different neighbours in India and London.

Mechanisms:

- `ARCHIVAL_NEIGHBOURHOOD_CHANGES_ACROSS_DERIVATIVE_STATES`;
- `DOCUMENTARY_CONTEXT_IS_PRODUCED_BY_ADMINISTRATIVE_REPACKAGING`.

This is important for paper history because technological material may become visible under a locality/despatch packet rather than a dedicated `paper` heading.

---

## 12. Revised relation between `IOR/P`, `F/4`, `E/4` and `L/PS/6`

Current hierarchy for the Political paper project:

### Closest to India-side consultation processing

`Political Original Consultation / Political Proceedings`
-> `IOR/P`.

### London subject duplicate / review packet

`IOR/F/4 Board's Collections`.

For Political material, BL calls this a virtually complete duplicate of `IOR/P` at series level.

### London outgoing draft correspondence

`IOR/E/4/740-855` original draft despatches to India and Bengal.

### London incoming Political-letter copies / later departmental transmission witnesses

`IOR/L/PS/6` and related E/4 received-letter series, where independently applicable.

Thus `L/PS/6` remains valuable but should not be treated as the primary mirror of an India-side consultation when an F/4 Political Collection exists.

---

## Source-control rules

1. British Library directly states that Board's Collections are extracted from Indian Government Proceedings and previous overseas correspondence.
2. British Library directly states that almost all Political Collections survive and may be considered a virtually complete duplicate of Indian Political Proceedings `IOR/P`.
3. This is a series-level duplication statement; it does not make one F/4 file identical to one consultation item.
4. `IOR/F/4/2006/89528` is now a direct member of this Political Proceedings-derivative class and directly contains Campbell's paper-experiment report.
5. `F4/89528 = Political Consultation 11 May 1842 No.70` remains pending document/register crosswalk.
6. Board's Collections are physically arranged according to associated draft despatch numbers/dates in `IOR/E/4`; their source-document dates can predate the despatch.
7. Use `IOR/Z/F/4/8` for 1842 Board's Collection registration and `IOR/Z/F/4/7` for 1841.
8. Do not equate the number ranges in those registers with consultation numbers or global Collection item numbers until images explain the numbering system.
9. Use `IOR/Z/F/3` as the draft-register route and `IOR/Z/E/4/16` as an independent India/Bengal despatch index.
10. `IOR/E/4/740-855` is the controlled original-draft series range for India/Bengal; exact target volume remains unresolved.
11. Continue to keep `IOR/P`, `F/4`, `E/4`, `L/PS/6` as distinct documentary states.
12. Search-engine non-discovery in the large alphabetical indexes is not evidence of archival absence.

## Immediate next actions

1. Inspect/request `IOR/Z/F/4/8` and locate the register entry corresponding to `IOR/F/4/2006/89528` or its Darjeeling subject.
2. Extract the associated draft number/date and any department/subject field.
3. Follow that draft through `IOR/Z/F/3` into the exact `IOR/E/4` original draft despatch.
4. Search `IOR/Z/E/4/16` as an independent check on the despatch identity.
5. Compare the recovered London despatch/Collection references with `IOR/P/196/12`, 11 May 1842 No.70 ± adjacent items.
6. Inspect/request `IOR/Z/F/4/7` for an 1841 Political Collection entry matching O'Shaughnessy's Darjeeling paper-bleaching report.
7. If recovered, use its associated draft/despatch to back-resolve the exact IOR/P volume containing 29 Nov 1841 No.147.
8. Search the nominal/subject index to the Board's Collections covering seasons through 1842 for Campbell, Darjeeling, O'Shaughnessy and paper.
9. Maintain the independent Halliday/Woodcock/Champaran material-logistics line.

## Bottom line

Wave 84 turns the Campbell paper file from a thematic London analogue into part of a formally documented derivative system. British Library states that Board's Collections were assembled by extracting subject papers from Indian Government Proceedings, that they were reorganised for Board of Control review of draft despatches, and that the surviving Political Collections constitute a virtually complete duplicate of Indian Political Proceedings `IOR/P`. Thus `IOR/F/4/2006/89528`, which directly contains Campbell's report on the result of his Darjeeling paper experiment, belongs to the same documentary family as the India Political Proceedings by archival design. The exact relation to Political Consultation 11 May 1842 No.70 still needs proof, but the proof now has a defined route: `IOR/Z/F/4/8 -> IOR/Z/F/3 -> IOR/E/4`, checked against `IOR/P/196/12`. The 1841 O'Shaughnessy bleaching report can be attacked symmetrically through `IOR/Z/F/4/7`, potentially solving its still-missing exact IOR/P volume from the London side rather than by chronological interpolation.