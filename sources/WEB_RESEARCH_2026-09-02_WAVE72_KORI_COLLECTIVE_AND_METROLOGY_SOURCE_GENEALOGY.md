# Web/archive research 2026-09-02 — Wave 72
## `Kori` is a general twenty-count collective applied to paper bundles; Landon’s paper table is not simply Wright 1877’s weights-and-measures appendix

Date: 2026-09-02

Status: active paper-history mainline. This wave clarifies the semantic architecture of `kori` and tightens the source genealogy behind Landon’s 1928 paper-metrology table. It also corrects a bibliographic trap in the Internet Archive record for Turnbull’s *Nepali Grammar and Vocabulary*.

## Executive result

Two separate results materially sharpen the `tau -> dhep -> kori` model.

### 1. `Kori` is not fundamentally a paper-specific package term

The textual state of A. Turnbull’s *Nepali Grammar and Vocabulary* accessible through Internet Archive directly places `kori` under the grammar of **special collectives**, alongside terms meaning a pair, a group of four and a group of five, and glosses it:

`kori — a twenty, score`.

This means the later paper equation:

`20 dhep = 1 kori`

is structurally intelligible as:

`twenty paper bundles = one score of paper bundles`,

rather than requiring `kori` to be a paper-exclusive container type.

Correct model:

`kori = GENERAL_TWENTY_COUNT_COLLECTIVE`

with

`paper kori = DOMAIN_APPLICATION_OF_GENERAL_COLLECTIVE`.

### 2. Landon 1928 did not simply copy the paper hierarchy from Wright 1877’s printed weights-and-measures appendix

Daniel Wright’s *History of Nepal* (1877), Appendix IV `Weights and Measures`, in the directly recoverable text, lists measures for gold, silver, metal utensils, dry measure and liquid measure. It does **not** contain the Landon paper lines `10 Tao = 1 Dhep; 20 Dheps = 1 Kori` in the available Appendix IV text.

Therefore Landon’s Appendix VI paper table has to come from another source layer, whether:

- contemporary Nepalese administrative knowledge;
- an informant or official under Chandra Shamsher;
- another earlier printed/manuscript source;
- or a mixed compilation.

Current source relation:

`WRIGHT_1877_APPENDIX_IV -> LANDON_1928_PAPER_TABLE = NO_DIRECT_TEXTUAL_SOURCE_EDGE_DEMONSTRATED`.

This is a useful narrowing of the provenance problem.

Mechanisms:

- `GENERAL_COLLECTIVE_CAN_BECOME_DOMAIN_METROLOGY`
- `PAPER_COUNT_HIERARCHY_REUSES_NON_PAPER_NUMERICAL_VOCABULARY`
- `METROLOGY_TABLES_HAVE_SOURCE_GENEALOGIES`
- `LATER_APPENDIX_CAN_ADD_MEASURES_ABSENT_FROM_EARLIER_STANDARD_REFERENCE`
- `BIBLIOGRAPHIC_METADATA_MUST_BE_CHECKED_AGAINST_INTERNAL_EDITION_STATEMENTS`.

---

## 1. Bibliographic correction: the accessible Turnbull scan is not an 1887 textual witness

Internet Archive item:

https://archive.org/details/nepaligrammarvoc0000turn

The item metadata gives publication date `1887` and identifies the work as A. Turnbull’s *Nepali Grammar and Vocabulary*.

But the actual OCR text begins with:

- `THIRD EDITION`;
- edited by R. Kilgour;
- Asian Educational Services reprint information;
- second AES reprint dated 1992.

More importantly, internal prefaces establish the edition genealogy.

Turnbull’s `PREFACE TO THE SECOND EDITION`, dated January 1904, explicitly says:

`This “second edition” of my 1887 attempt ... is really an entirely new work.`

Kilgour’s `PREFACE TO THE THIRD EDITION`, dated May 1923, then says the third edition is:

`practically a page for page reproduction of the earlier work with the correction of obvious mistakes`.

Thus the scanned object is:

`1992 AES reprint`
-> of `1923 third edition textual state`
-> described as essentially reproducing the `1904 second edition`.

It is **not** a direct scan of the 1887 first-edition textual state despite the Internet Archive metadata date.

Evidence coding:

- `IA_ITEM_METADATA_DATE = 1887`;
- `SCANNED_REPRINT_DATE = 1992`;
- `REPRINTED_EDITION_STATE = THIRD_EDITION_1923`;
- `THIRD_EDITION_RELATION_TO_1904 = PRACTICALLY_PAGE_FOR_PAGE_PER_EDITOR`;
- `DIRECT_1887_LEXICAL_EVIDENCE = NOT_ESTABLISHED_FROM_THIS_SCAN`.

Mechanism:

`CATALOGUE_PUBLICATION_DATE_CAN_MISIDENTIFY_DIGITIZED_EDITION_STATE`.

This matters because the current research question is chronological; a false 1887 lexical anchor would materially distort the evidence.

---

## 2. Direct `kori` locus in the accessible Turnbull textual state

Internet Archive full-text derivative:

https://archive.org/stream/nepaligrammarvoc0000turn/nepaligrammarvoc0000turn_djvu.txt

In the grammar section on numerals and collectives, the text first explains ordinary collective formation and then says:

`The following special collectives are used`.

The sequence is:

- `jorā` — two / couple / pair;
- `gaṇḍā` — four / quartet;
- `panjā` — five / quintet;
- `kori` — twenty / score;
- `saikarā` — hundred / per cent.

This places `kori` squarely inside a general numerical/collective system.

The text later uses `kori` in an ordinary numerical example involving sheep, confirming it is not restricted to paper.

Evidence state:

`KORI_GENERAL_COLLECTIVE = DIRECT_TEXTUAL_STATE_SECURE`.

Chronological control:

Because the scanned textual state is the 1923 third edition as reprinted in 1992, the safest direct date is:

`DIRECT_BY_1923_TEXTUAL_STATE`.

The third-edition preface makes continuity back to 1904 highly likely, but the exact `kori` locus has not been independently checked in a physical/digital 1904 second edition.

Therefore:

`KORI_PRESENT_IN_1904 = HIGHLY_PROBABLE_FROM_PAGE_FOR_PAGE_STATEMENT / NOT_DIRECTLY_VERIFIED`.

Do not date the lexical entry to 1887.

---

## 3. The Turnbull English–Nepali vocabulary does not itself supply the paper-count hierarchy

The same textual state’s English–Nepali vocabulary gives:

`Paper — kāgat`.

Its general English entry for:

`Sheet`

is glossed `chaddar`.

Searches of the full OCR for the forms:

- `dhep`;
- `dhepa`;
- `tau`;
- `tao`

return no direct matches.

This is not proof that no Devanagari or OCR-corrupted form occurs anywhere in the printed book, but it establishes that the easily searchable Roman vocabulary does not reproduce Landon’s paper-count equations.

Thus Turnbull’s current value is specifically:

- generic semantics of `kori`;
- edition/source control;

not:

- direct pre-Landon attestation of `dhep` or `tau`.

Mechanism:

`SEMANTIC_COMPONENTS_OF_A_METROLOGY_CAN_BE_ATTESTED_SEPARATELY_FROM_DOMAIN_TABLE`.

---

## 4. `Kori` changes the ontology of the paper-count system

Wave 69/70 represented:

`tau -> dhep -> kori`

as three levels in a local paper metrology.

That remains operationally correct for the paper domain, but the lexical ontology should now distinguish:

### paper-specific or paper-bound usage

`tau` — sheet-level paper count in the recovered paper-metrology sources;

`dhep` — handmade-paper bundle term with contextual package depth;

### general numerical collective applied to paper

`kori` — a score / twenty.

Therefore the paper hierarchy is partly **compositional**:

`20 × [dhep package] = kori [score] of dhep packages`.

This may explain why `kori` can function beyond paper and why its numerical value is more semantically stable than `dhep` package depth.

Under the ten-sheet convention:

`1 dhep = 10 tau`

and

`1 kori = 20 dhep = 200 tau`.

But `kori = twenty` does not itself imply that any one `dhep` contains ten sheets.

If a locality has a twenty-sheet `dhep`, a `kori` understood literally as a score of dheps would instead contain 400 sheets unless local usage overrides the simple compositional rule.

This is now an empirical question, not a conversion to assume.

Mechanisms:

- `GENERAL_COUNT_COLLECTIVE_DISTINCT_FROM_PACKAGE_DEPTH`
- `UPPER_LEVEL_COUNT_CAN_BE_STABLE_WHILE_LOWER_PACKAGE_DEPTH_VARIES`
- `COMPOSITIONAL_METROLOGY_REQUIRES_LEVEL_SPECIFIC_EVIDENCE`.

---

## 5. Wright 1877 provides an important source-genealogy negative

Source:

Daniel Wright (ed.), *History of Nepal*, Cambridge, 1877, Appendix IV `Weights and Measures`.

A directly recoverable transcription of Appendix IV lists:

- gold weight;
- silver weight;
- weights for metal utensils;
- dry measure;
- liquid measure.

Available text:
https://www.wisdomlib.org/history/book/history-of-nepl/d/doc1896459.html

The recovered appendix text does not contain:

- `Paper`;
- `Tao`;
- `Dhep`;
- `Kori`.

This is a bounded negative:

`PAPER_METROLOGY_NOT_PRESENT_IN_CURRENTLY_RECOVERED_WRIGHT_APPENDIX_IV_TEXT`.

It should not be inflated into a claim that no other section, manuscript state or ancillary document associated with Wright ever contained paper units.

But for Landon-source genealogy it is enough to reject one easy shortcut:

**Landon’s paper lines are not visibly inherited by straightforward reproduction of Wright’s printed Appendix IV table.**

---

## 6. Landon’s source problem is now narrower

Wave 71 established that Landon 1928 Appendix VI prints:

`10 Tao = 1 Dhep`

`20 Dheps = 1 Kori`

with the footnote:

`A tao is a sheet of any size.`

Landon also had:

- broad access to Nepalese archives;
- original documents supplied under Chandra Shamsher;
- Nepalese agents/informants explaining local knowledge;
- earlier British scholarship including Wright and Hodgson.

Wave 72 now eliminates one simplistic transmission hypothesis:

`Wright 1877 printed Appendix IV -> Landon paper lines`

is not directly supported, because the paper hierarchy is absent from the recovered Wright table.

Live source candidates therefore become more focused:

1. a Nepalese government/administrative metrology source available to Landon;
2. contemporary Kathmandu informant knowledge;
3. an army/intelligence/gazetteer source later than Wright but earlier than Landon;
4. another historical Nepalese account or lexicon;
5. a composite table assembled by Landon from multiple channels.

Immediate comparison targets should be:

- E. R. Elles, *Report on Nepal* (1884);
- later Gurkha handbooks derived from Elles;
- Grierson/Turnbull/other language manuals;
- Nepalese administrative metrology documents;
- Landon papers/notes if accessible.

---

## 7. Relation to Hodgson f.117

Hodgson/Wallich bill:

`MSS EUR HODGSON/12 f.117 — 1843`.

Cambridge catalogue:

- local paper unit romanized `ḍhyāp`;
- ten-sheet gloss.

Current temporal/semantic chain:

`1843 f.117 catalogue: ḍhyāp, ten-sheet gloss`

-> `[nineteenth-century immediate lexical bridge still missing]`

-> `1923 Turnbull textual state: kori = generic score/twenty`

-> `1928 Landon: 10 tao = 1 dhep; 20 dhep = 1 kori; tao = sheet of any size`

-> `1987–88 Paudel: same ten-sheet hierarchy`

-> `modern lexicography: standardized ten-sheet dhep`.

This strengthens the internal logic of the later hierarchy while keeping the nineteenth-century bridge honestly open.

The most important reinterpretation is:

`kori` need not be a historically mysterious paper-container word. It is a general collective numeral recruited into paper accounting.

The historically difficult term remains `dhep`, because that is where physical bundle depth varies.

---

## 8. Revised data model

For each metrological unit add:

- `semantic_scope`: general collective / paper-specific count / package term / dimensional measure;
- `domain_application`: paper / livestock / money / etc.;
- `package_depth`: if physically bundled;
- `count_multiplier`: if general numerical collective;
- `source_edition_state`;
- `catalogue_metadata_date` distinct from `actual_scanned_edition`.

For `kori`:

- `semantic_scope = GENERAL_COLLECTIVE`;
- `count_multiplier = 20`;
- `paper_application = DIRECT_BY_LANDON_1928_AND_PAUDEL_1987`;
- `physical_package_form = NOT_DEFINED_BY_LEXEME`.

For `dhep`:

- `semantic_scope = PAPER_BUNDLE_TERM`;
- `package_depth = CONTEXTUAL_ATTESTED_VALUES`.

For `tau`:

- `semantic_scope = PAPER_SHEET_COUNT` in the recovered paper metrology;
- `dimension = UNSPECIFIED_BY_COUNT`, explicitly supported by Landon’s `sheet of any size` footnote.

---

## Source-control rules

1. Do not cite the accessible Turnbull scan as an 1887 lexical witness.
2. Record the scan as a 1992 reprint of the 1923 third edition textual state.
3. Use the 1923 editor’s own claim of practical page-for-page reproduction to describe its relation to 1904, but do not silently backdate individual entries without a direct 1904 witness.
4. Treat `kori = twenty/score` as a general collective meaning directly secure in the accessible textual state.
5. Do not define `kori` as a paper-specific bundle.
6. Keep `20 dhep = 1 kori` as a domain application of a twenty-count collective unless contrary local evidence appears.
7. Treat the absence of paper units from the recovered Wright Appendix IV as a bounded source-genealogy negative, not proof of absence from all Wright-related material.
8. Do not derive Landon’s paper table from Wright without a source edge.
9. Keep the nineteenth-century lexical bridge between f.117 and 1920s sources unresolved.

## Immediate next actions

1. Recover an actual 1887 Turnbull first-edition scan or page images and search its fuller vocabulary for `dhep/tau/kori`.
2. Recover a 1904 second edition if possible and directly verify whether the `kori` collective entry is present there.
3. Inspect E. R. Elles 1884 `Report on Nepal`, especially its weights-and-measures section, for the paper hierarchy.
4. Search later Gurkha/intelligence handbooks for `tao/dhep/kori` to identify a likely Landon source chain.
5. Search Documenta Nepalica and Regmi collections for pre-1900 `ढेप`, `ताउ`, `कोरी` in paper/accounting contexts.
6. Continue to prioritize the original 1843 f.117 image, because it remains the earliest object-specific node in the current chain.

## Bottom line

Wave 72 separates two things that had been bundled together analytically. `Dhep` is a physical paper-package term whose numerical depth varies by production context; `kori`, by contrast, is directly attested in Nepali grammar as the general collective `a twenty, score`. A paper `kori` is therefore best understood as an application of an ordinary twenty-count term to paper bundles, not as a uniquely paper-specific container. At the same time, bibliographic checking removes a false 1887 anchor: the accessible Turnbull scan reproduces a 1923 third-edition state, not the first edition. Finally, Wright’s 1877 printed weights-and-measures appendix lacks Landon’s paper hierarchy in the recoverable text, narrowing the search for Landon’s immediate source toward Nepalese administrative/informant material or later intelligence and language manuals. The paper-metrology history is becoming a genealogy of counting operations as well as a genealogy of words.