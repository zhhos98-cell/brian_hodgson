# Web/archive research 2026-09-03 — Wave 81
## Abdul Ali's archival provenance, pre-1843 Political Department control, and the IOR/P consultation mirror

Date: 2026-09-03

Status: active paper-history mainline. Follow-up to Waves 79–80. This wave does **not** recover the exact images of Political Original Consultation 29 Nov 1841 No.147 or 11 May 1842 No.70. It strengthens their archival provenance, corrects the contemporaneous departmental chronology, and identifies a much closer London-side consultation witness in `IOR/P` than the `IOR/L/PS/6` transmission copies used provisionally in Wave 78.

## Executive result

Wave 80 decoded Abdul Ali's `Political O.C.` as `Political Original Consultation`. Wave 81 adds three converging controls.

First, A. F. M. Abdul Ali was not merely a later historian extracting isolated documents. The National Archives of India states that its earliest official publication, the 1925 *A Hand-book to the Records of the Government of India in the Imperial Record Department, 1748–1859*, was produced under the guidance of **A. F. M. Abdul Ali, Keeper of Records, Imperial Record Department**. NAI institutional history independently lists A. F. M. Abdul Ali as head of the Imperial Record Department from **1922 to 1938**. The 1944 article `The Daphne Paper of Nepal` is signed A. F. M. Abdul Ali, M.A., F.R.A.S.B. and itself cites Hilary Jenkinson's *Manual of Archive Administration*. Exact-name/initial identity, career chronology, archival publications and the article's archival vocabulary make identification of the 1944 author with the former Keeper of Records **very high confidence**, although no single biographical source recovered in this wave explicitly says “the author of The Daphne Paper of Nepal is the former Keeper”.

Second, the Political records used in 1841–42 belong to a **pre-Foreign-Department Political Department record regime**. The 1925 Imperial Record Department handbook's institutional chronology states that after the short-lived `Secret and Political Department` nomenclature in 1786–89, the Political Department formed a separate records series from 1790. The formal **Foreign Department was created in May 1843**. Therefore Abdul Ali's phrase `Foreign and Political Department` is best treated as retrospective archival/record-group language. For our target transactions in November 1841 and May 1842, the contemporaneous branch identity is `Political Department` unless a source itself assigns a specific item to another branch.

Third, London preserves a consultation-level counterpart in `IOR/P`. Published scholarship explicitly cites `India Political Consultations` by the same consultation date and number used in National Archives of India references. A particularly strong cross-repository control states that `India Political Consultation No.50, 1 March 1843` survives both in the National Archives of India and the India Office Records, where the London volume is `IOR/P/196/28`. Another academic citation gives `IOR/P/194/37 = India Political Consultations, 8 February 1837, No.62`. This means the immediate London recovery path for Abdul Ali's `Political O.C.` is not first the transmitted Political Letters in `IOR/L/PS/6`; it is the **India Political Consultations / Proceedings series in IOR/P**.

Known `IOR/P` chronological anchors narrow, but do not yet identify, the target volumes:

- `IOR/P/195/55`: India Political Consultations, 12–26 Apr 1841;
- `IOR/P/195/56`: 3–24 May 1841;
- `IOR/P/196/4`: 13–30 Dec 1841;
- `IOR/P/196/10`: 7–30 Mar 1842;
- `IOR/P/196/13`: includes 1 Jun 1842;
- `IOR/P/196/28`: includes 1 Mar 1843, No.50;
- `IOR/P/196/29`: 29 Mar–12 Apr 1843.

Thus:

`29 Nov 1841 No.147`
-> lies shortly before `IOR/P/196/4`;

`11 May 1842 No.70`
-> lies between the controlled March volume `IOR/P/196/10` and the controlled June volume `IOR/P/196/13`.

Do **not** convert those brackets into inferred exact shelfmarks. The target volumes remain unresolved pending direct catalogue/index control.

Core mechanisms:

- `ARCHIVIST_CITATION_PROVENANCE_RAISES_SERIES_CONFIDENCE`
- `CONSULTATION_ADDRESS_IS_REPOSITORY_NATIVE_NOT_LATER_PARAPHRASE`
- `POLITICAL_DEPARTMENT_PRECEDES_FORMAL_FOREIGN_DEPARTMENT`
- `NAI_AND_IOR_CAN_SHARE_CONSULTATION_DATE_NUMBER_IDENTITY`
- `IOR_P_IS_A_CONSULTATION_LEVEL_LONDON_WITNESS`
- `LPS_6_IS_A_LATER_TRANSMISSION_DERIVATIVE_NOT_THE_FIRST_MIRROR`
- `VOLUME_BRACKETING_NARROWS_WITHOUT_IDENTIFYING`
- `CONSULTATION_DATE_NUMBER_SURVIVES_REPOSITORY_TRANSFER`.

---

## 1. A. F. M. Abdul Ali was Keeper of Records of the Imperial Record Department

National Archives of India, catalogue of publications:

https://nationalarchives.nic.in/en/outreach-activities/catalogue-publications

NAI publication-history PDF:

https://nationalarchives.nic.in/sites/default/files/2023-08/Pub_Sec_A.pdf

The NAI states that the earliest official publication of the department was:

*A Hand book to the Records of the Government of India in the Imperial Record Department, 1748–1859*.

It further states that this work was brought out in 1925 under the guidance of:

`Shri A. F. M. Abdul Ali, Keeper of Records, Imperial Record Department`.

This is not incidental provenance. The handbook's purpose was specifically to make the record system searchable by historical researchers and to explain departmental provenance and finding aids.

Encode:

`A_F_M_ABDUL_ALI_1925_ROLE = KEEPER_OF_RECORDS_IRD = DIRECT_NAI`.

---

## 2. Abdul Ali headed the archive through 1922–1938

NAI institutional-history material lists heads of the Imperial Record Department / National Archives of India and gives:

`A. F. M. Abdul Ali — 1922 to 1938`.

A separate NAI history account describes his tenure as nearly seventeen years and notes that it was unusually long.

This matters chronologically because his 1944 article appeared only six years after the end of that tenure.

Encode:

`ABDUL_ALI_IRD_HEAD_TENURE = 1922_1938 = DIRECT_NAI`.

The article is therefore temporally close to his professional archival career.

---

## 3. Identity of the 1944 Nepal-paper author with the archivist is very high confidence

Direct 1944 article control:

A. F. M. Abdul Ali, `The Daphne Paper of Nepal`, *Bengal: Past and Present*, vol. 64, serial 127 (1944), pp.18–30.

Internet Archive text:

https://archive.org/stream/dli.calcutta.04040/H00220_djvu.txt

The contents and article identify the author as:

`A. F. M. Abdul Ali, M.A., F.R.A.S.B.`

The article uses record-series citations such as:

- `Pol. O.C., no.19, Jany. 13, 1832`;
- `Political O.C., 29 Nov. 1841, no.147`;
- `Political O.C., 11 May 1842, no.70`.

It also cites Hilary Jenkinson's *A Manual of Archive Administration*.

Other bibliographic traces attribute archive-focused publications to A. F. M. Abdul Ali, including work on Burma records in the Imperial Record Department.

Source-control level:

`1944_NEPAL_PAPER_AUTHOR = FORMER_IRD_KEEPER` -> `VERY_HIGH_CONFIDENCE_IDENTITY`.

Do not encode:

`DIRECT_BIOGRAPHICAL_LINK = SECURE`

until a source explicitly links the article title to the Keeper's biography. The present convergence is nevertheless strong enough to treat the article's archival citation language as professional repository-native usage rather than casual secondary shorthand.

Mechanisms:

- `ARCHIVIST_AUTHORED_SECONDARY_SOURCE_HAS_FINDING_AID_PROVENANCE`;
- `ARCHIVAL_SHORTHAND_CAN_PRESERVE_REPOSITORY_NATIVE_ADDRESS`.

---

## 4. Abdul Ali helped shape the finding-aid environment later used in his article

The 1925 handbook's foreword explains that it was prepared under the Indian Historical Records Commission resolution requiring record offices to compile descriptive handbooks supplementary to printed lists/catalogues and manuscript indexes.

A search-text copy is available at Tamil Digital Library:

https://tamildigitallibrary.in/Articles/%E0%AE%A8%E0%AF%82%E0%AE%B2%E0%AF%8D-24258-A%20hand%20book%20to%20the%20Records%20of%20the%20Government%20of%20India%20in%20the%20Imperial%20Record%20Department%2C%201748%20to%201859

The foreword is signed:

`A. F. M. ABDUL ALI`.

The handbook says its purpose is to let researchers determine whether the Imperial Record Department contains material for a specific line of inquiry before proceeding to printed lists and manuscript indexes. It also stresses preservation of original departmental groupings according to the `principle of origin`.

Thus the same archival professional later writing about Nepal paper had direct institutional experience with:

- departmental provenance;
- printed lists;
- manuscript indexes;
- original groupings;
- consultation/proceedings structures.

This strengthens Wave 80's interpretation of `Political O.C.` as a precise archival address.

---

## 5. 1841–42 records belong to the Political Department before the formal Foreign Department

The 1925 handbook's institutional narrative gives the following broad sequence:

- Secret Department created in 1763;
- during part of 1786–89, `Secret and Political Department` nomenclature used;
- Political Department then differentiated;
- from the beginning of 1790, Political proceedings form a separate series;
- formal Foreign Department created in **May 1843**.

Dewar's 1920 handbook independently lists Imperial Record Department holdings including:

- `Political Proceedings`, 1790–1859;
- `Political Consultations`, 1790–1859;
- `Foreign Proceedings`, 1784–1842;
- `Foreign Original Consultations`, 1783–1842.

Dewar:

https://archive.org/details/handbooktoenglis00dewa

1925 handbook bibliographic control:

https://openlibrary.org/works/OL6023493W/A_hand-book_to_the_records_of_the_Government_of_India_in_the_Imperial_Record_Department

This creates a necessary nomenclature distinction.

Abdul Ali's narrative says the nineteenth-century Nepal-paper evidence came from the `Foreign and Political Department`. That phrase is useful for archival provenance but should not be projected backward as the precise contemporaneous administrative title for 1841–42.

For the target records encode:

`1841_1842_CONTEMPORANEOUS_BRANCH = POLITICAL_DEPARTMENT` — high confidence;

`FOREIGN_AND_POLITICAL_DEPARTMENT = RETROSPECTIVE_ARCHIVAL_UMBRELLA / LATER_NOMENCLATURE` — working interpretation.

Guardrail:

Do not force all Darjeeling records into the Political series: contemporaneous archival holdings also contain Foreign and Secret streams. Use the exact citation or index to assign individual documents.

---

## 6. `Political O.C.` is especially credible because Abdul Ali knew the consultation system professionally

Wave 80 established from Dewar and Qeyamuddin Ahmad:

`O.C. = Original Consultation`.

The consultation model explains Abdul Ali's paired dates:

### 1831/32

`8 Dec 1831 Hodgson letter`
-> `Political Original Consultation, 13 Jan 1832, No.19`.

### 1842

`21 Apr 1842 Campbell to Bushby`
-> `Political Original Consultation, 11 May 1842, No.70`.

Wave 81 adds author provenance:

`ABDUL_ALI_CITATION`
+
`FORMER_KEEPER_OF_RECORDS / FINDING_AID_EDITOR`
->
`CONSULTATION_ADDRESS_HAS_HIGH_REPOSITORY_NATIVE_CREDIBILITY`.

This does not magically make his historical interpretation primary evidence. It changes confidence in the **archive address and archival terminology**.

Distinguish:

`ARCHIVAL_ADDRESS_RELIABILITY`
from
`HISTORICAL_INTERPRETATION_RELIABILITY`.

---

## 7. India Political Consultations have a London IOR/P witness

The crucial new retrieval result is that India Political Consultations survive in the India Office Records `IOR/P` series.

A cross-repository example from archival research identifies:

`India Political Consultation No.50, 1 Mar 1843`

in both:

- National Archives of India;
- India Office Records, London: `IOR/P/196/28`.

This shows that consultation date + number can survive as a stable documentary identity across the two repositories.

A second academic citation gives:

`IOR/P/194/37`
=
`India Political Consultations, 8 Feb 1837, No.62`.

Encode:

`NAI_POLITICAL_CONSULTATION_DATE_NO <-> IOR_P_DATE_NO = PROVEN_CROSS_REPOSITORY_IDENTITY_PATTERN`.

This is the most important retrieval correction after Wave 80.

---

## 8. IOR/P is now the first London-side consultation search, ahead of IOR/L/PS/6

Wave 78 used British Library `IOR/L/PS/6` to reconstruct London documentary redundancy:

`Political Letter from India`
-> `Board of Control copy`
-> `register / abstract / index`
-> `E/4 duplicate`.

That architecture remains valid **for transmitted Political Letters**.

But `Political O.C.` is an India-side consultation object. Its closest London counterpart is the series of India Political Consultations / Proceedings in `IOR/P`, not necessarily a Political Letter received in `L/PS/6`.

Revised path:

`INDIA-SIDE ORIGINAL CONSULTATION`
<-> `IOR/P INDIA POLITICAL CONSULTATION / PROCEEDINGS WITNESS`
-> `[if business transmitted to London as a Political Letter]`
-> `IOR/L/PS/6 Political Letter copy`
-> `IOR/E/4 duplicate`
-> `IOR/F/4 / Boards Collections or other enclosure derivatives`.

Thus:

`IOR_P = FIRST_LONDON_CONSULTATION_MIRROR_ROUTE`;

`IOR_L_PS_6 = SECOND_STAGE_TRANSMISSION_ROUTE`.

The word `mirror` should still be used cautiously because the precise physical relation between NAI originals and IOR/P copies can vary; document identity must be checked item by item.

---

## 9. Controlled IOR/P chronology around the targets

Published research provides multiple date/shelfmark anchors.

### 1841

`IOR/P/195/55`
-> India Political Consultations, 12–26 Apr 1841.

`IOR/P/195/56`
-> 3–24 May 1841.

`IOR/P/196/4`
-> 13–30 Dec 1841.

Target:

`29 Nov 1841 No.147`

falls before the controlled Dec volume.

Encode:

`TARGET_1841_IOR_P_VOLUME = BRACKETED_BEFORE_P_196_4 / EXACT_VOLUME_UNRESOLVED`.

Do **not** infer `P/196/2` or `P/196/3` as fact from sequence alone.

### 1842

`IOR/P/196/10`
-> 7–30 Mar 1842.

`IOR/P/196/13`
-> includes 1 Jun 1842.

Target:

`11 May 1842 No.70`

falls between these controlled anchors.

Encode:

`TARGET_1842_IOR_P_VOLUME = BRACKETED_BETWEEN_P_196_10_AND_P_196_13 / EXACT_VOLUME_UNRESOLVED`.

Do **not** silently assign it to `/11` or `/12` until a direct index/catalogue/citation confirms the volume.

### 1843 continuity

`IOR/P/196/28`
-> contains 1 Mar 1843 Political Consultation No.50.

`IOR/P/196/29`
-> 29 Mar–12 Apr 1843.

This confirms that the same volume sequence continues through 1843.

---

## 10. Same-date control on 11 May 1842 confirms local consultation numbering

A later historical study cites an unrelated National Archives of India item as:

`Foreign Department, Political, Consultation 11 May 1842, No.43`

with an underlying letter dated 14 Apr 1842 from Captain Gordon to T. Maddock.

This is valuable not for its subject but for archival mechanics.

On the same consultation date as Abdul Ali's paper item No.70, another transaction appears as No.43.

Thus:

`11 MAY 1842 = MULTI_ITEM POLITICAL CONSULTATION`;

`NO.43` and `NO.70` are compatible with a date-local sequence of distinct business.

This independently supports Dewar's statement that each sitting assigns serial item numbers.

Mechanism:

`SAME_DATE_MULTIPLE_NUMBERS_VALIDATE_CONSULTATION_LOCAL_SEQUENCE`.

---

## 11. The exact target search should use date + number before subject

Because NAI and IOR/P can preserve the same consultation date and number, the highest-value archive address is now:

### Target A

`India Political Consultation`
`29 Nov 1841`
`No.147`

then inspect surrounding numbers.

Subject keys only for verification:

`Maddock`, `O'Shaughnessy`, `Campbell`, `Darjeeling`, `paper`, `bleaching`, `chlorine`, `red lead`, `manganese`, `two packages`.

### Target B

`India Political Consultation`
`11 May 1842`
`No.70`

then inspect surrounding numbers.

Verification keys:

`Campbell`, `Bushby`, `21 Apr 1842`, `Darjeeling`, `paper factory`, `machinery`, `wire gauze`, `potass`, `economics`, `closure`.

This is stronger than broad subject search because period terminology may not include modern descriptors such as `Nepal paper programme`.

---

## 12. Adjacent numbers remain mandatory

Wave 80 established that one administrative transaction can span multiple numbered consultation items.

For `No.147` and `No.70`, retrieve at minimum several items on either side if the volume/index permits.

Possible packet architecture:

`incoming letter`
+
`enclosure/report`
+
`order/minute`
+
`draft reply`
+
`copy of reply`
=
`ONE ADMINISTRATIVE TRANSACTION / MULTIPLE CONSULTATION NUMBERS`.

Do not assume Abdul Ali's cited single number captures the whole paper transaction.

---

## 13. EAP880 remains a parallel Darjeeling/Sikkim surrogate route

British Library Endangered Archives Programme:

`EAP880/1/2/55/55`

contains 141 digitised images of Political consultations regarding Darjeeling/Sikkim, 17 Oct 1833–24 May 1843.

Catalogue:

https://searcharchives.bl.uk/catalog/040-003650839

Digitised-content landing page:

https://eap.bl.uk/archive-file/EAP880-1-2-55

This remains highly relevant because it covers both target dates and comes from Sikkim Palace Archives.

Current status:

`EAP880_TARGET_NO147 = UNPROVEN`;

`EAP880_TARGET_NO70 = UNPROVEN`.

The image viewer was inaccessible in the current environment due JavaScript/robot verification, so no content claim has been made.

---

## 14. Revised source hierarchy

For the paper targets:

### Level 1 — primary consultation address

- NAI Political Original Consultation / Political Consultation, exact date + number;
- IOR/P India Political Consultation exact date + number.

### Level 2 — consultation derivatives and finding aids

- Political Proceedings;
- indexes / press lists / registers;
- adjacent consultation items.

### Level 3 — transmitted London correspondence

- `IOR/L/PS/6` Political Letters Received;
- `IOR/E/4` duplicate correspondence;
- `IOR/F/4` / Boards Collections and separated enclosures;
- London response/despatch.

### Level 4 — private / regional / publication derivatives

- RAS Hodgson private copies;
- EAP880 Sikkim Palace consultation copies;
- Agricultural and Horticultural Society publication;
- Abdul Ali's 1944 archival extraction.

This hierarchy follows documentary derivation rather than repository prestige.

---

## 15. Revised interpretation of Abdul Ali's article

The article now occupies an unusual source position:

`SECONDARY HISTORICAL ARTICLE`
+
`AUTHORED BY VERY LIKELY FORMER HEAD OF THE ARCHIVE`
+
`USES REPOSITORY-NATIVE DATE/NUMBER ADDRESSES`
+
`PUBLISHED CLOSE TO HIS ARCHIVAL TENURE`.

Therefore its archival references can be treated as highly informed finding-aid traces.

But retain the distinction:

- Abdul Ali's quotation/paraphrase = secondary witness until original consultation image recovered;
- Abdul Ali's archival shelf-address/date-number syntax = high-confidence professional archival pointer;
- his causal/historical interpretation = ordinary secondary scholarship subject to verification.

Mechanism:

`ARCHIVIST_SECONDARY_SOURCE_CAN_FUNCTION_AS_HIGH_VALUE_ARCHIVAL_INDEX`.

---

## Source-control rules

1. `Political O.C.` remains `Political Original Consultation` for these pre-Mutiny targets.
2. A. F. M. Abdul Ali's role as Keeper of Records / IRD head is direct NAI evidence; identity with the 1944 author is very high confidence, not yet a single-source biographical proof.
3. Treat the 1925 handbook as part of Abdul Ali's professional finding-aid environment.
4. For 1841–42, prefer `Political Department` as contemporaneous branch language; treat `Foreign and Political Department` as retrospective/umbrella wording unless a specific item says otherwise.
5. `IOR/P` is now the first London-side consultation series to search for an Abdul Ali Political O.C. reference.
6. Date+number identity can survive between NAI and IOR/P, but exact physical/copy relation must be checked item by item.
7. Do not assign exact `IOR/P` target shelfmarks by sequential interpolation.
8. Encode the 1841 target only as bracketed before `P/196/4` until direct control.
9. Encode the 1842 target only as bracketed between `P/196/10` and `/13` until direct control.
10. Same-date No.43 on 11 May 1842 supports date-local consultation numbering but has no paper-content significance.
11. Inspect adjacent numbers for both targets.
12. Keep `IOR/L/PS/6` as a later transmission route, not the first consultation mirror.
13. Keep EAP880 as a surrogate candidate until images are inspected.
14. Preserve Political / Foreign / Secret branch distinctions.
15. Do not allow Abdul Ali's archival expertise to upgrade his paraphrases into primary evidence.

## Immediate next actions

1. Find an `IOR/P` catalogue/index/secondary citation that directly maps **29 Nov 1841** to its exact volume.
2. Find an `IOR/P` catalogue/index/secondary citation that directly maps **11 May 1842** to its exact volume.
3. Retrieve `No.147` and at least several adjacent consultation numbers.
4. Retrieve `No.70` and at least several adjacent consultation numbers.
5. Use `13 Jan 1832 No.19` as the calibration target for cross-repository NAI/IOR/P identity if the 1841/42 targets remain inaccessible.
6. Search IOR/P indexes rather than only full consultation volumes; exact date may be easier to resolve from index chronology.
7. After consultation packet identity is controlled, trace any Political Letter to London through `IOR/L/PS/6`, `IOR/E/4` and Boards Collections.
8. Continue EAP880 image route in a browser-capable environment.
9. Update structured chronology/datasets so `consultation_date`, `consultation_number`, `IOR/P volume`, `underlying_letter_date` and `London_transmission_date` are separate fields.
10. Continue the material route search for Halliday / Woodcock / Champaran independently of the consultation work.

## Bottom line

Wave 81 changes the weight and direction of the archive trail. Abdul Ali's cryptic-looking `Political O.C.` references were almost certainly written by someone who had spent sixteen-plus years running the Imperial Record Department and who had helped produce its principal pre-Mutiny records handbook. That makes the citation syntax itself a high-value archival finding aid. The same institutional handbook places the 1841–42 transactions in the Political Department before the formal creation of the Foreign Department in May 1843. Most importantly, London preserves India Political Consultations in `IOR/P`, and published examples show that the same consultation date and item number can identify a document in both NAI and India Office holdings. The paper search should therefore move one documentary layer closer to the original administrative act: recover Political Consultation 29 Nov 1841 No.147 and Political Consultation 11 May 1842 No.70 in NAI or `IOR/P`, inspect the adjacent numbered items that may contain forwarding orders, enclosures and draft replies, and only then follow any transmitted Political Letter into `L/PS/6`, `E/4` and Boards Collections. Exact IOR/P volumes for the two targets are now tightly bracketed but remain deliberately unwritten until a direct finding aid identifies them.