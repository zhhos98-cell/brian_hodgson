# Web/archive research 2026-09-03 — Wave 80
## `Political O.C.` = Political Original Consultation: consultation-date/number mechanics and correction of Wave 79

Date: 2026-09-03

Status: active paper-history mainline. Follow-up to Waves 78–79. **This wave supersedes Wave 79 on the expansion of `O.C.`.** Wave 79 correctly established that the date in Abdul Ali's `Political O.C.` citation is distinct from the date of the underlying letter, but it provisionally preferred `Original Collection`. Direct archival-method evidence now makes **`Original Consultation`** the controlled interpretation for this pre-Mutiny Foreign/Political record context.

## Executive result

Three independent evidence layers converge.

### 1. Archival-method handbook: original letters were literally styled `Original Consultations`

Douglas Dewar's 1920 *A Hand-book to the English Pre-mutiny Records in the Government Record Rooms of the United Provinces of Agra and Oudh* includes a chapter describing records in the Imperial Record Department, Calcutta. It explicitly explains the Government-of-India record mechanism:

- original letters received and drafts of letters issued, once recorded, were styled **`Original Consultations`**;
- a Council sitting/consultation could consider multiple letters;
- each letter issued or received received a number in the proceedings register;
- a fresh number series began for each consultation;
- the index called this the `Consultation no.`;
- the original documents were kept in thin cardboard covers carrying **the proceeding number and the date of the consultation/meeting**;
- Proceedings were copies/narrative register versions of the original consultations and might omit enclosures.

Dewar also lists, among the Imperial Record Department holdings:

- `Political Proceedings`, 1790–1859;
- `Political Consultations`, 1790–1859;
- `Foreign Proceedings`, 1784–1842;
- `Foreign Original Consultations`, 1783–1842;
- `Secret Proceedings`, 1763–1859.

This is almost exactly the architecture required to decode Abdul Ali's citations.

Source:

https://archive.org/details/handbooktoenglis00dewa

Open Library bibliographic control:

https://openlibrary.org/books/OL24236488M/A_hand-book_to_the_English_pre-mutiny_records_in_the_government_record_rooms_of_the_United_provinces

Public-domain scan / search-text mirrors:

https://commons.wikimedia.org/wiki/File:A_hand-book_to_the_English_pre-mutiny_records_in_the_government_record_rooms_of_the_United_provinces_of_Agra_and_Oudh_(IA_handbooktoenglis00dewa).pdf

https://pahar.in/pahar/Books%20and%20Articles/Indian%20Subcontinent/1920%20Hand-Book%20of%20English%20Pre-Mutiny%20Records%20in%20United%20Provinces%20of%20Agra%20and%20Oudh%20by%20Dewar%20s.pdf

### 2. Explicit abbreviation control: `O.C. = Original Consultation`

Qeyamuddin Ahmad's *The Wahhabi Movement in India*, based heavily on National Archives of India and other official records, has an explicit abbreviations page:

- `For.Dept.Pol.Cons. — Foreign Department Political Consultation`;
- `For.Dept.Sec.Cons. — Foreign Department Secret Consultation`;
- `O.C. — Original Consultation`.

The 2020 second revised edition preserves a work first published in 1966; Ahmad's preface describes extensive research in the National Archives, Delhi and other government record offices.

Source / page-image controlled PDF preview:

https://api.pageplace.de/preview/DT0400.9781000082029_A39686746/preview-9781000082029_A39686746.pdf

This is direct abbreviation evidence in precisely the archival-historiographical ecosystem relevant to Abdul Ali.

### 3. Modern NAI citations use the same `Political Consultations, date, nos.` syntax

Modern scholarship citing National Archives of India Foreign Department records uses forms such as:

- `Political Consultations, nos. 148–151, 19 October 1842, NAI`;
- `Political Consultations, nos. 87–89, 22 November 1841, NAI`;
- `Political Consultations, no. 27, 17 April 1837, NAI`;
- `Political Consultations, nos. 72–74, 10 July 1839, NAI`.

Sources:

https://distantreader.org/stacks/journals/transcultural/transcultural-23539.htm

https://dokumen.pub/darjeeling-reconsidered-histories-politics-environments-0199483558-9780199483556.html

This citation shape is isomorphic with Abdul Ali's:

`Political O.C., 11 May 1842, no.70`

and

`Political O.C., 29 Nov 1841, no.147`.

## Controlled reconstruction

The strongest current decoding is therefore:

`Political O.C.`
=
`Political Original Consultation`.

Operationally:

`underlying incoming letter/report/enclosure`
-> `put before Governor-General in Council / relevant consultation`
-> `considered on CONSULTATION DATE`
-> `assigned CONSULTATION/PROCEEDING NUMBER within that sitting`
-> `original document packet retained as ORIGINAL CONSULTATION`
-> `copied/narrated into PROCEEDINGS`
-> `[later index / press list / archival citation]`.

This directly explains the date split discovered in Wave 79.

---

## 1. Why the Abdul Ali date is later than the underlying letter

### Calibration case A: Hodgson 1831/32

Abdul Ali states:

- underlying Hodgson-to-H. T. Prinsep paper-specimen letter: **8 Dec 1831**;
- archival citation: `Pol. O.C., no.19, Jany. 13, 1832`.

Wave 79 established the date difference. Dewar's consultation mechanism now gives the best explanation:

`8 Dec 1831 HODGSON LETTER`
-> `received / circulated administratively`
-> `put before consultation on 13 Jan 1832`
-> `assigned consultation item No.19`
-> `original packet retained as Political Original Consultation`.

Thus:

`13 JAN 1832 = CONSULTATION / PROCEEDING DATE` — high confidence;

`NO.19 = ITEM / CONSULTATION NUMBER WITHIN THAT DATE'S PROCEEDINGS` — high confidence.

The exact day of receipt between 8 Dec and 13 Jan remains unknown.

### Calibration case B: Campbell 1842

Abdul Ali's note:

`Letter to Mr. G. A. Bushby, 21st April, 1842. Political O. C., 11 May, 1842, no.70.`

Reconstruction:

`21 Apr 1842 CAMPBELL -> BUSHBY LETTER`
-> `Foreign/Political Department handling`
-> `Political consultation on 11 May 1842`
-> `consultation item No.70`
-> `original consultation packet retained`.

This is now much stronger than the generic Wave-79 label `departmental control date of unresolved type`.

Encode:

`POLITICAL_OC_DATE = CONSULTATION_DATE` — HIGH CONFIDENCE.

`POLITICAL_OC_NO = CONSULTATION_ITEM_NUMBER` — HIGH CONFIDENCE.

---

## 2. `Original Consultation` is an archival packet, not merely a meeting label

Dewar gives the physical/documentary distinction:

### Original consultation

Consists of original records associated with business considered by Council/Board, including:

- original letters received;
- orders passed thereon;
- drafts or copies of replies;
- potentially enclosures not reproduced in Proceedings.

The originals could be stitched into thin cardboard covers carrying the date of consultation/meeting and proceeding number.

### Proceedings

Folio-register copies/narrative account of the consultation. They are easier to handle, but can omit enclosures.

Therefore the `O.C.` object is a **documentary packet/state** rather than a synonym for the underlying incoming letter.

Mechanisms:

- `ORIGINAL_CONSULTATION_IS_A_PACKET_STATE`;
- `CONSULTATION_DATE_IS_NOT_LETTER_DATE`;
- `CONSULTATION_NUMBER_IS_LOCAL_TO_A_SITTING`;
- `PROCEEDINGS_ARE_DERIVATIVES_OF_ORIGINAL_CONSULTATIONS`;
- `ENCLOSURE_RESOLUTION_CAN_BE_HIGHER_IN_OC_THAN_PROCEEDINGS`.

---

## 3. Why No.70 and No.147 should not be read as annual or London letter numbers

Dewar explicitly says a fresh series of numbers is assigned for **each consultation/sitting**. The number is the item's place in that consultation/proceedings sequence.

Therefore:

`11 MAY 1842 NO.70`

means, most likely:

`item No.70 in the Political consultation/proceedings of 11 May 1842`.

Likewise:

`29 NOV 1841 NO.147`

means, most likely:

`item No.147 in the Political consultation/proceedings of 29 Nov 1841`.

Do not encode:

- No.70 = 70th Political letter of 1842;
- No.147 = 147th Political letter of 1841;
- No.70 / No.147 = London Political Letter numbers;
- No.70 / No.147 = fixed file numbers independent of consultation date.

Mechanism:

`DATE_AND_NUMBER_FORM_A_COMPOSITE_ARCHIVAL_ADDRESS`.

---

## 4. Correction to Wave 79: `Original Collection` was the wrong primary expansion

Wave 79 found modern NAI scholarship in which `O.C.` is expanded as `Original Collection`. That usage is real in some archival citation systems and should not be erased.

However, for **pre-Mutiny Foreign/Political Government-of-India records**, the more specific evidence now dominates:

1. Dewar describes Political Consultations as an extant Imperial Record Department series for 1790–1859.
2. Dewar explicitly defines original letters/drafts in this record system as `Original Consultations`.
3. Qeyamuddin Ahmad explicitly abbreviates `O.C.` as `Original Consultation` while separately abbreviating Foreign Department Political Consultation.
4. Modern NAI citations for this period use `Political Consultations + consultation date + number(s)` in the same syntax as Abdul Ali.
5. Abdul Ali's own underlying-letter/OC-date split is exactly what the consultation model predicts.

Thus revise:

`O.C. = ORIGINAL COLLECTION` — **REJECT AS PRIMARY INTERPRETATION FOR THESE ABDUL ALI POLITICAL CITATIONS**.

`O.C. = ORIGINAL CONSULTATION` — **HIGH CONFIDENCE / CONTROLLED WORKING EXPANSION**.

A direct image of Abdul Ali's exact NAI wrapper or contemporary index remains the final archival confirmation, but the current convergence is strong enough for the mainline to use `Original Consultation` without hedging it as merely one of two equal alternatives.

---

## 5. Wave 78 London volume mapping is now more clearly secondary

Wave 78 located London Political Letters Received containers:

- `IOR/L/PS/6/57`, 5 Jul–22 Dec 1841;
- `IOR/L/PS/6/58`, 1842.

Wave 79 already downgraded the inference that these are direct date-matched mirrors of Abdul Ali's O.C. references.

Wave 80 explains why:

`29 Nov 1841` and `11 May 1842` are India-side consultation dates, not necessarily dates of Political Letters transmitted to London.

Correct retrieval order:

`INDIA-SIDE POLITICAL ORIGINAL CONSULTATION`
-> identify underlying letter(s), order(s), enclosure(s), draft reply/reply
-> identify whether/how the business entered a Political Letter to Court / London transmission
-> then map to `IOR/L/PS/6`, `IOR/E/4`, Boards Collections / `IOR/F/4`, or other derivative series.

London copying remains important, but document identity must drive the match, not consultation-date interpolation.

---

## 6. No.147: likely packet architecture around Maddock / O'Shaughnessy

Abdul Ali associates `Political O.C., 29 Nov 1841, no.147` with:

- Campbell's Darjeeling paper samples;
- T. Maddock, Political Department;
- W. B. O'Shaughnessy, Chemical Examiner;
- a bleaching process using chlorine solution;
- the use of red lead, salt, sulphuric acid and water rather than oxide of manganese.

The original-consultation model predicts that No.147 may preserve more than the technical text quoted by Abdul Ali. It may include a packet such as:

`Campbell/sample context`
-> `Maddock forwarding / request`
-> `O'Shaughnessy report or memorandum`
-> `order/minute`
-> `draft/copy reply`
-> `[enclosures/sample description]`.

This is a hypothesis about packet composition, not yet recovered content.

Retrieval terms:

`29 November 1841`, `No.147`, `Maddock`, `O'Shaughnessy`, `Campbell`, `Darjeeling`, `paper`, `bleaching`, `chlorine`, `red lead`, `manganese`, `two packages`.

---

## 7. No.70: likely packet around Campbell's 21 Apr letter and government response

Known directly through Abdul Ali:

`Campbell -> G. A. Bushby, 21 Apr 1842`
-> cited as
`Political O.C., 11 May 1842, No.70`.

The original-consultation model predicts No.70 can contain:

- Campbell's original 21 Apr letter;
- associated paper-manufacture description;
- factory economics / closure argument;
- departmental order/minute;
- draft or copy of reply;
- possibly related enclosure(s).

Again, packet membership beyond Campbell's letter is a retrieval hypothesis until images are controlled.

---

## 8. The consultation system predicts multiple numbers on the same date

Modern NAI citations show ranges such as:

- `Political Consultations, 19 Oct 1842, nos.148–151`;
- `Political Consultations, 22 Nov 1841, nos.87–89`;
- `Political Consultations, 10 Jul 1839, nos.72–74`.

This matches Dewar's explanation that many documents were considered in one sitting and numbered serially.

For the paper targets this means adjacent numbers may matter.

Do not retrieve only No.147 or No.70 in isolation if the surrounding consultation packet/index is available. Inspect at minimum:

`No.147 ± several items`

and

`No.70 ± several items`,

because the incoming letter, enclosure, order and reply can be separate numbered items in the same consultation sequence.

Mechanism:

`ADJACENT_CONSULTATION_NUMBERS_CAN_FORM_ONE_ADMINISTRATIVE_TRANSACTION`.

This is a new concrete retrieval instruction.

---

## 9. Direct Darjeeling/Sikkim consultation surrogate discovered in EAP880

British Library Endangered Archives Programme file:

`EAP880/1/2/55 — Cession of Darjeeling`

contains:

`EAP880/1/2/55/55: Political consultations regarding the negotiations for Darjeeling and the Sikkim Terai region, 17 Oct 1833–24 May 1843, [141 images]`.

Catalogue:

https://searcharchives.bl.uk/catalog/040-003650839

Digitised-content landing page:

https://eap.bl.uk/archive-file/EAP880-1-2-55

The 141-image item covers both target dates and directly concerns Darjeeling/Sikkim political business. The original material is held at the Sikkim Palace Archives; this is not the NAI original-consultation series itself.

Current access state during Wave 80:

- catalogue metadata: directly controlled;
- image set: identified as digitised;
- EAP viewer: blocked in the current research environment by JavaScript/robot verification;
- therefore **no claim that No.147 or No.70 is present in the image set**.

Its value is as a high-priority surrogate/copy route, especially for Campbell/Darjeeling context.

Encode:

`EAP880_1_2_55_55 = DIGITISED_DARJEELING_POLITICAL_CONSULTATION_SURROGATE_CANDIDATE`.

---

## 10. Modern Darjeeling scholarship validates Political Consultation date-number form near the targets

Jayeeta Sharma's research cites NAI Political Consultations around Darjeeling in forms including:

- 22 Nov 1841, nos.87–89;
- 19 Oct 1842, nos.148–151;
- 18 May 1842 Foreign Consultations, no.23;
- multiple earlier Political Consultation dates/numbers.

This does not recover the paper files, but it confirms that the exact archive/finding-aid regime Abdul Ali used remained legible to later Darjeeling historians.

It also makes the following search strategy concrete:

`consultation date + item number`

rather than

`underlying letter date alone`.

Sources:

https://distantreader.org/stacks/journals/transcultural/transcultural-23539.htm

https://d-nb.info/1129632822/34

---

## 11. Updated documentary chronology

### Hodgson 1831/32

- 8 Dec 1831: underlying Hodgson-to-Prinsep letter + paper specimens;
- 13 Jan 1832: Political consultation date;
- No.19: consultation item number.

### O'Shaughnessy 1841

- underlying technical/report date: unresolved;
- 29 Nov 1841: Political consultation date;
- No.147: consultation item number.

### Campbell 1842

- 21 Apr 1842: underlying Campbell-to-Bushby paper letter;
- 11 May 1842: Political consultation date;
- No.70: consultation item number.

The spring-1842 chronology therefore remains:

- 25 Mar — Hodgson pulp-forwarding letter;
- 16 Apr — Darjeeling factory closure reported by Abdul Ali;
- 21 Apr — Campbell substantive letter to Bushby;
- 11 May — Council/departmental consultation processing of at least that letter as No.70.

This is a far cleaner administrative sequence than treating 11 May as a second unknown paper letter.

---

## 12. Revised field model for the dataset

Replace vague `departmental_control_date` where the source is `Political O.C.` with:

- `underlying_letter_date`;
- `consultation_date`;
- `consultation_number`;
- `original_consultation_packet_id`;
- `proceedings_copy_reference`;
- `enclosure_numbers`;
- `order/minute_number` if distinct;
- `draft_reply_number` if distinct;
- `London_transmission_date`;
- `London_derivative_reference`.

For Abdul Ali citations:

`OC_DATE -> consultation_date`

`OC_NO -> consultation_number`.

This should be reflected in any structured chronology/dataset update.

---

## Source-control rules

1. For Abdul Ali's pre-Mutiny `Political O.C.` citations, use `O.C. = Original Consultation` as the controlled working expansion.
2. Mark Wave 79's `Original Collection` expansion as superseded for this specific record context.
3. `consultation date != underlying letter date`.
4. `consultation number` is a date-local/sitting-local documentary number, not automatically an annual letter number.
5. Treat original consultations as packet/document states that can preserve originals, orders, reply drafts/copies and enclosures.
6. Inspect adjacent consultation numbers because one administrative transaction can span several numbered items.
7. Political Proceedings are derivative/copy/register states of the consultation business and may omit enclosures.
8. Keep London Political Letters / Board of Control copies / E/4 duplicates separate from India-side Political Consultations.
9. Do not infer a London shelfmark from O.C. consultation date alone.
10. Keep EAP880/1/2/55/55 as a surrogate candidate, not a proven copy of Nos.147 or 70 until the images are inspected.
11. Retain Political/Secret cross-search as a fallback because Dewar notes historical classification overlap, but do not merge the categories evidentially.

## Immediate next actions

1. Retrieve the NAI Political Consultation index/press list for **29 Nov 1841** and inspect **No.147 plus adjacent numbers**.
2. Retrieve the NAI Political Consultation index/press list for **11 May 1842** and inspect **No.70 plus adjacent numbers**.
3. Use **13 Jan 1832 No.19** as calibration to verify that Abdul Ali's `Pol. O.C.` syntax maps exactly onto the surviving NAI Original Consultation object.
4. Search EAP880/1/2/55/55 images externally/through a browser capable of the EAP viewer for 1841–42 Darjeeling consultation copies.
5. Search later scholarship/press lists for exact date-number pairs; a citation reproducing `11 May 1842 No.70` or `29 Nov 1841 No.147` can reveal subject headings or adjacent item ranges.
6. Search Boards Collections / IOR/F/4 and London Political Letters only after the underlying India-side packet is identified.
7. Search No.147 by Maddock/O'Shaughnessy/bleaching terminology and No.70 by Campbell/Bushby/21 Apr 1842/Darjeeling paper-factory terminology.
8. Update structured datasets to separate underlying-letter date from consultation date/number.

## Bottom line

Wave 80 decodes the archival syntax that Waves 78–79 were circling. In the pre-Mutiny Government-of-India record system, `Original Consultation` was a specific documentary state: original incoming letters, associated orders and reply drafts/copies, potentially with enclosures, retained under the date on which the Council/Board considered the business and under a number assigned within that sitting. Proceedings were derivative register/copy versions. A 1920 handbook of pre-Mutiny records describes this mechanism explicitly and lists `Political Consultations, 1790–1859`; Qeyamuddin Ahmad's NAI-based archival scholarship explicitly defines `O.C.` as `Original Consultation`; modern NAI scholarship cites Political Consultations by precisely the same date-and-number syntax used by Abdul Ali. Consequently `Political O.C., 11 May 1842, No.70` is best read as Political Original Consultation, 11 May 1842, item No.70, containing or processing Campbell's 21 April letter to Bushby. `Political O.C., 29 Nov 1841, No.147` is likewise an item in the Political consultation of that date, associated by Abdul Ali with O'Shaughnessy's bleaching experiment. The search problem has now shifted from decoding the citation to retrieving two exact consultation packets and their adjacent numbered items.