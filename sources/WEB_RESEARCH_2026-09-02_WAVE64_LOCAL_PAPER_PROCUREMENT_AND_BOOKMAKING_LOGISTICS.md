# Web/archive research 2026-09-02 — Wave 64
## Local paper procurement inside a quantified copying, binding, packaging, and shipment economy

Date: 2026-09-02

Status: active paper-history mainline. This wave moves from sheet-format reconstruction to procurement and production accounting. It uses the Cambridge Hodgson inventory as direct catalogue evidence while preserving a strict distinction between catalogue transcription and unread original bills.

## Executive result

MSS EUR HODGSON/12 preserves a compact paper-production economy around the Nepal Residency.

The strongest nodes are:

1. **1843 f.117** — a bill made out to Dr Nathaniel Wallich for Nepali paper and book-binding material, signed by Hodgson at the Nepal Residency;
2. **1827 ff.128–130** — bills for manuscripts sent to Wallich in Calcutta, explicitly itemizing the wider costs of book-making: copying, binding, bundling, packaging, shipment, purchase of local paper and related materials, carpenters, labourers and porters;
3. **1827 f.176** — receipt for 109 bundles of Oriental manuscripts arriving at Fort William;
4. **1827 ff.179–182** — manuscript list recording leaves, verses and price paid for each manuscript;
5. **1824–25 correspondence** — copying priced by stanza and Government funds/barter supplied for manuscript acquisition.

The paper-history consequence is substantial:

**Nepali paper was not merely a support chosen after knowledge had been produced. It was a purchased input inside a Residency-managed manufacturing and logistics system that connected paper, copying labour, binding, bundling, waterproofing/covering materials, carpenters, porters and shipment to Calcutta.**

Material sequence:

`local paper manufacture/market`
-> `Residency procurement in named commercial/workshop units`
-> `copying`
-> `binding`
-> `bundling`
-> `wax-cloth/thread/twine packaging`
-> `carpenter/labour/porter work`
-> `shipment to Calcutta`
-> `receipt / institutional library custody`.

Core mechanisms:

- `LOCAL_PAPER_PROCUREMENT_IS_QUANTIFIED`
- `PAPER_PURCHASE_IS_EMBEDDED_IN_BOOKMAKING_ECONOMY`
- `PAPER_UNIT_IS_COMMERCIAL_OR_WORKSHOP_UNIT`
- `BOOKMAKING_COST_ACCOUNT_LINKS_SUPPORT_TO_LABOUR_AND_TRANSPORT`
- `PACKAGING_MATERIAL_IS_PART_OF_PAPER_OBJECT_LOGISTICS`
- `RESIDENCY_AS_ACCOUNTING_AND_PRODUCTION_NODE`
- `CATALOGUE_TRANSCRIPTION_REQUIRES_ARITHMETIC_CONTROL`.

---

## 1. 1843 f.117: direct catalogue evidence for local paper purchase

Cambridge Hodgson inventory:

https://hodgson.socanth.cam.ac.uk/chunkhtml/vol012.html

`MSS EUR HODGSON/12 item 3, f.117` is catalogued as:

`A bill made out to Dr. Wallich for Nepali paper and book-binding material`.

Material state of the bill itself:

- machine-made paper;
- fine condition;
- fair hand;
- signed by B. Hodgson;
- date/place given as `Nepal Residency`;
- date 1843.

The catalogue transcription records:

- Nepali Rupees `79.30`;
- calculated equivalent Indian Rupees `61.12`;
- `1,012 bundles (ḍhyāp)` of Nepali paper;
- parenthetical explanation: `10 sheets in one bundle`;
- rates described as `Rupees 10/- and Rupees 14/- per bundle`;
- three pieces of wax cloth;
- thread and twine;
- wax cloth Rupees `13/-`;
- thread/twine `/03 paisā`.

The inventory explicitly cross-references the 1827 Wallich manuscript bills at ff.128–130 and the manuscript list at ff.179–182.

This is the first current repo node in which **Nepali paper purchase, a local bundle unit, binding/packing material, currency conversion and Hodgson's Residency accounting are all joined in one bill**.

Mechanisms:

- `LOCAL_PAPER_AS_PURCHASED_INPUT`
- `PAPER_QUANTITY_RECORDED_IN_LOCAL_UNIT`
- `CURRENCY_CONVERSION_INSIDE_MATERIAL_ACCOUNTING`
- `PAPER_AND_BINDING_MATERIAL_PROCURED_TOGETHER`.

---

## 2. Critical source-control problem: the f.117 arithmetic does not currently reconcile

The catalogue transcription cannot safely be converted into `10,120 sheets` as a historical quantity without viewing the original bill.

If read literally:

`1,012 dhyāp × 10 sheets per dhyāp = 10,120 sheets`.

But that reading is difficult to reconcile with:

- total Nepali Rupees `79.30`;
- the catalogue's stated rates of Rupees `10/-` and `14/- per bundle`;
- added wax-cloth/thread/twine costs.

The old Cambridge image links for f.117 currently fail, so the original figures, punctuation, fraction marks, ditto marks and unit layout cannot yet be checked.

Therefore encode separately:

- `CATALOGUE_QUANTITY_TRANSCRIPTION = "1,012 bundles (dhyap)"`;
- `CATALOGUE_UNIT_GLOSS = "10 sheets in one bundle"`;
- `CATALOGUE_PRICE_TRANSCRIPTION = "Rs 10/- and Rs 14/- per bundle"`;
- `CATALOGUE_TOTAL = NRs 79.30 / IRs 61.12`;
- `ARITHMETIC_CONSISTENCY = FAILS_LITERAL_READING`;
- `ORIGINAL_IMAGE = UNREAD_CURRENT_ENDPOINT`;
- `NORMALIZED_SHEET_QUANTITY = DO_NOT_CALCULATE_AS_FACT`.

Possible explanations include a catalogue punctuation/fraction transcription problem, a misunderstood unit hierarchy, or a rate applying to a larger quantity rather than one ḍhyāp. None should be chosen without the image.

Mechanisms:

- `ACCOUNT_LAYOUT_IS_EVIDENCE`
- `CATALOGUE_TEXT_CAN_ERASE_NUMERIC_STRUCTURE`
- `ARITHMETIC_CONTROL_IS_SOURCE_CRITICISM`.

This unresolved arithmetic is not a nuisance. It identifies exactly what the physical bill must answer.

---

## 3. 1827 ff.128–130: paper purchase belongs to a complete book-making cost chain

`MSS EUR HODGSON/12 item 8, ff.128–130`:

- bills for manuscripts sent to Dr Wallich in Calcutta;
- April, June and November 1827;
- bills themselves survive on both Nepali handmade and machine-made paper.

The inventory explicitly says the costs include:

- copying;
- binding;
- bundling;
- packaging;
- sending manuscripts to Calcutta by shipment;
- purchasing local paper and related materials;
- wages of carpenters;
- regular labourers;
- porters;
- prices of local materials.

The inventory interprets these as Residency-prepared bills for reimbursement of costs incurred on behalf of Wallich and others.

This produces a much stronger paper-history object than a generic statement that Hodgson bought paper.

The Residency was operating as:

`commissioning/accounting office`
+
`paper/material purchaser`
+
`copy-production coordinator`
+
`binding/packaging coordinator`
+
`transport dispatcher`.

Mechanisms:

- `RESIDENCY_AS_BOOKMAKING_WORKSHOP_COORDINATOR`
- `PAPER_COST_IS_COACCOUNTED_WITH_LABOUR`
- `SUPPORT_PRODUCTION_AND_TRANSPORT_ARE_ONE_COST_SYSTEM`
- `LOCAL_MATERIAL_PURCHASE_FEEDS_TRANSREGIONAL_MANUSCRIPT_CIRCULATION`.

---

## 4. The bills themselves use mixed supports

The 1827 bills are catalogued as written on:

`Nepali hand-made and machine-made paper`.

Thus mixed-paper ecology exists not only in research drawings and manuscripts but inside the accounting apparatus that financed paper/manuscript production.

A bill about local paper procurement could itself be written on either local handmade or imported/machine-made support.

This prevents a simplistic functional rule such as:

`local paper = manuscript object; imported paper = administration`.

Instead:

`accounting operation -> mixed support ecology`.

Mechanisms:

- `ADMINISTRATIVE_ACCOUNTING_CAN_CROSS_SUPPORT_ORIGIN`
- `PAPER_FUNCTION_NOT_FIXED_BY_ORIGIN`.

This should be tested item-by-item once images are recovered.

---

## 5. Paper purchase is linked to copying rates and manuscript valuation

The same volume supplies the surrounding quantified manuscript economy.

### 1824 Carey letter, ff.161–162

The inventory records prices paid for manuscript copying at:

`Rs 2 per 100 stanzas`.

Thus textual labour was priced by a countable textual unit.

### 1827 ff.179–182

The manuscript list records:

- number of leaves;
- number of verses/slokas;
- price paid for each manuscript.

Thus the production/accounting system simultaneously quantified:

- paper/material input;
- textual extent;
- copying labour;
- finished manuscript price.

Potential accounting chain:

`paper bundle/unit`
+
`copying rate by textual quantity`
+
`binding/packaging labour/materials`
-> `priced manuscript object`.

Mechanism:

`PAPER_AND_TEXTUAL_LABOUR_HAVE_PARALLEL_ACCOUNTING_UNITS`.

Do not yet claim a formula linking leaves to paper cost until the bills themselves are transcribed.

---

## 6. Bundles operate at more than one material scale

The inventory uses bundle language in at least two connected contexts:

### Paper bundle

f.117: Nepali paper in `ḍhyāp` bundles, with the catalogue gloss that one bundle contains ten sheets.

### Manuscript bundle

f.176: receipt for arrival of `109 bundles` of Oriental manuscripts at Fort William in May 1827.

These are not the same material unit and must not be conflated.

But the recurrence of bundle-based accounting shows that the paper/manuscript system repeatedly converted large material populations into transportable/accountable packets.

Analytical distinction:

- `PAPER_STOCK_BUNDLE`;
- `MANUSCRIPT_TRANSPORT_BUNDLE`;
- `PACKAGE/BOX`;
- `LOOSE_LEAF`;
- `BOUND_COPY`.

Mechanisms:

- `BUNDLING_IS_A MATERIAL_SCALING_OPERATION`
- `ACCOUNTING_UNIT_CHANGES_ACROSS_PRODUCTION_STAGE`.

---

## 7. 1829 seven-box receipt shows the next logistics scale

`MSS EUR HODGSON/12 item 15, f.147` records seven boxes of Nepali and Tibetan books sent by Hodgson to Fort William College through Carey.

The inventory gives:

- seven boxes;
- 103 loose leaves;
- 13 packages;
- total 101 copies.

This is a nested material structure:

`leaf/copy`
-> `package`
-> `box`
-> `shipment`.

Placed beside the paper bills, the Residency manuscript economy now contains multiple conversion scales:

`paper sheets`
-> `copied leaves`
-> `bound/unbound manuscripts`
-> `bundles/packages`
-> `boxes`
-> `Calcutta institutional receipt`.

Mechanisms:

- `PAPER_OBJECTS_ARE_REPACKAGED_ACROSS_LOGISTICS_SCALES`
- `CONTAINERIZATION_FOLLOWS_PRODUCTION`.

---

## 8. Wax cloth, thread and twine belong inside the paper history

Wax cloth, thread and twine should not be treated as peripheral miscellaneous costs.

They materially determine how paper survives transport.

The f.117 bill connects Nepali paper directly with:

- wax cloth;
- thread;
- twine.

The 1827 bills add:

- bundling;
- packaging;
- carpenters;
- porters;
- shipment.

The research/manuscript paper therefore acquired a **protective material envelope** before leaving Nepal.

Potential sequence:

`paper/manuscript`
-> `binding or bundle`
-> `thread/twine fastening`
-> `wax-cloth protection`
-> `wooden box/crate via carpenter labour candidate`
-> `porter/transport system`
-> `shipment`.

Do not force the exact order or assign wax cloth to every manuscript until bills are read directly.

Mechanisms:

- `PACKAGING_IS_PART_OF_PAPER_SURVIVAL_TECHNOLOGY`
- `PAPER_HISTORY_EXTENDS_BEYOND_THE_SHEET`.

---

## 9. The Residency creates a two-way paper/manuscript economy with Calcutta

The paper-production system is not simply:

`Nepal -> Europe`.

The Wallich/Carey/College records show:

- money/authorization coming from Calcutta/Fort William;
- paper and copying labour purchased in Nepal;
- manuscripts made/acquired in Nepal;
- bills prepared at the Residency;
- finished material shipped back to Calcutta;
- institutional receipts and reimbursements generated there.

Thus:

`Calcutta institutional demand/funding`
-> `Nepal Residency procurement/production`
-> `Calcutta receipt/library incorporation`.

Paper sits inside a reciprocal administrative-material circuit.

Mechanisms:

- `PAPER_PROCUREMENT_IS_COMMISSION_DRIVEN`
- `TRANSREGIONAL_BOOKMAKING_CIRCUIT`
- `FUNDING_ROUTE_AND_MATERIAL_ROUTE_RUN_IN_OPPOSITE_DIRECTIONS`.

---

## 10. Relation to Wave 60–63 format work

Waves 60–63 reconstructed how imported drawing paper may have moved from commercial parent sheets into standardized working formats.

Wave 64 adds the procurement/accounting side for local Nepali paper.

The article can now compare two different paper economies without reducing them to `European vs Nepalese`:

### Imported drawing stock

`commercial named parent size`
-> `transport/stock`
-> `cut into working format`
-> `visual research`.

### Local manuscript paper

`local paper purchase in bundle/unit system`
-> `copying`
-> `binding/bundling/packaging`
-> `shipment to Calcutta`.

Both are allocation systems, but they expose different intermediate operations.

The comparison unit should be:

`paper supply chain + conversion operation + task`.

---

## 11. A second supply channel remains to be tested: Calcutta-imported commodity lists

`MSS EUR HODGSON/94 item 15, ff.89–123b`, dated 13 September 1831, is a 35-folio list of fabrics and commodities purchased at Calcutta and imported into Nepal, with prices.

Source:
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol094.html

The inventory does **not** state that paper is among the goods.

Therefore current status is:

`CALCUTTA_IMPORT_PRICE_LIST = HIGH_VALUE_PAPER_SUPPLY_SEARCH_TARGET`

not:

`PAPER_IMPORT_DIRECT`.

If paper/stationery occurs in the original list, it could directly connect the imported-paper stocks visible in Hodgson's surviving objects to an actual Residency/Nepal commodity route.

Until direct reading:

`PAPER_IN_LIST = UNRESOLVED`.

---

## Source-control rules

1. f.117 quantity and rates are catalogue transcriptions, not directly read from the original bill in this wave.
2. Do not state `10,120 sheets` as a secure purchased quantity until the arithmetic/layout problem is resolved.
3. Preserve `ḍhyāp` exactly as the catalogue's local-unit transcription; verify orthography and material meaning from the image/other Nepalese sources.
4. Do not infer that all wax cloth/thread/twine on f.117 was used for the paper listed there in one fixed packaging configuration.
5. Keep paper bundles distinct from manuscript bundles and boxes.
6. The 1827 bills' mixed Nepali/machine supports are direct catalogue support classifications, not yet item-level image observations by this run.
7. Do not claim paper occurs in the 1831 Calcutta import list until the text is directly read.
8. Treat arithmetic inconsistency as a source-control field, not something to silently normalize.

---

## Immediate next actions

1. Recover f.117 recto/verso image from a migrated Cambridge/archived media endpoint.
2. Transcribe the original account layout exactly, including currency columns, fraction marks, quantities, rates and unit placement.
3. Verify the meaning and historical spelling of `ḍhyāp` and whether `10 sheets` is correct.
4. Recover ff.128–130 images and build a line-item cost table: paper, copying, binding, packaging, carpenters, labourers, porters, shipment.
5. Recover ff.179–182 and connect manuscript leaf/verse counts to individual prices.
6. Test whether paper cost can be related to manuscript leaf counts without assuming one sheet = one leaf.
7. Read vol.94 ff.89–123b for paper/stationery terms, including `paper`, `kaghaz/kāghaz/kagaz`, ream/quire equivalents and named imported sizes.
8. Search related Residency bills and commodity lists for imported paper procurement.
9. Add `procurement_unit`, `currency`, `rate_basis`, `account_layout`, `packaging_material`, `labour_category`, `shipment_unit`, and `arithmetic_control` to the paper census.

---

## Bottom line

The Hodgson paper history now has a directly documented procurement and production economy. By the 1820s–40s the Nepal Residency was paying for local paper, copying, binding, bundling, packaging, carpenters, labourers, porters and shipment as parts of one manuscript-production system directed toward Calcutta institutions. The 1843 Wallich bill is especially important because it records Nepali paper in a named local bundle unit alongside wax cloth, thread and twine, but its catalogue-transcribed quantities and rates do not presently reconcile and must be checked against the original image. The material result is already secure without forcing the numbers: **paper was a budgeted, bundled and transported production input, embedded in labour and packaging before a manuscript ever entered an institutional library.**