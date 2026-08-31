# Paper support and manuscript geometry in Cowell & Eggeling's Hodgson catalogue, 1875

Date: 2026-08-31

Status: paper-centred quantitative source-control note. This analysis uses the full 79-entry Cowell & Eggeling catalogue as a descriptive corpus. It does not treat the catalogue as a random sample and does not infer a direct chronological palm-leaf-to-paper transition without matched witnesses.

## Executive result

The catalogue shows a clear support-format association, but not the simple result initially expected.

The strongest descriptive contrast is not in the long dimension. It is in the **short dimension and resulting aspect ratio**.

After direct entry-level support review:

- 12 manuscripts are explicitly palm leaf;
- 67 are paper under the catalogue's declared `Indian paper unless otherwise stated` baseline, including the blackened-paper family MSS 77–79;
- usable dimensions are available for all 12 palm-leaf items and 66 of the 67 paper items; MS 53 remains OCR-uncertain.

### Palm leaf

- median long dimension: 12.25 in.;
- IQR long dimension: 12.0–12.562 in.;
- median short dimension: 2.0 in.;
- IQR short dimension: 1.75–2.25 in.;
- median aspect ratio: 6.696;
- 11/12 have aspect ratio >=5;
- 10/12 have short dimension <=2.25 in.

### Paper

- median long dimension: 11.5 in.;
- IQR long dimension: 10.0–13.0 in.;
- median short dimension: 3.0 in.;
- IQR short dimension: 2.75–3.5 in.;
- median aspect ratio: 3.640;
- 8/66 dimensioned items have aspect ratio >=5;
- 6/66 have short dimension <=2.25 in.

The paper-history result is therefore best formulated as:

`overlapping long-axis scale + expanded short axis on paper -> less extreme oblong writing field`.

Mechanisms:

- `SUPPORT_FORMAT_ASSOCIATION`
- `LONG_AXIS_OVERLAP_SHORT_AXIS_EXPANSION`
- `PAPER_WRITING_FIELD_EXPANSION`
- `OBLONG_FORMAT_PERSISTENCE_WITH_PROPORTIONAL_CHANGE`

---

## 1. Correction: the catalogue contains twelve palm-leaf entries, not ten

The previous material catalogue censuses v0.1/v0.2 recorded ten explicit palm-leaf manuscripts.

Direct sequential review identifies twelve:

`1, 2, 13, 34, 37, 43, 46, 67, 68, 69, 70, 74`.

The omitted items were:

- MS 34, `Nāmasaṅgīti-ṭīkā`, 180 palm leaves;
- MS 37, `Saṃpuṭodbhava`, 127 palm leaves.

This correction matters because support-format comparison depends on complete support classification.

Mechanism:

`ENTRY_LEVEL_SUPPORT_REVIEW_SUPERSEDES_KEYWORD_CENSUS`.

---

## 2. The catalogue itself supplies a support baseline

Cowell and Eggeling state before the entries:

`The material of the MSS. consists of Indian paper, unless otherwise stated.`

Therefore support coding should operate as:

- explicit `palm leaves` -> palm leaf;
- explicit special paper state -> paper with special treatment/state;
- no support exception -> Indian paper by declared catalogue baseline.

This is an information-compression rule built into the catalogue.

The absence of the word `paper` in an individual entry does not mean support is unknown.

Mechanism:

`CATALOGUE_DEFAULT_SUPPORT_BASELINE`.

---

## 3. Palm leaf is overwhelmingly long and narrow

The twelve palm-leaf records include some striking extremes:

- MS 1: c.22.5 × 2.5 in.;
- MS 2: c.22.5 × 2 in. provisionally, with OCR conflict in the fractional long dimension;
- MS 37: 12.5 × 1.5 in.;
- MS 74: 12 × 1 in.

Eleven of twelve have aspect ratio >=5.

The one conspicuous broad exception is MS 46:

- 8.5 × 3 in.;
- aspect ratio c.2.83.

The palm-leaf corpus is therefore not perfectly uniform, but the long-narrow tendency is extremely strong.

---

## 4. Paper manuscripts remain oblong, but usually much wider

Paper does not imply a square or modern book-page geometry.

Many paper manuscripts remain horizontally elongated:

- MS 6: 17 × 3 in.;
- MS 7: 15.25 × 3 in.;
- MS 19: 16.5 × 3 in.;
- MS 35: 12 × 2 in.;
- MS 41: 13 × 2.5 in.;
- MS 64: 11.5 × 2.25 in.;
- MS 75: 13.25 × 2.25 in.

Eight dimensioned paper manuscripts still have aspect ratio >=5.

The paper corpus therefore preserves an oblong manuscript tradition in a subset of cases.

What changes at corpus level is degree, not orientation alone.

Mechanism:

`OBLONG_FORMAT_PERSISTENCE_WITH_PROPORTIONAL_CHANGE`.

---

## 5. The long dimension overlaps strongly across supports

The palm-leaf median long dimension is 12.25 in.; paper is 11.5 in.

Their central ranges overlap substantially:

- palm leaf IQR: 12.0–12.562 in.;
- paper IQR: 10.0–13.0 in.

This means the most visible support difference is not a wholesale rescaling of manuscript length.

A useful descriptive formulation is:

`long-axis scale remains in the same broad working range`.

Do not turn this into a direct historical continuity claim without matched copy states.

---

## 6. The short dimension carries the stronger support distinction

The short-dimension medians differ by a full inch:

- palm leaf: 2.0 in.;
- paper: 3.0 in.

The IQRs are largely separated:

- palm leaf: 1.75–2.25 in.;
- paper: 2.75–3.5 in.

Only 6 of 66 dimensioned paper manuscripts have short dimension <=2.25 in., compared with 10 of 12 palm-leaf manuscripts.

This supports a paper-centred hypothesis:

**paper often permits a wider writable field while retaining a broadly familiar long-axis scale.**

Mechanism:

`PAPER_WRITING_FIELD_EXPANSION`.

`permits` here is an affordance statement at corpus level, not a claim that support alone caused every format choice.

---

## 7. Aspect ratio makes the proportional change visible

Median aspect ratio:

- palm leaf: c.6.70;
- paper: c.3.64.

Thus paper manuscripts, although still often oblong, are typically less extremely elongated.

This is a more precise claim than either:

`paper preserves palm-leaf format`

or

`paper replaces palm-leaf format`.

The catalogue instead suggests:

`oblong manuscript convention persists + available paper field broadens proportionally`.

---

## 8. Broad paper outliers show that paper opens additional format space

Some paper manuscripts occupy dimensions far outside the central palm-leaf geometry:

- MS 36: 11.25 × 6 in.;
- MS 63: 15 × 7 in.;
- MS 9: 17 × 5.25 in.;
- MS 18: 13 × 4.5 in.

The secure observation is that the paper corpus spans a much broader short-dimension range, reaching 7 in., while the palm-leaf corpus reaches only 3 in.

Mechanism:

`PAPER_FORMAT_RANGE_EXPANSION`.

This may reflect textual, scribal, visual, ritual or production requirements, but those correlations must be tested rather than assumed.

---

## 9. This is not yet a transition history

The catalogue is cross-sectional. It places different manuscripts, dates and works side by side.

Therefore the statistics support:

`support <-> format association in the surviving Hodgson RAS corpus`.

They do not by themselves prove:

`a text copied from palm leaf onto paper keeps length and gains width`.

That stronger historical claim requires a matched pair or demonstrable copy lineage.

Mechanism code should remain:

`LONG_AXIS_OVERLAP_SHORT_AXIS_EXPANSION`

rather than:

`PALM_LEAF_TO_PAPER_WIDTH_EXPANSION`.

The latter is a hypothesis for future paired-witness testing.

---

## 10. A high-value matched-pair test now becomes obvious

Search for the same work in:

- palm-leaf witness;
- paper witness;
- demonstrable copy/translation relation if possible.

Record:

- long dimension;
- short dimension;
- line count;
- columns;
- cord-hole/blank-stripe structure;
- ruling;
- leaf count;
- support;
- hand/date;
- whether textual segmentation is preserved.

The strongest future result would be direct evidence that a paper copy retains one dimension or structural feature of the palm-leaf exemplar while expanding another.

---

## 11. Cord holes and blank stripes complicate pure dimensional comparison

Cowell and Eggeling's photographic discussion of old manuscripts explains that some pages are divided into columns by blank stripes through which cord holes pass.

A short dimension is therefore not simply `more or less writing space`.

It can include structural zones required by the manuscript's binding/cord system.

Direct page analysis should separate:

`total leaf dimension`

from

`effective written field`.

Mechanism:

`TOTAL_PAPER_GEOMETRY_VS_INSCRIBED_FIELD_GEOMETRY`.

This is crucial before making stronger affordance claims.

---

## 12. Relation to the blackened-paper family 77–79

MSS 77–79 form a catalogued material family at 8 × 2.75 in.

Their aspect ratio is only c.2.91, considerably broader than the palm-leaf median despite their small overall size.

This reinforces the point that support, treatment and format are separate variables.

Do not infer a ritual-format rule from this one family.

---

## 13. Source-control exceptions

### MS 2

Main catalogue OCR reads approximately 22 1/3 × 2 in.; a later duplicated catalogue summary in the same uploaded scan reads 22 1/2 × 2 in.

Use 22.5 provisionally and mark the fractional long dimension for image verification.

### MS 17

Main OCR loses the denominator of the short-dimension fraction. A later duplicated summary gives 13 × 2.75 in.

Use that value provisionally.

### MS 53

OCR does not securely preserve the long-dimension fraction. Exclude it from geometry statistics until the printed page is inspected.

### MSS 78–79

Dimensions are not repeated locally. They inherit size from preceding entries through the catalogue's explicit relational description and are coded 8 × 2.75 in. accordingly.

---

## 14. Article-level formulation

**Cowell and Eggeling's catalogue suggests that the shift between palm leaf and paper was not simply a substitution of one support for another or a replacement of one manuscript form by a modern book page. The twelve palm-leaf manuscripts are overwhelmingly long and narrow, with a median short dimension of about two inches and a median aspect ratio near 6.7. Paper manuscripts occupy a similar long-axis scale but broaden substantially, with a median short dimension of three inches and an aspect ratio near 3.6. Many remain recognizably oblong. Paper therefore appears to enlarge the available writing field mainly across the short axis while preserving, at corpus level, a familiar range of manuscript lengths.**

Immediately follow with the limit:

**This is a corpus association, not yet a demonstrated before-and-after transition. Matched witnesses are required to show how a particular work changed form when recopied onto paper.**

---

## 15. New/refined mechanism codes

- `ENTRY_LEVEL_SUPPORT_REVIEW_SUPERSEDES_KEYWORD_CENSUS`
- `CATALOGUE_DEFAULT_SUPPORT_BASELINE`
- `SUPPORT_FORMAT_ASSOCIATION`
- `LONG_AXIS_OVERLAP_SHORT_AXIS_EXPANSION`
- `PAPER_WRITING_FIELD_EXPANSION`
- `OBLONG_FORMAT_PERSISTENCE_WITH_PROPORTIONAL_CHANGE`
- `PAPER_FORMAT_RANGE_EXPANSION`
- `TOTAL_PAPER_GEOMETRY_VS_INSCRIBED_FIELD_GEOMETRY`

## Bottom line

The catalogue supplies a measurable paper/form result. Palm leaf and paper do not occupy wholly separate length scales, but they do occupy sharply different proportional regimes. Palm leaves are generally much narrower; paper expands the short axis and permits a wider range of writing fields while often retaining an oblong long-axis convention. This gives the paper article a quantitative material-form section without pretending that a cross-sectional catalogue is a direct history of support conversion.