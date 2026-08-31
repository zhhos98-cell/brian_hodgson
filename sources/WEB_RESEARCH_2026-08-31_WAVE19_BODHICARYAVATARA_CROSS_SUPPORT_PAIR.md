# Web research 2026-08-31 — Wave 19
## Bodhicaryāvatāra as the first exact-work cross-support comparison beyond the RAS 79

Date: 2026-08-31

Status: cross-collection follow-up to `sources/PAPER_MATCHED_WITNESS_TEST_RAS_CATALOGUE_1875.md`. The RAS 79-entry catalogue contains no secure exact-work palm-leaf/paper pair. This wave searches outside that corpus while retaining strict distinctions between text identity, recension identity, container relation and copy lineage.

## Executive result

A high-value exact-work cross-support comparison exists for the `Bodhicaryāvatāra`:

- **RAS Hodgson MS 13**: palm leaf, 47 leaves, 12½ × 1¾ in., 5 lines per page, 10 paricchedas, described as old;
- **Cambridge University Library Add. 869**: paper, 66 leaves, 10¼ × 4½ in., 7 lines per page, modern ordinary Devanāgarī hand, 10 paricchedas.

Bendall explicitly directs the Cambridge entry to `R. A. S. Cat. No. 13`, so the comparison is not based merely on title resemblance.

This is the first secure **same named work + same ten-section structure + different support** comparison in the current paper project.

It is still **not a copy-lineage matched pair**. There is no evidence yet that Cambridge Add. 869 was copied from RAS Hodgson MS 13 or from the same exemplar. The Cambridge witness is also described as the ninth section of an `Aśokāvadānamālā` textual/container context.

Mechanisms:

- `EXACT_WORK_CROSS_SUPPORT_PAIR_WITHOUT_COPY_LINEAGE`
- `TEXT_CONTROLLED_SUPPORT_COMPARISON`
- `CONTAINER_AND_CHRONOLOGY_CONFOUND_REMAINS`

---

## 1. RAS Hodgson MS 13: palm-leaf witness

Cowell and Eggeling catalogue the manuscript as:

- `Bodhicharyāvatāra`;
- ten paricchedas;
- 47 palm leaves;
- 12½ × 1¾ in.;
- five lines per page;
- old;
- unusual shapes in some numerals and letters.

The Royal Asiatic Society online collection independently confirms:

- Sanskrit;
- palm leaf;
- five lines on each page;
- ten chapter endings;
- acquired by Hodgson in Nepal and given to the Society in 1835–36.

Primary/local source: Cowell and Eggeling 1875, RAS Hodgson MS 13, parsed from `Adobe Scan 2025年3月28日.pdf_by_PaddleOCR-VL-1.6.json`.

Online collection record:
https://royalasiaticcollections.org/ras-hodgson-ms-13-bodhicaryavatara/

---

## 2. Cambridge Add. 869: paper witness

Cecil Bendall’s 1883 Cambridge catalogue gives:

- `Add. 869`;
- paper;
- 66 leaves;
- seven lines;
- 10¼ × 4½ in.;
- modern ordinary Devanāgarī hand;
- `Bodhicaryāvatāra`;
- verse text in ten paricchedas.

Most importantly for source control, Bendall writes: `See R. A. S. Cat. No. 13`.

He also notes copies at the India Office, Paris and Calcutta.

Primary source:
Cecil Bendall, *Catalogue of the Buddhist Sanskrit Manuscripts in the University Library, Cambridge* (Cambridge, 1883), p. 6, Add. 869.

Searchable text surrogate:
https://archive.org/stream/catalogueofbuddh00camb/catalogueofbuddh00camb_djvu.txt

The Cambridge witness is described as the ninth section of the `Aśokāvadānamālā` tradition/container. That relation must be carried as a confound rather than suppressed.

---

## 3. Geometry comparison

### RAS Hodgson MS 13 — palm leaf

- long axis: 12.5 in.;
- short axis: 1.75 in.;
- aspect ratio: c.7.14;
- leaf area proxy: c.21.88 sq. in.;
- lines/page: 5.

### Cambridge Add. 869 — paper

- long axis: 10.25 in.;
- short axis: 4.5 in.;
- aspect ratio: c.2.28;
- leaf area proxy: c.46.13 sq. in.;
- lines/page: 7.

### Relative change

Using the RAS palm-leaf witness as the comparison baseline:

- long axis decreases to c.82% of the palm-leaf length;
- short axis expands by c.2.57×;
- area proxy expands by c.2.11×;
- aspect ratio falls from c.7.14 to c.2.28;
- line count rises from 5 to 7.

This is a much stronger object-level illustration of the corpus-level pattern than the RAS-only near-pair MSS 34–35.

The paper witness does not simply preserve the palm-leaf outline while adding a little width. It occupies a substantially broader page regime.

Mechanisms:

- `SHORT_AXIS_EXPANSION_WITH_LONG_AXIS_REDUCTION`
- `PAPER_PAGE_AREA_EXPANSION`
- `EXTREME_OBLONG_TO_BROAD_OBLONG_SHIFT`

---

## 4. Why this pair is stronger than MSS 34–35

RAS MSS 34–35 share a root-text ecology (`Nāmasaṅgīti`) but are different commentaries. They are therefore a controlled near-pair, not the same work.

RAS MS 13 and Cambridge Add. 869 are both explicitly catalogued as `Bodhicaryāvatāra`, both have ten paricchedas, and Bendall cross-references the RAS catalogue entry.

That controls textual identity much more tightly.

However, this pair still does not establish a historical transition from one physical witness to the other.

Required distinction:

`same work across supports != same copy lineage`.

---

## 5. The pair supports affordance, not determinism

Taken alone, the Bodhicaryāvatāra pair could tempt a simple story:

`palm leaf -> paper = shorter + much wider page`.

The RAS corpus prevents that simplification.

Within the RAS catalogue:

- paper formats range widely;
- MS 35 is a narrow paper manuscript at 12 × 2 in.;
- MSS 59–60 show explicitly identical textual content in different paper geometries;
- the aggregate paper median short axis is 3 in., not 4½ in.

The correct formulation is therefore:

**Paper permits a much broader page geometry, and the Bodhicaryāvatāra comparison shows that this possibility can be realized even when the work itself is held relatively constant. It does not show that paper mechanically forces every copy into that geometry.**

Mechanism:

`SUPPORT_AFFORDANCE_VISIBLE_UNDER_TEXT_CONTROL`.

---

## 6. Remaining confounds

### Copy lineage

No direct genealogical relation between the RAS and Cambridge witnesses has been established.

### Chronology / hand

- RAS MS 13: old palm-leaf witness with unusual numeral/letter forms;
- Cambridge Add. 869: modern ordinary Devanāgarī paper witness.

Support and date/hand therefore move together in this comparison.

### Container / textual framing

Bendall places Add. 869 in relation to the `Aśokāvadānamālā`, describing the BCA as its ninth section. That may affect textual framing, copying programme or manuscript production.

### Leaf count

47 versus 66 leaves should not be interpreted as a direct efficiency measure until textual extent, omissions, verse segmentation, margins and writing-field dimensions are compared.

Mechanisms:

- `SUPPORT_DATE_HAND_CONFOUND`
- `TEXTUAL_CONTAINER_CONFOUND`
- `LEAF_COUNT_NOT_DIRECT_EFFICIENCY_METRIC`

---

## 7. Article-level use

This pair is strong enough for the paper article as a controlled comparative vignette:

**A Bodhicaryāvatāra witness in Hodgson’s RAS collection survives on palm leaf as a 12½ × 1¾ inch object with five lines to the page. Bendall’s Cambridge Add. 869, explicitly cross-referenced to the RAS entry and likewise arranged in ten sections, is on paper at 10¼ × 4½ inches with seven lines. Holding the named work and broad section structure relatively constant therefore reveals a dramatic widening of the available page field, although chronology, script, container relation and copy lineage remain uncontrolled.**

The wording `holding relatively constant` is essential. Do not call this a direct recopying event.

---

## 8. Next search

The Cambridge catalogue now becomes the first external comparison corpus.

Search the remaining eleven RAS palm-leaf titles for paper witnesses, prioritising:

1. `Aṣṭasāhasrikā Prajñāpāramitā`;
2. `Saṃpuṭodbhava`;
3. `Tattvajñānasaṃsiddhi-ṭippaṇī`;
4. `Caṇḍamahāroṣaṇa / Ekallavīra-tantra`;
5. `Nāmasaṅgīti-ṭīkā / Gūḍhapadā` with exact commentary identity rather than merely the root work.

For each candidate, record whether the external catalogue explicitly cross-references the RAS/Hodgson witness or merely shares a title.

## Bottom line

The RAS-only search produced no exact cross-support pair. Moving one collection outward immediately produces one: Bodhicaryāvatāra, palm leaf in Hodgson’s RAS MS 13 and paper in Cambridge Add. 869. The geometry contrast is large and runs in the same direction as the corpus-level paper association, but the historical claim remains carefully bounded: this is an exact-work support comparison, not yet a demonstrated palm-leaf-to-paper copy lineage.