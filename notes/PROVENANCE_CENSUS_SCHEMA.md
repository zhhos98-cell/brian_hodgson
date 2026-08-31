# Provenance census schema — Hodgson knowledge objects

Date created: 2026-08-31

Status: working schema. Designed from the evidence accumulated through public-web Waves 1–15, the Wilson paper-method notes, Fort William count reconstruction, and Mitra's 1882 catalogue-error diagnosis. It should be implemented later as CSV/JSON/SQLite only after enough real rows have tested the fields.

## 1. Purpose

The census is not a conventional object catalogue. It is designed to reconstruct **relations and transformations through time**.

The basic analytical problem is:

> How did an object, representation, identifier, container and institutional description remain linked — or cease to remain linked — as material moved between people, places, media and catalogues?

The schema therefore separates five layers that catalogues often collapse:

1. **knowledge object** — specimen, drawing, manuscript, list, note, table, photograph, etc.;
2. **identifier/representation** — number, name, label, title slip, drawing, description, catalogue entry;
3. **container/assemblage** — wrapper, bundle, basta, portfolio, box, crate, trunk, roll, packet;
4. **event/custody** — copy, pack, dispatch, receive, unpack, sort, compare, relabel, catalogue, redistribute, replace;
5. **claim/evidence** — what source lets us assert the relation, with what confidence.

A row may represent either one object-state or one event. Do not force every archival reference into a single `object` row.

---

## 2. Stable entity identifiers

Use repo-local identifiers so later records can be joined even when institutional shelfmarks change.

### `entity_id`
Format examples:

- `HOD-OBJ-000001` — object or document unit;
- `HOD-CNT-000001` — physical container/assemblage;
- `HOD-ID-000001` — identifier/label/name instance;
- `HOD-EVT-000001` — event;
- `HOD-PER-000001` — person/agent if needed;
- `HOD-INS-000001` — institution if needed;
- `HOD-SRC-000001` — source witness.

Do not derive the repo ID from a current catalogue number. Institutional shelfmarks belong in separate fields because they can change.

### `entity_type`
Controlled values:

- `object`
- `container`
- `identifier`
- `event`
- `person`
- `institution`
- `source`

---

## 3. Object fields

### Identity

- `entity_id`
- `object_class`
  - `zoological_specimen`
  - `osteological_specimen`
  - `drawing`
  - `painting`
  - `photograph`
  - `manuscript_coding_unit`
  - `manuscript_leaf`
  - `manuscript_copy`
  - `printed_text`
  - `letter`
  - `list`
  - `catalogue`
  - `table`
  - `map_route_survey`
  - `administrative_document`
  - `label_ticket_slip`
  - `paper_sample`
  - `wrapper_packet_surface`
  - `other`
- `short_description`
- `historical_name_as_written`
- `normalized_name`
- `taxon_or_text_title_if_applicable`
- `language_script`
- `creator_maker_copyist_artist`
- `estimated_date_from`
- `estimated_date_to`
- `date_basis`
- `current_repository`
- `current_shelfmark_accession`
- `previous_shelfmark_accession`

### Material support

- `support_material`
- `fibre_if_known`
- `handmade_machine_unknown`
- `laid_wove_other`
- `paper_colour`
- `surface_sizing_finish`
- `thickness_weight_if_known`
- `sheet_height_mm`
- `sheet_width_mm`
- `folded_format`
- `watermark_text_device`
- `watermark_date`
- `countermark`
- `watermark_orientation_position`
- `chain_line_spacing`
- `media`
  - ink / pencil / wash / paint / print / mixed
- `composite_construction`
  - pasted / double sheet / mounted / bound / sewn / attached slip / etc.
- `condition_current`
- `condition_historical`

### Affordance / function

- `physical_operation`
  - `write`
  - `draw`
  - `copy`
  - `label`
  - `wrap`
  - `interleave`
  - `dry`
  - `fold`
  - `bind`
  - `paste`
  - `bundle`
  - `protect`
  - `transport`
  - `collate`
  - `compare`
  - `display`
  - `archive`
- `inferred_affordance`
  - strength / flexibility / absorbency / drying / durability / surface suitability / portability / large format / low cost / etc.
- `affordance_evidence`
- `alternative_support_comparator`
- `affordance_confidence`

Do not infer an epistemic hierarchy directly from `European`, `Nepali`, `Whatman`, `machine-made`, `handmade`, etc.

---

## 4. Identifier fields

Identifiers are first-class entities because they can survive when objects move, detach, collide, or be replaced.

- `identifier_id`
- `identifier_type`
  - `specimen_number`
  - `drawing_number`
  - `box_number`
  - `bundle_number`
  - `folio_number`
  - `accession_number`
  - `catalogue_number`
  - `taxonomic_name`
  - `vernacular_name`
  - `sanskrit_title`
  - `wrapper_title`
  - `european_form_name`
  - `label_text`
  - `shelfmark`
  - `other`
- `identifier_value_as_written`
- `normalized_value`
- `language_script`
- `attached_to_entity_id`
- `physical_attachment_mode`
  - directly written / attached label / wrapper / separate list / catalogue / later pencil / etc.
- `assigned_by`
- `assigned_date`
- `first_attested_source`
- `last_attested_source`
- `status`
  - `current`
  - `superseded`
  - `incorrect`
  - `ambiguous`
  - `collision`
  - `detached`
  - `missing`
- `conflicts_with_identifier_id`
- `correction_event_id`

### Explicit warning

A number is not assumed to be a stable unique identifier. Wave 11 already shows:

- correct numbers paired with copied names that Gray called wrong;
- two differing kinds apparently carrying the same number;
- material unavailable for comparison because it remained unpacked or elsewhere.

Record `number collision` and `number/name divergence` directly rather than smoothing them out.

---

## 5. Container / assemblage fields

- `container_id`
- `container_type`
  - `wrapper`
  - `packet`
  - `bundle`
  - `basta`
  - `portfolio`
  - `roll`
  - `box`
  - `waterproof_box`
  - `crate`
  - `trunk`
  - `case`
  - `volume_binding`
  - `other`
- `historical_container_name`
- `container_number_label`
- `material`
- `dimensions`
- `waterproofing_protection`
- `closure_binding`
- `contents_list_present`
- `contents_list_entity_id`
- `inscription_on_container`
- `container_date_as_written`
- `container_date_interpretation`
  - production / packing / repacking / storage / dispatch / receipt / later archive / unknown
- `current_container_state`
- `nested_in_container_id`
- `contains_entity_ids`
- `relations_intended_to_preserve`
- `physical_preservation_effect`
- `relational_preservation_effect`
- `institutional_availability_effect`

### Container chronology rule

**Container date ≠ object date by default.**

Every date written on a case, wrapper, packet or box must be coded with an interpretation and independent chronological evidence where possible. The Foucher/Institut 1866 problem is the model warning case.

---

## 6. Event table

Each event should be a separate record whenever evidence permits.

### Core fields

- `event_id`
- `event_type`
- `date_from`
- `date_to`
- `date_precision`
- `place_from`
- `place_to`
- `agent_from`
- `agent_to`
- `institution_from`
- `institution_to`
- `object_entity_ids`
- `container_entity_ids`
- `identifier_entity_ids`
- `source_entity_ids`
- `event_description`
- `resulting_state`
- `failure_or_exception`
- `confidence`

### Controlled `event_type` vocabulary

#### Production / conversion
- `collect`
- `observe`
- `prepare_specimen`
- `draw`
- `copy_manuscript`
- `translate`
- `extract`
- `annotate`
- `tabulate`
- `make_label`
- `assign_number`
- `collate`
- `photograph`

#### Packaging / transport
- `wrap`
- `bundle`
- `pack`
- `repack`
- `interleave`
- `waterproof`
- `dispatch`
- `transship`
- `route_change`
- `transport_failure`
- `partial_loss_in_transit`

#### Custody / institutional handling
- `receive`
- `safe_arrival_acknowledged`
- `unpack`
- `delayed_unpacking`
- `inventory_reconciliation`
- `sort`
- `compare`
- `condition_assessment`
- `preserve_conserve`
- `rebind`
- `mount`
- `relabel`
- `remove_label`
- `recover_missing_object`

#### Identity / error control
- `exception_detected`
- `identifier_collision`
- `identifier_name_divergence`
- `metadata_correction`
- `reidentify`
- `synonymize`
- `missing_detected`
- `defect_detected`
- `replacement_requested`
- `replacement_sent`
- `supplement_added`

#### Distribution / publication / archive
- `duplicate_selected`
- `duplicate_distributed`
- `catalogue_compiled`
- `catalogue_printed`
- `catalogue_distributed`
- `catalogue_republished`
- `catalogue_annotated`
- `donate`
- `redistribute`
- `archive_reorganize`
- `shelfmark_change`

---

## 7. Receipt and reconciliation fields

Wave 11 makes this distinction mandatory.

For any shipment, record separately:

- `dispatch_event_id`
- `safe_arrival_event_id`
- `receipt_actor`
- `receipt_container_count_expected`
- `receipt_container_count_reported`
- `item_count_expected`
- `item_count_reported`
- `inventory_reconciliation_event_id`
- `exceptions_detected`
- `items_missing`
- `items_partial`
- `items_defective`
- `items_elsewhere_temporarily`
- `items_unpacked_status`
- `identifier_errors_detected`
- `condition_errors_detected`
- `replacement_event_id`

### Interpretive rule

`safe arrival` confirms a custody transition only to the granularity actually stated in the source. If a letter says three cases arrived, code three cases as arrived. Do not infer that every manuscript inside was present, correctly identified or undamaged.

---

## 8. Distribution / duplicate-set fields

Because Hodgson's zoological corpus was deliberately distributed, duplicate sets need explicit representation.

- `distribution_event_id`
- `source_collection`
- `destination_institution`
- `set_number_if_any`
- `specimen_count`
- `drawing_count`
- `osteology_count`
- `catalogue_or_list_accompanied`
- `catalogue_version_id`
- `list_version_id`
- `original_identifiers_retained`
- `new_local_identifiers_assigned`
- `later_relabelled`
- `later_redistributed`
- `current_survival_known`

### Key question

Was the metadata copy distributed with the physical duplicate set, and did later institutional practice keep the two synchronized?

This should become a major comparative field across British Museum, India House, Leiden, Paris and other recipients.

---

## 9. Catalogue / version fields

Catalogues are treated as versioned operational objects.

- `catalogue_entity_id`
- `title`
- `compiler_author_as_printed`
- `compiler_author_reconstructed`
- `imprint_date`
- `actual_availability_date`
- `source_list_version`
- `specimen_set_version`
- `drawing_set_version`
- `corrections_from_previous_version`
- `synonymy_changes`
- `identifier_changes`
- `taxonomic_allocation_changes`
- `marginal_annotations`
- `recipient_copies_known`
- `distribution_with_duplicates`
- `later_republication`
- `known_errors`
- `known_disagreements`

### Version graph to build

At minimum for zoology:

`Hodgson working lists/drawing numbers`
→ `Gray 1844 printed list`
→ `Gray & Gray 1847 British Museum catalogue`
→ `Hodgson marginal/correspondence corrections`
→ `later supplement/republication (including 1863)`

Do not flatten these into one `Hodgson catalogue`.

---

## 10. Relation table

Because the central unit is often composite, create explicit edges.

Fields:

- `relation_id`
- `subject_entity_id`
- `predicate`
- `object_entity_id`
- `date_from`
- `date_to`
- `source_entity_id`
- `confidence`
- `notes`

Useful predicates:

- `drawn_from`
- `represents`
- `label_for`
- `number_matches`
- `catalogued_as`
- `copy_of`
- `translation_of`
- `extract_from`
- `wrapper_for`
- `title_slip_for`
- `contained_in`
- `packed_with`
- `distributed_with`
- `duplicate_of`
- `replacement_for`
- `supersedes`
- `corrects`
- `contradicts`
- `received_with`
- `separated_from`
- `reunited_with`
- `same_batch_as`
- `same_paper_stock_as`
- `same_watermark_family_as`
- `same_catalogue_version_as`

---

## 11. Source / provenance fields

Every factual row should retain a source witness.

- `source_id`
- `source_type`
  - original letter / list / catalogue / manuscript / printed primary source / institutional catalogue / modern article / modern collection database / secondary monograph
- `repository_or_site`
- `shelfmark_or_url`
- `author_sender`
- `recipient`
- `date`
- `page_folio`
- `quotation_short`
- `transcription_status`
  - direct image verified / catalogue transcription / OCR / secondary quotation / search snippet
- `source_accessed_date`
- `archived_local_copy`
- `local_hash_if_any`
- `citation_ready`
- `notes`

### Evidence hierarchy

Prefer, in descending order where the question allows:

1. inspected original/digital image;
2. contemporary printed primary source;
3. reliable institutional full transcription;
4. institutional catalogue summary;
5. modern scholarly reconstruction;
6. search snippet or secondary quotation used only as a lead.

Do not silently upgrade a catalogue transcription into an inspected manuscript quotation.

---

## 12. Confidence / inference controls

Every non-trivial reconstruction should distinguish observation from inference.

### `claim_status`
- `direct`
- `strong_inference`
- `working_inference`
- `hypothesis`
- `disputed`
- `unresolved`

### `confidence`
- `high`
- `medium`
- `low`

### `inference_basis`
Free text, short.

Examples:

- `high/direct`: Gray letter explicitly says two different kinds have same number.
- `medium/strong_inference`: two catalogue entries probably refer to same drawing because number, measurements and annotation agree but physical comparison not yet made.
- `low/hypothesis`: a Whatman watermark may indicate a shared batch with another dossier; must be physically checked.

---

## 13. Failure-mode vocabulary

Use controlled tags so cases can be compared across Buddhist manuscripts, zoology and administrative documents.

- `loss_in_transit`
- `non_arrival`
- `route_delay`
- `water_damage`
- `condition_failure`
- `partial_object_only`
- `missing_leaf`
- `missing_drawing`
- `missing_specimen`
- `detained_by_intermediary`
- `not_yet_unpacked`
- `label_removed`
- `label_replaced`
- `identifier_collision`
- `copied_name_error`
- `catalogue_misidentification`
- `container_date_misread`
- `sequence_error`
- `copy_state_confusion`
- `provenance_loss`
- `priority_conflict`
- `media_trust_shift`
- `rebind_relation_loss`
- `reclassification_relation_loss`
- `catalogue_version_drift`

The article may ultimately be structured through failure modes because failures expose otherwise invisible infrastructure.

---

## 14. Minimal event example — British Museum, 6 Feb 1845

This is illustrative, not yet a final data row.

```text
event_id: HOD-EVT-TEMP-1845-02-06-01
event_type: inventory_reconciliation
date_from: 1845-02-06
institution_to: British Museum
source: NZSL/HOD/5/2/15
objects: Hodgson bird/mammal collection
exceptions_detected:
  - Tibetan pheasant escaped list because at stuffer
  - Ganges Pelican represented only by head
  - specimens in poor condition judged unsuitable for distribution
related_actions:
  - detailed catalogue of specimens received 1840-present
  - mammal/bone distribution list sent to Hodgson
  - bird list requested back so later distributions could be added
claim_status: direct
confidence: high
```

This single event already demonstrates why receipt, list, object state, institution and later distribution require separate fields.

---

## 15. Minimal object-relation example — Institut drawing

```text
object: drawing sheet
relations:
  drawing -> represents -> temple relief/painting
  Sanskrit note -> explanatory_annotation_for -> drawing
  European-form name -> identifier_for -> drawing
  drawing -> contained_in -> liasse/bundle
  bundle -> contained_in -> Institut case
later_event:
  explanatory material separated into another case
later_inference_failure:
  case note interpreted as 1866 shipment date
independent chronology:
  Saint-Hilaire discusses collection in 1863
```

This is the model for recording how a relation can survive, split, and later generate historical error.

---

## 16. Research workflow

For each new source:

1. extract only directly stated objects, containers, identifiers and events;
2. create provisional entity IDs;
3. record exact source level and transcription status;
4. add relations without assuming identity;
5. flag exceptions and contradictions;
6. only then infer shipment chains, copy families, batch relations or catalogue versions;
7. promote repeated mechanisms into article claims after multiple independent cases.

The census should remain capable of falsifying the article spine. It is not a database built to confirm the argument.

---

## 17. Immediate implementation test

Before converting this schema to structured data, manually code five stress-test cases:

1. 1837 Société Asiatique three-case manuscript arrival;
2. 1844–47 British Museum zoological receipt / reconciliation / catalogue / duplicate distribution loop;
3. 1858 Institut waterproof-box route and later Foucher chronology error;
4. 1870 `big deal box` / four portfolios / 1,104 sheets plus manuscript apparatus;
5. one Buddhist manuscript whose wrapper/title/folio state produced a later catalogue misidentification.

If those five can be represented without overloaded free-text fields, freeze schema v0.1 and then implement CSV/JSON/SQLite.

---

## 18. Wave 14 extension — counting ontology

Fort William and Mitra require count statements to become first-class historical records rather than generic `item_count` fields.

### Required fields

- `count_id`
- `count_value`
- `count_unit`
- `count_unit_class`
  - `TEXTUAL_WORK`
  - `PHYSICAL_VOLUME`
  - `LEAF`
  - `COPY`
  - `PACKAGE`
  - `BUNDLE`
  - `BOX`
  - `CATALOGUE_ENTRY`
  - `SPECIMEN`
  - `DRAWING_SHEET`
  - `OTHER`
- `count_operation`
  - production
  - packing
  - dispatch
  - receipt
  - shelving
  - inventory
  - cataloguing
  - retrospective_reconstruction
- `count_date`
- `count_actor`
- `count_source_id`
- `same_corpus_status`
  - `confirmed_same`
  - `partial_overlap`
  - `possible_overlap`
  - `unknown`
- `unit_conversion_demonstrated`
- `conversion_source_id`
- `conversion_relation`
- `count_version_status`
  - `contemporary`
  - `later_recount`
  - `retrospective_reconstruction`
  - `conflicting_same_source`
  - `unresolved`

### Hard rule

**Never subtract, ratio, reconcile or silently replace counts across `count_unit_class` unless a source demonstrates the conversion relation.**

`109 bundles`, `127 volumes` and `66 works` cannot be treated as three estimates of one count. They answer different operational questions.

### Direct calibration

Mitra 1882 provides a demonstrated non-identity: one distribution statement gives **85 bundles comprising 144 separate works** for the Asiatic Society of Bengal. The ratio is local to that statement and must not be generalized.

The same preface later states the Society collection under analysis as **86 bundles including 170 separate works**. Preserve both statements as separate count versions until the addition/recount/catalogue genealogy is demonstrated. Do not choose one as the `correct` total by default.

---

## 19. Wave 15 extension — segmentation and inspection protocol

Catalogue identity depends on how a composite object is inspected. Mitra 1882 directly diagnoses both false splitting and false lumping in the Calcutta Hodgson collection.

### Segmentation fields

- `segmentation_event_id`
- `physical_unit_entity_id`
- `pre_segmentation_object_count`
- `post_segmentation_object_count`
- `segmentation_basis`
  - binding_boundary
  - pagination_boundary
  - colophon
  - title_leaf
  - internal_title
  - script_hand_change
  - support_change
  - comparison_with_other_copy
  - catalogue_comparison
  - other
- `work_boundary_visible`
- `pagination_continuity`
- `multiple_works_in_physical_unit`
- `one_work_across_multiple_physical_units`
- `segmentation_error_type`
  - `FALSE_SPLIT`
  - `FALSE_LUMP`
  - `PHYSICAL_TEXTUAL_COLLAPSE`
  - `BOUNDARY_SAMPLING_ERROR`
  - `UNRESOLVED`
- `reidentification_basis`
- `comparison_witness_ids`

### Inspection-protocol fields

- `inspection_event_id`
- `inspection_actor`
- `inspection_goal`
- `inspection_depth`
  - boundary_only
  - sampled_internal
  - full_codex
  - comparative_collation
  - unknown
- `pages_or_leaves_examined`
- `first_leaf_examined`
- `last_leaf_examined`
- `internal_leaves_examined`
- `colophons_examined`
- `material_fields_recorded`
- `textual_fields_recorded`
- `inspection_time_or_labour_if_known`
- `expertise_language_script`
- `resulting_identity_change`

### Model warning case

Mitra reports that two or more works could be written continuously in one volume without a pagination break, while cursory examination read only the first and last page to determine the volume name. This can be coded as:

```text
physical_unit: codex
pagination_continuity: true
multiple_works_in_physical_unit: true
inspection_depth: boundary_only
pages_or_leaves_examined: first + last
segmentation_error_type: FALSE_LUMP
result: several textual works -> one catalogue identity
```

### B.5 calibration

Mitra explicitly says his earlier description of `B.5` did not give a full idea of its contents and that fuller analysis showed it comprised **39 Dharanis**. `B.65` contained another 12, some also included in B.5. This is a high-value test because increased inspection depth changes the represented internal object count under a stable institutional identifier.

---

## 20. Institutional legibility fields

Receipt, physical possession and catalogue existence must be separated from institutional usability.

- `institutional_legibility_event_id`
- `custody_confirmed`
- `physical_access_available`
- `unpacked_or_opened`
- `physical_units_delimited`
- `contents_identified`
- `identifier_assigned`
- `catalogue_entry_created`
- `catalogue_language`
- `catalogue_script`
- `catalogue_fields`
- `catalogue_arrangement`
- `required_expertise`
- `proposed_examiner`
- `competence_assessment`
- `authorised_examiner`
- `institutional_use_status`
  - received_only
  - physically_arranged
  - partly_identified
  - catalogued_limited_access
  - catalogued_operational
  - later_reidentified
  - unknown

Fort William is the model: a collection could be physically counted as volumes and still require a competent person to ascertain its contents. Its surviving Persian catalogue MS.PERS.130 further shows that shelfmark, title, condition and handwriting quality were selected institutional fields; catalogue usability depended on language/script as well as physical existence.

---

## 21. New failure and event vocabulary after Waves 14–15

Add failure tags:

- `false_split`
- `false_lump`
- `physical_textual_collapse`
- `boundary_sampling_error`
- `count_unit_conflation`
- `count_version_conflict`
- `institutional_legibility_failure`
- `expertise_bottleneck`
- `catalogue_language_interface_failure`
- `catalogue_shallow_inspection`

Add event types:

- `count`
- `recount`
- `segment`
- `resegment`
- `inspect_boundaries`
- `inspect_full_object`
- `identify_contents`
- `competence_assessed`
- `catalogue_entry_split`
- `catalogue_entries_merged`
- `count_version_superseded`

These additions make catalogue error and collection cardinality empirically reconstructible rather than forcing them into free-text `notes`.
