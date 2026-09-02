# Web/archive research 2026-09-02 — Wave 73
## Twenty-four packages of Nepalese paper pulp: route choice, freight accounting, and the transport history of an experimental material

Date: 2026-09-02

Status: active paper-history mainline. This wave adds a direct 1842 logistics witness to the manufacture/experiment story and keeps the shipment distinct from the Serampore machine trial until a direct source edge is recovered.

## Executive result

A previously unpublished letter of Brian Houghton Hodgson, later printed in the *Regmi Research Series*, gives a material logistics state missing from the current paper-history graph.

On **25 March 1842**, Hodgson wrote from the Nepal Residency to **G. Woodcock, Joint Magistrate, Champaran**, stating that, by direction of `Mr. Secretary Halliday`, he had sent from Nepal:

`twenty-four packages of Nepalese paper pulp`

`en route to Calcutta`.

The packages were to be delivered to Woodcock by `my people`; Woodcock was asked to forward them by the most convenient route and send Hodgson his `bill of charges`.

The next paragraph specifies two competing transport paths:

1. **land route**: send the packages onward to Patna, to the Magistrate's care and further disposal, with the critical cost segment being land carriage between Motihari and Patna;
2. **water route**: if land carriage appeared expensive relative to water carriage, send the packages directly from `Govind Gang` to Calcutta by a small safe boat under a Burkundaz.

The original is identified as:

`Register of Letters Received from January 1842 to June 1842`, pp.344–45, Bihar State Archives, Patna.

Mahesh C. Regmi's 1984 *The State and Economic Surplus* independently cites the same archival item and correctly dates the letter **25 March 1842**, resolving the `1942` typographical/OCR error in the *Regmi Research Series* heading.

This creates a directly evidenced material chain:

`Nepal Residency`
-> `prepared paper pulp divided into 24 packages`
-> `Hodgson's own people as first-stage carriers`
-> `Woodcock / Champaran forwarding node`
-> `route selection by relative freight cost`
-> `Motihari–Patna land route OR Govind Gang–Calcutta water route`
-> `Calcutta destination`
-> `[subsequent receiver/test state unresolved]`.

Core mechanisms:

- `PULP_AS_PACKAGED_TRANSPORT_COMMODITY`
- `RAW_MATERIAL_TRANSFER_HAS_A_LOGISTICS_HISTORY`
- `ROUTE_SELECTION_BY_RELATIVE_FREIGHT_COST`
- `ADMINISTRATIVE_FORWARDING_NODE`
- `TRANSPORT_COST_BILLED_BACK_TO_RESIDENCY`
- `MATERIAL_ROUTE_CAN_BRANCH_BEFORE_EXPERIMENT`
- `DESTINATION_CITY_DOES_NOT_IDENTIFY_TEST_SITE`.

---

## 1. Direct letter text and source control

Published transcript:

*Regmi Research Series*, cumulative volume XII, pp.143–144, `An Unpublished Letter of Brian H. Hodgson`.

Digital witnesses:

- https://pahar.in/pahar/Books%20and%20Articles/Nepal/Regmi%20Research%20Series/Regmi_12.pdf
- https://himalaya.socanth.cam.ac.uk/collections/journals/regmi/pdf/Regmi_12.pdf

The first paragraph identifies:

- sender: B. H. Hodgson, Resident;
- place: Nepal Residency;
- recipient: G. Woodcock Esq., Joint Magistrate, `Champaun` in the printed transcription;
- directive: `by direction of Mr. Secretary Halliday`;
- commodity: `twenty-four packages of Nepalese paper pulp`;
- intended direction: `en route to Calcutta`;
- first carrier: `my people`;
- Woodcock's function: forward the packages to their destination;
- accounting instruction: send Hodgson a `bill of charges`.

The published heading reads `March 25th 1942`, which is impossible in context and is independently corrected by Regmi 1984.

Mahesh C. Regmi, *The State and Economic Surplus: Production, Trade, and Resource-Mobilization in Early 19th Century Nepal* (Varanasi, 1984), footnote 45, cites:

`Hodgson's letter to G. Woodcock, Joint Magistrate, Champaran of March 25, 1842 regarding the supply of 24 packages of "Nepalese Paper Pulp" to Calcutta, in "Register of Letters Received from January 1842 to June 1842," pp.344-45, Bihar State Archives.`

Digital witness:

https://nepalindata.com/media/resources/items/0/b1984_The_State_and_Economic_Surplus--Production_Trade_and_Resourc.pdf

Correct evidence state:

- `LETTER_DATE = 1842-03-25 SECURE`;
- `RRS_HEADING_1942 = TYPOGRAPHICAL/OCR ERROR`;
- `ORIGINAL_ARCHIVE = BIHAR_STATE_ARCHIVES_REGISTER_OF_LETTERS_RECEIVED`;
- `ORIGINAL_PAGES = 344-345`;
- `ORIGINAL_IMAGE = NOT_DIRECTLY_INSPECTED_THIS_WAVE`.

Mechanism:

`LATER_ARCHIVAL_CITATION_CAN_CORRECT_TRANSCRIPT_DATE_ERROR`.

---

## 2. The paper material exists in a transport package state

Existing paper-history work already distinguishes:

`bark`
from
`prepared pulp`
from
`dried pulp brick`
from
`finished sheet`.

Wave 73 adds a further operational state:

`prepared/dried pulp`
-> `transport package`.

The letter does not tell us:

- how many pulp bricks or cakes were in each package;
- package weight;
- package dimensions;
- wrapper/container material;
- whether all 24 packages were equal;
- whether the pulp was dry or partly prepared in another state.

Therefore:

`24 packages != 24 bricks`

and

`package count != material mass`.

The correct object is:

`TWENTY_FOUR_TRANSPORT_PACKAGES_CONTAINING_NEPALese_PAPER_PULP`.

Mechanisms:

- `PACKAGE_COUNT_IS_NOT_MASS`
- `COMMODITY_STATE_REQUIRES_CONTAINER_STATE`
- `PULP_TRANSFER_IS_MEDIATED_BY_PACKAGING`.

This is important because earlier descriptions of long-distance pulp transfer can otherwise jump directly from manufacturing site to experimental site and erase the physical form in which the material travelled.

---

## 3. Hodgson's people are part of the first transport leg

The letter states that the packages `will be delivered to you by my people`.

Thus the Nepal Residency did not merely issue a bureaucratic instruction and hand the material immediately to a distant government carriage system.

The first leg was materially staffed by people attached to Hodgson/Residency.

Current chain:

`Residency material stock`
-> `Residency/Hodgson carriers`
-> `Woodcock intermediate official`
-> `downstream carriage`.

The identity and labour status of `my people` are unresolved.

Do not silently identify them as porters, sepoys, servants or manuscript carriers without another source.

Mechanisms:

- `RESIDENCY_PERSONNEL_ENTER_MATERIAL_SUPPLY_CHAIN`
- `MATERIAL_HANDOFF_IS_AN_ADMINISTRATIVE_AND_LABOUR_EVENT`.

---

## 4. Woodcock is not the final recipient; he is a forwarding node

Hodgson asks Woodcock to `forward` the packages to their destination.

Woodcock therefore occupies an intermediate position:

`carrier recipient / route selector / forwarding administrator / cost reporter`.

His locality matters because the route decision is made after the material has left Nepal but before final delivery to Calcutta.

This resembles other paper-history evidence in which administrative offices serve as:

- procurement nodes;
- receipt nodes;
- quality-control nodes;
- forwarding nodes.

Here the function is especially clear:

`INTERMEDIATE_OFFICIAL_AS_MATERIAL_LOGISTICS_BROKER`.

---

## 5. Route choice is explicitly economic and multimodal

The second paragraph is exceptionally valuable because it makes transport mode contingent on comparative freight cost.

Hodgson's preferred first plan appears to be:

`packages -> Patna -> Magistrate's care -> further disposal`.

But he instructs Woodcock to compare:

`land carriage between Motihari and Patna`

against

`water carriage`.

If land carriage is expensive, he proposes:

`Govind Gang -> Calcutta`

by

`a small safe boat`

under

`a Burkundaz`.

Thus the route was not a fixed line on a map. It was a decision problem involving:

- carriage mode;
- relative price;
- transfer points;
- custody/personnel;
- perceived safety;
- final destination.

Mechanisms:

- `ROUTE_IS_SELECTED_NOT_GIVEN`
- `FREIGHT_COST_SHAPES_MATERIAL_PATH`
- `LAND_WATER_MODAL_SUBSTITUTION`
- `TRANSPORT_SECURITY_IS_BUILT_INTO_ROUTE_CHOICE`.

The paper pulp's history before testing therefore includes an economic optimization problem.

---

## 6. The bill of charges closes the transport loop back into Residency accounting

Hodgson asks Woodcock to send him the `bill of charges`.

This connects Wave 73 directly to Wave 64, where the Residency manuscript-production bills joined:

- paper purchase;
- copying;
- binding;
- bundling;
- packing;
- carpenter/labour/porter work;
- shipment.

The 1842 pulp consignment shows the same accounting logic applied to an experimental raw-material transfer.

Material movement generates a documentary return:

`physical packages move outward`
while
`cost account returns to Residency`.

Mechanisms:

- `MATERIAL_ROUTE_GENERATES_ACCOUNTING_ROUTE`
- `TRANSPORT_IS_A_COSTED_EXPERIMENTAL_INPUT`
- `RESIDENCY_ACCOUNTING_EXTENDS_BEYOND_FINISHED_MANUSCRIPTS`.

This suggests that paper experimentation and manuscript production shared at least part of the same logistical/accounting infrastructure.

---

## 7. Halliday identifies a Government-of-Bengal administrative trigger

The letter says the shipment was made `by direction of Mr. Secretary Halliday`.

Independent contemporary/near-contemporary administrative evidence identifies **Frederick James Halliday** as Secretary to the Government of Bengal from 1 May 1838.

A British Library Board's Collection file contains a letter of 11 February 1842 addressed to:

`F J Halliday, Secretary to the Government of Bengal in the Judicial Department`.

British Library record:

https://searcharchives.bl.uk/catalog/041-002354718

The *Bengal and Agra Directory and Annual Register for 1849* likewise lists:

`Frederick James Halliday, secretary to the government of Bengal, 1st May 1838`.

Thus:

`MR_SECRETARY_HALLIDAY = FREDERICK_JAMES_HALLIDAY VERY_HIGH/SECURE_INSTITUTIONAL_MATCH`.

Do not yet infer which Government department initiated the paper-pulp experiment from Halliday's general secretaryship alone. The direct 1842 instruction that triggered Hodgson's shipment remains to be found.

Mechanisms:

- `GOVERNMENT_DIRECTION_PRECEDES_MATERIAL_SHIPMENT`
- `INITIATING_ORDER_IS_A_MISSING_DOCUMENT_NODE`.

---

## 8. Relation to the 1842 Serampore experiment: temporal alignment is not consignment identity

Existing repo evidence reconstructs an 1842 industrial test in which:

- O'Shaughnessy's bleaching work on Himalayan/Nepali paper material was passed to Marshman;
- practical larger-scale testing occurred at Serampore Paper Mills;
- mucilaginous behaviour interfered with machine-web flow and thickness control.

This creates obvious temporal/programmatic proximity to Hodgson's March 1842 shipment.

But current searches have **not** recovered a source saying that:

- the `twenty-four packages` were received by O'Shaughnessy;
- they were delivered to Marshman;
- they were the feedstock used at Serampore;
- all or part of the 24-package consignment went beyond Calcutta to Serampore.

Therefore encode:

`1842_24_PACKAGE_SHIPMENT <-> SERAMPORE_1842_TRIAL = POSSIBLE_SAME_BROADER_PROGRAM / DIRECT_CONSIGNMENT_EDGE_UNPROVEN`.

Do not write:

`Nepal -> 24 packages -> Serampore`

as a secure chain yet.

The secure chain stops at:

`Calcutta destination`.

Mechanisms:

- `DESTINATION_CITY_NOT_TEST_SITE`
- `TEMPORAL_ALIGNMENT_NOT_CONSIGNMENT_IDENTITY`
- `EXPERIMENTAL_PROGRAM_CAN_CONTAIN_MULTIPLE_MATERIAL_BATCHES`.

---

## 9. Relation to the 1831/1833 Britain shipment

The 1833 JASB report says dried Nepali paper pulp, made into bricks, had been sent to Britain by George Swinton in 1831 and worked up by British manufacturers including Charles Cowan.

The 1842 letter therefore documents a **second directly countable pulp-transfer episode**, separated by about a decade and aimed first at Calcutta rather than Britain.

Current distinction:

### 1831/1833 branch

`prepared pulp bricks`
-> `long-distance India–Britain transfer`
-> `British papermaker trial`
-> `poor remanufactured sheets`.

### March 1842 branch

`Nepalese paper pulp`
-> `24 transport packages`
-> `Nepal–Champaran forwarding chain`
-> `land/water route choice`
-> `Calcutta`
-> `[next material state unresolved]`.

The repeated experiment is therefore not only repeated manufacture/testing. It is repeated **material export in different logistics architectures**.

Mechanisms:

- `REPEATED_PULP_TRANSFER_PROGRAM`
- `SAME_MATERIAL_CLASS_DIFFERENT_LOGISTICS_ARCHITECTURE`
- `TRANSFER_HISTORY_IS_PART_OF_EXPERIMENTAL_HISTORY`.

---

## 10. Paper-history significance

Wave 23–24's main argument was that raw material identity does not preserve successful paper properties when process history is lost.

Wave 73 adds a prior layer:

before a pulp sample reaches a laboratory or mill, it already has a **transport history**.

That history includes:

- preparation into transportable commodity form;
- division into packages;
- first-stage carriers;
- administrative handoff;
- route alternatives;
- land/water interfaces;
- security personnel;
- freight costs;
- final forwarding and receipt.

Thus the experimental object should be represented as:

`material state × package state × route state × custody state × storage/transit duration × later process state`.

This matters because deterioration during transport/storage was already a live explanation for the poor British results of the 1831 material.

The route is therefore not external context around the material. It can become one of the variables that produces the material delivered to the next experiment.

Mechanisms:

- `TRANSPORT_HISTORY_CAN_MODIFY_EXPERIMENTAL_MATERIAL`
- `LOGISTICS_IS_PART_OF_MATERIAL_PROCESS_HISTORY`
- `EXPERIMENT_BEGINS_BEFORE_THE_TEST_SITE`.

---

## Source-control rules

1. Date the letter 25 March 1842; treat `1942` in the RRS heading as a typo/OCR error corrected by Regmi's archival citation and context.
2. Preserve exact source as Bihar State Archives, `Register of Letters Received from January 1842 to June 1842`, pp.344–45.
3. Keep `twenty-four packages` as package count only; do not infer weight, brick count, volume or equal package size.
4. Keep `Nepalese paper pulp` as Hodgson's material label; do not silently normalize to a specific botanical species or preparation state.
5. Do not identify `my people` more specifically without another witness.
6. Treat Woodcock as an intermediate forwarding official, not final recipient.
7. Preserve both route alternatives; do not infer which was actually used.
8. Keep the final Calcutta receiver unresolved.
9. Keep the 24-package shipment distinct from the Serampore trial until a direct receipt, forwarding order, matching package number or other consignment-level evidence is recovered.
10. Identify Secretary Halliday as Frederick James Halliday at very high confidence, but do not infer the initiating Government department/order without the missing directive.
11. Keep the 1831 Britain pulp-brick shipment and 1842 Calcutta shipment as separate material batches.

## Immediate next actions

1. Search Government of Bengal proceedings/correspondence for Halliday's order preceding 25 March 1842; keywords `Nepal paper`, `paper pulp`, `Hodgson`, `Woodcock`, `Halliday`, `Marshman`, `O'Shaughnessy`.
2. Search Calcutta receipt records after late March 1842 for `24 packages` or `Nepalese/Nipal paper pulp`.
3. Re-read the Agricultural and Horticultural Society 1841–42 paper correspondence for any matching consignment count, freight reference or Woodcock/Halliday routing detail.
4. Search Marshman/Serampore material for package count or explicit receipt from Hodgson.
5. Identify G. Woodcock and his 1842 Champaran posting; locate district/joint-magistrate letter registers if extant.
6. Reconstruct likely Motihari–Patna and Govind Gang–Calcutta transport corridors only after historical route evidence is recovered; do not substitute modern geography silently.
7. Search for Woodcock's `bill of charges`, which would determine the actual route and transport cost.
8. Add `package_count`, `package_type`, `carrier`, `forwarding_official`, `route_alternatives`, `actual_route`, `freight_cost`, `destination`, `receipt_state`, and `test_relation` to the paper-shipment data model.

## Bottom line

On 25 March 1842 Hodgson sent twenty-four packages of Nepalese paper pulp from the Nepal Residency toward Calcutta under a Government-of-Bengal direction. The surviving letter does more than record a consignment. It exposes the pulp as a packaged commodity moving through Hodgson's own carriers, an intermediate Champaran official, a choice between land and river transport, and a freight-accounting loop back to the Residency. The final route and downstream receiver remain unknown, and no direct source yet identifies these 24 packages as the batch later tested at Serampore. That uncertainty should be preserved. The key paper-history result is already secure: before Himalayan pulp became an experimental input at a mill or laboratory, its material state had already been shaped by packaging, custody, route selection, transport mode and costed circulation.