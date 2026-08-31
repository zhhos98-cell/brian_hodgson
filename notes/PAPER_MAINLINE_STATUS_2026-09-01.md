# Hodgson paper mainline status — 2026-09-01

Status: active paper-centred article mainline, superseding `PAPER_MAINLINE_STATUS_2026-08-31.md` for current work. Updated through Wave 34.

## Current paper-centred question

How did paper move through manufacture, procurement, stock, allocation, documentary versioning and custody, and how did those material transitions affect what Hodgson and collaborators could write, translate, tabulate, revise, publish and later reconstruct?

## Current combined model

`paper-object history = production history × supply/stock history × work allocation × documentary versioning × provenance marking × custody reorganisation`.

Paper remains one field inside a larger material version state rather than a symbolic proxy for local/colonial knowledge.

## Current argument stack

### A. Production history

1833 Cowan trial:

`same broad material source + different process history -> different paper properties`.

Mechanism: `PROCESS_HISTORY_EMBODIED_IN_SHEET`.

### B. Interface-relative affordance

Darjeeling and Serampore:

`property value = material property × technical interface × intended operation`.

Mechanism: `AFFORDANCE_REVERSAL`.

### C. Mixed-stock ecology and stock time

Hodgson-associated objects document Whatman, Joynson, Moinier's Patent, Newey/Darnford, Britannia and dated imported stocks alongside Nepalese handmade paper. Watermark dates can substantially predate use dates.

Mechanisms:

- `HODGSON_OBJECT_LEVEL_IMPORTED_PAPER_PLURALITY`
- `MIXED_STOCK_OPERATIONAL_ECOLOGY`
- `PAPER_STOCK_RETENTION_OR_REUSE`.

### D. Work allocation

Cambridge evidence suggests support tracks task/work setting and version state more strongly than subject or actor nationality.

The simple `British writer -> imported paper / local writer -> local paper` hypothesis is falsified.

Mechanisms:

- `PAPER_ALLOCATION_AS_RESEARCH_INFRASTRUCTURE`
- `ACTOR_ETHNICITY_DOES_NOT_DETERMINE_SUPPORT`
- `WORKPLACE_STOCK_ACCESS_AS_CANDIDATE_VARIABLE`
- `TASK_ALLOCATION_MEDIATES_SUPPORT_SELECTION`.

### E. Documentary versioning

Explicit source families show three outcomes:

- `SWITCH`;
- `CONTINUITY`;
- `BRANCHING`.

The strongest current model is:

`documentary version state = information selection + language + writer + support + format + scale + correction state + completeness + intended next operation`.

Mechanisms:

- `SUPPORT_SWITCH_AT_KNOWLEDGE_CONVERSION`
- `SUPPORT_CONTINUITY_THROUGH_KNOWLEDGE_CONVERSION`
- `BRANCHED_DERIVATIVE_SUPPORT_STATES`
- `DERIVATIVE_STATE_SELECTS_SUPPORT_WITHIN_SHARED_INFORMATION_LINEAGE`.

### F. Documentary compression

Jumla:

`c.36 source folios -> c.8 English chart folios -> 2 Farsi table folios`.

Peking:

`8 Nepali source folios -> 3 English imported-paper folios -> 2 incomplete Urdu/Farsi folios`.

Folio counts are not yet surface-area ratios; dimensions must be measured before quantitative compression claims.

Mechanism: `DERIVATIVE_COMPRESSION_AS_VERSIONING`.

### G. Provenance grammar on the derivative surface

Hodgson's 1856 Peking-route publication states that the route papers were literal translations and that his own inserted information was distinguished by brackets, with further additions in footnotes.

The English derivative/publication surface can therefore visibly separate:

`source-derived translation`

from

`Hodgson addition`

from

`explanatory note`.

Mechanism: `PROVENANCE_GRAMMAR_ON_DERIVATIVE_SURFACE`.

Physical comparison is required before asserting that surviving `vol.2/3` itself carries exactly the same bracket convention as print.

### H. Custody recombination

Hunter's reproduction of the August 1864 India Office transfer list states that the sixth large bundle contained the Jumla revenue statement `in Khas and in English`.

Thus materially differentiated documentary versions could later be intentionally regrouped in one transfer unit.

Mechanisms:

- `CUSTODY_RECOMBINES_VERSION_STATES`
- `CONTAINER_RELATION_DIFFERS_FROM_VERSION_RELATION`
- `TRANSFER_BUNDLE_AS_VERSION_FAMILY_UNIT`.

This joins documentary versioning directly to the custody argument.

### I. Denominator/source control

The conversion corpus continues to distinguish:

- Tier A explicit/declared edges;
- Tier B source-family/synthesis relations;
- Tier C similarity links.

`SUPPORT_UNSPECIFIED_IN_CATALOGUE` remains in the denominator.

No publication percentage should be reported until inventory coverage is demonstrably exhaustive.

## Strongest empirical scenes now

1. Cowan British remanufacture failure.
2. Darjeeling transfer of skilled makers after material transfer failure.
3. Serampore machine-interface mismatch.
4. Christie's lot 170 watermark plurality.
5. RAS 1841/1821 watermark stock-time evidence.
6. BL `Add Or 5338` mixed Nepalese/European support corpus.
7. Jumla branching:
   - `vol.59/38` Nepali handmade source;
   - `vol.8/1` Campbell English machine-paper 48.5×38 cm chart;
   - `vol.102/21` Farsi Nepali-paper neat table.
8. Jumla 1864 custody recombination: Khas + English in one large transfer bundle.
9. Peking branching:
   - `vol.59/23` Nepali handmade source;
   - `vol.2/3` fair corrected English imported-paper route-book state;
   - `vol.102/19` poor incomplete Urdu/Farsi Nepali-paper state.
10. Peking publication provenance grammar: literal translation distinguished from Hodgson additions by brackets and footnotes.

## Active datasets

- `data/paper_material_regime_comparison_v0_1.json`
- `data/hodgson_imported_paper_object_marks_v0_1.json`
- `data/hodgson_paper_custody_branching_v0_1.json`
- `data/hodgson_paper_custody_recombination_v0_1.json`
- `data/cambridge_support_operation_census_v0_1.json`
- `data/support_conversion_pairs_v0_2.json`
- `data/support_conversion_denominator_v0_1.json`
- `data/support_actor_workplace_pilot_v0_1.json`
- `data/branching_derivative_state_reconstruction_v0_1.json`

## Active article/source notes

- `notes/PAPER_MATERIAL_REGIMES_ARGUMENT_V0_2.md`
- `notes/PAPER_ARGUMENT_SUPPORT_CONVERSION_V0_2.md`
- `notes/PAPER_ARGUMENT_MATERIAL_VERSIONING_AND_PROVENANCE_SURFACE_V0_1.md`
- `sources/WEB_RESEARCH_2026-09-01_WAVE34_BRANCHING_DERIVATIVE_STATE_RECONSTRUCTION.md`

Earlier versions remain in repo as source-control history.

## Immediate research order

1. Physically compare `vol.59/38 -> vol.8/1 + vol.102/21`; check column-by-column retention and measure sheet sizes.
2. Identify the writer of `vol.102/21` and compare with other Farsi revenue hands.
3. Compare `vol.59/23`, `vol.58/28`, `vol.2/3`, `vol.102/19` line-by-line and determine the local-source stemma.
4. Inspect `vol.2/3` for brackets, pencil layers and other provenance marking; compare against 1856 print.
5. Reconstruct the 1864 Jumla large-bundle structure from original India Office accession/packing records if surviving.
6. Search the 1864 manifest for additional cases where originals/Khas/Hindi and English translations are deliberately co-bundled.
7. Continue Tier A denominator expansion without collapsing `summary`, `similar`, `related`, `translation` and `copy` into one relation.
8. Resolve Christie's 1997 lot 171 and BL old/new shelfmark conflict.
9. Run sheet-level support census on BL `Add Or 5338`.
10. Inspect MSS EUR HODGSON/6 paper sample against the 1831/32 manufacturing description.

## Guardrail

Do not recast the project as a biography, disciplinary survey, `local versus colonial paper` symbolism, or personnel-nationality model. The active object is paper inside operational histories of manufacture, stock, work allocation, versioning, provenance control and custody.