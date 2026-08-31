# Hodgson paper mainline status — Wave 41

Date: 2026-09-01

Status: current active paper-centred mainline, superseding earlier status notes for ongoing work while preserving them as version history.

## Current object

The article now follows paper across six linked operations:

`manufacture -> stock/allocation -> documentary versioning -> provenance/addressing -> custody packaging -> archival reclassification/reconstruction`.

Paper is not treated as a symbolic local/colonial binary. It is both a physical support and an addressable relational surface.

## Current combined model

`paper-object history = production history × stock history × work allocation × documentary version state × historical custody identity × modern archival identity`.

The newest requirement is to keep four identities separate:

1. support identity;
2. documentary version identity;
3. historical container/shipment identity;
4. modern shelfmark identity.

## Strongest argument stack

### 1. Process history embodied in sheet

1833 Cowan trial: same broad Himalayan raw material, different manufacturing sequence, different paper properties.

Mechanism: `PROCESS_HISTORY_EMBODIED_IN_SHEET`.

### 2. Affordance reversal at technical interface

Darjeeling/Serampore show that toughness/fibre behaviour changes value across hand-sheet and machine-web operations.

Mechanism: `AFFORDANCE_REVERSAL`.

### 3. Mixed-stock ecology and stock time

Hodgson-associated objects include multiple imported watermark families alongside Nepalese handmade paper; watermark date can substantially predate use date.

Mechanisms:

- `MIXED_STOCK_OPERATIONAL_ECOLOGY`
- `PAPER_STOCK_RETENTION_OR_REUSE`
- `WHATMAN_PRESENT_BUT_NOT_DEFAULT`.

### 4. Paper allocation as work infrastructure

Support correlates with operation/work state more strongly than with subject or actor nationality. The British/local-writer binary is falsified.

Mechanism: `PAPER_ALLOCATION_AS_RESEARCH_INFRASTRUCTURE`.

### 5. Documentary conversion as material versioning

Explicit source families show support switch, continuity and branching.

Highest-value quasi-experiments:

- Jumla: `vol.59/38 -> vol.8/1 + vol.102/21`;
- Peking: `vol.59/23 -> vol.2/3 + vol.102/19`.

Mechanisms:

- `BRANCHED_DERIVATIVE_SUPPORT_STATES`
- `DERIVATIVE_COMPRESSION_AS_VERSIONING`
- `PROVENANCE_GRAMMAR_ON_DERIVATIVE_SURFACE`.

### 6. Version-family custody

The 1864 transfer repeatedly co-bundles source, translation, abstract and multilingual derivatives.

Mechanisms:

- `VERSION_FAMILY_CO_BUNDLING_AS_ARCHIVAL_DESIGN`
- `TRANSFER_CONTAINER_PRESERVES_DERIVATIVE_RELATIONS`.

### 7. 1921 physical reclassification

Cambridge collection history states that papers were bound in 1921 into 95 volumes, with grouping partly by physical dimensions. Related items, including originals and translations, could therefore be separated because they were written on different sizes of paper.

Mechanisms:

- `PAPER_DIMENSION_DRIVES_ARCHIVAL_REBINDING`
- `ARCHIVAL_REBINDING_BREAKS_VERSION_FAMILIES`.

### 8. Surviving old container metadata enables reverse reconstruction

Wave 40 supplies the first direct historical-container -> modern-shelfmark edge:

`original shipment sack No.8`
-> contents/control leaf now `vol.58/18 f.65`
AND
-> a Limbu member manuscript explicitly marked sack 8 now `vol.85/4`.

This proves that an old shipment family crosses modern volume boundaries.

Additional surviving control surfaces:

- `vol.55/20 f.129v`: Box No.3 of original shipment;
- `vol.94/7 ff.40-44`: original Kathmandu bundle numbers/categories;
- `vol.58/14 f.59`: contents of papers sent from Kathmandu to India since 1821;
- vol.4 and vol.5 machine-paper notebooks: original shipment/sack numbers retained on covers.

Mechanisms:

- `OLD_CONTAINER_METADATA_SURVIVES_REBINDING`
- `RELATION_RECONSTRUCTION_FROM_MATERIAL_REMAINDERS`
- `PAPER_IDENTIFIER_AS_RELATIONAL_CHECKSUM`.

### 9. Historical shipment identifiers cross support and language

Wave 41 adds a decisive case:

`vol.1/8`
= Campbell English second copy
+ imported paper
+ Nepali title layer
+ original box and sack number in Nepali on the final page.

Likewise vol.4 and vol.5 English machine-paper notebooks preserve Nepali shipment metadata.

Therefore:

`historical custody identity != support identity != language identity != version identity`.

Mechanisms:

- `SHIPMENT_IDENTIFIER_CROSSES_SUPPORT_AND_LANGUAGE`
- `CONTAINER_IDENTITY_ORTHOGONAL_TO_SUPPORT_IDENTITY`
- `MULTIAXIAL_DOCUMENT_IDENTITY`
- `PAPER_AS_ADDRESSABLE_RELATIONAL_SURFACE`.

## Archive-list version chain

RAS evidence now establishes repeated custody-list states:

`1837 five boxes (BHH/11/1)`
-> `1837 MSS/version list (BHH/11/2)`
-> `1842 Trunk No.1 bastas/bundles (BHH/11/3)`
-> `1844 repacking onto Hardwicke`
-> `1852 Darjeeling trunks (BHH/11/10)`
-> `1855 Trunk No.2 papers (BHH/11/12)`
-> `1858 private store list`
-> `1864 donation list (BHH/11/14)`
-> `1864 annotated printed manifest (BHH/19/5)`
-> `1921 dimension-based rebinding`
-> `modern relational catalogue`.

The archival control object is itself versioned.

Mechanism: `ARCHIVE_ITSELF_HAS_VERSION_HISTORY`.

## Active datasets

- `data/paper_material_regime_comparison_v0_1.json`
- `data/hodgson_imported_paper_object_marks_v0_1.json`
- `data/cambridge_support_operation_census_v0_1.json`
- `data/support_conversion_pairs_v0_2.json`
- `data/support_conversion_denominator_v0_1.json`
- `data/support_actor_workplace_pilot_v0_1.json`
- `data/branching_derivative_state_reconstruction_v0_1.json`
- `data/india_office_1864_version_family_manifest_v0_1.json`
- `data/hodgson_paper_custody_recombination_v0_1.json`
- `data/india_office_transfer_control_surfaces_v0_1.json`
- `data/historical_container_metadata_crosswalk_v0_1.json`
- `data/pre1921_identifier_surface_census_v0_1.json`.

## Active research waves

- Wave 34: branching derivative-state reconstruction;
- Wave 35: 1864 version-family co-bundling;
- Wave 36: 1921 dimension-based rebinding and modern dispersion;
- Wave 37: inventory-version prehistory;
- Wave 38: India Office transfer control surfaces;
- Wave 39: surviving pre-1921 container metadata;
- Wave 40: old-container to modern-shelfmark crosswalk;
- Wave 41: identifier surfaces across supports.

## Immediate research order

1. Recover actual box/sack numerals on `vol.1/8 f.290b`.
2. Recover original shipment numbers from all four vol.4 notebook covers.
3. Recover original shipment/sack numbers from the six vol.5 notebook covers.
4. Transcribe the sack-8 contents list `vol.58 f.65` and enumerate all members.
5. Transcribe `vol.94 ff.40-44` bundle numbers/categories and search matching modern objects.
6. Transcribe `vol.55 f.129v` Box 3 and compare its contents with RAS `BHH/11/1` Box 3 before asserting continuity.
7. Build a bipartite graph: historical containers ↔ modern shelfmarks. Edge admission requires explicit identifier or direct content-list match.
8. Compare RAS `BHH/11/14` 1858 store state with `BHH/19/5` 1864 printed state to determine when version-family co-bundling emerged.
9. Continue denominator-controlled support-conversion census.
10. Return to physical paper inspection targets: MSS EUR HODGSON/6 sample, BL Add Or 5338, RAS 022 watermark series.

## Article-facing formulation

The strongest current archival claim is:

**Paper participated twice in the destruction and recovery of documentary relations. Sheet dimensions became an institutional criterion that helped separate historically related versions during twentieth-century rebinding; inscriptions on those same sheets—box numbers, sack numbers, shipment numbers, bundle covers and content lists—survived the rearrangement and now permit those older relations to be reconstructed.**

The paper archive is therefore neither a passive substrate nor a stable container of information. It is a material system in which physical properties, documentary versions and archival addresses remain partially independent and can be recombined across time.

## Guardrail

Do not reduce the argument to local paper versus imported paper, local writers versus British writers, or historical container versus modern catalogue as simple oppositions. The article tracks transformations among materially distinct but relationally connected states.