# Hodgson paper-history mainline — 2026-09-03, through Wave 77

Status: current active guardrail. Supersedes `PAPER_HISTORY_MAINLINE_STATUS_2026-09-03_WAVE76.md` for ongoing paper-history work. Wave 77 adds a **pre-1842 procurement/sample-circulation layer** and a new cross-wave node analysis for Govindgunge.

## Current paper object

The paper history now follows:

`fibre/raw material`
-> `manufacturing process`
-> `finished-sheet / pulp commodity state`
-> `quality/size classification`
-> `count metrology`
-> `procurement/market geography`
-> `package formation`
-> `transport metrology + route infrastructure`
-> `custody handoff + freight accounting`
-> `document generation / registration / forwarding`
-> `experimental sample circulation`
-> `commercial evaluation`
-> `learned-society publication`
-> `stock/storage time`
-> `cutting/folding/trimming`
-> `working-format allocation`
-> `writing/drawing/copying`
-> `support substitution`
-> `binding/bundling/container`
-> `shipment/custody`
-> `archive/catalogue state`.

Current propositions:

**material circulation is multi-metrological**;

**material circulation is multi-documentary**;

**the same paper object can change institutional function without losing material continuity: commodity, office support, proof-object, experimental sample, commercial sample, publication subject and transport package are different states rather than synonyms.**

---

## 1. Wave 76 documentary-routing model retained

The 25 March 1842 direct Hodgson letter still anchors the pulp event:

`Nepal Residency`
-> `24 packages Nepalese paper pulp`
-> `Champaran / Woodcock`
-> `Patna land branch OR Govind Gang water branch`
-> `Calcutta`.

Halliday's initiating directive, Woodcock's route decision/bill, Patna receipt and Calcutta receipt remain unrecovered.

Halliday's 1842 dual office profile continues to require separate Bengal and Government-of-India archival search branches.

---

## 2. Wave 77 direct primary result: a differentiated experimental sample set in 1837

*Transactions of the Agricultural and Horticultural Society of India*, vol. V (Serampore Press, 1838), directly records that on 20 November 1837 the Society requested from Campbell:

`a small supply of each size and quality of paper manufactured at Nepaul for experimental purposes`.

Campbell's 28 November reply:

- promises to transmit a quantity;
- suggests that samples of each variety be forwarded to the Chamber of Commerce;
- encloses copies of recent correspondence between T. C. Scott and himself concerning the paper.

The volume contents list:

`On Nepalese Paper, by Dr. Campbell`, p.220.

Thus a secure circulation sequence now exists:

`official correspondence`
-> `copied dossier to learned society`
-> `classified paper sample request by size/quality`
-> `experimental sample circulation`
-> `commercial sample forwarding proposed`
-> `publication as learned-society paper`.

Mechanisms:

- `SAMPLE_SET_PRESERVES_MATERIAL_VARIATION`;
- `GOVERNMENT_CORRESPONDENCE_BECOMES_LEARNED_SOCIETY_SOURCE`;
- `EXPERIMENTAL_SAMPLE_CAN_BECOME_COMMERCIAL_SAMPLE`;
- `SAMPLES_AND_DOCUMENTS_CIRCULATE_IN_PARALLEL`.

Guardrail:

`CHAMBER_OF_COMMERCE_FORWARDING = PROPOSED_DIRECT`

while

`CHAMBER_RECEIPT_OR_TEST = UNPROVEN`.

---

## 3. Campbell's 1837 government argument adds procurement as a material system

Abdul Ali's 1945 archival extraction preserves Campbell's 15 November 1837 correspondence with T. C. Scott as a secondary source pending direct image control.

The recovered argument includes:

- comparison of long-lived Nepal-paper Government records with English foolscap;
- use of archival survival as evidence of durability;
- proposal to substitute Nepal paper in Government offices;
- paper prices and market geography;
- Nepal-to-Patna carriage estimate;
- seasonal procurement and carriage planning.

This changes the object from a generic `durable indigenous paper` into an administratively evaluated stationery candidate.

Working equation:

`Government paper substitution = durability/performance × price × market access × season × transport`.

Mechanisms:

- `ARCHIVE_AS_LONGITUDINAL_MATERIAL_TEST`;
- `OLD_RECORDS_BECOME_PROOF_OBJECTS_FOR_NEW_PROCUREMENT_POLICY`;
- `GOVERNMENT_PAPER_SUBSTITUTION_IS_A_LOGISTICS_PROBLEM`;
- `PROCUREMENT_POLICY_IS_MATERIAL_HISTORY`.

Do not treat Abdul Ali as the primary Political archive. Direct image/file control remains required.

---

## 4. Govindgunge is now a triple-function node

Three evidence layers must remain distinct.

### 1825

`Govindgunge` appears in Company `Rates of Boat Hire` as an up-river destination with an administratively allowed trip period.

Role:

`COMPANY_ROUTE_METROLOGY_NODE`.

### 1837

Campbell's Nepal-paper market/procurement geography, as extracted by Abdul Ali from the Scott correspondence, includes `Govindgunge`.

Role:

`NEPAL_PAPER_MARKET_OR_SUPPLY_NODE`.

### 1842

Hodgson's direct instruction names `Govind Gang` as the possible point for forwarding the 24 pulp packages directly to Calcutta by water.

Role:

`SPECIFIC_EXPERIMENTAL_MATERIAL_FORWARDING_NODE`.

Combined proposition:

**Govindgunge repeatedly becomes relevant to paper circulation because market infrastructure and transport infrastructure overlap there, but market function, generic route metrology and one specific consignment decision remain separate evidence states.**

Mechanisms:

- `TRANSPORT_NODE_CAN_ACQUIRE_COMMODITY_SPECIFIC_FUNCTION`;
- `MARKET_AND_ROUTE_INFRASTRUCTURE_INTERLOCK_WITHOUT_BEING_IDENTICAL`.

---

## 5. 1837 finished-paper freight must remain separate from 1842 pulp freight

Abdul Ali reports Campbell estimating Nepal-to-Patna paper carriage at about Rs 1-12 per maund.

This demonstrates that Nepal-paper procurement was already represented through material-specific freight calculations before 1842.

But:

`1837 FINISHED PAPER FREIGHT != 1842 PULP PACKAGE FREIGHT`.

Do not use the 1837 rate to estimate Woodcock's missing bill.

Use it only to establish:

`MATERIAL_SPECIFIC_FREIGHT_ESTIMATE_PRECEDES_EXPERIMENTAL_PULP_ROUTE`.

---

## 6. Procurement has a seasonal time structure

Campbell's 1837 proposal, as extracted by Abdul Ali, links purchasing during the rains with later carriage toward the Ganges during the cold months.

This creates:

`purchase window`
-> `aggregation/storage`
-> `transport window`
-> `river-facing distribution`.

Mechanism:

`SEASONAL_PROCUREMENT_CALENDAR_STRUCTURES_MATERIAL_FLOW`.

Do not apply this proposed finished-paper calendar mechanically to the March 1842 pulp event.

---

## 7. Spring 1842 is now a dense paper-event window

Current chronology:

- 25 March 1842 — Hodgson 24-package pulp shipment;
- 16 April 1842 — Darjeeling paper operation reported by Abdul Ali as closed under existing economics;
- 21 April 1842 — Campbell paper-related letter to G. A. Bushby cited by Abdul Ali;
- 11 May 1842 — `Political O.C. No.70` archival pointer.

Encode:

`SPRING_1842_PAPER_EVENT_DENSITY = HIGH`

but retain:

`TEMPORAL_PROXIMITY != CONSIGNMENT_IDENTITY`

and

`TEMPORAL_PROXIMITY != CAUSAL_SEQUENCE`.

The direct relation between the 24 packages and the Darjeeling/Serampore experiment remains unresolved.

---

## 8. Political O.C. now becomes a specific retrieval problem

Abdul Ali supplies at least these useful archival addresses:

- `Political O.C., 29 Nov 1841, No.147`;
- `Political O.C., 11 May 1842, No.70`.

The exact expansion of `O.C.` and modern archive shelfmarks remain unresolved.

These should be treated as:

`DATED_NUMBERED_ARCHIVAL_POINTERS_FROM_SECONDARY_SOURCE`.

Next retrieval should identify the contemporary index/series first, then retrieve the files.

Do not silently expand `Political O.C.` or assign it to a modern IOR series without control.

---

## 9. RAS private-copy pathway adds another recovery route

RAS catalogue `GB 891 BHH/BHH/3/35` preserves a copy of a Campbell-to-G. A. Bushby letter dated 15 April 1842.

That specific letter concerns Csoma de Koros, not paper.

Its value is archival-form based:

Campbell's official correspondence with Bushby from the same week could be copied into Hodgson's private papers.

Therefore add a new retrieval branch:

`RAS HODGSON PAPERS ADJACENT CAMPBELL/BUSHBY COPIES`.

Guardrail:

`BHH/3/35 != 21 APRIL PAPER LETTER`.

Mechanism:

`PRIVATE_PAPER_COPY_CAN_PRESERVE_OFFICIAL_CORRESPONDENCE_EDGE`.

---

## 10. Serampore has multiple paper functions and must be disaggregated

Secure 1838 edge:

`Campbell paper correspondence -> Transactions publication -> Serampore Press`.

Later secure programme edge:

`O'Shaughnessy bleaching work -> Marshman -> Serampore Paper Mills industrial test`.

Still unproven:

`24-package March 1842 shipment -> Serampore`.

Therefore:

`SERAMPORE_PUBLICATION_EDGE = SECURE`

`SERAMPORE_INDUSTRIAL_TEST_EDGE = SECURE_AT_PROGRAM_LEVEL`

`SERAMPORE_24_PACKAGE_CONSIGNMENT_EDGE = UNPROVEN`.

Mechanism:

`SAME_PLACE_CAN_HOST_DIFFERENT_DOCUMENTARY_AND_MATERIAL_OPERATIONS`.

---

## 11. Programme continuity is now plausible but still bounded

The repo now contains direct or source-controlled evidence for repeated Government engagement with Nepal paper across:

- 1831/32 Hodgson description/sample transfer;
- 1837 Campbell Government substitution/procurement discussion;
- 1837/38 learned-society experimental sample circulation;
- 1841 Darjeeling manufacture/bleaching correspondence;
- 1842 pulp movement and industrial experimentation.

This supports:

`RECURRING_GOVERNMENT_PAPER_PROBLEM_SPACE_WITH_DOCUMENTED_CONTINUITIES_AND_GAPS`.

It does not yet support:

`ONE_UNINTERRUPTED_FORMAL_GOVERNMENT_PROGRAMME_1831_1842`.

A direct sequence of continuation orders, sanctions or proceedings is still needed for the stronger claim.

---

## Immediate research order

### Primary-source control

1. Recover/image-control `Transactions` vol. V p.220 and extract the Scott-Campbell paper correspondence directly.
2. Resolve exact 1837 market spellings, price figures, durability comparison and procurement calendar from the primary image.

### Political archive

3. Decode `Political O.C.` through contemporary indexes.
4. Map `29 Nov 1841 No.147` and `11 May 1842 No.70` to modern shelfmarks.
5. Retrieve the 21 Apr 1842 Campbell-to-Bushby paper letter.

### Private-copy route

6. Search adjacent RAS Hodgson material around BHH/3/35 for other Campbell/Bushby copies in April–May 1842.

### Commercial circulation

7. Search Chamber of Commerce minutes/correspondence after 28 Nov 1837 for Nepal-paper sample receipt, testing, price discussion or referral.

### Market/route continuity

8. Search Patna/Sarun/Govindgunge procurement evidence to test whether Campbell's proposed paper-market network was operationally used.
9. Continue Woodcock bill / Halliday directive search from Wave 76.

---

## Guardrails

1. Paper only unless another topic exposes a material paper operation.
2. Distinguish pulp, finished paper, sample set and archival paper objects.
3. Distinguish generic market geography from one specific shipment route.
4. Distinguish 1837 finished-paper freight from 1842 pulp-package freight.
5. Distinguish proposed Chamber forwarding from confirmed receipt.
6. Distinguish Abdul Ali's secondary archival extraction from direct primary witnesses.
7. Do not silently expand `Political O.C.`.
8. Keep spring-1842 date clustering separate from causal linkage.
9. Keep RAS BHH/3/35 separate from the paper letter it only helps us search for.
10. Keep Serampore publication, industrial experiment and consignment functions separate.
11. Treat 1831–42 as recurring programme-level continuity candidate, not a formally continuous programme until official continuation records are recovered.

## Current strongest proposition

**Nepal paper became administratively interesting not because it possessed one stable property, but because institutions repeatedly converted its material qualities into different operational questions. Old Government records made durability visible; procurement discussion translated durability into price, markets, season and freight; the Agricultural and Horticultural Society requested paper by size and quality as a differentiated experimental set; Campbell proposed further circulation as commercial samples; official correspondence itself was copied into a learned-society dossier and published at Serampore; and by 1842 pulp moved as twenty-four packages through a route chosen by relative carriage cost. The history is therefore neither a simple technology-transfer story nor a sequence of isolated paper experiments. It is a history of repeated institutional reclassification of the same broad material system: record support, procurement commodity, experimental sample, commercial specimen, raw-material package and industrial feedstock.**