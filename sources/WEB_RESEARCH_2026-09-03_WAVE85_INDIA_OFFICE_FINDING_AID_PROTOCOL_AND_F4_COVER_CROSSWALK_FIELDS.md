# Web/archive research 2026-09-03 — Wave 85
## India Office finding-aid protocol for later Board's Collections, and the draft / previous-communication / collection-number cover fields

Date: 2026-09-03

Status: active paper-history mainline. Follow-up to Wave 84. This wave does not identify the missing draft number for `IOR/F/4/2006/89528`. It establishes, from an India Office Library subject guide and digitised Board's Collection title pages, exactly how later F/4 material is meant to be traced and what cross-reference fields can physically appear on a Collection cover.

## Executive result

Amar Kaur Jasbir Singh's 1988 *Guide to Source Materials in the India Office Library and Records for Tibet, Sikkim and Bhutan, 1765–1950* gives an operational description of the `E/4`–`F/4` system highly relevant to Darjeeling.

The guide states that:

- `E/4` indexes should be used to trace relevant despatches;
- once a despatch is found, researchers can work backward to the Bengal/India letter under reply and across to Board's Collections for enclosures/background papers;
- Board's Collections contain copies of correspondence, minutes, resolutions and other papers cited in or enclosed with Bengal/India letters;
- most F/4 material consists of extracts from India Proceedings;
- their subject arrangement can make them easier to use than the Proceedings;
- but they are arranged according to the numbers and dates of the Court of Directors' **answering draft despatches**, not according to the dates/numbers of the Indian letters;
- for later Collections researchers should use `IOR/Z/F/4/1-18` Registers of Board's Collections;
- those registers are themselves **not indexed**, so one must either browse them or identify Collections through draft numbers and related details in `E/4` Despatch volumes.

Source:

Amar Kaur Jasbir Singh, *Guide to Source Materials in the India Office Library and Records for Tibet, Sikkim and Bhutan, 1765–1950* (1988).

Public scan:

https://www.pahar.in/pahar/Books%20and%20Articles/Indian%20Subcontinent/1988%20Guide%20to%20Source%20Materials%20in%20India%20Office%20Library%20on%20Tibet%20Sikkim%20and%20Bhutan%20by%20Singh%20s.pdf

This confirms that the bidirectional workflow defined in Wave 84 is the repository's own recommended retrieval logic, not a project-invented heuristic.

A second structural control comes from digitised Qatar Digital Library Board's Collection items. Title pages in neighbouring 1842–43 Political Collections visibly carry fields such as:

`Draft 612/43`

`P.C. [Previous Communication] 3902`

`Collection No 11`

or

`Collection No 12`.

Examples:

- `IOR/F/4/2006/89515` — title page records `Draft 612/43`, `P.C. 3902`, `Collection No 11`;
- `IOR/F/4/2006/89516` — title page records `Draft 612/43`, `P.C. 3902`, `Collection No 12`.

These are Gulf/Bombay Political items, not Darjeeling material, and their draft number must **not** be transferred to `89528`. Their significance is material-archival: F/4 cover sheets can encode precisely the crosswalk fields we need to recover for Campbell's file.

Thus the immediate object-level question becomes:

**what are the Draft, P.C./Previous Communication, and Collection No fields on the title page or register entry for `IOR/F/4/2006/89528`?**

Core mechanisms:

- `FINDING_AID_PROTOCOL_IS_BIDIRECTIONAL`
- `F4_REGISTERS_ARE_UNINDEXED_AND_REQUIRE_BROWSING_OR_DRAFT_CONTROL`
- `E4_DRAFT_NUMBER_CAN_RECOVER_F4_COLLECTION`
- `F4_COVER_CAN_ENCODE_DRAFT_PC_AND_COLLECTION_NUMBER`
- `GLOBAL_SHELFMARK_NUMBER_IS_NOT_COVER_COLLECTION_NUMBER`
- `BOARD_COLLECTION_SUBJECT_ORDER_REPLACES_INDIAN_CHRONOLOGICAL_ORDER`
- `FINDING_AID_METADATA_IS_A_DOCUMENTARY_STATE`.

---

## 1. India Office Library's own Sikkim/Tibet/Bhutan guide confirms the E/4 -> F/4 method

The 1988 guide is unusually well matched to this project because its remit includes Sikkim and therefore Darjeeling-related Political records.

Its description of E/4 says the indexes are comprehensive and useful for locating relevant despatches in long correspondence series. Once the despatch is identified, the researcher can:

`DESPATCH`
-> `LETTER FROM BENGAL / INDIA UNDER REPLY`
+
`BOARD'S COLLECTION FOR ENCLOSURES / BACKGROUND PAPERS`.

This produces a direct operational inversion of the India-first route:

`E4 DESPATCH`
-> `DRAFT NUMBER / SUBJECT`
-> `F4 COLLECTION`
-> `INDIAN PROCEEDINGS / LETTERS`.

The guide is therefore an independent repository-method control on Wave 84's bidirectional crosswalk.

Encode:

`BIDIRECTIONAL_CROSSWALK = INDIA_OFFICE_RECOMMENDED_METHOD`.

---

## 2. F/4 subject arrangement is a transformation, not merely duplication

The guide explains that most Board's Collection material consists of extracts from India Proceedings related to particular subjects. The subject arrangement can make F/4 easier to use than the Proceedings themselves.

But this convenience comes from reordering.

Proceedings logic:

`CONSULTATION DATE / ITEM NUMBER / ADMINISTRATIVE SEQUENCE`.

Board's Collection logic:

`SUBJECT EXTRACTION`
-> `ANSWERING DRAFT DESPATCH NUMBER / DATE`.

Thus the same Campbell report changes archival coordinates between India and London.

Mechanism:

`RETRIEVAL_EASE_IS_PRODUCED_BY_CONTEXTUAL_REORDERING`.

This helps explain why a single F/4 Darjeeling file can combine paper manufacture, roads, boundary marks and public works despite the underlying India-side business having been processed through date-local Political consultations.

---

## 3. Later F/4 registers are unindexed

The guide explicitly warns that the later Board's Collection registers are not themselves indexed.

For the relevant period:

- `IOR/Z/F/4/7` = 1839–1841;
- `IOR/Z/F/4/8` = 1842–1844.

Therefore a search failure for Campbell/O'Shaughnessy in web-indexed metadata tells us little. The primary finding-aid operation may simply require browsing register entries.

Two official/recommended methods:

### Method A — browse the register

`Z/F/4 volume`
-> inspect entries sequentially
-> identify subject / collection / draft relation.

### Method B — start from E/4

`relevant despatch / draft`
-> obtain draft number and related details
-> use them to locate the Board's Collection entry in Z/F/4.

This means the current bottleneck is expected from the archive's design, not evidence that the paper transaction disappeared.

Mechanism:

`UNINDEXED_REGISTER_CREATES_RETRIEVAL_FRICTION_WITHOUT_ARCHIVAL_GAP`.

---

## 4. Digitised F/4 title pages show the physical crosswalk vocabulary

Qatar Digital Library / British Library items in the same broad 1842–43 Political Board's Collection environment preserve title-page references.

### `IOR/F/4/2006/89515`

The title page carries:

- `Draft 612/43`;
- `P.C. [Previous Communication] 3902`;
- `Collection No 11`.

The item is a Bombay Political/Persian Gulf file.

### `IOR/F/4/2006/89516`

The title page carries:

- `Draft 612/43`;
- `P.C. 3902`;
- `Collection No 12`.

Again this is Bombay/Gulf business.

QDL/BL records:

https://searcharchives.bl.uk/catalog/041-000755008

https://www.qdl.qa/download/pdf/81055_vdc_100000000344.0x0002be_en.pdf

The first item is also represented in QDL/BL metadata as `IOR/F/4/2006/89515`.

These examples demonstrate that the paper title page / docket can preserve at least three retrieval dimensions:

`DRAFT NUMBER/YEAR`
+
`PREVIOUS COMMUNICATION REFERENCE`
+
`COLLECTION NUMBER`.

For `89528`, these fields are currently unknown because the file is not publicly digitised in the BL catalogue.

---

## 5. Do not propagate `Draft 612/43` from neighbouring Gulf items to Darjeeling

`89515` and `89516` share parent physical volume `IOR/F/4/2006` with `89528`, but the parent volume contains mixed Political business from multiple governments and regions.

The global sequence includes Persian Gulf, Mysore, Coorg, Rajasthan states, Nepal, Darjeeling, Gwalior, Hyderabad and Indore.

Therefore:

`SAME_PHYSICAL_F4_VOLUME != SAME_DRAFT_DESPATCH`.

Although two digitised neighbouring items happen to share `Draft 612/43`, the current evidence does not establish that later siblings in the volume do.

Encode:

`F4_89528_DRAFT_NUMBER = UNKNOWN`.

Do not encode:

`F4_89528 -> DRAFT_612_43`.

This guardrail is especially important because the nearby Gulf examples make a tempting but unsupported sequential interpolation possible.

---

## 6. Global Board's Collection item number and historical Collection No are distinct identifiers

Modern shelfmark:

`IOR/F/4/2006/89528`.

The neighbouring digitised examples show historical title-page values such as:

`Collection No 11`

or

`Collection No 12`.

Thus the terminal modern shelfmark number (`89515`, `89516`, `89528`) is not automatically the historical `Collection No` printed on the cover.

Likewise, `Political Consultation No.70` belongs to an India-side consultation numbering system.

At least three number systems must remain separate:

1. `POLITICAL CONSULTATION ITEM NUMBER` — e.g. No.70;
2. `HISTORICAL BOARD'S COLLECTION NUMBER` — to be recovered from F/4 cover/register;
3. `MODERN / GLOBAL F4 ITEM IDENTIFIER` — e.g. 89528.

Potential fourth system:

4. `DRAFT DESPATCH NUMBER/YEAR`.

Mechanism:

`ARCHIVAL_CROSSWALK_REQUIRES_NUMBER_SYSTEM_DISAMBIGUATION`.

---

## 7. Previous Communication (`P.C.`) is another derivative edge

The QDL examples expand `P.C.` as `Previous Communication`.

This field can connect one Board's Collection/draft to an earlier London communication.

For Campbell's paper experiment, recovery of a P.C. reference could reveal:

- earlier Darjeeling correspondence;
- prior Government/Court discussion of paper manufacture;
- continuity with a previous draft/despatch;
- or another administrative matter folded into the same subject chain.

No P.C. value is yet known for `89528`.

Encode:

`F4_COVER_PC_FIELD = POTENTIAL_DOCUMENT_GENEALOGY_EDGE`.

Do not assume that it refers to the 1841 O'Shaughnessy bleaching transaction or the 1837 paper programme without direct evidence.

---

## 8. Revised exact retrieval target for `89528`

Instead of asking only for “the Campbell report”, object-level extraction should capture the whole front matter and docket system.

When `IOR/F/4/2006/89528` is inspected, record:

1. full title page / cover transcription;
2. Draft number/year;
3. P.C. / Previous Communication reference;
4. historical Collection No;
5. any Department/branch label;
6. any letter/despatch number under reply;
7. contents page;
8. individual document dates;
9. sender/addressee of Campbell report;
10. Political Consultation / Proceedings citations;
11. enclosure numbers;
12. reply/minute/despatch references.

This metadata may solve the crosswalk before the full body text is transcribed.

Mechanism:

`COVER_METADATA_CAN_RESOLVE_DOCUMENT_GENEALOGY_BEFORE_TEXTUAL_ANALYSIS`.

---

## 9. Revised exact retrieval target for the 1841 O'Shaughnessy report

India-side address is secure:

`Political Consultation 29 Nov 1841, No.147`.

The 1937 IRD exhibit gives the report identity.

London-first route now becomes:

1. browse `IOR/Z/F/4/7` or use an E/4 Political despatch index;
2. identify Board's Collection subject entry for O'Shaughnessy / Darjeeling bleaching;
3. retrieve the F/4 file;
4. capture its Draft / P.C. / Collection No cover fields;
5. use those fields to locate the E/4 draft and back-resolve the IOR/P volume.

This is a more archival-native strategy than trying to guess the IOR/P volume solely by November chronology.

---

## 10. Information-resolution hierarchy is now clearer

The 1988 guide and BL series descriptions imply different information densities:

`FULL INDIA PROCEEDINGS / ORIGINAL CONSULTATION`
may preserve fuller transaction sequence;

`F4 SUBJECT COLLECTION`
preserves selected/copied material useful to a London answering draft, often with enclosures/background papers;

`E4 DRAFT DESPATCH`
preserves the proposed/approved London response rather than all source papers;

`INDEX / REGISTER`
preserves identifiers and routing metadata.

Thus even when F/4 is called a virtually complete duplicate of Political Proceedings at series level, the individual documentary state may be extractive and selectively reorganised.

Mechanism:

`SERIES_COMPLETENESS != ITEM_INFORMATION_EQUIVALENCE`.

---

## Source-control rules

1. The 1988 India Office Library guide independently confirms the E/4–F/4–Proceedings retrieval architecture.
2. Later F/4 registers are unindexed; browsing or draft-number control is expected.
3. Board's Collections are arranged by answering draft despatch numbers/dates, not by India-side letter/consultation dates.
4. QDL digitised title pages directly demonstrate `Draft`, `P.C.`, and `Collection No` cross-reference fields.
5. The Gulf/Bombay title-page values are structural controls only; do not transfer `Draft 612/43`, `P.C. 3902`, or Collection Nos 11/12 to Campbell's Darjeeling file.
6. `89528` is a modern/global F/4 item identifier, not automatically the historical Collection No.
7. Political Consultation No.70, F/4 historical Collection No, F/4 item 89528 and draft despatch number are separate numbering systems.
8. P.C. means Previous Communication in the controlled QDL examples; `89528` P.C. value remains unknown.
9. Capture F/4 front matter as archival evidence, not merely the Campbell report body.
10. Series-level virtual duplication between F/4 Political Collections and IOR/P does not imply item-level information equivalence.

## Immediate next actions

1. Obtain the cover/title page or register entry for `IOR/F/4/2006/89528` and recover Draft / P.C. / historical Collection No.
2. Use the recovered draft number in `IOR/Z/F/3` and the relevant `IOR/E/4` original draft despatch.
3. Cross-check the despatch in `IOR/Z/E/4/16`.
4. Map the resulting source references back to `IOR/P/196/12`, Political Consultation 11 May 1842 No.70 ± adjacent items.
5. Browse `IOR/Z/F/4/7` for the exact O'Shaughnessy 1841 Darjeeling bleaching subject.
6. Recover the corresponding F/4 cover metadata and use it to solve the exact IOR/P volume for No.147.
7. Preserve every identifier in separate dataset fields.
8. Continue the material Halliday/Woodcock/Champaran branch independently.

## Bottom line

Wave 85 converts the archival architecture into an object-level retrieval protocol. The India Office Library's own 1988 Sikkim/Tibet/Bhutan guide says that later Board's Collections must be traced either by browsing their unindexed `Z/F/4` registers or by starting from the answering `E/4` draft despatch and using its draft number to recover the Collection. Digitised F/4 title pages show why this works: their covers physically encode Draft number/year, Previous Communication reference, and historical Collection No. The missing fact for Campbell's `IOR/F/4/2006/89528` is therefore very specific. We need its cover metadata. Once the Draft/P.C./Collection fields are recovered, the London side can be joined to `IOR/E/4` and then tested directly against Political Consultation 11 May 1842 No.70 in `IOR/P/196/12`. The same method gives a non-interpolative route to the still-missing London volume for O'Shaughnessy's 29 Nov 1841 No.147.