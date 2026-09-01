# Web research 2026-09-02 — Wave 61
## Working sketch -> finished English-paper copy -> Nepalese-paper folder: support transformation in the 1843–46 architectural drawing system

Date: 2026-09-02

Status: paper-history mainline following Wave 60. This wave reconstructs a paper-based production chain across the Royal Asiatic Society and British Library Hodgson/Lawrence drawing corpora. It does not infer artistic authorship or exact copy direction beyond explicit catalogue cross-references.

## Executive result

British Library catalogue metadata makes a paper-production sequence directly visible.

The Lawrence Collection group `Add Or 5229–5255` consists of twenty-six Nepal drawings made mainly by Nepalese artists in 1843–46. The group-level record states:

- watercolour/body-colour;
- various sizes;
- the Nepal drawings are **normally on English paper with watermarks 1840–42**;
- the group is preserved **in a folder of Nepalese paper** inscribed `Pictures of Nepal`.

Source:
https://searcharchives.bl.uk/catalog/032-003279064

At least four individual British Library finished drawings are explicitly linked to `original pencil sketch` witnesses now in the Hodgson collection at the Royal Asiatic Society:

- RAS `022.058` -> BL `Add Or 5233`;
- RAS `022.055` -> BL `Add Or 5244`;
- RAS `022.054` -> BL `Add Or 5246`;
- RAS `022.052` -> BL `Add Or 5251`.

The material chain can therefore be written at high confidence as:

`working sketch on one paper surface`
-> `finished drawing on a new paper surface, normally English paper watermarked 1840–42`
-> `later custody inside a Nepalese-paper folder`.

The research object changes paper more than once.

Core mechanisms:

- `WORKING_SKETCH_IS_COPY_INFRASTRUCTURE`
- `FINISHING_CAN_TRIGGER_SUPPORT_SUBSTITUTION`
- `PAPER_SURFACE_BRANCHING_BY_WORK_STAGE`
- `ENGLISH_DRAWING_SUPPORT_INSIDE_NEPALese_PAPER_CONTAINER`
- `PAPER_FUNCTION_CHANGES_FROM_IMAGE_SUPPORT_TO_CONTAINER`
- `ONE_VISUAL_OBJECT_CAN_HAVE_MULTIPLE_PAPER_STATES`.

---

## 1. Group-level BL evidence: normally English paper, 1840–42

British Library `Add Or 5229–5255`:

> Twenty-six drawings of the people, monuments and landscape of Nepal.

The catalogue states that the Nepal drawings are normally on **English paper with watermarks 1840–42**.

This is unusually strong because it supplies three paper fields at collection level:

1. broad manufacture/provenance class: English paper;
2. watermark date range: 1840–42;
3. operation: finished watercolour/body-colour drawing corpus.

The group belongs to the Lawrence Collection. Henry Lawrence was Resident in Kathmandu 1843–46.

The watermark/use interval is therefore short at collection scale:

`1840–42 paper -> 1843–46 drawing use`.

This is a different stock-time profile from the RAS Hodgson architecture corpus, which includes paper catalogued with watermark dates 1821, 1837 and 1841 in c.1844 use.

Potential interpretation:

`Lawrence finished-drawing programme may have drawn more heavily on relatively recent English drawing stock than the broader Hodgson/RAS working corpus`.

Keep this as a candidate until item-level watermark census is complete.

Mechanisms:

- `WORK_STAGE_CAN_SAMPLE_A_DIFFERENT_STOCK_POOL`
- `COLLECTION_LEVEL_WATERMARK_RANGE_AS_STOCK_PROFILE_CANDIDATE`.

---

## 2. Four direct sketch -> finished-drawing links

### Pair A: Residency

RAS `022.058`:

- *British Ambassador's house, Kathmandu in the Gothic style*;
- pen-and-ink sketch;
- paper `29.3 × 44.8 cm`;
- c.1844.

Source:
https://royalasiaticcollections.org/british-ambassadors-house-kathmandu-in-the-gothic-style/

BL `Add Or 5233`:

- finished wash/watercolour/body-colour drawing of the British Residency;
- BL explicitly states that the original pencil sketch is RAS `022-058`;
- image/composition dimension `268 × 445 mm within a narrow black frame`.

Source:
https://searcharchives.bl.uk/catalog/040-003279069

### Pair B: Kathmandu Durbar / Kala-Bhairava

RAS `022.055`:

- *The Durbar, Kathmandu*;
- pen-and-ink sketch;
- paper `26.1 × 43.4 cm`;
- c.1844.

Source:
https://royalasiaticcollections.org/the-durbar-kathmandu/

BL `Add Or 5244`:

- pencil, wash and watercolour finished drawing;
- BL explicitly links original pencil sketch to RAS `022-055`;
- composition `240 × 420 mm within painted green frame`.

Source:
https://searcharchives.bl.uk/catalog/040-003279076

### Pair C: Krishna temple

RAS `022.054`:

- *Temple of Krishna, Patan*;
- pen-and-ink sketch;
- paper `31 × 41.5 cm`;
- RAS itself calls it a preliminary sketch for another finished drawing, `022.027`.

Source:
https://royalasiaticcollections.org/temple-of-krishna-patan/

BL `Add Or 5246`:

- pencil, wash and watercolour;
- BL explicitly says its original pencil sketch is RAS `022-054`;
- composition `262 × 420 mm within black frame`.

Source:
https://searcharchives.bl.uk/catalog/040-003279078

The same working sketch therefore participates in at least two finished-drawing relations in current catalogues:

`RAS 022.054 -> RAS 022.027`

and

`RAS 022.054 -> BL Add Or 5246`.

This should not yet be forced into a precise chronological copy stemma. But it already shows that one sketch surface could function as a **reusable copying reference**, rather than a disposable preparatory leaf tied to one unique final object.

Mechanism:

`ONE_WORKING_SKETCH_CAN_FEED_MULTIPLE_FINISHED_BRANCHES_CANDIDATE`.

### Pair D: Matsyendranath / Avalokitesvara

RAS `022.052`:

- *Temple of Avalokitesvara, Patan*;
- pen-and-ink sketch;
- paper `27.6 × 46 cm`;
- c.1844.

Source:
https://royalasiaticcollections.org/temple-of-avalokitesvara-patan/

BL `Add Or 5251`:

- pencil, wash and watercolour;
- BL explicitly links original pencil sketch to RAS `022-052`;
- composition `240 × 394 mm within black frame`.

Source:
https://searcharchives.bl.uk/catalog/040-003279083

---

## 3. Measurement source control: BL composition dimensions are not paper dimensions

Wave 60 reconstructs parent-sheet candidates from actual paper dimensions in the RAS catalogue.

The BL Lawrence item records use a different measurement convention. Examples are phrased:

- `262 by 420 mm within black frame`;
- `240 by 420 mm within painted green frame`;
- `240 by 394 mm within black frame`.

These measurements describe the drawn/framed field, not securely the full paper support.

Therefore do **not** compare:

`RAS paper size`

against

`BL within-frame dimensions`

as if both were sheet dimensions.

New census rule:

`DIMENSION_SEMANTIC_TYPE_MUST_BE_CODED`.

Required types:

- `PAPER/SHEET_DIMENSION`;
- `DRAWN_OR_IMAGE_FIELD_DIMENSION`;
- `MOUNT_DIMENSION`;
- `FRAME_DIMENSION`;
- `BOUND_LEAF_DIMENSION`;
- `UNKNOWN_CATALOGUE_DIMENSION`.

Mechanisms:

- `CATALOGUE_DIMENSIONS_ARE_OPERATIONALLY_TYPED`
- `MEASUREMENT_TYPE_MISMATCH_CAN_CREATE_FALSE_FORMAT_STEMMA`.

This is essential before any cross-institution format comparison.

---

## 4. The production chain implies support substitution at the finishing stage

The RAS preliminary/working witnesses are pen-and-ink sketches with directly stated paper dimensions.

The BL descendants are finished pencil/wash/watercolour works inside a corpus catalogued as normally on English paper watermarked 1840–42.

Thus the copy relation generally crosses both:

- medium;
- paper surface.

Safe material model:

`working sketch`
-> `visual transfer/copying`
-> `new finished drawing support`.

The paper does not simply carry an image through successive elaboration. A visual configuration is transferred from one support onto another support selected for a different operation.

This is materially different from revising the same sheet.

Mechanisms:

- `COPYING_TRANSFERS_INFORMATION_ACROSS_SUPPORTS`
- `WORK_STAGE_CAN_TRIGGER_NEW_PAPER_ALLOCATION`
- `FINISHED_DRAWING_IS_A_DERIVATIVE_PAPER_OBJECT_NOT_MERELY_LATER_STATE_OF_SAME_SHEET`.

---

## 5. English paper is normal, not absolute, within the Lawrence finished corpus

The BL group-level statement says Nepal drawings are **normally** on English paper.

`Add Or 5254` supplies a direct exception:

- outline sketch of a Buddhist stupa;
- wash and watercolour;
- explicitly **on Nepalese paper**;
- `352 × 363 mm within black ruled frames`.

Source:
https://searcharchives.bl.uk/catalog/040-003279086

This matters because it prevents a rigid allocation rule:

`finished Lawrence drawing = English paper`.

The actual state is:

`English paper dominant / normal in corpus`
+
`Nepalese-paper exception directly present`.

Mechanisms:

- `PAPER_ALLOCATION_IS_PROBABILISTIC_NOT_DETERMINISTIC`
- `LOCAL_PAPER_CAN_ENTER FINISHED_VISUAL_WORKFLOW`.

The next physical question is whether the Nepalese-paper exception differs in technique, function, original source, or stage from the English-paper majority.

---

## 6. A second Nepalese-paper role: folder/container

The `Add Or 5229–5255` group is held in a **folder of Nepalese paper** inscribed `Pictures of Nepal`.

The provenance note records that Mrs H. L. Hart found the pictures among her papers in January 1907 and gave them to Sir H. W. Lawrence; the catalogue does not securely date the Nepalese-paper folder itself.

Therefore the folder must be treated as:

`NEPALESE_PAPER_CONTAINER_DIRECT; DATE/FUNCTION_ORIGIN_UNRESOLVED`.

Do not assume it was the original 1840s transport portfolio.

Still, the extant object presents a nested support structure:

`finished drawings normally on English paper`
inside
`Nepalese-paper folder`.

Paper origin has changed function:

- English paper: image-bearing finished support;
- Nepalese paper: enclosing/container support;
- Nepalese paper also occasionally: image-bearing support (Add Or 5254).

This is a stronger model than `European paper versus Nepalese paper` because the same material class can occupy different operational roles.

Mechanisms:

- `PAPER_ORIGIN_DOES_NOT_FIX_FUNCTION`
- `LOCAL_PAPER_AS_CONTAINER`
- `NESTED_PAPER_OBJECT`
- `SUPPORT_FUNCTION_CAN_CHANGE_ACROSS_CUSTODY`.

---

## 7. Relation to Wave 60 format standardization

Wave 60 showed:

`heterogeneous parent stock -> standardized working format`.

Wave 61 adds a second transformation:

`working-format sketch -> finished copy on newly allocated paper`.

Combined visual-production sequence:

`stock sheet`
-> `cut/formatted sketch support`
-> `working drawing`
-> `visual transfer`
-> `new finished-paper support`
-> `mount/frame`
-> `paper folder/container`
-> `later institutional custody`.

Thus the history of one image family can involve several paper objects with distinct tasks.

The key unit is no longer `the drawing` but the **paper-mediated production family**.

Mechanism:

`VISUAL_WORK_HAS_A_MULTI_SUPPORT_STEMMA`.

This term is useful only materially: each branch must correspond to a distinct physical support.

---

## 8. New article proposition

**In Hodgson's visual research, paper was allocated by stage as well as by subject. Working sketches could survive as reusable copying references while finished images were recopied onto newly allocated sheets, often recent English paper in the Lawrence programme. The resulting drawings then acquired further paper layers through mounts, frames and a Nepalese-paper folder. The same visual object therefore existed not as one progressively perfected sheet but as a family of supports, each made for a different operation.**

This gives a paper-history route into work organization without leaving material evidence.

---

## Source-control rules

1. BL `within black frame` dimensions are not paper dimensions unless the record explicitly says so.
2. Do not use BL composition dimensions to infer Royal/Medium/Demy parent sheets.
3. `Normally on English paper` permits exceptions; Add Or 5254 is a direct Nepalese-paper exception.
4. Do not date the Nepalese-paper folder to the 1840s without physical/provenance evidence.
5. Keep `original pencil sketch` catalogue links as direct relation evidence, but do not infer exact copying personnel or chronology beyond the catalogue.
6. RAS 022.054's links to both RAS 022.027 and BL Add Or 5246 suggest reusable sketch infrastructure; exact branch sequence remains unresolved.
7. Treat paper support change and medium change as separate fields.
8. Distinguish working-support dimensions, image-field dimensions, mount dimensions and frame dimensions.

---

## Immediate next actions

1. Inspect physical BL `Add Or 5229–5255` to record **full sheet dimensions**, edge state and exact watermark/countermark on each item.
2. Build item-level table for BL watermark date `1840–42`, rather than relying only on group-level statement.
3. Compare RAS sketch paper formation/marks against BL finished-paper marks for the four explicit pairs.
4. Determine whether RAS 022.054 -> RAS 022.027 and RAS 022.054 -> BL 5246 represent two finished copies from one sketch or catalogue conflation.
5. Inspect Add Or 5254 Nepalese paper and compare fibre/formation with Add Or 5332–5334 and Cambridge Nepal-paper samples.
6. Inspect the `Pictures of Nepal` Nepalese-paper folder: dimensions, fibre, folds, inscriptions, wear, sewing/fastening and relation to enclosed sheets.
7. Add `dimension_semantic_type`, `paper_function`, `source_support_ref`, `derivative_support_ref`, and `container_support_ref` to paper census schema.

---

## Bottom line

The 1840s architectural drawing programme contains a recoverable paper workflow. Original pencil/ink sketches now at the RAS were used as sources for finished drawings in the Lawrence Collection; those finished Nepal drawings were normally made on English paper watermarked 1840–42; and the surviving group is housed in a Nepalese-paper folder. The same visual knowledge therefore passed through multiple supports rather than simply accumulating on one sheet. Paper history here is a history of **support substitution, copying, and nested paper functions**.