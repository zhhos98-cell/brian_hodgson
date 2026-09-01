# Web research 2026-09-02 — Wave 60
## Format standardization over heterogeneous stock: parent sheets, cutting, stock time, and working units

Date: 2026-09-02

Status: paper-history mainline. This wave deliberately recentres the project on paper manufacture, stock, format conversion and allocation. Textual/version questions are retained only where they reveal operations performed on paper.

## Executive result

The paper argument needs one more material stage between `stock` and `use`.

Earlier model:

`maker/mill -> procurement -> transport -> stock -> allocation -> use`.

Wave 60 adds:

`maker/mill -> commercial parent sheet -> procurement/transport -> stock time -> cutting/folding/trimming -> working-format unit -> use -> mounting/binding/custody`.

Three independent Hodgson-associated corpora now show that the paper support used for research was often a **formatted unit made from stock**, rather than the papermaker's original production sheet.

### 1. RAS architectural drawings, c.1844

A dominant group measures approximately `30 × 48.5 cm` despite explicit watermark dates of at least 1837 and 1841.

This size matches extremely closely **half of the old English Royal book/drawing sheet**, standardized at `19 × 24 in` (`48.26 × 60.96 cm`):

`Royal parent sheet 48.26 × 60.96 cm -> half sheet 48.26 × 30.48 cm`.

A controlled sample of seventeen RAS long-format sheets averages approximately:

`30.11 × 48.63 cm`.

Difference from theoretical Royal half-sheet:

- short dimension: about `-1.2%`;
- long dimension: about `+0.8%`.

This is sufficiently close to treat:

`RAS c.30 × 48.5 format = HALF_ROYAL_DRAWING_SHEET_CANDIDATE_HIGH`.

It is not yet proof: deckle/cut edges, watermark/countermark position, chain/laid structure and whole-sheet reconstruction remain necessary.

### 2. RAS shorter architectural formats

Several sheets cluster around `27–28 × 44–45 cm`.

Old English Medium book/drawing paper is `17.5 × 22.5 in` (`44.45 × 57.15 cm`), yielding a half-sheet of approximately:

`28.58 × 44.45 cm`.

Examples such as `27 × 43.8`, `27.1 × 45.4`, and `27.8 × 44 cm` are compatible with a trimmed half-Medium hypothesis, although the fit is materially looser than the Royal-half family.

State:

`RAS c.27–28 × 44–45 format = HALF_MEDIUM_CANDIDATE`.

Do not normalize every short sheet into this family: `022.026` is `31.6 × 43.8 cm`, and preliminary sketches around `31 × 41.5 cm` require separate explanation.

### 3. Christie's zoological sheets, c.1850

The Hodgson-associated bird corpus uses two repeated small formats:

- `25.1 × 20.3 cm`;
- `30.5 × 19.7 cm`.

The smaller family is strikingly close to a quarter of old English Demy drawing paper (`15.5 × 20 in = 39.37 × 50.8 cm`):

`quarter Demy = 19.69 × 25.4 cm`.

Observed `20.3 × 25.1 cm` differs by only a few percent.

State:

`20.3 × 25.1 zoological format = QUARTER_DEMY_CANDIDATE`.

The `30.5 × 19.7 cm` format currently has no equally secure standard-parent reconstruction and must remain unresolved rather than forced into Royal/Demy nomenclature.

Core mechanisms:

- `PARENT_SHEET_TO_WORKING_UNIT_CONVERSION`
- `CUTTING_IS_PAPER_ALLOCATION`
- `FORMAT_STANDARDIZATION_OVER_HETEROGENEOUS_STOCK`
- `STOCK_IDENTITY_NOT_EQUIVALENT_TO_OBJECT_FORMAT`
- `RESEARCH_SHEET_NOT_NECESSARILY_MILL_SHEET`.

---

## 1. RAS 022: a repeated working format survives across different watermark years

Key direct catalogue witnesses:

### RAS Hodgson 022.023

*The Asoka stupa, Langankhel, Patan*:

- Raj Man Singh Chitrakar;
- c.1844;
- paper watermark dated 1837;
- paper `30.6 × 48.8 cm`;
- mount `55 × 66 cm`.

Source:
https://royalasiaticcollections.org/the-asoka-stupa-langankhel-patan/

### RAS Hodgson 022.027

*Temple of Krishna and Radha, Patan*:

- Raj Man Singh;
- c.1844;
- pencil and wash;
- paper `30 × 48.5 cm`;
- mount `55 × 66 cm`.

Source:
https://royalasiaticcollections.org/temple-of-krishna-and-radha-patan-2/

Many other RAS 022 sheets explicitly catalogued as paper watermarked `1841` fall around the same `30 × 48.5 cm` family.

Therefore:

`1837 stock -> c.30 × 48.5 working format`

and

`1841 stock -> c.30 × 48.5 working format`.

This is stronger than the earlier statement that Hodgson's objects used paper of different ages.

It shows that **different stock-time layers could be converted into the same operational format**.

Mechanism:

`FORMAT_STANDARDIZATION_CAN_MASK_STOCK_HETEROGENEITY`.

The working format does not identify the stock batch.

---

## 2. Stock time is now a series-level property, not an isolated old-sheet anomaly

Earlier work treated RAS Hodgson 022.026 as the striking old-stock case:

### RAS Hodgson 022.026

*Temple of Krishna and Radha, Patan*:

- Raj Man Singh;
- c.1844;
- paper watermark dated 1821;
- paper `31.6 × 43.8 cm`;
- mount `55 × 66 cm`.

Source:
https://royalasiaticcollections.org/temple-of-krishna-and-radha-patan/

The use-date/watermark-date gap is about twenty-three years.

Wave 60 adds 1837 and 1841 dated paper inside the same c.1844 architectural corpus.

The series therefore contains at least three stock-time layers:

- 1821 -> c.1844 use;
- 1837 -> c.1844 use;
- 1841 -> c.1844 use.

Do not treat the catalogue watermark year as an infallible manufacture date without mark/maker verification. But even at catalogue-evidence level, the series requires a model of **stock coexistence across different ages**.

Mechanisms:

- `STOCK_TIME_IS_SERIES_LEVEL_NOT_OUTLIER`
- `WORKSHOP_CAN_DRAW_SIMULTANEOUSLY_FROM_DIFFERENT_AGE_STOCKS`
- `WATERMARK_DATE_NOT_USE_DATE`.

---

## 3. Same watermark year does not mean same working format

A tempting early hypothesis was:

`1841 watermark -> long c.30 × 48.5 finished-drawing format`.

RAS Hodgson 022.014 falsifies that simple mapping.

### RAS Hodgson 022.014

*Temple of Krishna and Radhan, Patan*:

- Raj Man Singh;
- 1844;
- watermark dates paper to 1841;
- paper `27 × 43.8 cm`;
- frame `60 × 71.5 cm`.

Source:
https://royalasiaticcollections.org/?p=2359

Thus:

`1841-marked paper -> long format`

AND

`1841-marked paper -> short format`.

Possible explanations include:

1. one maker/year supplied more than one commercial parent-sheet size;
2. different makers/marks share the same catalogue date;
3. one larger sheet was cut/trimmed into different working units;
4. current dimensions reflect later trimming or mounting history.

No option can yet be chosen without physical mark morphology, formation and edges.

The methodological consequence is secure:

`watermark date != stock identity != object format`.

---

## 4. Preliminary and finished states use distinguishable formats, but not a binary rule

RAS Hodgson 022.054 is explicitly described as a preliminary sketch for 022.027:

### RAS Hodgson 022.054

*Temple of Krishna, Patan*:

- Hodgson-associated preliminary sketch;
- pen and ink;
- `31 × 41.5 cm`;
- mount `55 × 66 cm`.

Source:
https://royalasiaticcollections.org/temple-of-krishna-patan/

The corresponding finished Raj Man Singh drawing 022.027 is `30 × 48.5 cm`.

This provides an operation-level pair:

`preliminary sketch 31 × 41.5`
-> `finished wash drawing 30 × 48.5`.

The change in paper format is real at this pair.

But it must not become a collection-wide binary because some Raj Man Singh numbered drawings use shorter sheets, including 022.014.

Safe mechanism:

`WORK_STAGE_CAN_TRIGGER_FORMAT_CHANGE`.

Not yet safe:

`all preliminary = short / all finished = half Royal`.

---

## 5. The long RAS format closely matches half Royal drawing paper

British Association of Paper Historians reference table:

https://baph.org.uk/resources/reference-material/old-english-paper-sizes/

Book and Drawing Papers include:

- Demy `15.5 × 20 in`;
- Medium `17.5 × 22.5 in`;
- Royal `19 × 24 in`;
- Super Royal `19.25 × 27 in`;
- Imperial `22 × 30.25 in`.

Royal converts to approximately:

`48.26 × 60.96 cm`.

A simple half-sheet cut gives:

`48.26 × 30.48 cm`.

The RAS dominant long format is extraordinarily close.

This suggests a new reconstruction target:

`commercial Royal drawing sheet`
-> `halving operation`
-> `c.30 × 48.5 working sheet`
-> `architectural drawing`
-> `55 × 66 mount`.

The final step matters: the RAS catalogue repeatedly distinguishes paper size from mount size. The mount is a later physical layer and should not be confused with research-use support.

Mechanisms:

- `COMMERCIAL_SHEET_SIZE_CAN_CONSTRAIN_RESEARCH_FORMAT`
- `CUTTING_OPERATION_BECOMES_VISIBLE_THROUGH_DIMENSION_CLUSTERING`
- `MOUNT_SIZE_NOT_WORKING_SHEET_SIZE`.

Required physical test:

- identify cut versus deckle edges;
- locate watermark/countermark relative to sheet centre and edges;
- inspect chain-line orientation;
- test whether paired half-sheets survive;
- reconstruct original mould-sheet dimensions.

---

## 6. Watermark visibility is censored by cutting

Visible watermark counts cannot be treated as direct frequencies of paper stock.

National Gallery of Australia notes that a watermark was often, though not invariably, placed at the centre of one half of a whole sheet, with the countermark in the other half. It also stresses exceptions and copied/forged marks.

Source:
https://nga.gov.au/art-artists/conservation/paper/listings-watermark-and-countermark-library/

If a full sheet is cut into halves or quarters, resulting working pieces can contain:

- full watermark;
- full countermark;
- partial mark;
- no visible mark at all.

Therefore an unmarked cut working sheet may be a batchmate of a marked sheet.

This directly changes how the Christie's bird corpus must be read.

Christie's lists visible marks among the c.1850 bird studies:

- `MOINIER'S PATENT 1848` (5);
- `JOYNSON 1848` (2);
- `I NEWEY DARNFORD 1847` (11);
- `BRITANNIA` (17);
- `1840` (1).

Source:
https://www.christies.com/zh/lot/lot-191301

Those numbers are **visible watermark observations**, not percentages of the paper stocks used across the corpus.

Mechanisms:

- `WATERMARK_OBSERVATION_IS_CUT_POSITION_DEPENDENT`
- `VISIBLE_MARK_COUNT_UNDERCOUNTS_STOCK_FREQUENCY`
- `UNMARKED_WORKING_UNIT_CAN_SHARE_MARKED_PARENT_STOCK`
- `PARENT_SHEET_RECONSTRUCTION_REQUIRED_BEFORE_STOCK_FREQUENCY_CLAIMS`.

This is especially important because the catalogue gives repeated small formats, which themselves imply systematic cutting.

---

## 7. Christie's zoological corpus: heterogeneous stocks converted into repeated small formats

Christie's lot 191301 describes more than four hundred bird studies, presented physically in repeated small sizes:

- `25.1 × 20.3 cm`;
- `30.5 × 19.7 cm`.

The same lot records at least five watermark/date classes.

Thus:

`multiple imported stock classes -> two repeated zoological working formats`.

This parallels the RAS architecture result:

`multiple stock dates -> repeated architectural working format`.

The operation, not the paper mill, may therefore explain the dimensional uniformity.

The `25.1 × 20.3 cm` format is close to quarter Demy drawing paper:

Demy parent:

`15.5 × 20 in = 39.37 × 50.8 cm`.

Quarter:

`19.69 × 25.4 cm`.

Observed:

`20.3 × 25.1 cm`.

State:

`QUARTER_DEMY_CANDIDATE`.

Do not yet infer that all objects of this size came from Demy sheets. Physical edges and watermark position must test the parent-sheet model.

---

## 8. Loose sketch pages show why a single visible WHATMAN mark cannot quantify Whatman use

Christie's lot 191304:

https://www.christies.com/en/lot/lot-191304

The catalogue describes:

- more than eighty temple/statue/shrine/figure studies;
- pencil, pen and ink;
- 41 loose pages;
- one recorded `WHATMAN` watermark;
- maximum size `24.8 × 39.6 cm`, with smaller sheets.

The correct inference is not:

`1 of 41 pages = Whatman stock`.

Because cutting determines mark visibility, the one marked piece can be one surviving marked sector of a wider Whatman batch.

Required claim state:

`WHATMAN_DIRECTLY_PRESENT_IN_CORPUS; STOCK SHARE UNRESOLVED`.

This also sharpens the existing repo rule:

`WHATMAN_PRESENT_BUT_NOT_DEFAULT`

into a stricter methodological form:

`VISIBLE_WATERMARK_COUNT_CANNOT_ESTABLISH_DEFAULT_STOCK`.

---

## 9. British Library iconographic drawings independently show format convergence across Nepalese and European paper

British Library `Add Or 5338(1–17)` is particularly important because the catalogue directly states:

- 17 sheets;
- some from a folded exercise book;
- pen-and-ink except one gouache;
- **on Nepalese and European paper**;
- various sizes, **mostly 25 × 40 cm**.

`Add Or 5338(18–28)` continues with 11 related iconographic sheets, also various sizes and mostly `25 × 40 cm`.

Source:
https://searcharchives.bl.uk/?f%5Brelated_subjects_ssim%5D%5B%5D=Buddhist+imagery&page=1&sort=date

This is direct evidence that:

`Nepalese paper + European paper -> convergent working format within one iconographic documentary system`.

The common format therefore cannot be read as a proxy for manufacture origin.

Moreover, `some from a folded exercise book` adds another conversion mechanism:

`bound/folded commercial stationery -> extracted working leaf`.

Mechanisms:

- `FORMAT_CAN_CROSS_PAPER_ORIGIN`
- `SUPPORT_ORIGIN_NOT_OPERATIONAL_FORMAT`
- `EXERCISE_BOOK_TO_LOOSE_WORKING_LEAF_CONVERSION`
- `WORKFLOW_CAN_NORMALIZE_HETEROGENEOUS_SUPPORTS`.

---

## 10. Nepalese country paper also appears in a distinct larger operation

British Library `Add Or 5332–5334`:

- three sheets of Nepalese caityas and mandalas;
- Hodgson-associated;
- ink and pencil;
- **Nepalese country paper**;
- `44 × 34 cm`.

Source:
https://searcharchives.bl.uk/catalog/032-003279156

This gives a useful controlled contrast to the mixed `25 × 40 cm` iconographic group and the imported-stock RAS architectural half-sheet candidates.

Do not yet infer a rigid task/support allocation from these catalogues alone.

But the cross-collection comparison now justifies the question:

**were paper origin, commercial parent size and cutting format independently selected for different drawing operations?**

Candidate operational families:

1. Nepalese country paper c.`44 × 34 cm` — caitya/mandala sheets;
2. mixed Nepalese/European paper mostly c.`25 × 40 cm` — iconographic sheets;
3. c.`30 × 48.5 cm` likely half-Royal imported drawing-paper format — architectural views;
4. c.`20 × 25 cm` and c.`19.7 × 30.5 cm` small repeated units — zoological studies.

State:

`OPERATIONAL_FORMAT_DIFFERENTIATION_CANDIDATE`.

Not yet:

`subject determines paper`.

---

## 11. Revised paper ontology

The repo's previous object equation was:

`sheet identity = manufacture state + mark/countermark state + formation state + supply route + stock duration + use operation`.

Wave 60 revises it to:

`research support identity = parent-sheet manufacture + commercial size + mark/countermark topology + supply route + stock duration + cutting/folding/trimming operation + working-unit format + medium/use operation + later mount/binding state`.

This matters because `sheet` is historically ambiguous.

At least four sheet-like objects may be involved:

1. **mould/machine sheet** — unit leaving manufacture;
2. **commercial stock sheet** — unit purchased/stored;
3. **working sheet** — cut/folded/trimmed unit assigned to research;
4. **archive/display object** — mounted, rebound, guarded or otherwise remade after use.

Mechanisms:

- `SHEET_IS_A_VERSIONED_MATERIAL_UNIT`
- `WORKING_SUPPORT_IS_PRODUCED_AFTER_PAPERMAKING`
- `CUTTING_HISTORY_IS_PART_OF_PAPER_HISTORY`
- `ARCHIVAL_DIMENSIONS_CAN_DIFFER_FROM RESEARCH_USE_DIMENSIONS`.

---

## 12. Why this changes the article argument

The earlier stock-history model correctly showed that a sheet could remain in inventory for years before use.

Wave 60 shows that stock did not necessarily enter research unchanged.

The workshop or office could impose an additional standardization step:

`heterogeneous parent stock`
-> `selected commercial size or available sheet`
-> `cut/fold into task format`
-> `research operation`.

This explains how a corpus can be materially heterogeneous in manufacture date and maker while visually/documentarily homogeneous in format.

A strong formulation is:

**Hodgson's research formats were not simply inherited from the mill. They were made again inside the research system. Imported and local papers of different ages and origins could be cut, folded or selected into recurrent working units; those units, rather than the original sheets, structured how drawings, measurements and iconographic series were produced.**

This connects procurement and craft to work organization without reducing paper to national provenance.

---

## 13. Source-control rules

1. Treat RAS `c.30 × 48.5` as a high half-Royal candidate, not proven parent-sheet descent.
2. Treat RAS `c.27–28 × 44–45` as a lower-confidence half-Medium candidate.
3. Treat Christie's `20.3 × 25.1` as a quarter-Demy candidate only.
4. Never assign a parent standard solely by dimensional similarity; confirm edges, watermark topology and formation.
5. `No watermark stated` in a catalogue is not `no watermark present`.
6. Visible watermark counts cannot be converted into stock percentages without modelling cutting and mark position.
7. Keep watermark date, maker/brand, parent-sheet size, working format and use date as separate fields.
8. Keep paper size separate from mount/frame size.
9. Do not equate local/European origin with a fixed task format: Add Or 5338 directly falsifies that simplification.
10. Keep trimming during later conservation/mounting as a live alternative until edges are inspected.

---

## 14. Immediate physical/archive tests

1. RAS 022 transmitted-light census: watermark/countermark, chain-line direction, exact edge state, and mark position on long-format sheets.
2. Test whether c.`30 × 48.5` sheets preserve the topology expected of half Royal parent sheets.
3. Pair 1837 and 1841 long-format papers by watermark morphology and formation to determine whether format persisted across different makers/batches.
4. Inspect 022.014 and other short 1841 sheets to test half-Medium or trimming hypotheses.
5. Inspect 022.026 directly: verify 1821 mark, identify maker/countermark and determine why its format differs.
6. Christie's bird corpus: recover current owners/photographs and record edges/marks for the `20.3 × 25.1` and `30.5 × 19.7` families.
7. Do not use raw watermark counts until marked and unmarked pieces can be reconstructed into possible parent-sheet batches.
8. British Library Add Or 5338: identify item-level paper origin and exact dimensions; test whether Nepalese and European sheets were trimmed into the same 25 × 40 workflow.
9. British Library Add Or 5332–5334: inspect deckle edges/formation on the `44 × 34 cm` Nepalese country-paper sheets.
10. Add `parent_sheet_candidate`, `cut_state`, `edge_state`, `mark_topology`, `working_format`, and `mount_state` to the paper census schema.

---

## Bottom line

Wave 60 changes the material unit of the paper history. The relevant object is no longer simply the sheet supplied by a mill or maker. Hodgson-associated drawing corpora show repeated research formats imposed across stocks of different watermark years and even across Nepalese and European paper. The dominant RAS architectural format is extraordinarily close to half of a standard Royal drawing sheet, while one zoological format approximates quarter Demy. These dimensional correspondences remain hypotheses pending edge and watermark-topology checks, but they identify a new historical operation that the article must reconstruct: **paper was not only manufactured, procured and stored; it was cut and formatted into research.**