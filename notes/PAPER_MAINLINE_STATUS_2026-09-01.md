# Hodgson paper mainline status — 2026-09-01

Status: active paper-centred article mainline, superseding `PAPER_MAINLINE_STATUS_2026-08-31.md` for current work. Updated through Wave 35.

## Current question

How did paper move through manufacture, procurement, stock, work allocation, documentary versioning, provenance control and later custody, and how did those transitions affect what Hodgson and collaborators could translate, tabulate, revise, publish, bundle and reconstruct?

## Combined model

`paper-object history = production history × supply/stock history × work allocation × documentary versioning × provenance marking × custody architecture`.

Paper is one material field inside a larger version state rather than a symbolic proxy for local/colonial knowledge.

## Argument stack

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

Cambridge evidence suggests support tracks task/work setting and version state more strongly than subject or actor nationality. The simple `British writer -> imported paper / local writer -> local paper` hypothesis is falsified.

Mechanisms:

- `PAPER_ALLOCATION_AS_RESEARCH_INFRASTRUCTURE`
- `ACTOR_ETHNICITY_DOES_NOT_DETERMINE_SUPPORT`
- `WORKPLACE_STOCK_ACCESS_AS_CANDIDATE_VARIABLE`
- `TASK_ALLOCATION_MEDIATES_SUPPORT_SELECTION`.

### E. Documentary versioning

Explicit source families show:

- `SWITCH`;
- `CONTINUITY`;
- `BRANCHING`.

Working model:

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

Folio counts are not surface-area ratios; physical dimensions are required before quantitative compression claims.

Mechanism: `DERIVATIVE_COMPRESSION_AS_VERSIONING`.

### G. Provenance grammar on derivative surfaces

Hodgson's 1856 Peking-route paper describes the route papers as literal translations and says his inserted information was distinguished by brackets, with further additions in footnotes.

The derivative/publication surface can therefore distinguish:

`source-derived translation`

from

`Hodgson addition`

from

`explanatory note`.

Mechanism: `PROVENANCE_GRAMMAR_ON_DERIVATIVE_SURFACE`.

Physical comparison is required before asserting that surviving `vol.2/3` itself carries exactly the same graphical convention as print.

### H. Custody recombination and version-family archival design

Wave 34 showed the Jumla case: Hunter's reproduction of the August 1864 India Office transfer list says one large bundle contained the Jumla revenue statement `in Khas and in English`.

Wave 35 shows that this was systematic rather than exceptional.

The 1864 transfer repeatedly co-bundles multilingual/source/derivative states:

- Newari chronicles: source histories + Persian translation + Jit Mohan abstract + repetitions + two volumes of English translations + Persian addenda;
- Gurkhali chronicles: twelve source/history states followed explicitly by five volumes of `English translations of the above` made by Hodgson's office people;
- itineraries: one custody family described as `Various Itineraries, in Nagri, in Persian, and in English`;
- Newar institutions: original palm-leaf title deeds retained with materials translated into English or Persian;
- army/classification/judicial/customs materials: English volumes retained with Persian and Khas papers on the same subjects;
- Jumla revenue: Khas + English states in one large bundle.

The historical transfer ontology therefore preserved **version families**, not merely language classes or paper types.

Mechanisms:

- `VERSION_FAMILY_CO_BUNDLING_AS_ARCHIVAL_DESIGN`
- `CUSTODY_RECOMBINES_VERSION_STATES`
- `TRANSFER_CONTAINER_PRESERVES_DERIVATIVE_RELATIONS`
- `ARCHIVAL_PACKING_AS_RELATIONAL_METADATA`
- `MODERN_SHELFMARK_DISPERSION_OBSCURES_HISTORICAL_VERSION_FAMILY`.

### I. Denominator/source control

The conversion corpus distinguishes:

- Tier A explicit/declared edges;
- Tier B source-family/synthesis relations;
- Tier C similarity links.

`SUPPORT_UNSPECIFIED_IN_CATALOGUE` remains in the denominator. No publication percentage should be reported until coverage is demonstrably exhaustive.

## Strongest empirical scenes

1. Cowan British remanufacture failure.
2. Darjeeling transfer of skilled makers after material-transfer failure.
3. Serampore machine-interface mismatch.
4. Christie's lot 170 watermark plurality.
5. RAS 1841/1821 watermark stock-time evidence.
6. BL `Add Or 5338` mixed Nepalese/European support corpus.
7. Jumla branching: `vol.59/38 -> vol.8/1 + vol.102/21`.
8. Jumla 1864 custody recombination: Khas + English in one transfer bundle.
9. Peking branching: `vol.59/23 -> vol.2/3 + vol.102/19`.
10. Peking provenance grammar: literal translation separated from Hodgson additions by brackets/footnotes in the 1856 publication state.
11. 1864 chronicle co-bundling: source, Persian, abstract and English office-translation states retained within the same large custody family.
12. 1864 itinerary co-bundling: Nagri, Persian and English route states treated as one functional transfer class.

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
- `data/india_office_1864_version_family_manifest_v0_1.json`

## Active article/source notes

- `notes/PAPER_MATERIAL_REGIMES_ARGUMENT_V0_2.md`
- `notes/PAPER_ARGUMENT_SUPPORT_CONVERSION_V0_2.md`
- `notes/PAPER_ARGUMENT_MATERIAL_VERSIONING_AND_PROVENANCE_SURFACE_V0_1.md`
- `sources/WEB_RESEARCH_2026-09-01_WAVE34_BRANCHING_DERIVATIVE_STATE_RECONSTRUCTION.md`
- `sources/WEB_RESEARCH_2026-09-01_WAVE35_1864_VERSION_FAMILY_COBUNDLING.md`

Earlier versions remain in repo as source-control history.

## Immediate research order

1. Build a manifest-to-modern-shelfmark crosswalk for the 1864 version families, beginning with chronicles and itineraries.
2. Search for the English and Hindi content lists Hodgson says were already in the India Office librarian's hands in 1864.
3. Locate original India Office accession/packing records and test Hunter's transcription/container hierarchy.
4. Physically compare `vol.59/38 -> vol.8/1 + vol.102/21`; measure sheets and compare columns/information retention.
5. Identify the writer of `vol.102/21` and compare other Farsi revenue hands.
6. Compare `vol.59/23`, `vol.58/28`, `vol.2/3`, `vol.102/19` line-by-line; inspect `vol.2/3` for brackets/pencil layers and compare against 1856 print.
7. Continue Tier A denominator expansion without collapsing `summary`, `similar`, `related`, `translation` and `copy`.
8. Resolve Christie's 1997 lot 171 and BL old/new shelfmark conflict.
9. Run sheet-level support census on BL `Add Or 5338`.
10. Inspect MSS EUR HODGSON/6 paper sample against the 1831/32 manufacturing description.

## Guardrail

Do not recast the project as biography, disciplinary survey, `local versus colonial paper` symbolism, or personnel-nationality model. The active object is paper inside operational histories of manufacture, stock, work allocation, documentary versioning, provenance control and custody architecture.