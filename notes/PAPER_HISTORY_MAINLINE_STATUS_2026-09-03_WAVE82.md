# Hodgson paper-history mainline — 2026-09-03, through Wave 82

Status: **current active guardrail**. Supersedes `PAPER_HISTORY_MAINLINE_STATUS_2026-09-03_WAVE80.md` and incorporates Waves 81–82.

## Critical updates since Wave 80

1. `Political O.C.` remains controlled as **Political Original Consultation**.
2. A. F. M. Abdul Ali is directly documented by NAI as Keeper of Records / long-serving head of the Imperial Record Department; identity with the 1944 Nepal-paper author is very high confidence.
3. The 1937 IHRC proceedings directly show Abdul Ali, as Keeper of the Records of the Government of India and ex-officio IHRC Secretary, signing the complete historical-exhibition list.
4. The Imperial Record Department's 1937 exhibits include:
   - `Pol. Con. 13 Jan 1832, Nos.18–20` — indigenous paper manufacture in Himalayan tracts / Nepal;
   - `Pol. Con. 29 Nov 1841, No.147` — W. B. O'Shaughnessy's report on bleaching paper manufactured at Darjeeling.
5. Therefore the 1832 calibration object is a **Nos.18–20 consultation cluster**, not No.19 alone.
6. No.147 is now directly controlled as an identifiable O'Shaughnessy bleaching report that survived in IRD custody to 1937.
7. India Political Consultations survive in London in `IOR/P`; date+number identity can persist across NAI and IOR.
8. A documentary citation places **11 May 1842 Political consultation material in `IOR/P/196/12`**. Treat this as the high-confidence first London volume for Abdul Ali's No.70, pending item-level image control.
9. Exact `IOR/P` volume for 29 Nov 1841 No.147 remains unresolved. Do not interpolate.

---

## Current coupled material/documentary model

### Material transformation

`plant / bark`
-> `pulp`
-> `manufacturing process`
-> `finished sheet`
-> `size / quality class`
-> `commodity / stationery candidate`
-> `classified sample`
-> `package`
-> `transport / freight state`
-> `experimental feedstock`
-> `working support`
-> `archival paper object`.

### Documentary transformation

`material event`
-> `underlying letter / report`
-> `departmental circulation`
-> `Political consultation`
-> `Original Consultation packet + date-local number(s)`
-> `Proceedings / index / press list`
-> `London IOR/P consultation witness`
-> `[possible Political Letter transmission]`
-> `IOR/L/PS/6 / E/4 / Boards Collection derivatives`
-> `private copy / learned-society publication`
-> `archival exhibition object`
-> `later scholarly extraction`.

Wave 82 adds explicitly:

`ARCHIVE OBJECT -> CURATED HISTORICAL EXHIBIT -> SCHOLARLY SECONDARY SOURCE`.

---

## 1. Direct material anchor remains 25 March 1842

Hodgson's direct instruction:

`Nepal Residency`
-> `24 packages Nepalese paper pulp`
-> `Champaran / Woodcock`
-> `Patna by land OR Govind Gang by water`
-> `Calcutta`.

Still missing:

- Halliday directive;
- Woodcock route decision / bill;
- route receipts;
- Calcutta receipt;
- exact experimental destination.

Keep:

`24_PACKAGE_PULP_SHIPMENT = DIRECT`;

`24_PACKAGES_TO_SERAMPORE = UNPROVEN`.

---

## 2. 1837 differentiated sample circulation remains direct

Agricultural and Horticultural Society evidence:

`each size and quality of paper manufactured at Nepaul`
requested for experimental purposes.

Campbell also proposes forwarding samples of each variety to the Chamber of Commerce and circulates copies of official correspondence.

Keep:

`CLASSIFIED_SAMPLE_CIRCULATION = DIRECT`;

`CHAMBER_FORWARDING = PROPOSED_DIRECT`;

`CHAMBER_RECEIPT_OR_TEST = UNPROVEN`.

---

## 3. Abdul Ali is now a source with direct archival-curatorial provenance

Directly recovered:

- 1920s–30s archival career / Keeper role;
- 1925 pre-Mutiny records handbook under his guidance;
- 1937 IHRC role as Keeper of the Records of the Government of India and ex-officio Secretary;
- signature beneath the complete exhibition list;
- 1944 `The Daphne Paper of Nepal`.

Therefore use three evidential layers:

`ABDUL_ALI_HISTORICAL_INTERPRETATION = SECONDARY`;

`ABDUL_ALI_ARCHIVAL_ADDRESS = HIGH_VALUE_PROFESSIONAL_FINDING_AID_TRACE`;

`ABDUL_ALI_PREPUBLICATION_CONTACT_WITH_TARGET_RECORD_FAMILY = DIRECTLY_ATTESTED_BY_1937_EXHIBITION_CONTEXT`.

Do not claim he personally selected each exhibit or that the 1944 article was written directly from exhibition notes.

---

## 4. 1932? correction: 1832 paper cluster is Nos.18–20

Correct object:

`Political Consultation, 13 Jan 1832, Nos.18–20`.

IRD 1937 description:

`Indigenous method of manufacturing paper in the Himalayan tracts (Nepal, etc.)`.

Abdul Ali 1944 uses No.19 for Hodgson's 8 Dec 1831 communication.

Therefore:

`NO19 = SPECIFIC CITED ITEM WITHIN A THREE-NUMBER PAPER CLUSTER`.

Immediate retrieval must include Nos.18, 19 and 20.

Do not assign document types until the packet is recovered.

This is now a direct confirmation of:

`ADJACENT_CONSULTATION_NUMBERS_CAN_FORM_ONE_PAPER_TRANSACTION`.

---

## 5. 1841 target is directly attested as an O'Shaughnessy report

Target:

`Political Consultation, 29 Nov 1841, No.147`.

IRD 1937 exhibit description:

`Report on the method of bleaching paper manufactured at Darjeeling by Dr. W. B. O'Shaughnessy, M.D., Chemical Examiner of Calcutta`.

Encode:

`NO147_DOCUMENT_TYPE = REPORT`;

`NO147_EXPERT = W_B_O_SHAUGHNESSY`;

`NO147_SUBJECT = DARJEELING_PAPER_BLEACHING`;

`NO147_SURVIVAL_IN_IRD_1937 = DIRECT`.

Still unresolved:

- exact modern NAI object/shelf reference;
- exact IOR/P volume;
- adjacent forwarding/order/reply items;
- exact relation of Campbell's samples to No.147's physical packet.

Do not infer the IOR/P volume from sequence.

---

## 6. 1842 target now has a high-confidence IOR/P volume

Underlying document:

`Campbell -> G. A. Bushby, 21 Apr 1842`.

Consultation address:

`Political Original Consultation, 11 May 1842, No.70`.

Independent documentary citation:

`11 May 1842 India Political consultation material -> IOR/P/196/12`.

Therefore encode:

`TARGET_1842_IOR_P_VOLUME = IOR/P/196/12 — HIGH CONFIDENCE`;

`TARGET_1842_ITEM_NO70 = NOT_YET_IMAGE_CONTROLLED`.

This supersedes the earlier bracket-only state between `/10` and `/13`.

First retrieval unit:

`IOR/P/196/12`
-> `11 May 1842`
-> `No.70`
-> `adjacent numbers`.

Verification terms:

`Campbell`, `Bushby`, `Darjeeling`, `paper`, `factory`, `machinery`, `wire gauze`, `potass`, `closure`, `21 Apr 1842`.

---

## 7. 11 May 1842 is consultation processing, not a new paper event

Chronology:

- 25 Mar — Hodgson 24-package pulp-forwarding instruction;
- 16 Apr — Campbell factory closure reported in Abdul Ali;
- 21 Apr — Campbell substantive paper letter to Bushby;
- 11 May — Political consultation processing, No.70, now sought in `IOR/P/196/12`.

Keep:

`CONSULTATION_DATE != UNDERLYING_LETTER_DATE`;

`DOCUMENTARY_PROCESSING_DATE != NEW_MATERIAL_EVENT`;

`TEMPORAL_PROXIMITY != CAUSAL_SEQUENCE`.

---

## 8. 1937 is a survival checkpoint

For No.147:

`1841 report`
-> `1937 IRD custody + historical exhibition`
-> `1944 Abdul Ali article`
-> `2026 retrieval attempt`.

Thus:

`NO147_EXISTED_IN_IRD_CUSTODY_IN_1937 = SECURE`.

Any present inability to retrieve it is a modern discovery/access problem, not evidence of nineteenth- or early-twentieth-century loss.

The same logic applies at cluster level to the 1832 Nos.18–20 paper-manufacture records.

---

## 9. Curatorial reclassification is now part of paper history

The Political Department originally generated these records as administrative business.

By 1937 the Imperial Record Department curated them as examples of:

- indigenous Himalayan/Nepal paper manufacture;
- chemical bleaching of Darjeeling paper.

Therefore:

`POLITICAL_ADMINISTRATIVE_RECORD`
-> `ARCHIVAL_RECORD`
-> `TECHNOLOGY_HISTORY_EXHIBIT`.

This is not external to the material history. The archive itself reclassified the paper object and its documentary witnesses into a history-of-technology frame before Abdul Ali's 1944 publication.

Mechanism:

`ARCHIVAL_CURATORSHIP_CREATES_A_NEW_DOCUMENTARY_FUNCTION`.

---

## 10. London recovery hierarchy

### First London layer

`IOR/P India Political Consultations / Proceedings`.

For 1842:

`IOR/P/196/12` first.

For 1841:

exact volume still open.

### Later transmission layers

Only after consultation identity:

- `IOR/L/PS/6` Political Letters Received;
- `IOR/E/4` duplicate correspondence;
- `IOR/F/4` / Boards Collections / separated enclosures;
- outgoing London response/despatch.

Never use consultation date as automatic London Political Letter date.

---

## 11. EAP880 remains parallel regional surrogate

`EAP880/1/2/55/55`
contains digitised Darjeeling/Sikkim Political consultations, 1833–24 May 1843, 141 images.

Status:

`DIGITISED_SURROGATE_EXISTS = DIRECT`;

`NO147_OR_NO70_PRESENT = UNPROVEN`.

Use if image access becomes available.

---

## 12. Programme continuity remains bounded

Controlled paper sequence:

- 1831/32 Hodgson specimens / office-record materiality;
- 1837 Campbell substitution/procurement;
- 1837/38 differentiated experimental samples;
- 1841 Darjeeling manufacture + O'Shaughnessy bleaching report;
- 1842 pulp logistics + factory economics + Campbell/Bushby consultation.

Supports:

`RECURRING_GOVERNMENT_PAPER_PROBLEM_SPACE_WITH_DOCUMENTED_CONTINUITIES_AND_GAPS`.

Still not:

`ONE_UNINTERRUPTED_FORMAL_PROGRAMME_1831_1842`.

---

## Immediate research order

1. Retrieve `IOR/P/196/12`, 11 May 1842, No.70 and adjacent numbers.
2. Search all published/catalographic traces of `IOR/P/196/12` to establish its exact date span and consultation-number range.
3. Identify exact IOR/P volume for 29 Nov 1841 using same-date or immediately adjacent Political Consultation citations; do not interpolate.
4. Retrieve 29 Nov 1841 No.147 plus adjacent items.
5. Retrieve 13 Jan 1832 Nos.18–20 as a complete cluster.
6. Search 1937 exhibition planning and IRD correspondence for exhibit selection/object descriptions.
7. Search IHRC/IRD publications, 1938–44, for further Nepal/Darjeeling paper records and especially 11 May 1842 No.70.
8. Continue Halliday / Woodcock / Champaran logistics independently.
9. Continue Chamber of Commerce 1837 sample-receipt search.
10. Add exhibition state and 1937 survival checkpoint to structured provenance data.

---

## Guardrails

1. `Political O.C. = Political Original Consultation`.
2. 1832 paper object = `Nos.18–20`, not No.19 alone.
3. No.147 = directly attested O'Shaughnessy Darjeeling-paper bleaching report in 1937 IRD exhibition.
4. `IOR/P/196/12` = high-confidence volume for 11 May 1842 consultation; No.70 itself remains unrecovered.
5. Exact 1841 IOR/P volume remains open.
6. Never interpolate exact shelfmarks.
7. Inspect adjacent consultation numbers.
8. Separate consultation date from underlying-letter date and London-transmission date.
9. Treat 1937 exhibition -> 1944 article as provenance continuity, not demonstrated textual derivation.
10. Abdul Ali's archival expertise strengthens address/provenance confidence, not the primary status of his paraphrases.
11. Keep Political / Foreign / Secret branches distinct.
12. Keep pulp, finished paper, classified samples and archival supports materially distinct.
13. Keep 1837 finished-paper freight separate from 1842 pulp freight.
14. Keep proposed Chamber forwarding separate from confirmed receipt.
15. Keep Serampore publication, industrial testing and shipment destination distinct.
16. Keep spring-1842 density separate from causality.

## Current strongest proposition

**The Nepal-paper archive now has a recoverable institutional afterlife as well as a nineteenth-century administrative history. The 1832 paper-manufacture consultation was not a single No.19 item but a Nos.18–20 cluster; in December 1937 the Imperial Record Department publicly exhibited that cluster alongside O'Shaughnessy's 29 November 1841 No.147 report on bleaching paper manufactured at Darjeeling. A. F. M. Abdul Ali, then Keeper of the Records of the Government of India and ex-officio Secretary of the Indian Historical Records Commission, signed the complete exhibition list, and seven years later published `The Daphne Paper of Nepal` using the same consultation families. This creates a direct archival-curatorial provenance chain without yet proving a textual genealogy from exhibition notes to article. Meanwhile the London search has moved one level closer to the consultation itself: 11 May 1842 Political consultation material is independently tied to `IOR/P/196/12`, making that volume the first exact London target for Campbell's No.70. The decisive next task is item-level packet recovery, not further abbreviation decoding.**