# Hodgson paper census protocol v0.1

Date: 2026-08-31

Status: working protocol derived from the Wilson deep scan. This is deliberately narrower than the general provenance census. Its unit is the **paper object as material**, before asking what text/drawing/catalogue it carries.

## 1. Governing rule

Do not begin from `book`, `dossier`, `portfolio`, `archive file`, `European paper`, `Nepali paper`, or `Whatman` as self-explanatory categories.

Begin from the smallest observable paper unit and reconstruct upward:

**sheet / leaf / slip / fragment / wrapper / label / mount → attachment/assembly → working object → later archival unit**.

Where a unit cannot be physically separated without damage, record it analytically rather than physically.

## 2. Observation must be separated from interpretation

Every important paper claim should be representable at three levels:

### Observation
What is directly visible or measured?

Examples:
- watermark reads `J WHATMAN 1831`;
- chain lines visible at approximately X mm spacing;
- no chain lines visible under transmitted light;
- sheet is 412 × 267 mm;
- lower edge appears deckled;
- blue fibres/inclusions visible;
- black ink feathers into fibres;
- sheet is pasted to a secondary support.

### Technical interpretation
What manufacturing or use process best explains the observation?

Examples:
- mould-made laid paper;
- wove paper;
- possible machine-made wove stock;
- later mounting;
- paper cut from a larger sheet;
- local repair/reinforcement.

### Historical inference
What does this imply for Hodgson's practice?

Examples:
- same stock may connect two drawing sequences;
- paper was probably procured before the dated inscription;
- wrapper may be a later archival addition;
- material properties may have suited repeated folding/transport.

Never merge these three levels into one field.

## 3. Core paper-unit identity

Suggested ID prefix: `HOD-PAP-`.

Fields:

- `paper_unit_id`
- `parent_object_id`
- `current_repository`
- `current_shelfmark`
- `current_folio_leaf_page`
- `unit_type`
  - whole_sheet
  - leaf
  - bifolium
  - slip
  - label_ticket
  - wrapper
  - packet_surface
  - fragment
  - pasted_layer
  - mount
  - interleaf
  - drying_or_pressing_sheet
  - unknown
- `unit_state`
  - independent
  - bound
  - pasted
  - sewn
  - pinned
  - folded
  - nested
  - mounted
  - detached
  - fragmentary
- `recto_verso_identified`
- `analytical_parent_sheet_id_if_reconstructed`

## 4. Dimensions and edges

Record dimensions before assuming historical format names.

- `height_mm`
- `width_mm`
- `thickness_microns_if_measured`
- `weight_gsm_if_measured`
- `edge_top`
- `edge_bottom`
- `edge_left`
- `edge_right`

Edge vocabulary:
- deckle_possible
- cut_clean
- cut_irregular
- torn
- folded_break
- trimmed_by_binder
- obscured
- unknown

Also record:
- `fold_lines_count`
- `fold_line_orientation`
- `crease_pattern`
- `sewing_holes`
- `pin_holes`
- `paste_residue`
- `mounting_residue`
- `former_attachment_evidence`

## 5. Formation and manufacture

Fields:

- `manufacture_mode_observed_or_inferred`
  - handmade
  - machine_made
  - mould_made_uncertain
  - unknown
- `formation_type`
  - laid
  - wove
  - other
  - indeterminate
- `chain_lines_visible`
- `chain_line_spacing_mm`
- `laid_lines_visible`
- `laid_line_density_or_spacing`
- `wire_or_screen_irregularity`
- `deckle_edge_present`
- `formation_irregularity`
- `visible_fibre_inclusions`
- `fibre_description_visual_only`
- `fibre_identification_scientific`
- `fibre_identification_method`
- `fibre_identification_confidence`

### Technology warning

Mould-pair / twin-watermark reasoning appropriate to early mould-made paper must not be automatically transferred to nineteenth-century machine-watermark or dandy-roll production. First determine the likely manufacturing technology.

## 6. Watermark / countermark

Each mark should be a separately locatable observation.

- `watermark_present`
- `watermark_text_as_seen`
- `watermark_device_description`
- `watermark_date_as_seen`
- `countermark_present`
- `countermark_text_as_seen`
- `mark_complete_or_fragmentary`
- `mark_orientation_relative_to_inscription`
- `mark_position_x_y_or_quadrant`
- `mark_relation_to_chain_lines`
- `mark_dimensions_mm`
- `mark_image_available`
- `mark_image_mode`
  - transmitted_light
  - reflected_light
  - raking_light
  - beta_radiography
  - other
- `maker_mill_identification`
- `maker_mill_identification_source`
- `watermark_technology_interpretation`
- `same_mark_family_candidate_ids`
- `same_stock_candidate_ids`
- `watermark_claim_confidence`

### Absence rule

`No watermark visible in an ordinary reflected-light scan` does **not** equal `no watermark`.

Record imaging conditions whenever absence is used as evidence.

## 7. Colour, surface and body

Wilson's brown/white discussion is a warning that named paper categories can conceal a spectrum of material qualities. Therefore record the variables separately.

- `paper_colour_observed`
- `colour_description_source`
  - direct_physical
  - calibrated_image
  - uncalibrated_image
  - catalogue_description
- `surface_texture`
  - smooth
  - moderately_smooth
  - rough
  - fibrous
  - glazed_or_highly_finished
  - variable
  - unknown
- `surface_irregularities`
- `visible_pulp_or_plant_inclusions`
- `opacity_translucency`
- `thickness_uniformity`
- `sizing_finish_observation`
- `sizing_finish_interpretation`
- `absorbency_evidence`
- `stiffness_flexibility_observation`
- `wet_strength_evidence_if_historical`

Do not infer `quality` directly from colour, nationality, or maker.

## 8. Media interaction

Paper properties become historically meaningful through operations with ink, pencil, wash, paint, paste and moisture.

Record:

- `media_present`
- `ink_feathering`
- `ink_bleedthrough`
- `showthrough`
- `wash_cockling`
- `wash_tide_lines`
- `pencil_tooth_response`
- `surface_abrasion`
- `erasure_evidence`
- `scraping_evidence`
- `paste_penetration`
- `adhesive_failure`
- `media_transfer_to_adjacent_sheet`
- `water_staining`
- `mould_damage`
- `insect_damage`

These can become direct evidence for affordance/failure analysis.

## 9. Historical operation

A single paper unit may have multiple operations through time. Use event rows rather than one permanent function.

Controlled candidate operations:

- write
- copy
- draw
- paint_or_wash
- trace
- print
- label
- tabulate
- calculate
- fold
- cut
- paste
- mount
- sew
- bind
- wrap
- packet
- interleave
- dry
- press
- absorb
- protect
- waterproof_or_water_resist
- transport
- collate
- compare
- display
- archive
- rebind
- remount
- conserve
- digitize

For each operation record:

- `operation_event_id`
- `paper_unit_id`
- `operation`
- `date_or_range`
- `agent_if_known`
- `evidence`
- `state_before`
- `state_after`

## 10. Affordance test

Do not code affordance as a free-floating adjective.

For each claimed affordance use:

- `affordance_id`
- `paper_unit_or_stock_id`
- `operation`
- `observed_property`
- `enabled_action`
- `constrained_action`
- `failure_mode`
- `conditions`
- `alternative_support_comparator`
- `actor_response_or_workaround`
- `direct_evidence`
- `historical_inference`
- `confidence`

Working formula:

> In operation X, paper A was selected or reused because property P enabled action Y under conditions C; the same property created, prevented, or redistributed failure mode F relative to alternative B.

## 11. Candidate paper failure vocabulary

Use only when evidence supports it.

### Mechanical
- tear_at_fold
- edge_tearing
- cracking
- puncture_failure
- sewing_failure
- delamination
- paste_failure
- label_detachment
- mount_detachment
- dimensional_distortion
- excessive_bulk
- transport_crushing

### Wet / liquid interaction
- ink_feathering
- ink_bleed
- wash_cockling
- wash_migration
- water_transmission
- slow_drying
- excessive_absorption
- inadequate_absorption
- wet_strength_failure

### Surface / mark making
- too_rough_for_fine_line
- too_smooth_for_graphite
- abrasion
- flaking_media
- poor_paste_key
- transparency_problem
- opacity_problem

### Biological / ageing
- mould
- insect_damage
- brittleness
- discolouration
- embrittlement_at_fold

### Relational failure
- detached_label
- separated_wrapper
- lost_slip
- cut_watermark
- trimming_destroyed_evidence
- rebinding_destroyed_sequence
- mounting_obscured_verso

## 12. Composition/decomposition timeline

Prefer cumulative state history to an `original/later` binary.

Possible chain:

**formed sheet → cut/folded unit → inscribed working unit → assembled with other paper/object → detached/damaged → repaired/replaced → rebound/remounted → institutional description → digitized surrogate**.

Each transition can create or destroy evidence.

## 13. Imaging / surrogate protocol

Wilson's coda is directly relevant: digitization is itself a later mode of paper use that determines what can be studied.

For every digital surrogate used for paper analysis record:

- `surrogate_id`
- `repository`
- `image_source`
- `recto_or_verso`
- `full_sheet_or_crop`
- `scale_present`
- `colour_target_present`
- `reflected_light`
- `transmitted_light`
- `raking_light`
- `multispectral_or_other`
- `resolution_if_known`
- `watermark_legibility`
- `chain_line_legibility`
- `edge_legibility`
- `surface_texture_legibility`
- `verso_accessible`
- `binding_or_mount_obscures_area`
- `digital_processing_known`

### Surrogate rule

Treat `not visible digitally` as a statement about the surrogate until physical inspection or appropriate imaging establishes otherwise.

## 14. Historical category vs physical diagnosis

Keep labels such as these in a separate `historical_category_as_written` field:

- European paper
- English paper
- country paper
- Nepal paper / Nepali paper
- native paper
- Whatman paper
- drawing paper
- cartridge paper
- brown paper
- white paper
- fine paper
- common paper

Then separately record physical diagnosis.

A historical category may encode price, origin, prestige, use expectation, administrative vocabulary, or only a convenient label. It is evidence in its own right, but not a substitute for material description.

## 15. Priority research questions generated by Wilson

1. Do the same Whatman watermark/date/stock clusters recur across Hodgson zoological drawings, lists, correspondence and manuscript work?
2. Are there cases where named `Nepali` or `country` paper appears in scientific operations usually assumed to require European paper?
3. Can paper dimensions and cut/fold patterns reconstruct original working assemblages later split by repositories?
4. Do media failures cluster by paper stock, especially wash/pencil/ink work?
5. Can wrappers, labels and slips be shown to have had multiple operational lives before becoming archival paracontent?
6. Which archival/catalogue paper descriptions are based on direct material observation, and which merely reproduce inherited labels?
7. Which current digital images are physically inadequate for watermark, chain-line, fibre, edge or surface analysis and therefore require a quick-win request for transmitted-light or uncropped photography?

## 16. Immediate next implementation

Do not ingest thousands of rows yet.

Build a **10–20 unit pilot** deliberately mixing:

- known Whatman/wove sheets;
- known or probable Nepali handmade paper;
- zoological drawings;
- manuscript leaves;
- labels/slips/wrappers;
- at least one pasted/mounted/composite object;
- at least one case with transmitted-light imagery;
- at least one case where only ordinary digital imaging exists.

The pilot succeeds only if it can answer both:

1. `What physically is this paper?`
2. `What operation did those properties enable, constrain, or cause to fail?`
