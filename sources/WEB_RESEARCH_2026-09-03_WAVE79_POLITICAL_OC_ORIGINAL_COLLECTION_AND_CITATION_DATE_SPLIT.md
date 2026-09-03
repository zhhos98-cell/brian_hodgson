# Web/archive research 2026-09-03 — Wave 79
## `Political O.C.` citation-layer split, likely `Original Collection`, and correction of the 1841–42 retrieval model

Date: 2026-09-03

Status: active paper-history mainline. Follow-up to Waves 77–78.

This wave returns to A. F. M. Abdul Ali's own article rather than treating his two 1841–42 archival citations as isolated strings. The direct 1944 *Bengal: Past and Present* version is now text-controlled through the Internet Archive OCR of vol. 64, serial 127, pp. 18–30. Bibliographic sources also identify the 1945 *B. C. Law Volume* version, part I, pp. 377–391, as a second publication of the same title.

The decisive result is that Abdul Ali repeatedly distinguishes the date of an underlying letter from the date and number of the cited `Political O.C.` record. Therefore `29 Nov 1841 No.147` and `11 May 1842 No.70` should no longer be treated first as dates of Government-of-India Political Letters transmitted to London. They are more plausibly identifiers of an India-side archival/documentary wrapper, collection or registered record state that contains, abstracts, or preserves an earlier underlying communication.

A second result substantially narrows the abbreviation. Modern scholarship using National Archives of India records explicitly expands `O.C.` as **Original Collection**, in a citation syntax closely matching Abdul Ali's: department/branch + date + `O.C.` + number. This makes `Political O.C.` = `Political Original Collection` a **high-confidence working expansion**, but not yet a contemporaneously catalogued expansion for Abdul Ali's exact series. Until a National Archives of India guide, catalogue, index, or original wrapper directly confirms the Political series label, retain the expansion as `HIGH_CONFIDENCE_INFERENCE`, not `DIRECT_SERIES_CONTROL`.

## Executive result

### Direct date split 1: Hodgson / Prinsep

Abdul Ali states that on **8 December 1831** B. H. Hodgson sent H. T. Prinsep specimens of Nepal paper for presentation to Lord William Bentinck.

His footnote is:

`Pol. O. C., no. 19, Jany. 13, 1832.`

Thus:

`UNDERLYING_HODGSON_LETTER_DATE = 1831-12-08`

while

`POLITICAL_OC_DATE = 1832-01-13`

and

`POLITICAL_OC_NUMBER = 19`.

This proves that the `Pol. O.C.` date is not necessarily the date of the underlying letter quoted by Abdul Ali.

### Direct date split 2: Campbell / Bushby

Abdul Ali's footnote 31 reads, in the 1944 OCR:

`Letter to Mr. G. A. Bushby, 21st April, 1842. Political O. C., 11 May, 1842, no. 70.`

Thus:

`UNDERLYING_CAMPBELL_BUSHBY_LETTER_DATE = 1842-04-21`

while

`POLITICAL_OC_DATE = 1842-05-11`

and

`POLITICAL_OC_NUMBER = 70`.

Again:

`UNDERLYING_LETTER_DATE != POLITICAL_OC_DATE`.

This is the most important correction to the Wave 78 retrieval model.

### 29 November 1841 No.147

Abdul Ali cites:

`Political O. C., 29 Nov., 1841, no. 147`

for O'Shaughnessy's bleaching process and again for the note explaining the advantage of red lead over oxide of manganese.

The cited record supports technical content concerning bleaching of Campbell's Darjeeling paper samples. The date/number should now be treated as the archival/documentary identifier of the Political O.C. record state, not automatically as the date/number of a transmitted London Political Letter.

### `O.C.` expansion

A modern study citing National Archives of India material explicitly gives:

`Home Department, Public Branch ... Original Collection (here after O.C.), 19th October, No. 23, National Archives of India, New Delhi.`

Another archival study gives the parallel form:

`Home, Public, 7 Dec, 1836, O.C., no.20, NAI; Foreign, P.C., 15 August, 1836, 46, NAI.`

The syntax is materially close to Abdul Ali's:

`Political O.C., [date], no.[number]`.

Encode:

`OC_EXPANSION_ORIGINAL_COLLECTION = HIGH_CONFIDENCE_INFERENCE`

but retain:

`POLITICAL_OC_EXACT_NAI_SERIES_LABEL = NOT_YET_DIRECTLY_CONTROLLED`.

---

## 1. Direct source recovery: Abdul Ali 1944, not only the 1945 reprint

Internet Archive item:

- *Bengal: Past and Present*, vol. 64, serial 127;
- A. F. M. Abdul Ali, `The Daphne Paper of Nepal`;
- 1944;
- pp. 18–30.

Internet Archive full-text OCR:

https://archive.org/stream/dli.calcutta.04040/H00220_djvu.txt

Bibliographic control independently gives:

- Abdul Ali, `The daphne paper of Nepal`, *Bengal Past and Present*, LXIV, 127, Jan–Dec 1944, pp. 18–30;
- republication in *B. C. Law Volume*, Calcutta, Indian Research Institute, 1945, part I, pp. 377–391.

Bibliographic source:

https://pahar.in/pahar/Books%20and%20Articles/Nepal/1969%20Bibliographie%20Du%20Nepal%20Volume%201%20Sciences%20Humaines%20by%20Boulnois%20s.pdf

Source-control consequence:

`ABDUL_ALI_1944_BPP_TEXT = DIRECTLY_RECOVERED_SECONDARY_SOURCE`

and

`ABDUL_ALI_1945_BC_LAW_VERSION = BIBLIOGRAPHICALLY_CONTROLLED_REPUBLICATION`.

The paper-history notes should therefore stop describing the Abdul Ali evidence only as a 1945 extraction pending recovery of the article text.

---

## 2. Abdul Ali identifies the source domain as the Foreign and Political Department

Immediately before quoting Hodgson's December 1831 description of Nepal paper, Abdul Ali writes that contemporary records of the **Foreign and Political Department** yield information on the nineteenth-century industry.

He then quotes Hodgson's description of Nepal paper as cheap, available in large quantities, tough, durable and especially suitable for office records.

His nearby notes 4–5 and 8 use `Pol. O. C.`.

Thus the source logic is internally coherent:

`FOREIGN_AND_POLITICAL_DEPARTMENT_RECORD_DOMAIN`
-> `POLITICAL O.C. CITATION`.

This substantially reduces the chance that `Political O.C.` is an unrelated London India Office shorthand invented by later cataloguing.

Mechanism:

`SECONDARY_CITATION_LABEL_PRESERVES_INDIA_SIDE_DEPARTMENTAL_PROVENANCE`.

---

## 3. First proven wrapper-date split: 8 Dec 1831 -> 13 Jan 1832 No.19

Abdul Ali's narrative says:

- 8 Dec 1831: Hodgson, Resident at Kathmandu, sends H. T. Prinsep specimens of Nepal paper;
- purpose: presentation to Lord William Bentinck;
- Hodgson recommends Nepal paper for durable office records.

Footnote 26:

`Pol. O. C., no. 19, Jany. 13, 1832.`

This is not a marginal chronological discrepancy. It establishes a documentary transformation:

`HODGSON LETTER 8 DEC 1831`
-> `[administrative receipt / forwarding / consultation / collection state]`
-> `POLITICAL O.C. 13 JAN 1832 NO.19`.

The bracketed intermediate operation remains to be recovered.

Do not yet encode whether 13 Jan 1832 is:

- consultation date;
- collection date;
- proceedings date;
- registration date;
- forwarding date;
- abstract date;
- another departmental control date.

What is secure is only:

`POLITICAL_OC_DATE_CAN_POSTDATE_UNDERLYING_LETTER`.

---

## 4. Second proven wrapper-date split: 21 Apr 1842 -> 11 May 1842 No.70

Abdul Ali discusses Campbell's Darjeeling paper manufacture and cites Campbell writing to G. A. Bushby, Secretary to the Government of India, Political Department.

The crucial footnote reads:

`Letter to Mr. G. A. Bushby, 21st April, 1842. Political O. C., 11 May, 1842, no. 70.`

This produces a 20-day separation:

`21 APR 1842 UNDERLYING LETTER`
-> `11 MAY 1842 POLITICAL O.C. RECORD`.

This is direct evidence against the previous operational shortcut:

`POLITICAL_OC_DATE = LETTER_DATE`.

Correct encoding:

`POLITICAL_OC_DATE = DOCUMENTARY_CONTROL_DATE_OF_UNRESOLVED_TYPE`.

Mechanisms:

- `DOCUMENT_WRAPPER_HAS_OWN_DATE_AND_NUMBER`;
- `UNDERLYING_LETTER_AND_ARCHIVAL_COLLECTION_ENTRY_ARE_DISTINCT_STATES`;
- `SECONDARY_CITATION_CAN_PRESERVE_BOTH_DOCUMENTARY_LAYERS`.

---

## 5. The 29 Nov 1841 No.147 citation belongs to the bleaching experiment

Abdul Ali says that in 1841 T. Maddock, Secretary to the Governor-General in the Political Department, sent two sample packages of Campbell's paper to Dr W. B. O'Shaughnessy, Chemical Examiner, for bleaching.

He then gives O'Shaughnessy's process using chlorine solution and cites:

`Political O. C., 29 Nov., 1841, no. 147`.

The same citation is repeated in the note on red lead, salt, sulphuric acid and the advantage of avoiding oxide of manganese.

Thus No.147 is not merely a generic Nepal-policy entry. It is directly tied, through Abdul Ali's extraction, to:

- Campbell's Darjeeling paper samples;
- transfer to O'Shaughnessy;
- bleaching chemistry;
- materials and cost/practical availability.

Encode:

`POLITICAL_OC_1841_11_29_NO147_SUBJECT = DARJEELING_NEPAL_PAPER_BLEACHING / O_SHAUGHNESSY`.

This gives a much better subject-search key than `Nepal paper` alone.

High-value names/terms:

`Maddock`, `O'Shaughnessy`, `Campbell`, `Darjeeling`, `bleaching`, `chlorine`, `red lead`, `oxide of manganese`, `paper samples`, `two packages`.

---

## 6. The 11 May 1842 No.70 citation contains at least the 21 Apr Campbell-Bushby letter

The 1842 pointer now has a secure internal object:

`Campbell -> G. A. Bushby, 21 Apr 1842`.

Abdul Ali uses it in the discussion of Campbell's manufacturing method and the economics/closure of the Darjeeling experiment.

The same section says the experimental paper factory worked until 16 Apr 1842 and was closed because Campbell considered the existing operation uneconomical without better and more expensive machinery.

Therefore the retrieval target is no longer an abstract anonymous Political item:

`POLITICAL_OC_1842_05_11_NO70`
contains/preserves/refers to at least
`CAMPBELL_TO_BUSHBY_1842_04_21_PAPER_LETTER`.

Search terms:

`Campbell`, `Bushby`, `paper`, `Darjeeling`, `factory`, `machinery`, `wire gauze`, `potass`, `alkaline solution`, `16 April 1842`, `21 April 1842`.

---

## 7. `O.C.` is very likely `Original Collection`

A modern NAI citation explicitly spells out:

`Original Collection (here after O.C.)`.

Its citation architecture is:

`Home Department`
-> `Public Branch`
-> `year/pages`
-> `Original Collection / O.C.`
-> `date`
-> `number`
-> `National Archives of India`.

Another source gives:

`Home, Public, 7 Dec, 1836, O.C., no.20, NAI`

next to:

`Foreign, P.C., 15 August, 1836, 46, NAI`.

Sources:

https://www.nam-sism.org/Fucina%20di%20marte/Carbone%20%28cur%29%20Forza%20alla%20legge%20Studi%20storici%20su%20Carabinieri%20Gendarmerie%20e%20polizie%20armate%20n%2014.pdf

https://pmml.nic.in/downloadSeries/356

The first source is explicit expansion evidence; the second is useful pattern evidence.

Working reconstruction:

`Political O.C.`
≈
`Political [branch], Original Collection`.

Confidence:

`HIGH` for `O.C. = Original Collection` as an NAI archival abbreviation;

`MEDIUM-HIGH` that this is exactly Abdul Ali's intended expansion in the Political citation;

`UNRESOLVED` for the precise modern NAI shelfmark/series and for the administrative operation represented by the O.C. date.

Do not upgrade to `DIRECT` until an authoritative archival guide/catalogue or the original Political O.C. wrapper confirms it.

---

## 8. Wave 78 London mirror dates must be downgraded

Wave 78 mapped:

`Political O.C., 29 Nov 1841, No.147`
-> `IOR/L/PS/6/57` because that London volume covers 5 Jul–22 Dec 1841;

and

`Political O.C., 11 May 1842, No.70`
-> `IOR/L/PS/6/58` because that London volume covers 1842.

Those remain chronologically possible London mirrors of related correspondence, but the new evidence changes their status.

Previously:

`POLITICAL_OC_DATE` was provisionally used as a chronological key into London Political Letters Received.

Now:

`POLITICAL_OC_DATE` is shown to differ from the underlying communication date.

Therefore encode:

`LPS_6_57_AS_MIRROR_OF_OC_NO147 = POSSIBLE / NOT_DATE_PROVEN`

`LPS_6_58_AS_MIRROR_OF_OC_NO70 = POSSIBLE / NOT_DATE_PROVEN`.

For No.70, the better London chronological key for the underlying item may be **21 Apr 1842**, not 11 May 1842, depending on what was later transmitted to London and when.

For No.19, the same method would distinguish 8 Dec 1831 from 13 Jan 1832.

General rule:

`INDIA_SIDE_COLLECTION_DATE != UNDERLYING_LETTER_DATE != LONDON_TRANSMISSION_DATE`.

All three dates can coexist.

---

## 9. Retrieval priority should move India-side before London-side

Revised hierarchy:

### Tier 1 — decode and recover India-side `Political O.C.`

1. National Archives of India catalogue/guide/index for Foreign / Political records;
2. identify `Original Collection` or equivalent historical series;
3. locate 29 Nov 1841 No.147;
4. locate 11 May 1842 No.70;
5. locate 13 Jan 1832 No.19 as a calibration case.

The 1832 case is particularly useful because Abdul Ali gives the underlying 8 Dec 1831 Hodgson letter and its O.C. wrapper date. It can reveal how the series transformed correspondence.

### Tier 2 — recover underlying letters/enclosures

- Hodgson to Prinsep, 8 Dec 1831;
- Campbell/Bushby, 21 Apr 1842;
- O'Shaughnessy bleaching memorandum/report associated with No.147;
- any Maddock forwarding letter;
- any Campbell sample enclosure.

### Tier 3 — then trace London documentary derivatives

Only after the India-side document identity is clearer should we map:

- Government-of-India Political Letter to London;
- `IOR/L/PS/6` received-letter copies;
- `IOR/E/4` duplicate branch;
- London register/abstract/index;
- outgoing Political despatch response.

This prevents a false equivalence between a departmental O.C. control date and a London transmission date.

---

## 10. The 1832 case becomes a calibration object for the entire retrieval architecture

Wave 78 concentrated on 1841–42 because those are the immediate paper-factory targets.

Wave 79 shows that `13 Jan 1832 No.19` is methodologically more valuable than it first appeared.

Why:

- underlying letter date is explicitly given: 8 Dec 1831;
- sender is known: B. H. Hodgson;
- recipient is known: H. T. Prinsep;
- object is known: Nepal paper specimens;
- intended onward recipient is known: Lord William Bentinck;
- O.C. record date/number is known: 13 Jan 1832 No.19;
- Abdul Ali quotes substantive content from it.

Thus this one case can test:

`LETTER -> O.C. WRAPPER / COLLECTION ENTRY`.

If the 1832 O.C. object can be recovered first, its physical/archival form may decode the 1841–42 records faster than searching those targets blind.

Mechanism:

`EARLIER_WELL_SPECIFIED_CASE_CAN_CALIBRATE_LATER_ARCHIVAL_CITATIONS`.

---

## 11. Document chronology must now be multi-date

For each paper event, store separate fields:

- `event_date`;
- `underlying_letter_date`;
- `departmental_collection_or_proceedings_date`;
- `registration_date` if known;
- `forwarding_date`;
- `London_received_letter_date`;
- `London_reply/despatch_date`;
- `publication_date`;
- `later_archival_citation_date`.

Do not collapse these into one `date` field.

Example:

### Hodgson 1831/32

`event / letter = 8 Dec 1831`

`Political O.C. control = 13 Jan 1832 No.19`

### Campbell 1842

`underlying letter = 21 Apr 1842`

`Political O.C. control = 11 May 1842 No.70`.

Mechanism:

`DOCUMENTARY_DERIVATION_PRODUCES_MULTIPLE_CHRONOLOGIES`.

This is the chronological counterpart of Wave 78's documentary-derivation graph.

---

## 12. Source-control revision for Abdul Ali

Old shorthand in the repo:

`Abdul Ali 1945 archival extraction = secondary source pending direct article control`.

Revised:

`Abdul Ali 1944 BPP article = directly recovered secondary witness to archival citations and quoted content`.

Still required:

`Political O.C. original record = primary archival witness`.

Therefore:

`DIRECT_ARTICLE_CONTROL != DIRECT_ARCHIVE_CONTROL`.

But direct article control allows us to distinguish Abdul Ali's own citation syntax from later paraphrase or bibliographic error.

The article also makes clear that he was using Foreign and Political Department records for the nineteenth-century section.

---

## 13. Revised spring 1842 chronology

Current controlled sequence:

- **25 Mar 1842** — Hodgson directs movement of 24 packages of Nepalese paper pulp through Champaran, with Patna-land / Govind Gang-water routing alternatives;
- **16 Apr 1842** — Abdul Ali reports Campbell's Darjeeling experimental factory as closing under existing economic conditions;
- **21 Apr 1842** — Campbell writes G. A. Bushby about the paper experiment;
- **11 May 1842** — the Campbell/Bushby letter appears under `Political O.C. No.70` in Abdul Ali's citation system.

This improves the chronology because 11 May is now documentary processing/control, not necessarily a new substantive paper event.

Encode:

`21_APR_1842 = SUBSTANTIVE_CORRESPONDENCE_EVENT`

`11_MAY_1842 = DOCUMENTARY_CONTROL_EVENT_OF_UNRESOLVED_TYPE`.

The distinction matters when testing causal relation to the 25 Mar pulp consignment.

---

## 14. Revised research questions

### A. What exactly is an O.C. object?

Need direct evidence for whether `Original Collection` denotes:

- loose original incoming papers arranged under a consultation date;
- a separately numbered collection under departmental proceedings;
- a compilation created for record preservation;
- another NAI series form.

### B. Why does the O.C. date postdate the underlying letter?

For the two controlled examples the lag is:

- 8 Dec 1831 -> 13 Jan 1832: 36 days;
- 21 Apr 1842 -> 11 May 1842: 20 days.

Do not assume a fixed administrative lag. Recover the workflow.

### C. Does No.147 preserve O'Shaughnessy's report itself or a Political forwarding wrapper?

Search for Maddock and O'Shaughnessy together.

### D. Does No.70 contain multiple enclosures?

Abdul Ali uses it both for Campbell's manufacturing process and closure/economic argument. It may represent a packet rather than a single letter.

### E. What London record corresponds to the India-side O.C. object?

This must be established by document identity, not date interpolation.

---

## Source-control rules

1. `O.C. = Original Collection` is now a high-confidence NAI-based inference; do not label it direct confirmation of Abdul Ali's exact Political series until an authoritative series record is recovered.
2. `Political O.C. date` and `underlying letter date` are demonstrably distinct in at least two Abdul Ali citations.
3. Do not use 29 Nov 1841 or 11 May 1842 as automatic London transmission dates.
4. Keep `IOR/L/PS/6/57` and `/58` as possible related London containers, not date-proven mirrors of O.C. Nos.147/70.
5. For No.70, store 21 Apr 1842 as the underlying Campbell-Bushby letter date and 11 May 1842 as the O.C. control date.
6. For No.19, store 8 Dec 1831 as the underlying Hodgson-Prinsep letter date and 13 Jan 1832 as the O.C. control date.
7. No.147 is securely associated through Abdul Ali with O'Shaughnessy's bleaching experiment, but the exact underlying document date remains unresolved.
8. Direct control of Abdul Ali's 1944 article does not substitute for recovery of the Political O.C. primary records.
9. Use the 1832 No.19 case as a calibration target for decoding archival form.
10. Maintain separate date fields for event, letter, departmental control, forwarding, London transmission and publication.

## Immediate next actions

1. Search National Archives of India / Abhilekh Patal guides for `Original Collection`, especially Foreign and Political Department records around 1831–42.
2. Use `13 Jan 1832 No.19` as the calibration target because its underlying Hodgson letter is independently specified by Abdul Ali.
3. Search the 1841 target by `Maddock + O'Shaughnessy + bleaching + Campbell + Darjeeling + two packages`, not only Nepal/paper.
4. Search the 1842 target by `Campbell + Bushby + 21 Apr 1842 + paper + Darjeeling factory`.
5. Recover any original O.C. wrapper/index image and determine what the O.C. date and number signify administratively.
6. Only after India-side identity is controlled, remap related correspondence into `IOR/L/PS/6`, `IOR/E/4`, registers and abstracts.
7. Revise the mainline chronology so that 11 May 1842 is a documentary-control event, not a substantive letter date.
8. Revise Abdul Ali provenance from `1945-only extraction` to `1944 article directly recovered + 1945 republication bibliographically controlled`.

## Bottom line

Wave 79 turns `Political O.C.` from an opaque date-number pair into a partially decoded archival form. Abdul Ali himself proves that an O.C. citation can postdate the underlying correspondence: Hodgson's 8 Dec 1831 paper letter is cited as `Pol. O.C., 13 Jan 1832, No.19`, while Campbell's 21 Apr 1842 letter to Bushby is cited as `Political O.C., 11 May 1842, No.70`. Modern National Archives of India citation practice independently shows `O.C.` expanded as `Original Collection` in the same broad department/date/number syntax. The strongest current model is therefore an India-side Political Original Collection or closely related collection state with its own control date and number. This is not yet a fully decoded modern shelfmark, but it is enough to change retrieval order: recover the India-side O.C. object first, then trace its letters, enclosures and London derivatives. The paper programme now has not only a documentary derivative graph but a multi-date chronology in which the material event, underlying letter, departmental collection entry and London transmission may all occupy different dates.