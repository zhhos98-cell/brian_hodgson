# Hodgson paper-history mainline — 2026-09-03, through Wave 85

Status: **current active guardrail**. Supersedes `PAPER_HISTORY_MAINLINE_STATUS_2026-09-03_WAVE84.md`. Wave 85 converts the `IOR/P -> F/4 -> E/4` architecture into an India Office Library-controlled retrieval protocol and adds the cover-level metadata fields required to crosswalk Campbell's Board's Collection file.

## Current active crosswalk problem

Campbell 1842:

`21 Apr 1842 Campbell -> G. A. Bushby`
-> `11 May 1842 Political Original Consultation No.70`
-> `IOR/P/196/12 = high-confidence consultation-volume target`
-> `[exact copied/extracted papers pending]`
-> `IOR/F/4/2006/89528 = direct Board's Collection file containing Campbell's result report on making paper from paper-tree bark`
-> `[COVER METADATA UNKNOWN: Draft / P.C. / historical Collection No]`
-> `IOR/Z/F/4/8 = 1842–44 Board's Collection register`
-> `[associated draft pending]`
-> `IOR/Z/F/3 = draft register`
-> `IOR/E/4 original draft despatch`.

The immediate missing object is no longer a generic “London reference”. It is the **title-page/register crosswalk metadata for `89528`**.

---

## 1. India Office Library confirms the bidirectional method

Amar Kaur Jasbir Singh's 1988 guide to Tibet/Sikkim/Bhutan source material in the India Office Library states that:

- researchers can locate an E/4 despatch through the indexes;
- work backward to the Bengal/India letter under reply;
- use Board's Collections for enclosures/background papers;
- later Board's Collection registers `IOR/Z/F/4/1-18` are not indexed;
- therefore later Collections must be found either by browsing the register or by using Draft Numbers and related details in E/4 Despatches.

Encode:

`BIDIRECTIONAL_CROSSWALK = INDIA_OFFICE_RECOMMENDED_METHOD`.

This is now the active retrieval method.

---

## 2. Political Board's Collections remain a direct derivative class of IOR/P

British Library direct series architecture retained:

- F/4 copies papers by subject from Indian Proceedings;
- Political Collections survive as a virtually complete duplicate of `IOR/P` at series level;
- Collections are reorganised around associated answering draft despatch numbers/dates.

Keep:

`F4_POLITICAL_COLLECTIONS_DERIVE_FROM_IOR_P = DIRECT_SERIES_LEVEL`.

Keep simultaneously:

`SERIES_COMPLETENESS != ITEM_INFORMATION_EQUIVALENCE`.

An F/4 subject file can select, combine and reorder Proceedings material.

---

## 3. Digitised F/4 covers demonstrate the required crosswalk fields

Qatar Digital Library examples in neighbouring 1842–43 Political Board's Collections show title-page fields:

`Draft [number/year]`
+
`P.C. [Previous Communication] [number]`
+
`Collection No [number]`.

Controlled examples:

### `IOR/F/4/2006/89515`

`Draft 612/43`

`P.C. 3902`

`Collection No 11`.

### `IOR/F/4/2006/89516`

`Draft 612/43`

`P.C. 3902`

`Collection No 12`.

These are Bombay/Persian Gulf files and are **structural examples only**.

Do not transfer their values to Darjeeling.

---

## 4. `89528` title-page metadata is now the first object-level target

When `IOR/F/4/2006/89528` is inspected, capture before anything else:

- Draft number/year;
- P.C. / Previous Communication number;
- historical Collection No;
- branch/department label;
- letter/despatch number under reply;
- contents page;
- Political Proceedings / consultation references;
- individual enclosure numbers and dates.

Reason:

`COVER_METADATA_CAN_RESOLVE_DOCUMENT_GENEALOGY_BEFORE_FULL_TEXT_TRANSCRIPTION`.

The Campbell report body remains important, but the cover can solve the archive graph faster.

---

## 5. Number systems must remain disambiguated

Current Campbell chain already contains several independent numbers:

1. `Political Consultation No.70` — India-side item number for 11 May 1842;
2. `IOR/F/4/2006/89528` — modern/global F/4 shelfmark item identifier;
3. historical `Collection No` — currently unknown for 89528;
4. associated `Draft No/year` — currently unknown;
5. potential `P.C. / Previous Communication` number — currently unknown.

Never equate them by visual similarity or sequence.

Encode:

`ARCHIVAL_CROSSWALK_REQUIRES_NUMBER_SYSTEM_DISAMBIGUATION`.

---

## 6. Do not infer `Draft 612/43` for Campbell from physical adjacency

`89515` and `89516` share `Draft 612/43`, but `IOR/F/4/2006` contains mixed Political business from Persian Gulf, Mysore, Coorg, Rajasthan, Nepal, Darjeeling, Gwalior, Hyderabad and Indore.

Thus:

`SAME_F4_PHYSICAL_VOLUME != SAME_ASSOCIATED_DRAFT`.

Current Campbell value:

`F4_89528_DRAFT = UNKNOWN`.

This remains a hard guardrail.

---

## 7. Previous Communication can expose a longer paper genealogy

The controlled QDL examples expand `P.C.` as `Previous Communication`.

For `89528`, a recovered P.C. field could point to earlier London correspondence related to:

- Darjeeling administration;
- paper manufacture;
- Campbell's experiment;
- another component of the locality packet.

Do not assume the P.C. will point to the 1841 O'Shaughnessy bleaching experiment.

Use:

`P.C. = POTENTIAL_PRIOR_DOCUMENTARY_EDGE`.

---

## 8. 1841 target now has an equivalent London-cover strategy

India-side identity:

`Political Consultation 29 Nov 1841, No.147`
=
O'Shaughnessy's report on bleaching paper manufactured at Darjeeling.

Exact IOR/P volume remains unresolved.

Active London-first route:

`O'Shaughnessy report identity`
-> browse/search `IOR/Z/F/4/7`
-> recover F/4 subject file
-> capture Draft / P.C. / historical Collection No
-> resolve E/4 draft/despatch
-> use that relation to back-resolve the IOR/P volume.

Do not continue relying on chronological interpolation for the IOR/P shelfmark.

---

## 9. 1832 adjacent-number calibration retained

`Pol. Con. 13 Jan 1832, Nos.18–20`

is the controlled Nepal-paper transaction cluster, with Abdul Ali's No.19 corresponding to Hodgson's 8 Dec 1831 letter.

Use as direct proof that one paper transaction can span adjacent consultation numbers.

For No.70 and No.147, inspect neighbours.

---

## 10. Campbell 1842 documentary states remain formally constrained but not collapsed

### Underlying state

`Campbell -> Bushby, 21 Apr 1842`.

### Consultation state

`Political Original Consultation, 11 May 1842, No.70`.

### London proceedings witness

`IOR/P/196/12` high-confidence target.

### London subject-extract state

`IOR/F/4/2006/89528` direct Campbell paper-experiment report.

### London answering-draft state

Unknown exact E/4 draft, to be recovered from cover/register metadata.

Keep:

`F4_89528 = NO70 = UNPROVEN_ITEM_LEVEL`.

But series architecture makes a direct derivational relation strongly constrained and testable.

---

## 11. Material chain remains independent

Direct 25 Mar 1842 Hodgson pulp shipment:

`24 packages Nepalese paper pulp`
-> `Champaran / Woodcock`
-> `Patna by land OR Govind Gang by water`
-> `Calcutta`.

Still missing Halliday directive, Woodcock bill/choice, receipts, final destination.

No amount of documentary crosswalking between No.70 and F/4 proves that these 24 packages supplied Campbell's Darjeeling experiment.

Keep:

`HODGSON_PULP -> CAMPBELL_EXPERIMENT = UNPROVEN`.

---

## Immediate research order

1. Obtain `IOR/F/4/2006/89528` title page/cover or its entry in `IOR/Z/F/4/8`.
2. Record Draft / P.C. / historical Collection No.
3. Resolve associated draft in `IOR/Z/F/3`.
4. Retrieve exact `IOR/E/4` draft despatch and its answering context.
5. Cross-check in `IOR/Z/E/4/16`.
6. Use the resulting references to test against `IOR/P/196/12`, No.70 ± adjacent items.
7. Browse `IOR/Z/F/4/7` for O'Shaughnessy's 1841 bleaching report and repeat the cover-metadata workflow.
8. Preserve every number system in separate structured fields.
9. Continue Halliday/Woodcock/Champaran logistics separately.

---

## Guardrails

1. `Political O.C. = Political Original Consultation`.
2. `IOR/P`, `F/4`, `E/4` are distinct documentary states within a controlled derivative system.
3. Later F/4 registers are unindexed; browsing is normal archival workflow.
4. `89528` modern item number != historical Collection No.
5. `No.70` consultation number != historical Collection No != draft number.
6. `Draft 612/43`, `P.C.3902`, Collection Nos11/12 from Gulf siblings must not be propagated to Darjeeling.
7. P.C. means Previous Communication in the controlled QDL examples; 89528 P.C. remains unknown.
8. `IOR/P/196/12` is high-confidence 11 May 1842 volume targeting, not page-level recovery.
9. Exact IOR/P volume for 29 Nov 1841 No.147 remains unresolved.
10. Series-level virtual duplication does not imply item-level information equivalence.
11. Campbell documentary convergence does not prove Hodgson 24-package material identity.

## Current strongest proposition

**The Campbell 1842 paper problem has now become a finite metadata-crosswalk problem. India Office Library guidance confirms that later Board's Collections were intended to be traced either by browsing the unindexed `Z/F/4` registers or by starting from the answering `E/4` draft despatch and using its draft number to recover the Collection. Digitised Board's Collection covers show the fields that make this possible: Draft number/year, Previous Communication reference and historical Collection No. For `IOR/F/4/2006/89528`, those fields are presently missing from public metadata. Recovering that one title page or register entry should connect Campbell's London Board's Collection file to an exact draft despatch and thereby give a controlled test against Political Consultation No.70 in `IOR/P/196/12`. The same method through `IOR/Z/F/4/7` offers the cleanest non-interpolative route to O'Shaughnessy's still-unlocated 29 Nov 1841 No.147 London Proceedings volume.**