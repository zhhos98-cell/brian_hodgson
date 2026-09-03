# Hodgson paper-history mainline — 2026-09-03, through Wave 76

Status: current active guardrail. Supersedes `PAPER_HISTORY_MAINLINE_STATUS_2026-09-02_WAVE75.md` for ongoing paper-history work. Wave 76 adds a **documentary-routing layer** to the 1842 pulp shipment. It does not recover the actual Woodcock freight bill or Halliday directive; it reconstructs the administrative branches and record forms through which those missing nodes should now be pursued.

## Current paper object

The paper history now follows:

`fibre/raw material`
-> `manufacturing process`
-> `pulp / sheet commodity state`
-> `count metrology`
-> `procurement/acquisition`
-> `package formation`
-> `transport metrology + route infrastructure`
-> `custody handoff + freight accounting`
-> `document generation / registration / forwarding`
-> `stock/storage time`
-> `cutting/folding/trimming`
-> `working-format allocation`
-> `writing/drawing/copying`
-> `support substitution`
-> `binding/bundling/container`
-> `shipment/custody`
-> `archive/catalogue state`.

Paper/material circulation now carries at least eleven distinguishable histories:

1. process;
2. material/commodity state;
3. count metrology;
4. acquisition;
5. package state;
6. route metrology;
7. physical transport/custody;
8. freight/accounting;
9. documentary routing;
10. stock/format/work allocation and copying/containerization;
11. later archive/catalogue state.

Core equation:

`paper object = manufacture × material state × count metrology × acquisition × packaging × route metrology × physical route/custody × cost/accounting × documentary state × stock/work allocation × later custody`.

Current propositions:

**material circulation is multi-metrological**

and

**material circulation is also multi-documentary**.

A shipment can be counted as packages, placed into a route standardized by time/capacity/price, and simultaneously generate instructions, incoming registrations, forwarding decisions, bills, receipts and higher-level proceeding copies.

---

## 1. Secure 1842 material event retained

Direct Hodgson letter, 25 March 1842:

- sender: Nepal Residency;
- Government direction through `Mr. Secretary Halliday`;
- `twenty-four packages of Nepalese paper pulp`;
- destination Calcutta;
- first-stage carrier `my people`;
- intermediate forwarding official printed as `G. Woodcock Esq., Joint Magistrate, Champaun`;
- Woodcock instructed to choose the convenient route and send Hodgson his `bill of charges`;
- land option via Motihari/Patna;
- water option from `Govind Gang` to Calcutta by `a small safe boat` under a Burkundaz.

Secure archival citation:

`Register of Letters Received from January 1842 to June 1842`, pp.344–45, Bihar State Archives, Patna.

Unknown remains:

- package weight/dimensions/construction;
- actual route;
- actual freight cost;
- actual transport time;
- Woodcock bill;
- final receiver;
- Calcutta receipt;
- direct relation to Serampore.

Rule:

`DIRECT_LETTER_ESTABLISHES_BRANCHING_ROUTE_INSTRUCTION`

but

`DIRECT_LETTER_DOES_NOT_ESTABLISH_BRANCH_SELECTED`.

---

## 2. Woodcock identity retained without silent transcript repair

Edward E. Woodcock remains the probable forwarding official at high-to-very-high confidence from the administrative record, including his appointment as joint magistrate and deputy collector of Chumparun on 8 February 1842.

Keep:

`RECIPIENT_NORMALIZED = EDWARD_E_WOODCOCK_PROBABLE_HIGH_TO_VERY_HIGH`

while preserving:

`RECIPIENT_TRANSCRIPT_EXACT = G. Woodcock`.

The original BSA image remains an active control target.

---

## 3. Physical and route-metrology layers retained

### Physical infrastructure — Rankine 1838

- difficult and seasonally nearly impassable roads;
- bridge deficiencies;
- human carriage as costly fallback;
- small-boat navigation with channel/season constraints;
- `Govind Gunge` embedded in the same regional route problem.

### Administrative transport metrology — Company 1825

- `Govindgunge` as an up-river destination;
- Company allowed trip period `2 months 0 days`;
- baggage-boat carrying-capacity classes 200–1000 maunds;
- monthly hire rates by capacity.

Guardrails retained:

`STANDARD_TIME != ACTUAL_1842_TRANSIT_TIME`

`BOAT_CAPACITY_CLASS != ACTUAL_BOAT`

`24 PACKAGES != MASS`.

Combined:

`physical feasibility × administrative route calculation × package state`.

---

## 4. Wave 76: Halliday's office profile splits the upstream archive search

The contemporary *East-India Register and Directory for 1842* identifies Frederick James Halliday simultaneously as:

- secretary to the Government of Bengal, Judicial and Revenue Department;
- junior secretary to the Government of India, Revenue, Judicial and Legislative Departments.

This strengthens the personal identification:

`MR_SECRETARY_HALLIDAY = FREDERICK_JAMES_HALLIDAY VERY_HIGH/SECURE`.

But it prevents a one-branch archival inference:

`HALLIDAY_IDENTITY_SECURE != INITIATING_DEPARTMENT_SECURE`.

The missing instruction may have generated traces in more than one governmental record architecture.

Mechanisms:

- `OFFICIAL_ROLE_MULTIPLICITY_SPLITS_ARCHIVAL_SEARCH`;
- `PERSON_IDENTITY_DOES_NOT_FIX_DEPARTMENTAL_PROVENANCE`.

Do not describe Halliday's directive as specifically Bengal Judicial, Bengal Revenue, General Department, or Government of India until the actual order or proceeding is found.

---

## 5. The 1842 pulp event now has a documentary route

Material route:

`Nepal Residency`
-> `24 pulp packages`
-> `Champaran handoff`
-> `Patna land branch OR Govind Gang water branch`
-> `Calcutta`.

Documentary route:

`Halliday directive [missing]`
-> `Hodgson action`
-> `Hodgson-to-Woodcock instruction [direct transcript / BSA incoming register]`
-> `Woodcock route decision [missing]`
-> `Woodcock bill of charges [missing]`
-> `Patna/Calcutta forwarding or receipt [missing]`
-> `[possible higher-government proceeding/copy branches]`.

The two routes are linked but not identical.

Mechanisms:

- `MATERIAL_MOVEMENT_GENERATES_DOCUMENT_MOVEMENT`;
- `DOCUMENTARY_ROUTE_PARALLELS_BUT_DOES_NOT_EQUAL_MATERIAL_ROUTE`;
- `DOCUMENTARY_STATE_IS_PART_OF_MATERIAL_HISTORY`.

Working proposition:

**the logistics of an experimental material generated a parallel logistics of documents. Administrative handoffs distributed evidence across instructions, registers, bills, proceedings and receipts.**

---

## 6. Bengal proceedings now provide a retrieval architecture, not a consignment match

British Library catalogue evidence identifies `IOR/P/13/39` as an early-1842 Bengal Proceedings container and surfaces individual matters by exact proceeding dates and numbers, including January, February, March and April 1842 examples.

The currently surfaced items are unrelated medical returns.

Therefore encode:

`IOR/P/13/39 = EARLY_1842_BENGAL_PROCEEDINGS_CANDIDATE_CONTAINER`

not:

`IOR/P/13/39 = PULP_SHIPMENT_FILE`.

Operational consequence:

keyword search alone is insufficient. The next useful move is date/number index inspection for the pre-25-March window.

Mechanism:

`PROCEEDING_DATE_AND_NUMBER_FORM_A_RETRIEVAL_ADDRESS`.

---

## 7. West Bengal State Archives General Department becomes a candidate branch

Published scholarship cites 1842 `General Department (General) Proceedings`, West Bengal State Archives, by exact date and proceeding number.

This establishes that a period-appropriate General Department proceeding series exists and can be searched structurally.

It does not establish that the Nepal paper-pulp experiment was filed there.

Current state:

`WBSA_GENERAL_DEPARTMENT_GENERAL_PROCEEDINGS = HIGH_VALUE_CANDIDATE_SERIES`

`PULP_ENTRY = UNPROVEN`.

Priority search window:

`January 1842 -> 25 March 1842`.

This is a retrieval window, not a claim about the exact date of Halliday's order.

Search vocabulary should include spelling and institutional variants:

`Hodgson / Resident Nepal / Halliday / Nepal paper / Nipal paper / paper pulp / paper manufacture / packages / Darjeeling / O'Shaughnessy / Marshman`.

---

## 8. Champaran incoming-register ecology is now better controlled

The 1842 Hodgson letter already has a secure BSA incoming-register citation.

A separate 1839 Champaran archival citation identifies:

`Register of Letters Received from February 1839 to December 1839`, `Vol. 6`, Champaran District Records, Bihar State Archives, Patna,

and demonstrates an enclosure surviving in the same documentary ecology.

This adds structural confidence that the incoming-register sequence was volume-organized and could preserve more than minimal metadata.

Do not infer:

- that the 1842 register is Vol. 6;
- that Hodgson's 1842 letter necessarily had an enclosure;
- that adjacent pages automatically preserve Woodcock's response.

Instead raise image priority:

`1842 pp.344-45 + adjacent folios + endorsements + docketing + enclosure marks`.

Mechanism:

`INCOMING_REGISTER_ANCHORS_ONE_SIDE_OF_HANDOFF`.

---

## 9. Woodcock's bill must be searched on the outgoing side

A later Bihar State Archives citation documents a Champaran record form titled:

`Register of Letters Issued (General Department) from April 1859 to January 1862`.

This is later than the 1842 event and does not prove an identically titled 1842 volume survives.

Its retrieval significance is nevertheless direct: Hodgson's known letter is an incoming Champaran item, whereas Woodcock's reply and charge account would have been outgoing acts from the district office.

Therefore:

`KNOWN_INCOMING_REGISTER != EXPECTED_LOCATION_OF_OUTGOING_REPLY`.

Search 1842 for:

- Register of Letters Issued;
- General Department outgoing correspondence;
- contingent charges/accounts;
- bill/voucher registers;
- Patna Commissioner/Magistrate correspondence.

Mechanisms:

- `HANDOFF_GENERATES_OPPOSITE_DIRECTION_RECORDS`;
- `MISSING_BILL_MUST_BE_SEARCHED_AT_BOTH_SENDER_AND_RECIPIENT_SIDES`.

---

## 10. The missing bill is no longer a single-file problem

Potential recovery paths:

### Champaran side

`Woodcock outgoing letter / bill / account / forwarding order`.

### Nepal Residency side

`incoming reply / copied bill / contingent-charge record / voucher / correspondence register`.

### Patna side

`Magistrate or Commissioner receipt / forwarding instruction / charge correspondence`.

### Calcutta side

`receipt / acknowledgement / downstream institutional delivery`.

### higher-government side

`proceeding / copy / sanction / initiating instruction`.

Thus:

`one transaction edge -> multiple documentary traces`.

Mechanism:

`TRANSACTION_REDUNDANCY_CREATES_MULTIPLE_RECOVERY_PATHS`.

This is now the governing retrieval assumption.

---

## 11. Negative result is bounded

Wave 76 public-web searching has not recovered:

- Halliday's direct initiating instruction;
- Woodcock's reply;
- the `bill of charges`;
- actual route selection;
- Patna receipt;
- Calcutta receipt.

Encode only:

`PUBLICLY_SEARCHABLE_WEB_WITNESSES_EXAMINED_2026-09-03 = NO_DIRECT_MATCH`.

Do not encode:

`DOCUMENT_LOST`

or

`ARCHIVE_DOES_NOT_SURVIVE`.

The main result of Wave 76 is an archival graph and retrieval strategy, not a substitute for the missing direct witness.

---

## 12. Other paper-history lines retained

### Manufacture/process

1831/1833 Britain, 1841 Darjeeling and 1842 Serampore remain distinct process experiments. Material identity alone does not preserve successful process properties.

### Count metrology

Company `sheet / quire / ream / chest` and Nepal `tau / dhep / kori` remain non-equivalent counting systems that make paper accountable in different institutional contexts.

### Imported drawing stock

RAS architectural programme remains a very high half-Royal working-format candidate with multiple watermark years inside a tight dimensional regime.

### Support substitution

Working sketch support can feed a different finished support.

### Local procurement and collaborator acquisition

1843 f.117 paper/binding bill, 1827 manuscript-production bills, Raj Man Singh and unnamed Chitrakar acquisition paths remain separate evidence types.

---

## Immediate research order — paper only

### A. 1842 documentary route: highest priority

1. Recover West Bengal State Archives Jan–Mar 1842 General Department (General) proceeding indexes.
2. Search Bengal Judicial/Revenue proceedings for Halliday/Hodgson/Nepal-paper terms.
3. Search Government-of-India Revenue/Judicial/Legislative proceedings because Halliday simultaneously held a junior Government-of-India secretaryship.
4. Inspect British Library early-1842 Bengal Proceedings by date/number index, treating `IOR/P/13/39` only as a candidate container.
5. Search Nepal Residency incoming/copy registers for Halliday's directive.

### B. Woodcock bill and actual route: equally high priority

6. Recover original BSA `Register of Letters Received from January 1842 to June 1842`, pp.344–45, plus adjacent folios.
7. Resolve the 1842 Champaran incoming-register volume number.
8. Identify any March–April 1842 Champaran `Register of Letters Issued`, General Department outgoing record, accounts, contingent charges or voucher series.
9. Search Edward E. Woodcock outgoing correspondence using `charges / packages / paper / Patna / Govind / Calcutta`.
10. Search Patna and Calcutta receipt/forwarding chains for `24 packages` or `Nepalese/Nipal paper pulp`.

### C. After the direct documentary route

11. Test 1830s–1840s route-metrology continuity toward 1842.
12. Continue Calcutta imported drawing-paper supplier search.
13. Continue f.117 and RAS watermark/edge image recovery.
14. Continue Serampore only for consignment-level identifiers.

---

## Guardrails

1. Paper only unless another topic exposes a material paper operation.
2. Keep standard route allowance separate from actual route duration.
3. Keep carrying-capacity categories separate from actual package mass and actual boat used.
4. Keep physical route conditions separate from administrative route standards.
5. Keep Halliday personal identification separate from departmental provenance.
6. Keep Government of Bengal and Government of India secretariat branches separate until the directive is found.
7. Keep candidate proceeding containers/series separate from proven consignment records.
8. Keep incoming-register evidence separate from an unrecovered outgoing reply.
9. Preserve exact historical place/person strings in transcription fields.
10. Keep Calcutta destination separate from Serampore test site.
11. Keep public-web non-recovery separate from archival non-survival.
12. Treat endorsements, adjacent folios, enclosures, bills, receipts and proceedings as material evidence with different documentary functions.

## Current strongest proposition

**Hodgson's experimental paper materials became research objects through more than manufacture and use. They were repeatedly translated into systems of count, package, route, price, custody and documentation. The March 1842 pulp shipment makes that especially visible: twenty-four packages left the Nepal Residency, entered a transport corridor whose routes were physically constrained and administratively metrized, and simultaneously generated an official paper trail that crossed governmental levels and district offices. The surviving Hodgson-to-Woodcock letter is therefore one node in a second circulation running alongside the pulp itself. Reconstructing the experiment requires following packages and documents together: the route chosen, the charges incurred, the instruction that initiated movement, the register that received the order, the bill that should have returned, and the receipts that may have marked subsequent custody. Material history here is inseparable from the documentary infrastructures that made movement administratively actionable and later archivally recoverable.**