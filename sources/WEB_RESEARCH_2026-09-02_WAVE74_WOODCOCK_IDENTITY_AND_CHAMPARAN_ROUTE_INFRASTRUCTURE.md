# Web/archive research 2026-09-02 — Wave 74
## The forwarding official and the road system: Edward E. Woodcock, Chumparun, and the infrastructure behind Hodgson's 1842 pulp-route choice

Date: 2026-09-02

Status: active paper-history mainline. Follow-up to Wave 73. This wave corrects/problematizes the published transcript's recipient initial and supplies directly contemporary transport-infrastructure evidence for the land/water cost comparison in Hodgson's 25 March 1842 pulp letter. It does **not** determine the actual route taken by the 24 packages.

## Executive result

Wave 73 recovered Hodgson's instruction to an intermediate Champaran official, printed by Regmi as `G. Woodcock Esq., Joint Magistrate, Champaun`, asking him to forward twenty-four packages of Nepalese paper pulp toward Calcutta and to choose between land and water carriage according to relative cost.

Two new controls sharpen that witness.

### 1. The forwarding official was very probably Edward E. Woodcock

The 1844 *Bengal and Agra Directory* civil list records:

`Edward E. Woodcock, joint magistrate and deputy collector of Chumparun, 8th February 1842.`

This appointment precedes Hodgson's 25 March 1842 letter by only about six weeks and exactly matches:

- surname;
- office: joint magistrate;
- station: Chumparun/Champaran;
- date.

The 1840 *Bengal Directory* records the same Edward E. Woodcock as joint magistrate and deputy collector at Balasore from 12 February 1839, showing a plausible preceding posting.

Therefore current source state is:

- `REGMI_TRANSCRIPT_RECIPIENT = G. Woodcock`;
- `DIRECTORY_MATCH = Edward E. Woodcock`;
- `RECIPIENT_NORMALIZATION = EDWARD_E_WOODCOCK_PROBABLE_HIGH`;
- `TRANSCRIPT_INITIAL_G = POSSIBLE_MISREADING_OR_TYPESETTING_ERROR`;
- `ORIGINAL_BIHAR_STATE_ARCHIVES_LETTER_REQUIRED_FOR_FINAL_INITIAL_CONTROL`.

Do not silently replace the transcript's `G.` in quotation or transcription fields.

### 2. Hodgson's route-cost comparison fits a directly documented seasonal transport problem

Robert Rankine's *Notes on the Medical Topography of the Districts of Sarun*, written as a report dated 22 January 1838 and printed by order of Government at Calcutta in 1839, directly describes the road and river infrastructure of Sarun/Chumparun only a few years before the pulp shipment.

Rankine states that:

- the Great and Little Gunduck rivers were navigable for small boats through the year, although the Great Gunduck could be difficult to navigate and in dry-season stretches might admit only very small boats;
- the great road toward Goruckpore was badly constrained for wheeled traffic;
- the same remarks applied to the `Govind Gunge` and Bettiah roads;
- the road to Sutter Ghat on the Gunduck, described as the high road to Chumparun, was `hardly passable` in many places for five or six months of the year;
- bridges were urgently required to make it passable for wheeled carriages during the rainy season;
- cross roads were neglected, and for roughly six months inhabitants often had to carry produce to market on the heads of coolies, with Rankine emphasizing the resulting expense.

This gives the 1842 Hodgson letter a materially specific background.

Hodgson's instruction was not simply:

`choose the cheapest route abstractly`.

It operated in a corridor where:

`road passability × season × bridge availability × wheeled carriage × human carriage × river navigation`

could materially alter freight cost and feasible route.

Core mechanisms:

- `ROUTE_COST_IS_INFRASTRUCTURE_DEPENDENT`
- `SEASONAL_ROAD_PASSABILITY_SHAPES_MATERIAL_CARRIAGE`
- `LAND_WATER_SUBSTITUTION_RESPONDS_TO_TRANSPORT_INFRASTRUCTURE`
- `PAPER_PULP_ROUTE_CHOICE_IS_A_MATERIAL_INDUSTRIAL_VARIABLE`
- `TRANSCRIPT_IDENTITY_CAN_BE_CORRECTED_BY_ADMINISTRATIVE_CONTEXT`
- `ORIGINAL_DOCUMENT_REMAINS_FINAL_CONTROL`.

---

## 1. Recipient control: Regmi's `G. Woodcock` versus the official civil list

Published Hodgson transcript:

*Regmi Research Series*, cumulative vol. XII, pp.143–144.

The letter is addressed in the transcription to:

`G. Woodcock Esq., Joint Magistrate, Champaun`.

Regmi's later 1984 archival footnote similarly describes the letter as addressed to `G. Woodcock, Joint Magistrate, Champaran`.

The archival original is cited as:

`Register of Letters Received from January 1842 to June 1842`, pp.344–45, Bihar State Archives, Patna.

Administrative directory control:

*The Bengal and Agra Directory* (1844), civil list, records:

`Edward E. Woodcock, joint magistrate and deputy collector of Chumparun, 8th February 1842.`

Digital text witness:
https://ia601402.us.archive.org/13/items/in.ernet.dli.2015.68567/2015.68567.The-Bengal-And-Agra-Directory1844_text.pdf

Earlier directory control:

*The Bengal Directory and Annual Register* (1840) records Edward E. Woodcock as joint magistrate and deputy collector at Balasore from 12 February 1839.

Digital witness:
https://upload.wikimedia.org/wikipedia/commons/6/6d/THE_BENGAL_DIRECTORY_AND_ANNUAL_REGISTER%281840%29_%28IA_dli.bengal.10689.19796%29.pdf

No competing `G. Woodcock` has yet been recovered holding the Chumparun joint-magistrate office in March 1842.

The match is therefore unusually strong, but source discipline requires preserving two fields:

`printed_transcript_name`

and

`administratively_normalized_recipient`.

Mechanisms:

- `OFFICE_DATE_PLACE_TRIANGULATION_CAN_CORRECT_TRANSCRIPT_IDENTITY`
- `ARCHIVAL_TRANSCRIPTION_ERROR_CAN_DISTORT_LOGISTICS_NETWORK`.

---

## 2. Why this identity matters to the paper route

Woodcock was not a random private carrier. The office match places the paper pulp inside district administration.

Hodgson's material chain becomes:

`Nepal Residency`
-> `Hodgson's people`
-> `Edward E. Woodcock candidate / Chumparun joint magistrate and deputy collector`
-> `district route decision + forwarding`
-> `Patna or river route`
-> `Calcutta`.

The forwarding node therefore had:

- administrative authority;
- knowledge of current roads/water carriage;
- ability to place material under another magistrate's care;
- responsibility for forwarding charges.

This makes the local magistracy part of experimental-material infrastructure.

Mechanism:

`DISTRICT_MAGISTRACY_AS_MATERIAL_FORWARDING_INFRASTRUCTURE`.

---

## 3. Rankine 1838/1839: directly contemporary road and river evidence

Primary source:

Robert Rankine, *Notes on the Medical Topography of the Districts of Sarun*, Calcutta: G. H. Huttmann, Military Orphan Press, 1839, printed by order of Government.

Digital scan:
https://upload.wikimedia.org/wikipedia/commons/c/c3/Notes_On_The_Medical_Topography_Of_The_Districts_Of_Sarun_%28IA_dli.granth.37773%29.pdf

The title page gives 1839. Rankine's prefatory letter is signed:

`R. Rankine, Civil Assistant Surgeon, Sarun, January 22, 1838.`

He says he had resided in Sarun for nearly twelve years and visited much of the interior, making this a close contemporary district description rather than a later retrospective transport history.

### River conditions

Rankine states that the Great and Little Gunduck were navigable for small boats throughout the year.

But he immediately qualifies the Great Gunduck:

- substantial breadth and strong rainy-season flow;
- shifting sands;
- navigation difficult at all times;
- in dry season, some places admit only very small boats.

Thus `water route` itself was not frictionless or season-independent.

Mechanisms:

- `WATER_CARRIAGE_HAS_SEASONAL_AND_CHANNEL_CONSTRAINTS`
- `NAVIGABLE_DOES_NOT_MEAN_UNIFORM_TRANSPORT_CAPACITY`.

---

## 4. `Govind Gunge` is explicitly inside the bad-road discussion

On printed p.8 Rankine describes a bad road toward Goruckpore, narrow for wheeled carriages and requiring bridges, then states:

`These remarks also apply to the Govind Gunge and Bettiah roads.`

Hodgson's 1842 published transcript proposes direct water carriage from `Govind Gang` to Calcutta if land carriage is expensive.

The spelling is not identical, so encode:

`HODGSON_TRANSCRIPT_GOVIND_GANG <-> RANKINE_GOVIND_GUNGE = VERY_HIGH_GEOGRAPHIC_CANDIDATE / SPELLING_NORMALIZATION_NOT_YET_FORMALLY_CONTROLLED`.

Do not silently modernize to a current place name without historical map/gazetteer control.

The important paper-history point is already secure: a locality named in Hodgson's water-route option appears in a contemporary district report precisely within a discussion of difficult roads.

Mechanism:

`ROUTE_NODE_HAS_DOCUMENTED_MODAL_PRESSURE`.

---

## 5. The high road to Chumparun was seasonally unreliable

Rankine, printed p.9, describes the road to Sutter Ghat on the Gunduck as the `high road to Chumparun`.

He says it was:

`hardly passable in many places, for five or six months in the year`.

He then says that, now a Joint Magistrate had been established in Chumparun, communication would increase and several bridges were urgently needed to make the road passable for wheeled carriages during the rainy season.

This is direct evidence for the physical transport environment associated with the same office Hodgson uses four years later as his forwarding node.

Important source-control point:

Rankine's `a Joint Magistrate has been established` refers to the existence of the office by 1838. It does **not** refer to Edward E. Woodcock personally, who was appointed there in 1842.

Mechanisms:

- `OFFICE_INFRASTRUCTURE_PRECEDES_SPECIFIC_OFFICEHOLDER`
- `SEASONAL_PASSABILITY_CAN_SHIFT_FREIGHT_MODE`.

---

## 6. Cross-road conditions explain why carriage cost could rise sharply

Rankine, printed p.10, says cross roads were largely neglected. For six months of the year, he reports, inhabitants in many places were obliged to carry agricultural produce to neighboring markets on the heads of coolies.

He gives twenty seers as the maximum a man could carry for distance and explicitly emphasizes the expense produced by these transport constraints.

This should **not** be used to assert that Hodgson's paper pulp was carried by coolies or that the 24 packages weighed twenty seers each.

Its proper value is structural:

`poor roads -> reduced wheeled-carriage availability -> increased dependence on human carriage -> higher carriage cost`.

That is the kind of cost differential Hodgson asks Woodcock to evaluate.

Mechanisms:

- `CARRIAGE_MODE_CONSTRAINS_FREIGHT_COST`
- `HUMAN_CARRIAGE_IS_A_FALLBACK_TRANSPORT_TECHNOLOGY`.

---

## 7. Revised interpretation of Hodgson's land/water instruction

Wave 73 correctly treated route choice as an economic decision.

Wave 74 specifies what that economic decision was materially responding to.

The route-choice function is better represented as:

`expected freight cost = distance × road condition × season × bridge/ferry availability × carriage mode × package handling × custody/security`.

Hodgson himself names only relative land versus water cost and a safe boat/Burkundaz arrangement. Rankine independently documents several underlying physical constraints in the relevant district.

Therefore the historical claim should be:

**Hodgson delegated a route choice whose cost structure was embedded in a corridor where road accessibility varied strongly by season and where river carriage offered an alternative, itself subject to channel and boat constraints.**

Do not infer which route was selected.

---

## 8. Why this matters for experimental material history

The experimental material does not arrive at Calcutta with only a botanical or chemical identity.

By the time it arrives, its history can include:

- preparation as pulp;
- division into 24 packages;
- first-stage human handling;
- handoff to district official;
- possible repeated loading/unloading;
- land or water transport;
- seasonal exposure;
- package storage at administrative nodes;
- transit duration;
- freight and security decisions.

Any later change in moisture, contamination, compression, deterioration or processability could in principle belong partly to this logistics history.

Current evidence does not demonstrate such change in this 1842 batch. The point is methodological:

`transport is a material process capable of producing experimental state`.

Mechanisms:

- `LOGISTICS_CAN_BE_PART_OF_MATERIAL_PREPARATION_HISTORY`
- `EXPERIMENTAL_INPUT_HAS_PRELABORATORY_STATE_HISTORY`.

---

## Source-control rules

1. Preserve Regmi's published recipient as `G. Woodcock` in transcript fields.
2. Normalize the recipient to Edward E. Woodcock only as a high-probability administrative identification until the Bihar State Archives original is inspected.
3. Cite Edward E. Woodcock's Chumparun appointment to the 1844 directory: 8 February 1842.
4. Do not confuse Rankine's 1838 reference to establishment of a Joint Magistrate office with Woodcock's 1842 appointment.
5. Keep `Govind Gang` (Hodgson transcript) and `Govind Gunge` (Rankine) as separate exact strings; geographic identity is a very high candidate, not yet a normalized certainty.
6. Use Rankine only as infrastructure context; it does not prove the route actually followed by the pulp packages.
7. Do not infer coolie carriage of the pulp from Rankine's general district observation.
8. Do not infer package weight from Rankine's twenty-seer human-load example.
9. Preserve both land and water alternatives until Woodcock's bill/forwarding record or a receipt is recovered.
10. Keep the Serampore consignment relation unresolved.

## Immediate next actions

1. Recover the Bihar State Archives original pp.344–45 and inspect the recipient initials directly.
2. Search 1842 Chumparun/Sarun district correspondence under `Edward E. Woodcock`, especially March–April, for Hodgson paper pulp, forwarding instructions, and bill of charges.
3. Search Patna magistrate correspondence/receipts for twenty-four packages from Woodcock/Champaran.
4. Search Calcutta receipt and Government proceedings for the consignment.
5. Search Halliday's outgoing instruction to Hodgson preceding 25 March 1842.
6. Compare historical maps/gazetteers to resolve `Govind Gang/Govind Gunge` and reconstruct the proposed water route without modern-name substitution.
7. Search whether package transit occurred before or during rains; exact dispatch/receipt dates could materially change route feasibility.
8. Only after receipt evidence, revisit possible identity with the O'Shaughnessy/Marshman Serampore test batch.

## Bottom line

The 1842 pulp shipment can now be placed inside a more exact administrative and infrastructural landscape. The official who most plausibly received Hodgson's twenty-four packages was Edward E. Woodcock, appointed joint magistrate and deputy collector of Chumparun on 8 February 1842; Regmi's printed `G. Woodcock` is therefore a strong candidate for an initial-level transcription error, though the original remains decisive. Four years earlier Robert Rankine had described the same district's high road to Chumparun as hardly passable for five or six months of the year, identified the Govind Gunge and Bettiah roads with the region's bad-road problem, and documented both small-boat river transport and severe cross-road carriage constraints. Hodgson's comparison of land cost against water carriage was consequently a decision about real transport infrastructure. Paper pulp became an experimental material not only through chemistry and manufacture, but through package formation, district administration, seasonal roads, boats, carriage labour and freight accounting before it reached Calcutta.