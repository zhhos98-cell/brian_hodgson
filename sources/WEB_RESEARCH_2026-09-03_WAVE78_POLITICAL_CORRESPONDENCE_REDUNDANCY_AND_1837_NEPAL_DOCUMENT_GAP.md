# Web/archive research 2026-09-03 — Wave 78
## Political-correspondence redundancy, London recovery mirrors, and the 1837 Nepal missing-enclosure case

Date: 2026-09-03

Status: active paper-history mainline. Follow-up to Waves 76–77. This wave does **not** decode Abdul Ali's abbreviation `Political O.C.` and does **not** recover the underlying 29 Nov 1841 No.147 or 11 May 1842 No.70 paper files. It reconstructs a date-controlled London-side documentary redundancy architecture through which those archival pointers can now be pursued, and adds a directly documented 1837 Nepal case in which source enclosures are missing while a documentary derivative survives.

## Executive result

Wave 76 treated the missing Halliday directive and Woodcock bill as distributed documentary problems. Wave 78 shows that the higher-level Political correspondence itself was also systematically transformed into multiple documentary states.

British Library catalogue structure gives a concrete London-side chain for Government-of-India Political correspondence:

`Political Letter from India`
-> `Board of Control copy in IOR/L/PS/6/49-82`
-> `volume index`
-> `register in IOR/Z/L/PS/6/4`
-> `abstract in IOR/L/PS/6/1-7`
-> `abstract index in IOR/Z/L/PS/6/2`
-> `duplicate in General Correspondence IOR/E/4`
-> `[enclosures may survive in a different departmental/proceedings series]`
-> `[possible later London Political despatch response]`.

The Political Letters Received subseries explicitly states that it consists of Board of Control copies of Political letters from the Government of India to the East India Company Court of Directors, and that these letters are **duplicated in General Correspondence [E/4]**. Volumes 3–34, covering 1837–1858, have indexes.

For Abdul Ali's two high-value paper references, chronological volume control is now exact at the container level:

- `IOR/L/PS/6/57`, Political Letters Received from India, Vol. 9: **5 July 1841–22 December 1841**;
- `IOR/L/PS/6/58`, Political Letters Received from India, Vol. 10: **1842**.

Thus:

`Political O.C., 29 Nov 1841, No.147`
-> `IOR/L/PS/6/57 = DATE-CONTROLLED CANDIDATE LONDON MIRROR`;

`Political O.C., 11 May 1842, No.70`
-> `IOR/L/PS/6/58 = DATE-CONTROLLED CANDIDATE LONDON MIRROR`.

These are **not yet exact item identifications**. Abdul Ali's numbering system and abbreviation still require decoding.

The same correspondence has further control points:

- `IOR/L/PS/6/4`, *Abstracts of Political Letters from India, Vol. 4*, Jan 1839–Dec 1846;
- `IOR/Z/L/PS/6/2`, *Indexes to Abstracts of Political Letters from Bengal and India*, 1839–1858;
- `IOR/Z/L/PS/6/4`, *Registers of Political Letters from India, Bengal, Madras and Bombay*, 1838–1846.

Meanwhile `IOR/E/4` supplies a formally separate duplicate architecture. Its catalogue states that non-secret branches including Political correspondence are regularly represented; letters received from India and Bengal are `IOR/E/4/148-288` (1834–1858). The catalogue also warns that enclosures are generally **not bound with the letters received** and may instead survive in departmental/proceedings series such as `IOR/F/4`, `IOR/L/F/3`, `IOR/L/MIL/3`, `IOR/L/PWD/3` or `IOR/P`, depending on subject and department.

This produces a key source-control principle:

**letter copy, enclosure, register, abstract, index and duplicate can have different archival destinations.**

A second direct case shows why this matters. `IOR/L/PS/5/128, ff.313–316`, `Nepal Affairs`, concerns Secret Committee Despatches Nos.18–20, 17 Nov–20 Dec 1837. A note states that the enclosures to those Secret Letters are not in the collection. The only item present is an abstract of Despatch No.19, dated 17 Nov 1837, describing four letters between the Resident at Kathmandu and the Government of India. The item's date range is 5 Oct–17 Nov 1837.

This overlaps the same month as Campbell's 15 Nov 1837 Nepal-paper letter to T. C. Scott, but there is **no evidence** that the missing Secret enclosures concern paper. The significance is structural: in a contemporaneous Nepal correspondence branch, a derivative abstract survives after the source packet/enclosures disappear.

Core mechanisms:

- `DOCUMENT_REDUNDANCY_IS_A_RECOVERY_STRATEGY`
- `REGISTER_AND_ABSTRACT_FORM_SECONDARY_DOCUMENTARY_LIVES`
- `DOCUMENTARY_DERIVATIVE_CAN_OUTLIVE_SOURCE_PACKET`
- `LETTER_COPY_AND_ENCLOSURE_CAN_HAVE_DIFFERENT_ARCHIVAL_DESTINATIONS`
- `LONDON_TRANSMISSION_CHAIN_CAN_RECOVER_INDIA_SIDE_LOSS`
- `CHRONOLOGICAL_VOLUME_CONTROL_NARROWS_UNRESOLVED_REFERENCE`
- `MISSING_ARCHIVE_IS_STRUCTURALLY_BOUNDED_NOT_EMPTY`
- `DOCUMENTARY_STATE_HAS_DERIVATIVE_HISTORY`.

---

## 1. Political Letters Received from India are explicitly a copy/duplicate series

British Library series:

`IOR/L/PS/6/49-82 : Political Letters Received from India`

Catalogue:

https://searcharchives.bl.uk/catalog/037-000539505

Scope statement:

- Board of Control copies of Political letters from Government of India to the EIC Court of Directors in London;
- duplicated in `General Correspondence [E/4]`;
- Vols 3–34, 1837–1858, have indexes.

This is directly relevant to source recovery because it establishes that a single Government-of-India Political letter could have at least two London documentary lives before considering registers, abstracts or enclosures.

Correct model:

`INDIA POLITICAL LETTER`
-> `L/PS POLITICAL COPY`
+
`E/4 GENERAL CORRESPONDENCE DUPLICATE`.

Mechanisms:

- `INSTITUTIONAL_DUPLICATION_PRECEDES_ARCHIVAL_SURVIVAL`
- `ONE_ADMINISTRATIVE_ACT_CAN_PRODUCE_MULTIPLE_LONDON_WITNESSES`.

---

## 2. Exact date-controlled candidate volume for the 29 Nov 1841 reference

British Library:

`IOR/L/PS/6/57`

Title:

`Political Letters Received from India, Vol 9`

Date range:

`5 Jul 1841-22 Dec 1841`.

Catalogue:

https://searcharchives.bl.uk/catalog/040-000539514

Abdul Ali's archival pointer:

`Political O.C., 29 Nov 1841, No.147`.

Because 29 Nov 1841 falls within this volume's explicit date range, encode:

`POLITICAL_OC_1841_11_29_NO147 -> LPS_6_57 = DATE_CONTROLLED_CANDIDATE_MIRROR`.

Do not encode:

`POLITICAL_OC_NO147 = LPS_6_57_ITEM147`.

The numbering relation remains unproven.

Mechanism:

`CHRONOLOGICAL_VOLUME_CONTROL_NARROWS_UNRESOLVED_REFERENCE`.

---

## 3. Exact date-controlled candidate volume for the 11 May 1842 reference

British Library:

`IOR/L/PS/6/58`

Title:

`Political Letters Received from India, Vol 10`

Date range:

`1842`.

Catalogue:

https://searcharchives.bl.uk/catalog/040-000539515

Abdul Ali's archival pointer:

`Political O.C., 11 May 1842, No.70`.

Encode:

`POLITICAL_OC_1842_05_11_NO70 -> LPS_6_58 = DATE_CONTROLLED_CANDIDATE_MIRROR`.

This volume is especially high priority because Abdul Ali links the archival reference to Campbell's 21 Apr 1842 paper-related correspondence to G. A. Bushby.

Again:

`DATE_MATCH != ITEM_NUMBER_MATCH`.

---

## 4. Abstract volume gives a second documentary life

British Library:

`IOR/L/PS/6/1-7 : Abstracts of Political Letters from India`.

The catalogue explains that `India` means Government of Bengal for 1798–1834 and Government of India for 1834–1859, and that some secret correspondence is included.

For the target period:

`IOR/L/PS/6/4`

`Abstracts of Political Letters from India, Vol 4`

Date range:

`Jan 1839-Dec 1846`.

Catalogue:

https://searcharchives.bl.uk/catalog/040-000539457

Thus both 1841 and 1842 target references lie inside one abstract volume.

This creates a recovery possibility even if the full Political-letter volume is difficult to search:

`FULL LETTER`
-> `ABSTRACT ENTRY`.

An abstract cannot automatically substitute for the full text, but it may recover:

- subject identity;
- letter date/number;
- institutional sender/receiver;
- enclosure description;
- cross-reference to a despatch or response.

Mechanism:

`ABSTRACT_IS_A_DERIVATIVE_DOCUMENTARY_STATE`.

---

## 5. Register and abstract index give two additional control layers

British Library Political and Secret Department indexes/registers:

`IOR/Z/L/PS/6/2`

`Indexes to Abstracts of Political Letters from Bengal and India`

Date range:

`1839-1858`.

and

`IOR/Z/L/PS/6/4`

`Registers of Political Letters from India, Bengal, Madras and Bombay`

Date range:

`1838-1846`.

Catalogue series:

https://searcharchives.bl.uk/catalog/037-001616091

These are not merely auxiliary finding aids. For a missing or ambiguously cited object they constitute separately surviving documentary derivatives.

Practical sequence:

`NAME/SUBJECT INDEX`
-> `ABSTRACT ENTRY`
-> `REGISTER ENTRY`
-> `RECEIVED LETTER VOLUME`.

Alternative sequence:

`DATE/NUMBER FROM ABDUL ALI`
-> `REGISTER`
-> `LETTER VOLUME`
-> `ABSTRACT/INDEX CROSS-CHECK`.

Mechanisms:

- `INDEX_CAN_RECOVER_DOCUMENT_IDENTITY_WITHOUT_DOCUMENT_TEXT`
- `REGISTER_CAN_RECONSTRUCT_CORRESPONDENCE_SEQUENCE`.

---

## 6. E/4 is an explicit duplicate branch

British Library:

`IOR/E/4 : Correspondence with India`

Catalogue:

https://searcharchives.bl.uk/catalog/036-001036642

For 1834–1858:

`IOR/E/4/148-288 : Letters received from India and Bengal`.

The catalogue states that branches regularly included in E/4 include Political correspondence among many other departments.

More importantly, `IOR/L/PS/6/49-82` itself states that the Political Letters Received are duplicated in E/4.

Current state:

`E4_DUPLICATE_BRANCH = SECURE_AT_SERIES_LEVEL`.

But:

`EXACT_1841_E4_VOLUME = UNRESOLVED`

and

`EXACT_1842_E4_VOLUME = UNRESOLVED`.

Do not derive an exact E/4 volume from chronological interpolation.

Mechanism:

`DUPLICATE_SERIES_CREATES_INDEPENDENT_RECOVERY_PATH`.

---

## 7. Enclosures may leave the letter's archival home

The `IOR/E/4` catalogue explicitly warns that enclosures are generally not bound into the letters-received volumes. Depending on government and department, they may instead be found in:

- `IOR/F/4`;
- `IOR/L/F/3`;
- `IOR/L/MIL/3`;
- `IOR/L/PWD/3`;
- `IOR/P`.

This changes the retrieval logic for the paper project.

Suppose a Political letter mentions:

- Campbell's report;
- paper samples;
- a cost table;
- O'Shaughnessy's experiment;
- a manufacturing statement;
- an enclosed local correspondence copy.

The top-level letter and the material enclosure need not survive together.

Therefore:

`LETTER_RECOVERED / ENCLOSURE_MISSING`

and

`LETTER_MISSING / ENCLOSURE_OR_COPY_SURVIVES_ELSEWHERE`

are both structurally plausible states.

Mechanisms:

- `LETTER_COPY_AND_ENCLOSURE_CAN_HAVE_DIFFERENT_ARCHIVAL_DESTINATIONS`
- `DOCUMENTARY_PACKET_CAN_FRAGMENT_ACROSS_DEPARTMENTS`.

---

## 8. 1837 Nepal Affairs gives a directly documented missing-enclosure case

British Library/Qatar Digital Library:

`IOR/L/PS/5/128, ff 313-316`

Title:

`Nepal Affairs`.

Catalogue:

https://searcharchives.bl.uk/catalog/041-003431775

Digital record:

https://www.qdl.qa/en/archive/81055/vdc_100083822146.0x000008

Scope:

Enclosures to Secret Committee Despatches Nos.18–20, dated 17 Nov–20 Dec 1837.

A note on folio 314 states that the enclosures to Secret Letters Nos.18–20 are not in the collection.

The sole surviving item is an Abstract of Contents of Despatch No.19, dated 17 Nov 1837, describing four letters between the Resident at Kathmandu and Government of India concerning Nepal affairs.

Item date range:

`5 Oct-17 Nov 1837`.

This establishes a directly witnessed transformation:

`SECRET LETTER / ENCLOSURE PACKET`
-> `[ENCLOSURES ABSENT]`
-> `ABSTRACT SURVIVES`.

Mechanism:

`DOCUMENTARY_DERIVATIVE_CAN_OUTLIVE_SOURCE_PACKET`.

---

## 9. The 1837 missing packet must not be turned into a paper claim

Campbell's Nepal-paper letter to T. C. Scott is dated 15 Nov 1837.

The surviving Nepal Affairs abstract ends on 17 Nov 1837.

This temporal overlap is striking but evidentially insufficient.

The catalogue describes the surviving abstract as four letters between the Resident at Kathmandu and Government of India concerning Nepal affairs. Campbell at Darjeeling is a different sender/context from Hodgson as Resident at Kathmandu.

Therefore encode:

`CONTEMPORARY_NEPAL_SECRET_CORRESPONDENCE_GAP = SECURE`

but:

`MISSING_SECRET_ENCLOSURES_CONTAIN_CAMPBELL_PAPER_CORRESPONDENCE = UNPROVEN / DO_NOT_INFER`.

The use of this case is archival-methodological, not substantive evidence of paper policy.

---

## 10. Secret and Political branches are related but not interchangeable

British Library has a separate Secret Letters stream for the same period, e.g.:

- `IOR/L/PS/5/10`, Secret Letters received from Bengal and India, 9 Nov 1840–22 Mar 1842;
- `IOR/L/PS/5/11`, Secret Letters received from Bengal and India, 6 Apr 1842–28 Dec 1843.

These demonstrate that March and April 1842 also cross a boundary between Secret-letter volumes.

However there is currently no evidence that Halliday's paper directive, the 24-package pulp shipment or Abdul Ali's `Political O.C.` entries belong to the Secret stream.

Use these only as contextual archival architecture unless a direct index points there.

Rule:

`POLITICAL != SECRET` unless the source itself identifies the overlap.

---

## 11. Documentary derivation should now be treated like material derivation

The paper-history project already distinguishes material transformations:

`bark`
-> `pulp`
-> `sheet`
-> `package`
-> `working support`
-> `bound/archive object`.

Wave 78 shows a parallel documentary derivative chain:

`original administrative letter`
-> `official copy`
-> `duplicate copy`
-> `register entry`
-> `abstract`
-> `index entry`
-> `enclosure separated to another series`
-> `private copy/extract`
-> `learned-society publication`
-> `later archival citation`.

These documentary objects share referents but are not interchangeable witnesses.

Working proposition:

**colonial paper history has a documentary derivative history. A material event may survive not as one stable file but as a family of transformed documentary states, each preserving and deleting different information. Retrieval therefore requires reconstructing derivation and duplication, not merely locating an original.**

Mechanisms:

- `DOCUMENTARY_STATE_HAS_DERIVATIVE_HISTORY`
- `SOURCE_TRANSFORMATION_CHANGES_INFORMATION_RESOLUTION`
- `ARCHIVAL_RECOVERY_REQUIRES_DERIVATION_GRAPH`.

---

## 12. Revised recovery map for the two Political O.C. targets

### Target A

`Political O.C., 29 Nov 1841, No.147`

Candidate London path:

1. `IOR/Z/L/PS/6/2` — subject/name index;
2. `IOR/Z/L/PS/6/4` — Political Letters register;
3. `IOR/L/PS/6/4` — abstract volume, Jan 1839–Dec 1846;
4. `IOR/L/PS/6/57` — Political Letters Received, 5 Jul–22 Dec 1841;
5. E/4 duplicate branch — exact physical volume unresolved;
6. enclosure/proceedings branch if the letter refers to material attachments;
7. possible Court/Board response in Political Despatches to India.

### Target B

`Political O.C., 11 May 1842, No.70`

Candidate London path:

1. `IOR/Z/L/PS/6/2`;
2. `IOR/Z/L/PS/6/4`;
3. `IOR/L/PS/6/4`;
4. `IOR/L/PS/6/58` — Political Letters Received, 1842;
5. E/4 duplicate branch — exact physical volume unresolved;
6. enclosure/proceedings branch;
7. possible outgoing Political Despatch response.

Search names/terms:

`Campbell`, `Bushby`, `Hodgson`, `Nepal/Nepaul/Nipal`, `paper`, `paper manufacture`, `Darjeeling`, `O'Shaughnessy`, `Marshman`, `pulp`.

---

## Source-control rules

1. `Political O.C.` remains unresolved; do not expand the abbreviation without a controlled contemporary/archive source.
2. `IOR/L/PS/6/57` is a date-controlled candidate London mirror for 29 Nov 1841, not proven item No.147.
3. `IOR/L/PS/6/58` is a date-controlled candidate London mirror for 11 May 1842, not proven item No.70.
4. Do not assume Abdul Ali's `No.147` or `No.70` equals the numbering inside L/PS/6.
5. Treat `IOR/L/PS/6/4`, `IOR/Z/L/PS/6/2` and `IOR/Z/L/PS/6/4` as derivative control layers.
6. Treat E/4 duplication as secure at series level; exact 1841/42 E/4 volumes remain unresolved.
7. Do not interpolate exact E/4 shelfmarks from nearby volume dates.
8. Enclosures may survive outside E/4; identify department before assigning an enclosure series.
9. `IOR/L/PS/5/128 ff.313-316` proves missing Nepal Secret enclosures with surviving abstract; it does not prove those missing enclosures concern paper.
10. Keep Political and Secret correspondence branches distinct unless a source explicitly links them.
11. Treat abstracts, indexes and registers as evidence with lower/different information resolution than the full source document.
12. Preserve the distinction between original, official copy, duplicate, enclosure, abstract, register, index, private copy and published extraction.

## Immediate next actions

1. Inspect `IOR/Z/L/PS/6/2` for Campbell/Bushby/Hodgson/Nepal-paper subject and name entries.
2. Inspect `IOR/Z/L/PS/6/4` around 29 Nov 1841 and 11 May 1842 to identify Political Letter numbers and receipt metadata.
3. Inspect `IOR/L/PS/6/4` abstracts for those dates/subjects.
4. Request/search `IOR/L/PS/6/57` and `/58` using the volume indexes before page-level browsing.
5. Map the relevant entries to exact E/4 duplicate volumes rather than inferring them chronologically.
6. If a recovered letter names enclosures, follow the department-specific enclosure/proceedings trail separately.
7. Search Political Despatch-to-India indexes for any London response to the paper matter.
8. Continue decoding Abdul Ali's `Political O.C.` notation through contemporary Indian-side record guides/indexes.
9. Keep the 1837 Nepal Secret missing-enclosure case as a structural control, not a paper-content claim.
10. Fold any direct paper hit back into the 1841–42 programme chronology and test against the 25 Mar 1842 pulp consignment.

## Bottom line

Wave 78 changes the archival search from a hunt for one elusive file into reconstruction of a derivative record family. Government-of-India Political letters were copied for the Board of Control, duplicated into E/4, indexed, registered and abstracted; their enclosures could then be separated into other departmental or proceedings series. The target dates supplied by Abdul Ali now fall inside exact London Political-letter containers: 29 Nov 1841 inside `IOR/L/PS/6/57`, and 11 May 1842 inside `IOR/L/PS/6/58`, with both also covered by the 1839–46 abstract volume and corresponding index/register volumes. A directly documented 1837 Nepal case shows why these derivatives matter: the Secret-letter enclosures are absent, but an abstract survives. Paper history therefore has to reconstruct two transformations at once. The physical material changes state as bark, pulp, sheet, sample and package; the evidence about it changes state as original letter, copy, duplicate, enclosure, register, abstract, index, private copy and publication. Archival survival belongs to that second material history.