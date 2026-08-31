# Matched-witness test for palm leaf and paper in the Cowell–Eggeling Hodgson catalogue, 1875

Date: 2026-08-31

Status: follow-up to `sources/PAPER_SUPPORT_FORMAT_ASSOCIATION_COWELL_EGGELING_1875.md`. This note tests whether the 79-entry Royal Asiatic Society Hodgson catalogue contains a secure same-work palm-leaf/paper pair capable of supporting a direct before/after format argument.

Primary source: E. B. Cowell and J. Eggeling, “Catalogue of Buddhist Sanskrit Manuscripts in the possession of the Royal Asiatic Society (Hodgson Collection),” *Journal of the Royal Asiatic Society*, new series, 8.1 (1875), pp. 1–52, parsed from `Adobe Scan 2025年3月28日.pdf_by_PaddleOCR-VL-1.6.json`.

## Executive result

The strong matched-witness test fails inside this catalogue in a useful way.

After sequential review of all 79 catalogue entries and correction of the support census to twelve palm-leaf manuscripts, **no secure exact-work pair was found in which one witness is palm leaf and the other paper**.

This means the catalogue can support a cross-sectional association between support and geometry, but it cannot by itself demonstrate a direct transformation of one work from palm leaf to paper.

Mechanisms:

- `NO_SECURE_EXACT_WORK_CROSS_SUPPORT_PAIR_IN_RAS79`
- `CORPUS_ASSOCIATION_NOT_COPY_TRANSITION`
- `MATCHED_WITNESS_REQUIREMENT_UNSATISFIED_IN_SINGLE_COLLECTION`

This is a negative result, not evidence that such pairs did not exist historically. It only establishes that the 79 catalogued RAS entries do not supply a secure one.

---

## 1. Corrected palm-leaf set

Direct entry-level review identifies twelve palm-leaf manuscripts:

`1, 2, 13, 34, 37, 43, 46, 67, 68, 69, 70, 74`.

The two entries omitted by the earlier keyword-oriented census were:

- MS 34, `Nāmasaṅgīti-ṭīkā`, entitled `Gūḍhapadā`: 180 palm leaves;
- MS 37, `Saṃpuṭodbhava`: 127 palm leaves.

The omission arose because the OCR renders `palm-leaves` with a hyphen in these entries. A support parser restricted to the literal phrase `palm leaves` therefore undercounted the corpus.

Mechanism:

`HYPHEN_VARIANT_CAUSES_KEYWORD_CENSUS_UNDERCOUNT`.

The support baseline remains Cowell and Eggeling’s explicit rule that manuscripts are Indian paper unless otherwise stated.

---

## 2. Exact-title / exact-work cross-support search

The twelve palm-leaf entry titles were checked against the sixty-seven paper entries.

No secure exact-title cross-support duplicate appears.

The catalogue does contain exact-title repetition within paper:

- MSS 56 and 57 are both `Pañcarakṣā` and both are paper under the catalogue baseline.

It also contains explicit same-text relations within paper:

- MS 59 contains the `Grahamātṛkā-dhāraṇī` as its final portion;
- MS 60 is `Grahamātṛkā` and is explicitly described as `Identical with the last portion of the preceding MS.`

These are valuable controls, but neither is a palm-leaf/paper conversion.

Mechanism:

`SAME_TEXT_VARIATION_WITHOUT_SUPPORT_CHANGE`.

---

## 3. The strongest cross-support near-pair is MSS 34–35, but it is not a matched witness

### MS 34

`Nāmasaṅgīti-ṭīkā`, entitled `Gūḍhapadā`:

- support: palm leaf;
- 180 leaves;
- 12 × 2¼ in.;
- seven lines per page;
- old;
- fifteen chapters.

### MS 35

`Nāmasaṅgīti-tippaṇī`, entitled `Amṛtakaṇikā`:

- support: paper by catalogue baseline;
- 62 leaves, with discontinuous numbering;
- 12 × 2 in.;
- ten lines per page;
- very minutely written;
- dated palaeographically by the cataloguers to about the end of the eighteenth century.

Cowell and Eggeling explicitly introduce MS 35 as `Another commentary on the same work`.

This creates a controlled relation at the level of **root text / commentary ecology**, not manuscript identity or copy lineage.

Mechanisms:

- `SAME_ROOT_TEXT_DIFFERENT_COMMENTARY`
- `CROSS_SUPPORT_NEAR_PAIR_NOT_COPY_PAIR`

### Material result

The near-pair does not reproduce the corpus-level width-expansion pattern:

- both have the same long dimension: 12 in.;
- the paper manuscript is slightly narrower: 2 in. versus 2¼ in.;
- the paper manuscript carries ten lines per page versus seven on palm leaf.

Thus the first controlled cross-support comparison available inside the catalogue points in the opposite geometrical direction from a simple `paper -> wider page` rule.

The correct interpretation is not that the corpus result is wrong. It is that support is one variable among several, and scribal density, textual function, copying convention and format tradition can override or mediate support affordances at the object level.

Mechanisms:

- `SUPPORT_AFFORDANCE_NOT_FORMAT_DETERMINISM`
- `NARROW_PAPER_POTHI_PERSISTENCE`
- `LINE_DENSITY_MEDIATES_WRITING_FIELD`

This is precisely why the aggregate claim should remain:

`paper often permits a wider short axis`

rather than:

`paper causes width expansion`.

---

## 4. Same-support controls show that text identity does not fix geometry

### MSS 56–57: Pañcarakṣā / paper–paper

MS 56:

- 152 leaves;
- 12 × 2¾ in.;
- five lines per page;
- dated Samvat 887 / A.D. 1767;
- some leaves supplied by a more modern hand.

MS 57:

- 40 leaves;
- 10 × 2¾ in.;
- five lines per page;
- described as oldish.

The same catalogue title appears on the same support with different long dimensions and radically different extents. Title identity alone is therefore insufficient to infer identical textual extent, copying state or format history.

### MSS 59–60: Grahamātṛkā / explicit same-text paper–paper control

MS 59:

- a collection of dhāraṇīs called `Saptavāra` on the wrapper;
- 26 leaves;
- 8½ × 2½ in.;
- five lines per page;
- oldish;
- foll. 17–26 contain the `Grahamātṛkā-dhāraṇī`.

MS 60:

- `Grahamātṛkā`;
- explicitly `Identical with the last portion of the preceding MS`;
- 13 leaves;
- 9½ × 2¾ in.;
- five lines per page;
- dated Samvat 818 / A.D. 1698.

This is the strongest internal control for the proposition that **even the same textual content can occupy different paper geometries**.

Mechanisms:

- `TEXT_IDENTITY_DOES_NOT_FIX_PAPER_GEOMETRY`
- `SAME_SUPPORT_FORMAT_VARIABILITY`
- `COLLECTION_CONTEXT_CHANGES_TEXTUAL_OBJECT_GEOMETRY`

The comparison also warns against treating the physical leaf count of an excerpt embedded in a collection as directly equivalent to the leaf count of a standalone witness.

---

## 5. Consequence for the paper-support argument

The corpus-level support/format result remains descriptive and strong:

- palm leaf: median short dimension c.2.0 in.;
- paper: median short dimension c.3.0 in.;
- palm leaf: median aspect ratio c.6.7;
- paper: median aspect ratio c.3.64.

But the internal pair tests establish three limits:

1. there is no secure palm-leaf/paper exact-work matched witness in the 79-entry catalogue;
2. the best cross-support near-pair, MSS 34–35, does not widen on paper;
3. same-text paper witnesses can vary materially even without support change.

The article-level claim should therefore be tightened to:

**Paper expands the available format space of the Hodgson RAS manuscript corpus, especially across the short axis, but support does not determine the geometry of any individual witness. The catalogue contains no secure same-work palm-leaf/paper pair that would justify turning this corpus association into a direct copy-transition history.**

---

## 6. What the next matched-witness search must do

The search must now leave the RAS 79-entry catalogue and move across collections.

High-value target design:

- start from the twelve palm-leaf RAS works;
- search Hodgson-related holdings in other repositories for the same work on paper;
- prefer witnesses with a demonstrable Hodgson acquisition/copying relation;
- distinguish exact work, recension, commentary, extract and merely shared textual family;
- record dimensions, support, foliation, line count, columns, cord-hole/blank-stripe structure, ruling, hand/date and collection provenance;
- only call a pair `matched` when title/content identity and witness relation are independently defensible.

Candidate priority from the RAS palm-leaf set:

1. `Nāmasaṅgīti-ṭīkā / Gūḍhapadā` because a paper commentary on the same root work already provides a local near-pair;
2. `Aṣṭasāhasrikā Prajñāpāramitā` because the wider Prajñāpāramitā tradition is heavily represented across collections, while recension identity must be controlled strictly;
3. `Bodhicaryāvatāra`;
4. `Saṃpuṭodbhava`;
5. `Tattvajñānasaṃsiddhi-ṭippaṇī`;
6. `Caṇḍamahāroṣaṇa / Ekallavīra-tantra`.

Do not treat a shared generic title family as a matched pair.

---

## 7. Data correction generated by this test

This review supersedes the support counts in `data/ras_hodgson_material_catalogue_census_v0_2.json`.

Corrected support totals:

- palm leaf: 12;
- paper: 67;
- total: 79.

The corrected data layer is stored separately as `data/ras_hodgson_material_catalogue_census_v0_3.json` rather than silently rewriting v0.2, so the source-control history preserves how the counting error arose and was corrected.

## Bottom line

The first real matched-witness test changes the argument by refusing an attractive shortcut. The RAS catalogue demonstrates a support-format association, but it does not contain the exact cross-support pair required to narrate a direct palm-leaf-to-paper transformation. Its strongest cross-support near-pair instead shows a narrow, denser paper manuscript beside a palm-leaf commentary on the same root work. The paper history is therefore one of enlarged possibility space and variable operations, not a deterministic replacement geometry.