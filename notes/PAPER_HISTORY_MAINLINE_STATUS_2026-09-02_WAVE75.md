# Hodgson paper-history mainline — 2026-09-02, through Wave 75

Status: current active guardrail. Supersedes `PAPER_HISTORY_MAINLINE_STATUS_2026-09-02_WAVE74.md` for ongoing work. Wave 75 adds **transport metrology** to the paper-history model: a pulp consignment entered not only roads and rivers but an already standardized Company system of allowed travel time, carrying capacity and monthly boat-hire rates.

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
-> `stock/storage time`
-> `cutting/folding/trimming`
-> `working-format allocation`
-> `writing/drawing/copying`
-> `support substitution`
-> `binding/bundling/container`
-> `shipment/custody`
-> `archive/catalogue state`.

Paper now carries at least ten distinguishable histories:

1. process;
2. material/commodity state;
3. count metrology;
4. acquisition;
5. package state;
6. route metrology;
7. physical transport/custody;
8. stock/format/work allocation;
9. copying/containerization;
10. later archive/catalogue state.

Core equation:

`paper object = manufacture × material state × count metrology × acquisition × packaging × route metrology × physical route/custody × stock time × format/work allocation × later custody`.

New proposition:

**material circulation is multi-metrological.**

The object can be counted in packages while the route is separately standardized in time, capacity and price.

---

## 1. Manufacture/process line retained

### 1831/1833 Britain

Dried/prepared Himalayan/Nepal paper pulp sent to Britain did not reproduce the successful properties of finished Nepal-made sheets when remanufactured by British paper manufacturers.

Mechanisms:

- `PROCESS_HISTORY_EMBODIED_IN_SHEET`;
- `MATERIAL_IDENTITY_DOES_NOT_PRESERVE_PROCESS_PROPERTIES`.

### 1841 Darjeeling

Moving skilled papermakers reconstructed embodied process knowledge that material movement alone had not preserved.

### 1842 Serampore

Machine-interface testing made long-fibre/mucilaginous behavior an affordance reversal.

Keep this experiment distinct from the new 24-package shipment until consignment identity is proven.

---

## 2. 1842 twenty-four-package shipment retained

Direct Hodgson letter, 25 March 1842:

- sender: Nepal Residency;
- Government direction through `Mr. Secretary Halliday`, very high-confidence Frederick James Halliday;
- `twenty-four packages of Nepalese paper pulp`;
- destination Calcutta;
- first-stage carrier `my people`;
- intermediate forwarding official at Chumparun;
- bill of charges requested.

Unknown:

- package weight/dimensions/construction;
- number of pulp bricks per package;
- final receiver;
- actual route;
- freight cost;
- arrival date;
- relation to Serampore.

Rule:

`package count != mass`.

---

## 3. Edward E. Woodcock remains the probable forwarding official

Regmi transcript:

`G. Woodcock Esq., Joint Magistrate, Champaun`.

1844 official directory:

`Edward E. Woodcock, joint magistrate and deputy collector of Chumparun, 8 February 1842`.

Current state:

`RECIPIENT = EDWARD_E_WOODCOCK_PROBABLE_HIGH_TO_VERY_HIGH`

while

`TRANSCRIPT_INITIAL = G / ORIGINAL_UNREAD`.

Do not silently normalize quotation text.

---

## 4. Rankine supplies the physical transport layer

Rankine's report dated 22 January 1838, printed 1839, establishes:

- small-boat river navigation existed but was constrained by channels/season;
- Govind Gunge and Bettiah roads belonged to the bad-road problem;
- high road to Chumparun could be hardly passable in many places for five or six months;
- bridge deficiencies limited wheeled traffic;
- poor cross-roads could make human carriage a costly fallback.

This explains the material stakes of Hodgson's land/water comparison but does not determine the actual route.

Mechanisms:

- `ROUTE_COST_IS_INFRASTRUCTURE_DEPENDENT`;
- `SEASONAL_PASSABILITY_SHAPES_CARRIAGE`;
- `LAND_WATER_MODAL_SUBSTITUTION`.

---

## 5. Wave 75: Govindgunge was already in Company river-transport metrology by 1825

*The New Annual Bengal Directory and General Register* (1825), `RATES OF BOAT HIRE`, states:

`Time allowed for Boats to proceed to any of the undermentioned Places, as per Company's Allowance.`

Under `UP THE RIVER`, `Govindgunge` is listed with an allowed period of:

`2 months 0 days`.

Nearby comparison points include:

- Patna group — 1 month 28 days;
- Goruckpore — 2 months 8 days;
- Bettiah — 2 months 15 days.

Thus Govindgunge was already an administratively recognized river destination before Hodgson's 1842 instruction.

Exact place strings:

- 1825 `Govindgunge`;
- 1838 `Govind Gunge`;
- 1842 `Govind Gang`.

Current identity state:

`SAME_HISTORICAL_TRANSPORT_NODE = VERY_HIGH`.

Preserve source spellings.

Mechanisms:

- `ROUTE_NODE_PREEXISTS_EXPERIMENT`;
- `TRANSPORT_ROUTE_IS_ADMINISTRATIVELY_METRIZED`;
- `TIME_ALLOWANCE_IS_LOGISTICS_STANDARDIZATION`.

---

## 6. Standard time is not actual travel time

The 1825 table supplies `Company's Allowance`, not observed voyage duration.

Therefore:

`Govindgunge two months`

cannot be used as the actual duration of the 1842 shipment.

The value is institutional:

space and route difficulty were converted into a payable/allowable time unit.

Mechanism:

`ADMINISTRATIVE_METROLOGY_CONVERTS_ROUTE_INTO_PAYABLE_UNIT`.

Continuity of the exact 1825 allowance into 1842 remains unproven. Searchable 1844 directory text has not yet reproduced the same table.

---

## 7. Boat carrying capacity and monthly rate form a second route metric

The 1825 directory follows the destination/time table with `BAGGAGE BOATS, &c.`.

Recovered carrying-capacity classes range from:

`200 -> 1000 maunds`.

Example monthly rates:

- 200 maunds — Rs 22;
- 500 maunds — Rs 49;
- 1000 maunds — Rs 94.

Before detailed quantitative publication, visually control the table because OCR punctuation can be noisy.

Do not infer the capacity class used for the 24 packages; package mass remains unknown.

Transport metrology now contains:

`destination`
× `allowed travel time`
× `boat capacity`
× `monthly rate`.

Mechanisms:

- `BOAT_CAPACITY_IS_LOGISTICS_METROLOGY`;
- `FREIGHT_COST_CAN_BE_CALCULATED_FROM_CAPACITY_AND_TIME`;
- `MATERIAL_PACKAGES_ENTER_A_PRICED_CARRIAGE_SYSTEM`.

---

## 8. Physical and administrative infrastructures are different layers

### Physical layer — Rankine 1838

roads, bridges, rivers, channels, seasons, carriage modes.

### Administrative layer — Company 1825

destination classes, allowed time, boat capacity, monthly price.

Combined:

`physical feasibility × administrative calculation = transport regime`.

Hodgson's 1842 route instruction enters this regime.

Do not infer that Hodgson consulted the 1825 directory itself.

Correct relation:

`PREEXISTING_COMPANY_TRANSPORT_KNOWLEDGE_INFRASTRUCTURE`.

---

## 9. Paper metrology and route metrology can now be compared without conflation

### Paper-count systems

- Company `sheet / quire / ream / chest`;
- Nepal `tau / dhep / kori`;
- regional `dasta` variants.

These turn material sheets into countable/accountable stocks or packages.

### Route system

- destination;
- allowed time;
- carrying capacity;
- monthly rate.

This turns spatial movement into calculable freight.

The similarity is operational, not numerical.

Working proposition:

**a material shipment was made calculable more than once: first as a number of physical packages, then as a journey assigned to standardized time/capacity/cost relations.**

Mechanisms:

- `MATERIAL_CIRCULATION_IS_MULTI_METROLOGICAL`;
- `PAPER_QUANTITY_AND_TRANSPORT_QUANTITY_INTERLOCK_WITHOUT_EQUIVALENCE`.

---

## 10. The missing Woodcock freight bill becomes even more important

Wave 75 clarifies what the missing `bill of charges` could potentially bridge:

`standard transport regime`
-> `actual twenty-four-package event`.

Possible but unproven bill fields:

- actual route;
- actual hire period;
- water or land mode;
- boat capacity/rate;
- porter/cart/ferry costs;
- security/custody;
- transshipment.

Mechanism:

`FREIGHT_BILL_IS_DOCUMENTARY_INTERFACE_BETWEEN_ROUTE_STANDARD_AND_MATERIAL_EVENT`.

Do not invent the bill format.

---

## 11. Calcutta trade infrastructure: current bounded result

The 1844 *Bengal and Agra Directory* contains a Calcutta trade list explicitly including:

`Publishers, Booksellers, Stationers, Music Sellers`.

Recoverable named firms include:

- Lattey Brothers and Co., Government Place Library;
- Ostell and Lepage, British Library, Tank Square;
- W. Thacker and Co., St Andrew's Library, Government Place;
- P. S. D'Rozario and Co.;
- W. Rushton;
- Samuel Smith and Co.;
- book binders and separate boat agents.

This establishes a commercial environment for books/stationery and logistics.

It does **not** yet prove any named firm supplied Hodgson's imported drawing paper or sold Whatman/Royal drawing paper in 1844.

Current searches for `Whatman` and `drawing paper` in the directory text returned no direct product statement.

Rule:

`NAMED_STATIONER/BOOKSELLER != HODGSON_PAPER_SUPPLIER_WITHOUT_PRODUCT_OR_ACCOUNT_EDGE`.

This remains an active supply-side retrieval target.

---

## 12. Other paper-history lines retained

### Imported drawing stock

RAS architectural programme remains a very high half-Royal working-format candidate with multiple watermark years inside one tight dimensional regime.

### Support substitution

Working sketch support can feed a different finished support.

### Local procurement

1843 f.117 paper/binding bill and 1827 manuscript-production bills retain paper purchase, labor and package logistics.

### Collaborator acquisition

Paper acquired through Raj Man Singh and from an unnamed Chitrakar remains separate from billed purchase.

### Count metrology

- `tau` sheet count independent of size;
- `dhep` paper bundle with context-variable depth;
- `kori` general twenty/score collective applied to paper.

---

## Immediate research order — paper only

### Actual 1842 pulp movement

1. Recover Woodcock's bill of charges.
2. Recover Halliday's initiating instruction.
3. Search Patna and Calcutta receipt/forwarding records.
4. Search Marshman/O'Shaughnessy records only for consignment-level identifiers.

### Route-metrology continuity

5. Search 1830s–1840s Government rules/directories for Govindgunge boat-time/rate continuity.
6. Keep absence from searchable 1844 directory bounded; it may reflect changed directory structure or OCR.

### Imported paper supply

7. Search Calcutta Gazette, trade advertisements and stationer catalogues 1837–45 for `Whatman`, `drawing paper`, `Royal`, `Medium`, `Demy`, `ream`, `quire`, `artists' materials`.
8. Treat Ostell & Lepage, Lattey, Thacker and other firms as candidates only when product-level evidence appears.
9. Search Hodgson/Wallich accounts and correspondence for stationer names/indents.

### Objects

10. Continue f.117 image recovery.
11. Continue RAS watermark/countermark/edge reconstruction.

---

## Guardrails

1. Paper only unless another topic exposes a material paper operation.
2. Keep standard route allowance separate from actual route duration.
3. Keep carrying-capacity categories separate from actual package mass.
4. Keep named commercial firms separate from proven supplier relations.
5. Keep exact historical place spellings in source fields.
6. Keep physical route conditions separate from administrative route standards.
7. Keep Calcutta destination separate from Serampore test site.
8. Keep material-package count separate from paper-sheet count.
9. Treat freight bills, indents, receipts, advertisements, watermarks and dimensions as equally material but differently mediated evidence.

## Current strongest proposition

**Hodgson's paper objects were not only manufactured, bought and used; they were repeatedly translated into different systems of material accountability. Nepalese paper could be counted as sheets and bundles, imported drawing stock could be cut from commercial parent formats into standardized working units, and experimental pulp could be divided into transport packages and inserted into a river system where destinations had standard time allowances and boats were priced by carrying capacity and month. The material history therefore does not end at the mill or begin at the manuscript. It includes the metrologies, packages, route standards, transport bottlenecks and accounting documents through which paper and pulp became movable research materials.**