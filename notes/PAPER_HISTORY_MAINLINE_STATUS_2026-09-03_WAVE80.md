# Hodgson paper-history mainline — 2026-09-03, through Wave 80

Status: **current active guardrail**. Supersedes `PAPER_HISTORY_MAINLINE_STATUS_2026-09-03_WAVE79.md` and incorporates Waves 78–80. Wave 80 corrects one specific Wave-79 inference: for Abdul Ali's pre-Mutiny Foreign/Political citations, `O.C.` should now be read as **Original Consultation**, not Original Collection.

## Critical supersession notice

Retain from Wave 79:

- Abdul Ali 1944 article directly recovered as a secondary witness;
- underlying-letter dates differ from the cited `Political O.C.` dates;
- the India-side record must be recovered before matching London derivatives;
- 8 Dec 1831 -> 13 Jan 1832 No.19 and 21 Apr 1842 -> 11 May 1842 No.70 are secure date splits.

Supersede from Wave 79:

`Political O.C. = Political Original Collection`.

Current controlled reading:

`Political O.C. = Political Original Consultation`.

Evidence basis:

1. Douglas Dewar's 1920 pre-Mutiny archival handbook explicitly says original letters received and drafts/copies of letters issued, when recorded, were styled `Original Consultations` and explains consultation-date/item-number mechanics.
2. The same handbook lists `Political Consultations, 1790–1859` among Imperial Record Department holdings.
3. Qeyamuddin Ahmad's NAI-based archival scholarship explicitly gives `O.C. — Original Consultation` and `For.Dept.Pol.Cons. — Foreign Department Political Consultation`.
4. Modern NAI scholarship cites Political Consultations by `date + no./nos.` in the same syntax as Abdul Ali.

Use `Original Consultation` in all continuing retrieval work.

---

## Current coupled object

### Material chain

`plant / bark`
-> `pulp`
-> `manufacturing process`
-> `finished sheet`
-> `size / quality class`
-> `count unit`
-> `commodity / office stationery candidate`
-> `sample set`
-> `package`
-> `transport / freight state`
-> `experimental feedstock`
-> `working support`
-> `bound / bundled / archival paper object`.

### Documentary chain

`material event`
-> `underlying letter / report`
-> `receipt / departmental circulation`
-> `Council / Board consultation`
-> `Original Consultation packet + date-local item number`
-> `Proceedings copy / narrative`
-> `index / press list / register`
-> `enclosure split`
-> `London transmission / official copy`
-> `E/4 / Boards Collection derivative`
-> `private copy / extract`
-> `learned-society publication`
-> `later archival citation`.

Central proposition:

**material transformation and documentary transformation are coupled but run on different clocks. The date of the material act, the date of the incoming letter, the date on which Council considered the business, the date of a London Political Letter, and the date of publication can all differ.**

---

## 1. Direct material anchor: 25 March 1842 pulp consignment

The direct Hodgson letter still anchors the specific pulp event:

`Nepal Residency`
-> `24 packages Nepalese paper pulp`
-> `Champaran / Woodcock`
-> `Patna by land OR Govind Gang by water`
-> `Calcutta`.

Route choice is explicitly conditional on relative carriage cost.

Still unrecovered:

- Halliday's initiating directive;
- Woodcock's route decision and bill;
- Patna receipt if land branch used;
- Govind Gang / river forwarding record if water branch used;
- Calcutta receipt;
- final experimental destination of the 24 packages.

Keep:

`24_PACKAGE_PULP_SHIPMENT = DIRECT`;

`24_PACKAGES_TO_SERAMPORE = UNPROVEN`.

---

## 2. 1837 classified sample circulation remains direct

*Transactions of the Agricultural and Horticultural Society of India*, vol. V records the Society requesting from Campbell on 20 Nov 1837:

`a small supply of each size and quality of paper manufactured at Nepaul for experimental purposes`.

Campbell's 28 Nov reply:

- promises a quantity;
- proposes forwarding samples of each variety to the Chamber of Commerce;
- encloses copies of recent Scott-Campbell correspondence.

Secure sequence:

`official correspondence`
-> `copied dossier`
-> `learned-society circulation`
-> `classified sample request`
-> `experimental sample circulation`
-> `[commercial sample forwarding proposed]`
-> `publication`.

Keep:

`CHAMBER_FORWARDING = PROPOSED_DIRECT`;

`CHAMBER_RECEIPT / TEST = UNPROVEN`.

---

## 3. Abdul Ali provenance

Directly recovered secondary witness:

A. F. M. Abdul Ali, `The Daphne Paper of Nepal`, *Bengal: Past and Present*, vol. 64, serial 127 (1944), pp.18–30.

Bibliographically controlled republication:

*B. C. Law Volume* (1945), part I, pp.377–391.

Encode:

`ABDUL_ALI_1944_ARTICLE = DIRECTLY_RECOVERED_SECONDARY_WITNESS`;

`POLITICAL_ORIGINAL_CONSULTATIONS = PRIMARY_ARCHIVAL_WITNESSES_STILL_UNRECOVERED`.

Abdul Ali explicitly places his nineteenth-century evidence in the **Foreign and Political Department** record domain.

---

## 4. `Political O.C.` now has controlled archival semantics

### Dewar 1920 record mechanism

The pre-Mutiny record system distinguishes:

#### Original Consultations

Original documentary packets consisting of original letters received, orders passed, and drafts/copies of replies; enclosures can survive here even when omitted from Proceedings.

#### Proceedings

Folio-register copies/narrative versions of the consultation business.

At each Council/Board sitting:

- multiple letters could be considered;
- documents were numbered in the order considered;
- a fresh number sequence was used for each consultation;
- the original cover could carry proceeding number + consultation date.

Therefore:

`POLITICAL_OC_DATE = CONSULTATION_DATE` — HIGH CONFIDENCE;

`POLITICAL_OC_NO = DATE-LOCAL CONSULTATION / PROCEEDING ITEM NUMBER` — HIGH CONFIDENCE.

### Explicit abbreviation

Qeyamuddin Ahmad:

`O.C. = Original Consultation`.

Use this expansion as current controlled reading.

---

## 5. Calibration case: Hodgson 8 Dec 1831 -> consultation 13 Jan 1832 No.19

Abdul Ali:

- underlying letter: Hodgson to H. T. Prinsep, **8 Dec 1831**;
- object: Nepal-paper specimens for Lord William Bentinck;
- archival address: `Pol. O.C., no.19, Jany. 13, 1832`.

Reconstruction:

`8 Dec Hodgson letter`
-> `receipt / circulation`
-> `Political consultation, 13 Jan 1832`
-> `item No.19`
-> `Original Consultation packet`.

Use this as the best calibration object for confirming the surviving NAI archival form.

Do not treat 13 Jan as letter date.

---

## 6. Target A: Political Original Consultation, 29 Nov 1841, No.147

Abdul Ali ties No.147 to Campbell's Darjeeling paper samples and W. B. O'Shaughnessy's bleaching process.

Controlled subject cluster:

- T. Maddock;
- W. B. O'Shaughnessy;
- Campbell;
- Darjeeling paper;
- two sample packages;
- bleaching;
- chlorine;
- red lead;
- salt;
- sulphuric acid;
- avoidance of oxide of manganese.

Encode:

`POLITICAL_OC_1841_11_29_NO147 = POLITICAL_ORIGINAL_CONSULTATION_ITEM`;

`CONSULTATION_DATE = 1841-11-29`;

`CONSULTATION_NO = 147`;

`SUBJECT = DARJEELING_PAPER_BLEACHING / O_SHAUGHNESSY`.

Likely but unproven packet composition:

`sample context / forwarding`
-> `Maddock action`
-> `O'Shaughnessy report`
-> `order/minute`
-> `draft/copy reply`
-> `[enclosure description]`.

Inspect adjacent numbers, not only 147.

---

## 7. Target B: Campbell 21 Apr 1842 -> Political Original Consultation, 11 May 1842, No.70

Abdul Ali's citation gives both layers explicitly:

`Letter to Mr. G. A. Bushby, 21st April, 1842. Political O.C., 11 May, 1842, no.70.`

Encode:

`UNDERLYING_LETTER_DATE = 1842-04-21`;

`SENDER = Archibald Campbell`;

`RECIPIENT = G. A. Bushby`;

`CONSULTATION_DATE = 1842-05-11`;

`CONSULTATION_NO = 70`;

`RECORD_STATE = POLITICAL_ORIGINAL_CONSULTATION`.

Likely but unproven packet composition:

- Campbell original letter;
- manufacturing/process description;
- factory economics / closure argument;
- departmental order/minute;
- draft/copy reply;
- enclosure(s).

Inspect adjacent numbers.

---

## 8. Revised spring 1842 chronology

- **25 Mar 1842** — direct Hodgson 24-package pulp-forwarding instruction;
- **16 Apr 1842** — Darjeeling experimental factory reported by Abdul Ali as closing under existing economics;
- **21 Apr 1842** — Campbell substantive paper letter to Bushby;
- **11 May 1842** — Campbell's business appears in Political consultation as at least No.70.

Thus 11 May is an **administrative processing/consultation event**, not evidence for a second substantive paper letter.

Keep:

`TEMPORAL_PROXIMITY != CAUSAL_SEQUENCE`;

`25_MAR_PULP != PROVEN_INPUT_TO_CAMPBELL_FACTORY`.

---

## 9. Adjacent consultation numbers are now a mandatory retrieval unit

Dewar explains that one sitting numbers documents serially; modern NAI citations commonly cite ranges such as `nos.148–151` or `nos.87–89` for related business.

Therefore search:

`29 Nov 1841 No.147 ± adjacent numbers`

and

`11 May 1842 No.70 ± adjacent numbers`.

Reason:

`incoming letter`
+
`enclosure`
+
`order/minute`
+
`reply draft`

can occupy separate item numbers in one consultation transaction.

Mechanism:

`ADJACENT_CONSULTATION_NUMBERS_CAN_FORM_ONE_ADMINISTRATIVE_TRANSACTION`.

---

## 10. London derivative architecture remains valid but secondary

Wave 78 securely established:

`Government-of-India Political Letter`
-> `Board of Control copy in IOR/L/PS/6`
-> `index/register/abstract`
-> `E/4 duplicate`
-> `[enclosures can move elsewhere]`.

Chronological London containers:

- `IOR/L/PS/6/57`, 5 Jul–22 Dec 1841;
- `IOR/L/PS/6/58`, 1842.

Current status:

`L/PS/6/57 AS MIRROR OF OC NO147 = POSSIBLE, NOT DATE-PROVEN`;

`L/PS/6/58 AS MIRROR OF OC NO70 = POSSIBLE, NOT DATE-PROVEN`.

Reason:

`India-side consultation date != underlying letter date != London transmission date`.

Retrieval order must be:

`identify Original Consultation packet`
-> `identify underlying business and any India-side reply`
-> `establish whether/when transmitted to London`
-> `match London copies / Boards Collections / enclosures`.

---

## 11. EAP880 gives a digitised surrogate route for Darjeeling political consultations

British Library Endangered Archives Programme:

`EAP880/1/2/55 — Cession of Darjeeling`.

Contained item:

`EAP880/1/2/55/55 — Political consultations regarding the negotiations for Darjeeling and the Sikkim Terai region, 17 Oct 1833–24 May 1843, [141 images]`.

Originals are at the Sikkim Palace Archives.

Current evidential state:

`CATALOGUE_METADATA = DIRECT`;

`DIGITISED_IMAGE_SET_EXISTS = DIRECT`;

`NO147_OR_NO70_PRESENT = UNPROVEN` because the EAP image viewer is blocked in the present research environment by JavaScript/robot verification.

Use as:

`DIGITISED_DARJEELING_POLITICAL_CONSULTATION_SURROGATE_CANDIDATE`.

This is high-priority for a browser-enabled pass.

---

## 12. Modern Darjeeling scholarship validates the date-number regime around 1841–42

NAI citations in later scholarship include:

- Political Consultations, 22 Nov 1841, nos.87–89;
- Foreign Consultations, 24 May 1841, nos.59–62;
- Political Consultations, 19 Oct 1842, nos.148–151;
- Foreign Consultations, 18 May 1842, no.23.

This validates the same consultation-date + number architecture in the immediate Darjeeling record environment.

It also confirms that Political and Foreign branches can both matter around Darjeeling.

Keep branch distinctions explicit.

---

## 13. Political / Secret / Foreign branch control

Dewar describes the Foreign Department classification broadly as:

- Secret;
- Political;
- Foreign.

He also warns of historical confusion between Political and Secret classification.

Therefore retrieval strategy:

1. Political first for Abdul Ali's explicitly Political addresses;
2. Foreign branch cross-search where Darjeeling administrative business points there;
3. Secret as controlled fallback if Political search fails or an index cross-reference requires it.

Do not merge the branches into one evidential category.

---

## 14. 1837 Nepal missing-enclosure case remains structural control

`IOR/L/PS/5/128, ff.313–316`, `Nepal Affairs`, documents a Secret-letter packet where source enclosures are absent but an abstract survives.

Use for:

`DOCUMENTARY_DERIVATIVE_CAN_OUTLIVE_SOURCE_PACKET`.

Do not infer those missing enclosures concern paper.

---

## 15. Govindgunge retains three distinct functions

- 1825: Company route-metrology node;
- 1837: Nepal-paper market/procurement geography;
- 1842: specific possible water-forwarding node for 24 pulp packages.

Combined:

`MARKET_INFRASTRUCTURE` and `TRANSPORT_INFRASTRUCTURE` overlap without becoming identical claims.

---

## 16. Finished paper vs pulp freight remains separated

Campbell's 1837 procurement discussion concerns finished-paper carriage.

Hodgson's 1842 instruction concerns 24 packages of pulp.

Keep:

`1837 FINISHED PAPER FREIGHT != 1842 PULP PACKAGE FREIGHT`.

Do not use the 1837 rate to reconstruct Woodcock's missing bill.

---

## 17. Serampore remains functionally disaggregated

Secure:

`Campbell paper correspondence -> Transactions publication -> Serampore Press`.

Secure at programme level:

`O'Shaughnessy bleaching / industrial-paper experimentation -> Marshman / Serampore context`.

Unproven:

`25 Mar 1842 24-package consignment -> Serampore`.

Do not collapse publication site, industrial-test site and shipment destination.

---

## 18. Programme continuity remains bounded

Controlled evidence shows recurrent Government engagement with Nepal paper across:

- 1831/32 Hodgson specimens and office-record argument;
- 1837 Campbell substitution/procurement discussion;
- 1837/38 differentiated sample circulation;
- 1841 Darjeeling manufacture and O'Shaughnessy bleaching;
- Mar–May 1842 pulp logistics + factory economics + Campbell/Bushby consultation processing.

Supports:

`RECURRING_GOVERNMENT_PAPER_PROBLEM_SPACE_WITH_DOCUMENTED_CONTINUITIES_AND_GAPS`.

Still does not prove:

`ONE_UNINTERRUPTED_FORMAL_GOVERNMENT_PROGRAMME_1831_1842`.

---

## Structured chronology fields

For Political O.C. targets store separately:

- `material_event_date`;
- `underlying_letter_date`;
- `consultation_date`;
- `consultation_number`;
- `original_consultation_packet_reference`;
- `adjacent_consultation_numbers`;
- `enclosure_numbers`;
- `order/minute_number`;
- `draft_reply_number`;
- `proceedings_reference`;
- `London_transmission_date`;
- `London_derivative_reference`;
- `publication_date`;
- `later_archival_citation`.

Never collapse consultation date into letter date.

---

## Immediate research order

### Exact Political Original Consultations

1. Recover NAI **Political consultation 29 Nov 1841, No.147**, with several adjacent numbers.
2. Recover NAI **Political consultation 11 May 1842, No.70**, with several adjacent numbers.
3. Recover **Political consultation 13 Jan 1832, No.19** as calibration against Hodgson's known 8 Dec 1831 letter.
4. Determine exact packet boundaries and whether original letters/enclosures remain with the consultation.

### Darjeeling surrogate route

5. Inspect EAP880/1/2/55/55's 141 images in a browser-capable environment, prioritising late 1841 and Apr–May 1842.
6. Cross-check Jayeeta Sharma's cited 1841–42 Darjeeling consultation ranges to understand surrounding filing sequence.

### Underlying documents

7. Recover Campbell-to-Bushby, 21 Apr 1842.
8. Recover O'Shaughnessy bleaching report/memorandum and Maddock forwarding material.
9. Recover Hodgson-to-Prinsep, 8 Dec 1831, ideally in original-consultation form.

### London derivatives

10. Only after packet identity is controlled, trace corresponding Political Letter(s) to London, `IOR/L/PS/6`, `IOR/E/4` and relevant Boards Collections / `IOR/F/4`.

### Material/logistics

11. Continue Halliday directive / Woodcock bill / Champaran route search.
12. Continue Chamber of Commerce 1837 sample-receipt search.
13. Continue Govindgunge operational-node testing.

---

## Guardrails

1. `Political O.C. = Political Original Consultation` for the active paper targets.
2. Wave 79's `Original Collection` expansion is superseded in this context.
3. Consultation date and underlying-letter date are different documentary fields.
4. Consultation number is sitting/date-local unless the source proves otherwise.
5. Inspect adjacent consultation numbers as one potential transaction cluster.
6. Original Consultation and Proceedings are distinct witnesses.
7. Proceedings may omit enclosures preserved in the original packet.
8. India-side consultation and London Political Letter are distinct documentary states.
9. Never infer London shelfmark from consultation date alone.
10. EAP880 is a surrogate candidate, not yet evidence for No.147/70 contents.
11. Political, Foreign and Secret branches remain distinct even when cross-searching.
12. Pulp, finished paper, classified sample and archival support remain distinct material states.
13. 1837 finished-paper freight remains separate from 1842 pulp freight.
14. Proposed Chamber forwarding remains separate from confirmed receipt/testing.
15. Serampore publication, industrial testing and shipment destination remain separate.
16. Spring-1842 date density remains separate from causal linkage.
17. Abdul Ali 1944 is a directly controlled secondary witness, not the primary archive.
18. 1831–42 remains a recurrent programme-level continuity candidate, not proven formally uninterrupted programme.

## Current strongest proposition

**The Nepal-paper programme can now be reconstructed through a coupled material/consultation system rather than a flat chronology of letters. Materially, bark, pulp, finished paper, classified samples, freight packages and archival supports changed function as they moved through government, learned-society and industrial settings. Administratively, the underlying letters were themselves transformed: received correspondence was put before Council or Board, grouped into a dated consultation, assigned item numbers within that sitting, retained with orders and reply drafts as an Original Consultation packet, and copied into Proceedings before some business was transmitted onward to London. Abdul Ali's two previously opaque archival addresses therefore have a specific meaning. Campbell's 21 April 1842 paper letter to Bushby was processed as Political Original Consultation No.70 on 11 May; the O'Shaughnessy bleaching material appears under Political Original Consultation No.147 on 29 November 1841. The next decisive move is no longer abbreviation decoding. It is packet recovery: retrieve those two dated consultation items with their adjacent numbers, identify the original letters, enclosures, orders and draft replies, then trace the resulting London derivatives.**