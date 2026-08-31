# Web research 2026-08-31 — Wave 27
## Auction custody branching and mixed paper supports

Date: 2026-08-31

Status: paper-centred custody follow-up to Wave 26.

## Executive result

Three new findings change the paper census.

1. British Library `Add Or 5338(1–17)`, a Hodgson Buddhist-iconography group dated 1820–1843, is explicitly catalogued as being on **Nepalese and European paper**. Mixed local/imported support therefore occurs directly inside a Hodgson visual corpus, not only in the later Darjeeling bird drawings.
2. British Library `Add Or 5332–5334` consists of three Hodgson-associated caitya/mandala sheets on **Nepalese country paper**, 44 × 34 cm. This gives a local-paper comparator inside the same wider visual archive.
3. The 1997 Christie's Hodgson material later followed multiple custody routes. A 2016 Christie's catalogue traces eight reptile/fish-study sheets from the 10 June 1997 sale, lot 172 (part), into Justin Coldwell's Linley Hall collection and then back to auction. Published scholarship also links 1997 Christie's groups to British Library holdings, but one old shelfmark now conflicts with the current BL catalogue.

The material biography must therefore extend beyond research use:

`production -> supply -> stock -> research operation -> later custody`.

Mechanisms:

- `MIXED_SUPPORT_WITHIN_HODGSON_BUDDHIST_VISUAL_CORPUS`
- `AUCTION_INDUCED_CUSTODY_BRANCHING`
- `POST_RESEARCH_PAPER_CUSTODY_HISTORY`
- `SHELFMARK_CATALOGUE_DRIFT`
- `PUBLIC_PROVENANCE_BREAK_NOT_OBJECT_LOSS`

---

## 1. Add Or 5338 gives direct mixed-support evidence

British Library catalogue result:

https://searcharchives.bl.uk/?f%5Brelated_subjects_ssim%5D%5B%5D=Buddhist+divinities&page=1&per_page=100&sort=hierarchy

`Add Or 5338(1–17)` is described as 17 sheets of Buddhist iconography, mainly pen-and-ink, with one gouache, on `Nepalese and European paper`, mostly about 25 × 40 cm.

Secure conclusion:

`Hodgson visual research in Nepal = locally made paper + imported paper in the same working corpus`.

This makes paper allocation testable across operations. The next question is which support was selected for which medium, size, copy-state and intended recipient.

Mechanism:

`MIXED_SUPPORT_WITHIN_HODGSON_BUDDHIST_VISUAL_CORPUS`.

---

## 2. Add Or 5332–5334 supply the Nepalese-paper comparator

British Library record:

https://searcharchives.bl.uk/catalog/032-003279156

The three sheets depict Nepalese caityas and mandalas. The catalogue records:

- ink and pencil;
- Nepalese country paper;
- 44 × 34 cm;
- likely original membership in Hodgson collections formed 1820–44;
- apparent earlier custody in the Institut Impérial de France / Académie des Inscriptions et Belles Lettres.

This proves that locally produced paper could circulate internationally while remaining identifiable as a support type.

Mechanisms:

- `LOCAL_PAPER_LONG_DISTANCE_INSTITUTIONAL_CIRCULATION`
- `SUPPORT_TYPE_CAN_SURVIVE_CUSTODY_CHANGE`.

---

## 3. Collection shelfmark must not replace sheet-level census

The BL divides `Add Or 5338` into several materially different groups:

- 1–17 Buddhist iconography;
- 18–28 sculpture/iconography;
- 29–34 architecture/shrines;
- 35–41 figure and animal studies.

The 35–41 record contains pencil, pen-and-ink, wash and watercolour on sheets of several sizes:

https://searcharchives.bl.uk/catalog/040-003279164

Therefore:

`collection shelfmark != homogeneous paper type`.

Required census unit: **sheet**.

Mechanism:

`COLLECTION_SHELFMARK_COMPRESSES_SHEET_MATERIAL_HETEROGENEITY`.

---

## 4. A private custody branch from the 1997 Christie's sale is traceable

A 2016 Christie's Linley Hall sale catalogue describes eight sheets containing ten snake studies, two eel studies and one lizard study, Darjeeling/Nepalese School, circa 1850.

Searchable catalogue:

https://electronicsandbooks.com/edt/manual/Art/Auction/Christies/2016/20160309%20CKS12451%20Linley%20Hall%2C%20Shropshire%20Property%20from%20The%20Collection%20of%20The%20Late%20Sir%20Jasper%20%26%20Lady%20More%20%5B7%5D.pdf

Its provenance states:

`Brian Houghton Hodgson`
-> `Christie's, 10 June 1997, lot 172 (part)`
-> `acquired there by Justin Coldwell, Linley Hall`
-> `Christie's 2016`.

Thus at least one branch of the 1997 material remained in named private custody for nineteen years before returning to auction.

This should be coded as custody branching, not disappearance.

Mechanisms:

- `AUCTION_INDUCED_CUSTODY_BRANCHING`
- `PUBLIC_PROVENANCE_BREAK_NOT_OBJECT_LOSS`.

Source-control: this is specifically **part of lot 172**. Do not use it to assign the Wave 26 bird-watermark corpus to Coldwell without an explicit lot mapping.

---

## 5. Published shelfmark vs current catalogue: preserve the conflict

J. P. Losty, in David Waterhouse (ed.), *The Origins of Himalayan Studies*, cites Christie's `Visions of India`, London, 10 June 1997, lots 170–172. The searchable digital text states that one group became BL `OIOC Add.Or.5338`, and that preliminary natural-history lot 171 became BL `OIOC Add.Or.5339`; it also describes the latter material as carrying Nepali inscriptions on late-1840s/1850s watermarked paper.

Digital source:

https://www.discoveringbuddha.org/wp-content/uploads/2024/10/2005-Origins-of-Himalayan-Studies-Brian-H-Hodgson-by-Waterhouse.pdf

Current British Library catalogue search, however, lists:

`Add Or 5339 — Not used.`

Current catalogue:

https://searcharchives.bl.uk/?f%5Bcollection_area_ssi%5D%5B%5D=Visual+Arts&f%5Bmaterial_type_si%5D%5B%5D=Archives+and+Manuscripts&per_page=20&search_field=all_fields

Do not silently reconcile these records.

Possible explanations to test:

- old OIOC identifier later cancelled or renumbered;
- catalogue migration/concordance problem;
- temporary accession identifier;
- printed citation error;
- material transferred to another BL/NHM sequence.

Mechanism:

`SHELFMARK_CATALOGUE_DRIFT`.

---

## 6. The Wave 26 bird corpus remains publicly unresolved in custody

The Christie's bird corpus with watermark classes `MOINIER'S PATENT 1848`, `JOYNSON 1848`, `I NEWEY DARNFORD 1847`, `BRITANNIA`, and `1840` still lacks a secure named present holder in the public sources checked in this pass.

Code:

`current_public_custody = unresolved`.

Do not code `lost` or `private collection`.

A public provenance break is a documentary condition, not evidence of physical disappearance.

---

## 7. Revised paper-object formula

Wave 26:

`research-paper affordance = production history × supply history × stock history × intended operation`.

Wave 27 adds:

`post-use custody history`.

Revised model:

`paper-object history = production history × supply history × stock history × research operation × post-use custody history`.

Present access to watermark, formation and surface evidence depends partly on later splitting, mounting, rebinding, sale, institutional accession and recataloguing.

---

## 8. Required custody-event table

Keep material description and custody history separate.

Per custody event record:

- object/corpus ID;
- event date;
- event type;
- holder/institution;
- location;
- shelfmark or auction lot number at that event;
- split/merge status;
- source;
- confidence;
- next known identifier.

This prevents:

`current shelfmark = stable historical identity`.

---

## Immediate targets

1. Ask BL Asian and African Studies / Visual Arts for the accession and renumbering history of old `OIOC Add.Or.5339`.
2. Recover acquisition records for `Add Or 5338` and map them to the 1997 Christie's sale.
3. Recover the printed 10 June 1997 catalogue pages for lots 170–173 and stop inferring lot mappings from web object IDs.
4. Trace the 2016 Linley Hall Hodgson sheets after resale.
5. Run sheet-level support census on `Add Or 5338`, identifying exactly which sheets are Nepalese versus European paper.
6. Inspect European sheets for watermark/countermark and compare them with Wave 26 marks.
7. Compare `Add Or 5332–5334` Nepalese country paper against manuscript and administrative Hodgson sheets.

## Source-control rules

- `auction lot != current shelfmark` without explicit provenance.
- `old published shelfmark != current retrievable shelfmark` when catalogues conflict.
- `public provenance break != object loss`.
- `part of lot 172 -> Linley Hall` does not imply other 1997 lots followed the same route.
- `Nepalese and European paper` is a catalogue-level support distinction, not maker or formation identification.
- support census must be sheet-level.

## Bottom line

Mixed local/imported paper use is now visible directly in a Hodgson Buddhist visual corpus, not merely inferred from Calcutta supply or Darjeeling natural-history watermarks. At the same time, later custody determines what paper evidence survives in an inspectable form: 1997 auction material branched into private and institutional routes, at least one private branch resurfaced in 2016, and an older published BL shelfmark now conflicts with the current catalogue. Paper in the Hodgson archive therefore retains a fifth history after manufacture, supply, storage and research use: **post-use custody history**.