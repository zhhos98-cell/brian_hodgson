# Paper catalogue field inheritance, 1875 — material families encoded by relational description

Date: 2026-08-31

Status: paper-centred source-control correction to `data/ras_hodgson_material_catalogue_census_v0_1.json`. The earlier census correctly noticed that MSS 78–79 inherit material descriptors from MS 77, but its aggregate field `blackened_paper_entries: 1` counts only explicit wording. This note separates explicit mention from historically warranted material inheritance.

## Core result

Cowell and Eggeling's 1875 catalogue does not always repeat paper descriptors item by item. It sometimes establishes a material description once and then transmits that description to subsequent entries through relational phrases such as:

- `Size, paper and handwriting as in the preceding MS.`
- `Paper, size and handwriting as in preceding MSS.`

The strongest case is entries 77–79.

### MS 77

`Mahāpratyangirā-mahāvidyārājñī-Dhāraṇī`

- 21 leaves;
- explicitly described as **blackened paper**;
- 8 × 2 3/4 in.;
- five lines per page;
- alternating yellow and white paint, three lines of one and two of the other;
- dated Samvat 944 / A.D. 1824.

### MS 78

`Dhvajāgrakeyūrā-Dhāraṇī`

- 3 leaves;
- catalogue states: **`Size, paper and handwriting as in the preceding MS.`**

Therefore the paper field of MS 77 is explicitly inherited by MS 78.

### MS 79

`Collection of Dhāraṇīs`

- 21 leaves;
- catalogue states: **`Paper, size and handwriting as in preceding MSS.`**
- it independently confirms the visual writing regime: generally three white and two yellow lines per page.

Therefore MS 79 belongs to the same material-description chain.

## Correction to the census

The earlier field:

`blackened_paper_entries = 1`

is valid only if interpreted as:

`entries where the words blackened paper are explicitly printed = 1`.

It is not a valid estimate of manuscripts that the catalogue describes as using that paper state.

The corrected ontology is:

- `explicit_blackened_paper_mentions = 1` -> MS 77;
- `blackened_paper_by_direct_field_inheritance = 2` -> MSS 78–79;
- `effective_blackened_paper_material_family = 3` -> MSS 77–79.

Mechanisms:

- `CATALOGUE_MATERIAL_FIELD_INHERITANCE`
- `RELATIONAL_MATERIAL_DESCRIPTION`
- `EXPLICIT_MENTION_VS_EFFECTIVE_ATTRIBUTE`
- `CATALOGUE_COMPRESSION_BY_PRECEDING_ENTRY`

## Why this matters for paper history

This is not simply a data-cleaning issue. The catalogue turns manuscript materiality into a compressed relational information system.

Instead of:

`MS 77 -> paper field`

`MS 78 -> paper field`

`MS 79 -> paper field`

it can write:

`MS 77 -> full material tuple`

`MS 78 -> inherit tuple from 77`

`MS 79 -> inherit tuple from preceding MSS`

The printed catalogue itself therefore creates a dependency graph among paper descriptions.

A reader can reconstruct a material family only by following those paper references across entries.

## Material family versus production batch

The secure claim is descriptive:

**Cowell and Eggeling catalogue MSS 77–79 as sharing paper, size and handwriting.**

Do not yet infer:

- same historical production event;
- same scribe as a biographical person;
- same workshop;
- same original bundle;
- same procurement batch.

Those stronger claims require direct manuscript inspection and provenance evidence.

What the catalogue itself warrants is a `CATALOGUED_MATERIAL_FAMILY`.

## Important quantitative consequence

Corpus statistics derived by keyword search will systematically undercount any field represented through inheritance phrases.

General rule:

`explicit descriptor frequency != effective material attribute frequency`.

This applies not only to blackened paper. The full catalogue should now be re-parsed for relational phrases involving:

- paper/support;
- size/dimensions;
- handwriting;
- line count;
- age;
- wrapper/title relations;
- supplied/replacement leaves.

Every inherited field should preserve:

- `source_entry`;
- `target_entry`;
- `inherited_fields`;
- `inheritance_phrase`;
- `confidence`.

## Paper-specific historiographical value

The catalogue's economy resembles other paper infrastructures in the Hodgson archive. Repeated information is not always recopied locally; relations are externalized through identifiers or references.

But this case should remain specifically bibliographical:

**paper materiality becomes remotely operable through a printed cross-reference.**

The original manuscripts need not be physically side by side for a later reader to reconstruct that Cowell and Eggeling treated them as materially alike.

Mechanism:

`PRINTED_REFERENCE_RECONSTRUCTS_MATERIAL_SIMILARITY`.

## Article-level formulation

A concise usable claim:

**Cowell and Eggeling did not describe every manuscript as a self-contained metadata record. In the final entries of the Hodgson catalogue, one manuscript is fully specified as blackened paper with alternating yellow and white writing, while the next two inherit paper, size and hand by reference to preceding entries. Paper materiality was therefore converted into a relational catalogue field. Counting only explicit material words would reduce a three-manuscript material family to one. The catalogue made physical similarity portable by encoding it as dependency between printed descriptions.**

## Next tests

1. Parse all 79 entries for `preceding MS`, `preceding MSS`, `same as`, `as above`, `ditto` and comparable relational phrases.
2. Separate `explicit_field` from `inherited_field` in the material census.
3. Inspect MSS 77–79 directly for actual support treatment, dimensions, hand and colour sequence.
4. Test whether MS 78 really preserves the alternating colour regime or only inherits paper/size/hand.
5. Determine whether MS 79's independent three-white/two-yellow statement confirms a shared ruled/painted production template.
6. Compare material-family clustering with textual genre only after material clustering is independently established.
7. Keep v0.1 as the historical census state and supersede it explicitly with v0.2 rather than silently rewriting it.

## Bottom line

The 1875 Hodgson catalogue contains a paper-level compression mechanism. Material attributes can be stated once and inherited by later entries. MSS 77–79 are therefore not one explicit blackened-paper manuscript plus two unspecified manuscripts; in the catalogue's own descriptive logic they form a three-item material family linked by paper, size and handwriting. For the paper project, this shows that nineteenth-century cataloguing did not merely record paper: it created relational paper metadata whose meaning depends on following references between entries.