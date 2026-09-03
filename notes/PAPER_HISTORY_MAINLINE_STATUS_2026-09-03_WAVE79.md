# Hodgson paper-history mainline — 2026-09-03, through Wave 79

Status: current active guardrail. Supersedes `PAPER_HISTORY_MAINLINE_STATUS_2026-09-03_WAVE77.md` for ongoing paper-history work and incorporates the documentary-redundancy result of Wave 78 plus the `Political O.C.` correction of Wave 79.

## Current object

The paper-history mainline now follows two coupled transformation chains.

### Material chain

`plant / bark`
-> `pulp`
-> `manufacturing process`
-> `finished sheet`
-> `size / quality class`
-> `ream / local counting unit`
-> `commodity / stationery state`
-> `sample set`
-> `package`
-> `transport / freight state`
-> `experimental feedstock`
-> `working support`
-> `bound / bundled / archival paper object`.

### Documentary chain

`material event`
-> `underlying letter / report`
-> `departmental receipt / forwarding`
-> `Original Collection / proceedings / registered state`
-> `official copy`
-> `duplicate copy`
-> `register`
-> `abstract`
-> `index`
-> `enclosure split`
-> `private copy / extract`
-> `learned-society publication`
-> `later archival citation`.

Current propositions:

**material circulation is multi-metrological**;

**material circulation is multi-documentary**;

**documentary derivation is multi-chronological: event date, underlying-letter date, departmental control date, forwarding date, London transmission date and publication date must be stored separately.**

---

## 1. Direct material anchor: 25 March 1842 pulp consignment

The direct Hodgson letter remains the strongest material anchor:

`Nepal Residency`
-> `24 packages Nepalese paper pulp`
-> `Champaran / Woodcock`
-> `Patna by land OR Govind Gang by water`
-> `Calcutta`.

The route is explicitly conditional on relative carriage cost.

Still missing:

- Halliday's initiating directive;
- Woodcock's route decision;
- Woodcock's bill;
- Patna receipt if the land route was used;
- Govind Gang / river forwarding evidence if the water route was used;
- Calcutta receipt;
- exact experimental destination of the 24 packages.

Guardrail:

`24_PACKAGE_PULP_SHIPMENT = DIRECT`

but

`24_PACKAGES_TO_SERAMPORE = UNPROVEN`.

---

## 2. 1837 primary sample-circulation anchor retained

*Transactions of the Agricultural and Horticultural Society of India*, vol. V directly records that the Society requested from Campbell on 20 Nov 1837:

`a small supply of each size and quality of paper manufactured at Nepaul for experimental purposes`.

Campbell's 28 Nov reply promises supply, proposes sending samples of each variety to the Chamber of Commerce, and encloses copies of recent Scott-Campbell correspondence.

Secure sequence:

`official correspondence`
-> `copied dossier`
-> `learned-society receipt`
-> `classified sample request`
-> `experimental sample circulation`
-> `[commercial sample forwarding proposed]`
-> `publication`.

Keep:

`CHAMBER_FORWARDING = PROPOSED_DIRECT`

and

`CHAMBER_RECEIPT / TEST = UNPROVEN`.

---

## 3. Abdul Ali provenance is revised

Previous mainline language treated the paper evidence primarily as Abdul Ali's 1945 extraction pending article control.

Wave 79 directly recovers the earlier publication:

A. F. M. Abdul Ali, `The Daphne Paper of Nepal`, *Bengal: Past and Present*, vol. 64, serial 127 (1944), pp. 18–30.

A bibliographic source independently records the 1945 republication in *B. C. Law Volume*, part I, pp. 377–391.

Encode:

`ABDUL_ALI_1944_ARTICLE = DIRECTLY_RECOVERED_SECONDARY_WITNESS`

`ABDUL_ALI_1945_REPUBLICATION = BIBLIOGRAPHICALLY_CONTROLLED`

`POLITICAL_OC_PRIMARY_RECORDS = STILL_UNRECOVERED`.

Direct control of the secondary article matters because its citation syntax can now be analysed without relying on later paraphrase.

---

## 4. Abdul Ali explicitly places the archival evidence in the Foreign and Political Department

In the nineteenth-century section Abdul Ali says that contemporary records of the **Foreign and Political Department** provide information on Nepal paper.

His nearby citations use `Pol. O. C.` / `Political O. C.`.

Thus:

`FOREIGN_AND_POLITICAL_DEPARTMENT`
-> `POLITICAL O.C. CITATION DOMAIN`.

This strongly favours an India-side departmental archival meaning.

---

## 5. `Political O.C.` is no longer an opaque date-number pair

Modern National Archives of India scholarship explicitly uses:

`Original Collection (here after O.C.)`

in department/branch/date/number citations.

A parallel NAI citation form is:

`Home, Public, 7 Dec 1836, O.C., no.20`.

Working expansion:

`Political O.C.` ≈ `Political Original Collection`.

Confidence state:

`O.C. = ORIGINAL COLLECTION = HIGH_CONFIDENCE_NAI_USAGE`

`ABDUL_ALI_POLITICAL_O.C._EXACT_EXPANSION = MEDIUM-HIGH / NOT_YET_DIRECT_SERIES_CONTROL`

`MODERN_NAI_SHELFMARK = UNRESOLVED`.

Do not revert to “completely undecoded abbreviation”; do not upgrade to fully direct until an authoritative guide/index/wrapper is recovered.

---

## 6. Proven date split: Hodgson 8 Dec 1831 -> Political O.C. 13 Jan 1832 No.19

Abdul Ali states:

- 8 Dec 1831: Hodgson sends H. T. Prinsep Nepal-paper specimens for presentation to Lord William Bentinck;
- citation: `Pol. O. C., no.19, Jany. 13, 1832`.

Therefore:

`UNDERLYING_LETTER_DATE = 1831-12-08`

`POLITICAL_OC_CONTROL_DATE = 1832-01-13`

`POLITICAL_OC_NUMBER = 19`.

Secure principle:

`POLITICAL_OC_DATE_CAN_POSTDATE_UNDERLYING_LETTER`.

The administrative meaning of the 13 Jan date remains unresolved.

This case is now the best calibration target for decoding O.C. form because sender, recipient, object, purpose, letter date and O.C. date/number are all known.

---

## 7. Proven date split: Campbell 21 Apr 1842 -> Political O.C. 11 May 1842 No.70

Abdul Ali's footnote gives both documentary layers:

`Letter to Mr. G. A. Bushby, 21st April, 1842. Political O. C., 11 May, 1842, no.70.`

Therefore:

`UNDERLYING_CAMPBELL_BUSHBY_LETTER = 1842-04-21`

`POLITICAL_OC_CONTROL = 1842-05-11_NO70`.

The 20-day gap is direct evidence that 11 May is not the underlying paper-letter date.

Encode:

`21_APR_1842 = SUBSTANTIVE_CORRESPONDENCE_EVENT`

`11_MAY_1842 = DOCUMENTARY_CONTROL_EVENT_OF_UNRESOLVED_TYPE`.

This replaces the earlier chronology that treated 11 May as if it might itself be the substantive letter date.

---

## 8. 29 Nov 1841 No.147 now has a tightly controlled subject

Abdul Ali links `Political O.C., 29 Nov 1841, no.147` to the bleaching of Campbell's Darjeeling paper samples by W. B. O'Shaughnessy.

The surrounding narrative identifies:

- T. Maddock, Secretary to the Governor-General, Political Department;
- Dr W. B. O'Shaughnessy, Chemical Examiner;
- two sample packages of Campbell's paper;
- bleaching with chlorine solution;
- red lead, salt, sulphuric acid and water;
- avoidance of oxide of manganese.

Encode:

`OC_1841_11_29_NO147 = DARJEELING_PAPER_BLEACHING / O_SHAUGHNESSY CLUSTER`.

Search by names and technical terms, not only `Nepal paper`.

---

## 9. London political-letter architecture from Wave 78 remains valid, but its relation to O.C. is downgraded

Wave 78 securely established the London derivative architecture:

`Government-of-India Political Letter`
-> `Board of Control copy in IOR/L/PS/6/49-82`
-> `index`
-> `register`
-> `abstract`
-> `abstract index`
-> `E/4 duplicate`
-> `[enclosure may be filed elsewhere]`.

It also located chronological containers:

- `IOR/L/PS/6/57`: 5 Jul–22 Dec 1841;
- `IOR/L/PS/6/58`: 1842.

What Wave 79 changes is the inferential link.

Old provisional logic:

`Political O.C. date -> same-date London Political Letter container`.

Revised logic:

`India-side O.C. control date != necessarily underlying-letter date != necessarily London transmission date`.

Therefore:

`L/PS/6/57 AS MIRROR OF OC NO147 = POSSIBLE, NOT DATE-PROVEN`

`L/PS/6/58 AS MIRROR OF OC NO70 = POSSIBLE, NOT DATE-PROVEN`.

The London architecture remains a recovery path after document identity is established India-side.

---

## 10. 1837 Nepal missing-enclosure case retained as structural control

`IOR/L/PS/5/128, ff.313–316`, `Nepal Affairs`, shows a contemporaneous Nepal-related documentary packet in which Secret-letter enclosures are absent but an abstract survives.

Use only for:

`DOCUMENTARY_DERIVATIVE_CAN_OUTLIVE_SOURCE_PACKET`.

Do not use as evidence that the missing enclosures concerned paper.

Keep:

`POLITICAL != SECRET` unless a source directly links the streams.

---

## 11. Govindgunge remains a triple-function node

### 1825

Company boat-hire metrology:

`COMPANY_ROUTE_METROLOGY_NODE`.

### 1837

Campbell's Nepal-paper market/procurement geography:

`NEPAL_PAPER_MARKET_OR_SUPPLY_NODE`.

### 1842

Hodgson's direct water-route option for the 24 pulp packages:

`SPECIFIC_EXPERIMENTAL_MATERIAL_FORWARDING_NODE`.

Combined proposition:

**market and transport infrastructure overlap at Govindgunge without becoming the same evidential claim.**

---

## 12. Finished-paper freight and pulp-package freight remain separate

Campbell's 1837 finished-paper procurement discussion includes material-specific carriage estimates.

The 1842 Hodgson letter concerns 24 packages of pulp and a missing Woodcock carriage bill.

Keep:

`1837 FINISHED PAPER FREIGHT != 1842 PULP PACKAGE FREIGHT`.

Use the earlier estimate only to establish that paper procurement had already been translated into freight calculation before the pulp experiment.

---

## 13. Serampore functions remain disaggregated

Secure:

`Campbell paper correspondence -> learned-society publication -> Serampore Press`.

Secure at programme level:

`O'Shaughnessy bleaching / paper experimentation -> Marshman / Serampore industrial context`.

Unproven:

`24 packages of 25 Mar 1842 -> Serampore`.

Do not collapse publication site, industrial test site and consignment destination.

---

## 14. Programme continuity remains bounded

Evidence now shows recurrent Government engagement with Nepal paper across:

- 1831/32 Hodgson description + specimen circulation;
- 1837 Campbell office-record substitution / procurement discussion;
- 1837/38 learned-society classified sample circulation;
- 1841 Darjeeling manufacture and O'Shaughnessy bleaching;
- Mar–May 1842 pulp logistics, factory economics and Campbell-Bushby correspondence.

This supports:

`RECURRING_GOVERNMENT_PAPER_PROBLEM_SPACE_WITH_DOCUMENTED_CONTINUITIES_AND_GAPS`.

Still unproven:

`ONE_UNINTERRUPTED_FORMAL_GOVERNMENT_PROGRAMME_1831_1842`.

Need continuation orders, sanctions, proceedings or explicit cross-references for the stronger claim.

---

## 15. Revised spring 1842 chronology

- **25 Mar 1842** — direct Hodgson 24-package pulp-forwarding instruction;
- **16 Apr 1842** — Campbell's Darjeeling factory reported by Abdul Ali as closed under existing economics;
- **21 Apr 1842** — substantive Campbell paper letter to G. A. Bushby;
- **11 May 1842** — that letter appears under `Political O.C. No.70` in Abdul Ali's archival citation system.

Keep:

`TEMPORAL_PROXIMITY != CAUSAL_SEQUENCE`

and

`DOCUMENTARY_CONTROL_DATE != NEW_MATERIAL_EVENT`.

The relation between the 25 Mar pulp consignment and the Campbell factory remains unresolved.

---

## 16. Store multi-date documentary records explicitly

Each reconstructed event should use separate fields where possible:

- `material_event_date`;
- `underlying_letter_date`;
- `departmental_O.C./proceedings_date`;
- `registration_date`;
- `forwarding_date`;
- `London_transmission_date`;
- `London_receipt_date`;
- `reply/despatch_date`;
- `publication_date`;
- `later_archival_citation_date`.

Never collapse these merely because a secondary citation supplies one visible date.

Mechanism:

`DOCUMENTARY_DERIVATION_PRODUCES_MULTIPLE_CHRONOLOGIES`.

---

## Immediate research order

### India-side Political O.C. first

1. Search National Archives of India / Abhilekh Patal guides and indexes for `Original Collection` under Foreign / Political records.
2. Use `13 Jan 1832 No.19` as a calibration object and recover the relationship to Hodgson's 8 Dec 1831 letter.
3. Recover `29 Nov 1841 No.147` via Maddock + O'Shaughnessy + bleaching + two paper packages.
4. Recover `11 May 1842 No.70` via Campbell + Bushby + 21 Apr 1842 + Darjeeling paper factory.
5. Determine what O.C. date and number mean administratively.

### Underlying documents

6. Recover/image-control Hodgson-to-Prinsep, 8 Dec 1831.
7. Recover/image-control Campbell-to-Bushby, 21 Apr 1842.
8. Recover O'Shaughnessy's bleaching report/memorandum and Maddock forwarding documents.

### London derivatives after identity control

9. Search `IOR/L/PS/6`, its registers/abstracts/indexes and `IOR/E/4` by controlled sender/subject/document identity rather than only O.C. date.
10. Follow department-specific enclosures separately.

### Material/logistics mainline

11. Continue Halliday directive / Woodcock bill / Champaran receipt routing.
12. Continue Chamber of Commerce search for 1837 sample receipt or commercial evaluation.
13. Continue testing Govindgunge as an operational paper-market/transport node.

---

## Guardrails

1. Distinguish pulp, finished paper, specimen/sample set and archival support.
2. Distinguish material event from every later documentary state.
3. `O.C. = Original Collection` is a high-confidence working expansion, not yet direct exact-series control.
4. Distinguish underlying letter date from O.C. date.
5. Do not map O.C. dates directly into London volumes without independent document identity.
6. Keep `IOR/L/PS/6/57` and `/58` as possible related containers, not proven O.C. mirrors.
7. Keep Political and Secret streams separate.
8. Keep 1837 finished-paper freight separate from 1842 pulp freight.
9. Keep proposed Chamber forwarding separate from confirmed receipt.
10. Keep Serampore publication, industrial testing and consignment destination distinct.
11. Keep spring-1842 density separate from causal linkage.
12. Treat Abdul Ali 1944 as a directly recovered secondary witness, not as the unrecovered primary archive.
13. Treat 1831–42 as recurrent programme continuity candidate, not one formally continuous programme.

## Current strongest proposition

**Nepal paper moved through a coupled material and documentary system. Its fibre became pulp, finished sheet, classified specimen, procurement commodity, experimental package and archival support; information about those objects simultaneously became letters, departmental collection entries, copies, registers, abstracts, publications and later archival citations. Wave 79 shows that those documentary states also have different clocks. Hodgson's 8 December 1831 paper letter reappears in Abdul Ali's citation as `Political O.C., 13 January 1832, No.19`; Campbell's 21 April 1842 letter to Bushby reappears as `Political O.C., 11 May 1842, No.70`. `O.C.` is very likely the National Archives of India archival abbreviation `Original Collection`. Consequently, paper history can no longer be reconstructed by treating one cited archival date as the date of the material event. The immediate task is to recover the India-side collection state, identify its underlying correspondence and enclosures, and only then trace the resulting London copies and duplicates.**