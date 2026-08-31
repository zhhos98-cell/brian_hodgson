# Balston / Whatman nineteenth-century calibration for the Hodgson paper project

Date: 2026-08-31

Status: working technical note based on Library OCR of Thomas Balston, *James Whatman, Father & Son* and J. N. Balston, *The Elder James Whatman*. Purpose: prevent direct transfer of Georgina Wilson's largely early-modern mould-paper diagnostics into Hodgson's nineteenth-century paper corpus.

## 1. Why this calibration is necessary

Wilson gives the project a strong method: begin from the sheet, reconstruct formation and use, and treat material affordance as a combination of enablement, constraint and failure. But Hodgson's career sits across a paper regime in transition:

- handmade laid papers;
- handmade wove papers;
- increasingly industrial/machine-made papers;
- nineteenth-century watermark technologies that cannot all be treated as wire profiles sewn to a traditional mould;
- British papers entering East India Company supply systems;
- local Nepali handmade papers with a different fibre and sheet-forming history.

Accordingly, the presence of `WHATMAN`, a watermark date, or the absence of visible chain lines cannot be interpreted without identifying manufacturing technology and historical firm/mill context.

---

## 2. The 1806 split is crucial for Hodgson-period watermark interpretation

Balston states that the Whatman-successor firm broke up in **1806**.

After the split:

- the Hollingworth brothers remained at **Turkey Mill** and used the countermark **`J WHATMAN TURKEY MILL`** on their **hand-made papers**;
- William Balston worked first for a year at Hollingbourne Mill and thereafter at **Springfield Mill**, using **`J WHATMAN`**;
- in **1859** the Hollingworths sold their mark to Balston's sons, after which both marks belonged to the Balston descendants.

### Hodgson implication

For a Hodgson-period sheet dated/used between roughly 1806 and 1859:

`J WHATMAN TURKEY MILL` and `J WHATMAN` should not be normalized into one generic `Whatman paper` label.

They potentially encode different mill/firm histories and therefore different supply batches.

Minimum census distinction:

- `mark_as_seen`
- `mark_variant`
- `probable_mill`
- `probable_firm`
- `mark_usage_window`
- `manufacture_mode`
- `evidence_source`

This may allow batch or procurement differences to emerge across Hodgson's drawings, correspondence and working papers.

---

## 3. Whatman and East India Company paper supply

Balston links the Whatman business directly to the East India Company.

He notes that Jacob Bosanquet began a long association with the East India Company as Director/Chairman in 1782 and that the Company required **large quantities of paper both at home and abroad**. Balston states that Whatman had a **considerable share** in this supply, citing a later draft letter to the Directors.

The draft itself was written on paper countermarked `J WHATMAN 1804`.

### Hodgson implication

This materially strengthens a supply-infrastructure question already latent in the project:

> Was Hodgson's imported/Whatman paper simply purchased ad hoc in South Asia, or did some of it move through an established East India Company paper-procurement ecology?

This should be pursued through:

- East India Company stationery contracts;
- Bengal/Calcutta stationery procurement;
- India Office paper purchasing records;
- residency stationery accounts;
- stationers handling Whatman/Turkey Mill/Springfield papers;
- paper sent as Company stores vs private purchase.

Do not yet claim a direct supply chain from Turkey/Springfield Mill to Hodgson without documentary linkage.

---

## 4. Watermark date is not automatically paper-making year or use year

The Excise legislation of 1794 required dates in paper watermarks for certain duty/drawback purposes. Balston notes:

- the dating requirement began in 1794;
- the relevant clause was repealed in 1811;
- manufacturers initially did not always change dates annually;
- irregularities in dated Whatman sequences around 1794–1804 are well established;
- by the end of the first decade of the nineteenth century annual updating appears to have become more regular.

A related passage says that from 1794 until abolition of paper duties in 1861 most white papers displayed a date, although the date was not invariably correct.

### Hodgson rule

A watermark date is a **terminus / manufacturing clue**, not a self-interpreting object date.

Record separately:

- `watermark_date_as_seen`
- `probable_paper_manufacture_date`
- `inscription_or_drawing_date`
- `first_documented_use_date`
- `date_gap_years`
- `dating_confidence`

Potentially important phenomenon: long-held paper stock. A sheet bearing an earlier watermark may have been used many years later.

---

## 5. `Wove` is a physical formation technology, not merely a prestige label

Balston describes the wove-wire mould as designed to eliminate the chain and laid-wire furrows of ordinary laid paper and produce a more uniformly smooth sheet. Whatman often placed countermarks toward the **edges** of wove sheets.

This creates two Hodgson implications.

### A. Surface affordance is testable

A smoother, more uniform surface could matter for:

- fine ink line;
- pencil;
- watercolour/wash;
- tracing;
- drawing reproduction;
- tabular/administrative writing.

But this must be demonstrated from use and media interaction, not assumed.

### B. Crop/mounting can destroy watermark visibility

If countermarks sit at sheet edges, later trimming, binding or mounting may remove or conceal the mark while preserving most of the working surface.

Therefore `no mark visible` is especially weak evidence in a trimmed/mounted Hodgson drawing.

---

## 6. Thick papers can hide their own watermark

Balston's discussion of Whatman's large `Antiquarian` / Double Atlas paper is methodologically important. Thick sheets can make marks difficult to detect, particularly once mounted. In one watercolour example, a `J WHATMAN TURKEY MILL 1792` countermark was found at the bottom of a sheet only through close examination.

### Hodgson implication

For large zoological drawings or mounted sheets:

- ordinary reflected-light photography is insufficient for a reliable negative watermark claim;
- transmitted light should be requested where possible;
- edge areas deserve specific imaging;
- mounting status must be recorded;
- a watermark/countermark may survive only fragmentarily or under a mount/window.

This directly supports the `PAPER_CENSUS_PROTOCOL_V0_1` surrogate rule.

---

## 7. A mark alone may not identify a maker

J. N. Balston shows that watermark attribution can fail if based on one graphic element alone.

Examples include:

- similar `W` marks used across different makers;
- mould makers supplying related designs;
- older/cast-off moulds moving into other manufacturers' hands;
- attribution strengthened only when mark construction is combined with chain-wire spacing, laid-wire density and other design components.

### Hodgson rule

Never code `maker = Whatman` solely because an isolated `W` resembles a known Whatman mark.

Preferred evidence stack:

1. full wording (`J WHATMAN`, `J WHATMAN TURKEY MILL`, etc.);
2. date;
3. mark construction;
4. sheet formation (laid/wove);
5. chain/laid measurements where relevant;
6. sheet dimensions;
7. countermark relation;
8. comparison to a dated/reference corpus;
9. archival date/use context.

---

## 8. Nineteenth-century watermark technology warning

J. N. Balston explicitly distinguishes traditional **wire profiles** sewn onto mould covers from other watermarking methods introduced in the nineteenth century.

This validates the technology warning already added to the Hodgson paper census:

> identify the watermark-making mechanism before applying mould-pair/twin-mark reasoning.

Potential categories to distinguish as research develops:

- traditional mould wire profile;
- wove-mould countermark;
- machine-made/dandy-roll watermark;
- embossed/other nineteenth-century marking technologies;
- unknown.

---

## 9. Paper type is more granular than maker name

Balston describes materially distinct Whatman products, including a `Yellow Wove` that was very thick and stiff, later appearing pale cream. He also documents large-format papers designed for specific tasks, including `Antiquarian`, made for copper-plate engraving.

Thus `Whatman paper` is not one material.

For Hodgson we need to distinguish, where evidence permits:

- maker/brand;
- mill;
- grade/type;
- formation;
- thickness/bulk;
- stiffness;
- surface;
- colour;
- size;
- intended commercial category;
- actual Hodgson use.

The same brand can support different affordance profiles.

---

## 10. Named paper sizes are historical technical categories

Balston's paper history repeatedly uses historically regulated/commercial sizes such as:

- Post;
- Demy;
- Double Demy;
- Foolscap;
- Royal;
- Double Elephant;
- Double Atlas / Antiquarian.

One example gives `Double Elephant` at about 3 ft 4 in × 2 ft 2.5 in; `Antiquarian/Double Atlas` was still larger and designed for plate work.

### Hodgson rule

Record measured dimensions first. Assign a historical paper-size name only when dimensions, production context and period usage support it.

This matters because later cutting/trimming can turn a historical half-sheet into dimensions that resemble another named format.

---

## 11. Lined wove shows paper as instrument before inscription

Balston identifies a special `Lined Wove`: a wove-wire mould was supplemented by thicker wires at regular intervals so the resulting sheet contained visible lines strong enough to guide level handwriting before printed ruling became normal.

This is a particularly good bridge to Wilson's `paper as instrument` formulation.

The operative feature is made **during sheet formation**, before the user writes anything.

### Hodgson implication

When examining administrative tables, lists or correspondence, look for:

- watermark-like structural ruling;
- printed ruling;
- pencil ruling;
- blind/embossed ruling;
- fold-generated guides;
- hand-drawn column lines.

Different ruling technologies distribute cognitive/administrative work differently between paper manufacturer, stationer, clerk and writer.

---

## 12. Paper sizing is an operational variable

Balston's account of Whatman's sizing process describes whole batches of paper immersed until saturated and then pressed. This reinforces sizing as a manufacturing operation capable of changing later interaction with liquid media.

For Hodgson, `sizing` should not remain a vague conservation descriptor. Where observable/testable, connect it to:

- ink penetration/feathering;
- wash behaviour;
- surface abrasion;
- wet strength;
- folding;
- paste adhesion;
- later conservation treatment.

No causal claim should be made from appearance alone.

---

## 13. Wilson → Balston → Hodgson: revised analytical stack

### Wilson supplies the method

**sheet biography + affordance + composition/decomposition + reuse + failure**.

### Balston supplies technical calibration

**mill/firm history + watermark variation + dated marks + paper sizes + wove/laid technology + commercial supply + nineteenth-century transition**.

### Hodgson archive supplies the historical test

For every paper unit ask:

1. What is directly observable?
2. Which manufacturing technology produced it?
3. Which mill/brand/stock attribution is justified?
4. Through what procurement/supply route could it have reached Hodgson?
5. What operation was performed on it?
6. What material property enabled that operation?
7. What constraint or failure followed?
8. What workaround, repair, reuse or archival transformation followed?

This stack keeps the project anchored in paper rather than turning `Whatman` into a prestige keyword.

---

## 14. High-priority Hodgson tests generated by this calibration

1. Search Hodgson material separately for `J WHATMAN` and `J WHATMAN TURKEY MILL`, especially 1820s–1840s drawings and correspondence.
2. Compare watermark dates with inscription dates to measure paper-stock lag.
3. Check whether drawing papers cluster by Turkey Mill vs Springfield marks.
4. Search East India Company / Bengal stationery procurement for Whatman/Balston/Hollingworth contracts or shipments.
5. Request transmitted-light images of large/mounted zoological drawings where ordinary images show no mark.
6. Test whether sheet dimensions correspond to commercial drawing/plate paper sizes before and after trimming.
7. Distinguish handmade wove Whatman sheets from generic catalogue descriptions of `machine-made paper` where possible; repository catalogue terminology may collapse technology.
8. Look for ruling technologies in Hodgson administrative and list papers as paper instruments.

## 15. Current caution

The Balston works are themselves historical reconstructions, not substitutes for physical comparison or mill ledgers. Use them to generate and constrain identifications, then verify individual Hodgson paper units against object images, repository descriptions, and where possible physical/transmitted-light inspection.
