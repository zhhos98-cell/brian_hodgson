# Archive research wave 37 — material capture states, paper-geometry triage, and corrected printed paper as a working scientific surface

Date: 2026-08-31

Status: paper-centred analysis of the uploaded Linnean and RAS OCR/VLM JSONs. This wave deliberately distinguishes **historical paper state** from **digital capture state**. OCR bounding boxes are used to identify likely duplicate/material views and layout transitions, but not to infer historical dimensions, margins, folds or watermarks unless the underlying object image is independently inspected.

## Executive result

The uploaded scans do not map one digital page to one historical folio in a simple way. Several files preserve different capture states of the same or related paper object:

- duplicate or differently framed views of the same letter;
- pages that contain little/no semantic text and are likely material-documentation views;
- a printed offprint explicitly marked `corrected autograph` alongside another copy/state of the same printed article;
- a later collected reprint whose editorial note says the papers have been materially changed through the author's annotations and revision.

This produces two major paper-history mechanisms:

1. `DIGITAL_CAPTURE_STATE_NONCOINCIDENCE` — scan/OCR page identity is not historical sheet/leaf identity;
2. `PRINTED_PAPER_AS_REVISION_SURFACE` — print is not necessarily the terminal state of a scientific paper object; a printed copy can become a new working surface for authorial revision and later reprinting.

The immediate methodological consequence is strict:

**OCR/VLM coordinates can triage paper geometry, but they cannot by themselves establish historical sheet geometry.**

---

## 1. Linnean SP 514: communication letter and classified catalogue occupy different graphic regimes

Uploaded source:

`Linnean DA-ENG-2-SP-514 ... pdf_by_PaddleOCR-VL-1.6.json`

The file contains:

- cover/archive identifier page;
- Hodgson's covering letter to the Linnean Society, 20 Feb. 1838;
- a long `Classified Catalogue of Nipalese Mammals`;
- a final page detected entirely as an image rather than readable text.

### Covering-letter layout

The letter begins with institutional/address metadata:

- `Resident at the Court of Nepal`;
- sending date;
- `The Secretary, Linnean Society`;
- prose submission through Wallich.

OCR layout treats the prose as relatively continuous blocks.

The letter explicitly explains that:

- the catalogue consolidates forms already described piecemeal;
- classification remains partly provisional;
- further enquiry may alter distinctions.

### Catalogue layout

From the catalogue title onward, the paper surface changes graphic function:

- numbered/generic entries;
- species counts;
- taxonomic names;
- repeated abbreviations;
- compact descriptive clauses;
- near-continuous use of available writing area in the digital crop.

### Mechanism

Codes:

- `LETTER_TO_REFERENCE_SURFACE_TRANSITION`
- `GRAPHIC_DENSIFICATION_FOR_CATALOGUE_USE`

### Paper-history claim

The same transmitted documentary package performs two different operations through paper layout:

`covering letter = route / explanation / institutional address`

`catalogue = dense reference / enumeration / revisable classification`.

The epistemic shift is visible as a change in graphic organization before any claim about different paper stocks is made.

### Caution

The OCR crop geometry is not enough to prove different historical margins, sheet sizes or paper types. These require direct object-image inspection.

---

## 2. SP 514 final image-only page is a material-capture candidate

The final digital page of SP 514 is detected as one full-page image block (`c. 910 x 1683` in OCR coordinates) with no readable text layer.

### Code

`MATERIAL_CAPTURE_CANDIDATE_IMAGE_ONLY`

### Why it matters

Given the user's scan target (`paper / layout / transfer traces / folds`), an image-only terminal page may represent:

- watermark/transmitted-light documentation;
- verso/blank-paper inspection;
- fold/edge detail;
- some other material view.

### Source-control rule

Do **not** call it a watermark page without seeing the underlying image.

The secure statement is only:

`the digital file contains a non-text material-image state that should not be counted as another textual folio`.

This changes how page counts and object structure are reconstructed from OCR JSON.

---

## 3. Linnean CR 48: recommendation certificate as an accretive endorsement surface

Uploaded source:

`Linnean DA-EN-G-1-CR-48 Certificates of Recommendation ... pdf_by_PaddleOCR-VL-1.6.json`

The first digital page has a clear spatial sequence:

1. recommendation text in the upper portion;
2. proposal date below;
3. signatures accumulating across the lower portion.

OCR securely identifies several signatories including Thomas Bell, N. B. Ward, S. B. Booth and W. A. Broderich, while other hands remain uncertain.

### Mechanisms

- `PRECOMPOSED_CREDENTIAL_PLUS_ACCRETIVE_SIGNATURES`
- `ENDORSEMENT_SURFACE`

### Paper-history claim

The certificate sheet does not merely carry a statement. Its lower surface is reserved/used for **distributed validation by additional hands**.

Operational sequence:

`credential proposition -> proposed date/state -> successive signatures -> institutionally actionable recommendation object`.

This is a strong example of paper making a social/scientific credential through **spatial accumulation of assent**.

### Comparison target

This can later be compared with:

- scientific lists that accumulate corrections;
- testimonial notebooks that accumulate copied praise;
- catalogues that accumulate distribution annotations.

The common operation is not semantic similarity but **paper-enabled accretion of validation states**.

---

## 4. CR 48 second digital page is semantically unsafe and may be a different capture state

The second digital page produces highly unstable OCR dominated by apparently nonsensical numerical/word sequences and does not reproduce the recommendation text in a reliable way.

### Code

`LOW_SEMANTIC_HIGH_MATERIAL_CAPTURE_STATE`

### Source-control rule

Do not use this page for substantive biography or certificate wording.

It should be inspected as a possible:

- reverse/verso view;
- transmitted-light/material view;
- bleed-through state;
- unrelated adjacent sheet captured in the same scan batch.

No choice among those states is secure from OCR alone.

---

## 5. Linnean LL-8 proves digital capture state and historical paper state can diverge

Uploaded source:

`Linnean DA-ENG-9-LL-8 ... pdf_by_PaddleOCR-VL-1.6.json`

The first two digital pages both contain the same dated letter opening:

`The Rangers / Dursley / May 15, 1861`.

But they are framed very differently.

### Digital page 1

Text occupies nearly the whole OCR crop.

### Digital page 2

The same letter is detected only in the **right half** of a much wider digital canvas.

This is not good evidence that Hodgson historically wrote only on the right half of a large sheet.

It is evidence that the same object has been digitally represented under different framing/cropping conditions.

### Mechanism

`DUPLICATE_WITNESS_DIFFERENT_CAPTURE_GEOMETRY`

### Methodological consequence

Never calculate historical margins or half-sheet use directly from OCR bounding boxes unless:

- the capture state is known;
- page edges are visible;
- scale is known;
- duplicate captures are reconciled.

This is a concrete warning generated by the archive itself, not an abstract digital-humanities caveat.

---

## 6. LL-8 page 3 is a likely material-inspection view, not a substantive third page of prose

Digital page 3 contains almost no intelligible text and is represented as one large OCR region with a weak reading resembling `E. J. Orden`.

### Code

`MATERIAL_VIEW_OR_FAINT_MARK_CANDIDATE`

Possible historical/material targets include faint paper marks, verso marks or watermark-like features, but none should be identified from the current OCR.

### Important use

The page is still valuable because it shows that the scan batch contains frames intended to document something other than semantic handwriting.

This strengthens the rule:

`digital page count != historical textual page count`.

---

## 7. The LL-8 scan bundle also contains different paper objects

Later digital pages in LL-8 contain:

- a Linnean Society/financial letter;
- banking/agency terms dated 1834;
- other text not continuous with the 1861 Dursley letter.

### Mechanism

`SCAN_BATCH_MULTIPLE_OBJECT_AGGREGATION`

### Consequence

A PDF/JSON batch can be a researcher's material grouping rather than a historical dossier.

Do not infer historical adjacency from scan adjacency.

This is the digital equivalent of the 1921 India Office problem:

`later grouping operation -> new adjacency -> possible false historical relation`.

---

## 8. Buddhist `Notice on Buddhist Symbols`: printed offprint marked as a corrected autograph state

Uploaded source:

`Adobe Scan 2025年3月28日 (3) (1)`.

One page is recognizably printed:

- header: `[From the Journal of the Royal Asiatic Society.]`;
- title: `NOTICE ON BUDDHIST SYMBOLS`;
- printed authorship and date;
- printed body and footnote.

The same page also contains the text/annotation:

`corrected autograph`.

### Mechanisms

- `PRINTED_OFFPRINT_AS_AUTHORIAL_WORK_SURFACE`
- `PRINT_TO_MANUSCRIPT_HYBRID_STATE`

### Safe claim

The surviving witness is not simply `the publication` and not simply `the manuscript`.

It is a printed paper object explicitly identified as a **corrected autograph state**.

The exact hand responsible for the words `corrected autograph` still requires palaeographic/object inspection.

---

## 9. The same article appears again in a different printed state within the scan corpus

A later page in the same uploaded file again begins:

`[From the Journal of the Royal Asiatic Society.]`

`NOTICE ON BUDDHIST SYMBOLS.`

with the same 26 Sept. 1860 letter text and the same two-sheet / 143-symbol description, but without the OCR-visible `corrected autograph` note in the same position.

### Mechanism

`PARALLEL_PRINTED_WITNESS_STATES`

### Research significance

This creates a direct collation target:

`printed witness A: explicitly corrected-autograph state`

versus

`printed witness B: parallel printed state`.

A page-by-page comparison can identify:

- added/deleted text;
- manuscript correction incorporated into print;
- changed footnotes;
- altered punctuation/nomenclature;
- whether the later state descends from the corrected copy.

This is a much stronger paper-history case than generic `authorial correction` because the **material witnesses for before/after states coexist in the same scan corpus**.

---

## 10. A collected reprint explicitly defines print as revisable paper

A later page in the same corpus opens `THE LITERATURE AND RELIGION OF THE BUDDHISTS` and includes an editorial note stating that the following papers are mostly reprints but have been so changed by the **annotations and revision of the author** that they warrant renewed publication; the originals are described as difficult to obtain.

### Mechanisms

- `ANNOTATED_REPRINT_TO_REVISED_EDITION`
- `PRINTED_PAPER_VERSION_CHAIN`
- `SCARCITY_OF_ORIGINALS_AS_REPRINT_DRIVER`

### Core HPS point

Publication does not terminate the paper workflow.

Sequence:

`journal article -> printed/offprint copy -> annotation/revision -> revised reprint/collection`.

This is the print analogue of:

`working manuscript -> correction -> fair copy`.

The scientific paper object remains generative after printing.

---

## 11. The Buddhist-symbol article itself makes the sheet an explicit comparative unit

The article states that Hodgson transmits:

`two sheets containing collectively 143 symbols`.

It further says the first 33 occupy the two uppermost lines and derive from printed coin sources, while the rest derive from Nepalese Saugata temples/images; six additional separate figures come from stone images and illuminated manuscripts.

### Mechanisms

- `SHEET_AS_COMPARATIVE_ARRAY`
- `SOURCE_GROUPING_BY_PLANAR_POSITION`

### Important refinement

Wave 36 treated the two sheets as a finite comparative field. Wave 37 adds a stronger textual point:

**source provenance is partly encoded spatially** (`first 33` / `two uppermost lines`).

The paper layout therefore does not merely hold 143 signs; it may preserve a source distinction inside the comparison array.

### Next test

Directly inspect the two symbol sheets to determine whether:

- upper-line grouping visibly separates numismatic symbols;
- numbering follows source or semantic grouping;
- empty space or line breaks mark distinct provenance classes.

---

## 12. Paper state and digital state need separate ontologies

### Historical paper-state fields

- sheet / leaf / bifolium / notebook / offprint;
- recto / verso;
- full sheet / half sheet;
- folded / unfolded;
- original / copy / translation / print / corrected print;
- watermark / countermark;
- hand / ink / pencil;
- pasted/attached layer;
- binding state.

### Digital capture-state fields

- full-object capture;
- cropped text capture;
- duplicate capture;
- transmitted-light capture;
- verso capture;
- watermark/detail capture;
- rotated capture;
- material-only frame;
- OCR-only derivative;
- VLM-unwarped derivative.

### Mechanism

`HISTORICAL_OBJECT_STATE_DIGITAL_CAPTURE_STATE_SEPARATION`

A material-history dataset must carry both.

---

## 13. Revised rule for OCR geometry

OCR polygon/bounding-box data can support:

- identifying duplicated textual witnesses;
- identifying dense vs sparse graphic regimes;
- detecting text confined to one region of a digital frame;
- detecting pages with no semantic text;
- locating candidate annotations relative to print.

OCR geometry cannot by itself support:

- physical dimensions;
- true historical margins;
- paper edge location;
- fold position;
- conjugacy;
- watermark identity;
- chain-line spacing;
- full-sheet reconstruction.

### Mechanism

`OCR_GEOMETRY_AS_TRIAGE_NOT_CODICOLOGY`

---

## 14. Article-level refinement

A strong methodological paragraph is now available:

**The paper object is already transformed before the historian begins interpretation. A single letter may survive in several digital framings; a scan batch may aggregate unrelated sheets; a material view may enter OCR as nonsense text; a corrected printed offprint may be flattened into the same page sequence as a later reprint. Consequently, digital page order and OCR geometry cannot substitute for sheet reconstruction. They are themselves a later paper-to-image conversion state that redistributes what can be seen.**

This gives the article's digital coda a direct archival basis.

---

## 15. New mechanism codes

- `DIGITAL_CAPTURE_STATE_NONCOINCIDENCE`
- `LETTER_TO_REFERENCE_SURFACE_TRANSITION`
- `GRAPHIC_DENSIFICATION_FOR_CATALOGUE_USE`
- `MATERIAL_CAPTURE_CANDIDATE_IMAGE_ONLY`
- `PRECOMPOSED_CREDENTIAL_PLUS_ACCRETIVE_SIGNATURES`
- `ENDORSEMENT_SURFACE`
- `LOW_SEMANTIC_HIGH_MATERIAL_CAPTURE_STATE`
- `DUPLICATE_WITNESS_DIFFERENT_CAPTURE_GEOMETRY`
- `MATERIAL_VIEW_OR_FAINT_MARK_CANDIDATE`
- `SCAN_BATCH_MULTIPLE_OBJECT_AGGREGATION`
- `PRINTED_OFFPRINT_AS_AUTHORIAL_WORK_SURFACE`
- `PRINT_TO_MANUSCRIPT_HYBRID_STATE`
- `PARALLEL_PRINTED_WITNESS_STATES`
- `ANNOTATED_REPRINT_TO_REVISED_EDITION`
- `PRINTED_PAPER_VERSION_CHAIN`
- `SCARCITY_OF_ORIGINALS_AS_REPRINT_DRIVER`
- `SHEET_AS_COMPARATIVE_ARRAY`
- `SOURCE_GROUPING_BY_PLANAR_POSITION`
- `HISTORICAL_OBJECT_STATE_DIGITAL_CAPTURE_STATE_SEPARATION`
- `OCR_GEOMETRY_AS_TRIAGE_NOT_CODICOLOGY`

---

## 16. Immediate next tasks

1. Build a digital-capture manifest for the uploaded Linnean files: historical object ID, digital page, duplicate-state confidence, semantic/material capture type.
2. Directly inspect SP 514 final image-only page before labeling any watermark/fold feature.
3. Directly inspect LL-8 page 3 to determine whether the faint reading represents watermark, verso mark, ownership mark or OCR noise.
4. Directly inspect CR 48 second capture and determine whether it is verso/transmitted-light/unrelated adjacency.
5. Collate the two `Notice on Buddhist Symbols` printed states line by line.
6. Identify manuscript corrections on the `corrected autograph` witness and test whether they enter the later printed/reprint state.
7. Recover the two physical 143-symbol sheets and map number, source provenance and planar arrangement.
8. Add `capture_state` to all paper-surface datasets.
9. Never derive sheet dimensions from OCR coordinate width/height without a visible edge/scale witness.
10. Link corrected-print chains to the broader `INTERMEDIATE_STATE_FIXATION` argument.

## Bottom line

The paper-centred project now has a second-order material problem: the surviving paper objects are themselves mediated by photography, scanning, OCR and rebundling. The uploaded archive shows this directly. The same 1861 letter appears under different digital framings; some pages are material views rather than semantic text pages; and Hodgson's Buddhist publication survives as a corrected printed witness alongside another printed state and a later reprint explicitly justified by authorial annotation and revision. Paper therefore remains a working scientific technology after publication, while digitization becomes the latest conversion layer through which that paper must be reconstructed.