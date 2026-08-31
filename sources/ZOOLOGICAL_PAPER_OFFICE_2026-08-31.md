# Zoological paper office — shikaree observation, writer translation, drawing numbers, and seriality

Date: 2026-08-31

Status: article-facing archive reconstruction centred on Zoological Society of London `NZSL/HOD/1/3`, checked against later drawing-count and custody evidence already ingested in this repository. Observation, translation, notebook entry, drawing identifier, represented subject and physical sheet are kept as distinct historical operations/units.

## Executive result

The Zoological Society catalogues `NZSL/HOD/1/3` under Hodgson's own title:

> `Memoranda of manners and habits of birds of my Collection (according to the numbers attached to the drawings). Done by my native sportsmen or Shikarees and translated by my writer`

The catalogue further describes a notebook of bird descriptions numbered by reference to numbered drawings, preserving three sequence blocks:

- No.1, Vol.1: 1–169;
- No.3, Vol.3: 340–488;
- No.6, Vol.6: 755–855.

The secure source-controlled chain is:

`field observation by sportsmen/shikarees -> translation by writer -> serial notebook description -> number-based cross-reference -> numbered drawing`.

The important point is not simply that Hodgson employed local assistants. **Labour roles and paper identifiers were coupled into a recoverable production architecture.** Behavioural observation and linguistic conversion entered a serial paper system in which numbers allowed descriptions to be re-associated with drawings after observers, specimens, drawing sheets and notebooks were physically separated.

Primary mechanism:

`OBSERVATION_TRANSLATION_SERIALIZATION_CHAIN`.

## 1. Source-controlled role differentiation

`NZSL/HOD/1/3`, dated by ZSL 1846–1857, explicitly supplies:

- `native sportsmen or Shikarees`: production of memoranda concerning `manners and habits`;
- `my writer`: translation;
- `numbers attached to the drawings`: cross-reference system;
- surviving serial notebook ranges: 1–169, 340–488, 755–855.

The public record does not identify the first recording medium, language of first report, physical hand of every surviving entry, or whether Hodgson edited every translated statement. Those remain direct-inspection questions.

Mechanism:

`ROLE_SPECIFIC_LOCAL_KNOWLEDGE_PIPELINE`.

The historiographical gain is precision: `local collaboration` becomes a sequence of evidenced operations rather than a single social category.

## 2. Translation as pre-circulation scientific infrastructure

A safe operational model is:

`observed behaviour -> linguistic conversion -> serial notebook entry -> numbered relation to drawing`.

The first recording state remains unknown, but translation is clearly built into the production architecture before the corpus becomes a portable notebook series.

Mechanism:

`TRANSLATION_AS_PRE_CIRCULATION_INFRASTRUCTURE`.

Translation here is not metropolitan reception work applied to an already complete object. It helps constitute the documentary object that later circulates.

## 3. Number as cross-media relation key

The notebook is explicitly organized `according to the numbers attached to the drawings`.

At minimum:

`notebook description <-> number <-> drawing`.

The number acts as an address across separate paper objects. It permits behavioural text and visual representation to be reunited after physical separation.

Mechanism:

`NUMBER_AS_CROSS_MEDIA_RELATION_KEY`.

Potential joins to specimens, catalogues and later institutional lists require number-level comparison rather than assumption.

## 4. Surviving serial ranges are not original completeness

The surviving ranges are discontinuous: 1–169, 340–488 and 755–855. These gaps cannot automatically be treated as missing observations in Hodgson's original research programme. They may reflect lost volumes, survival elsewhere, accession history, selective transfer, numbering breaks or later cataloguing state.

Mechanism:

`SURVIVING_SERIAL_RANGE_NOT_ORIGINAL_COMPLETENESS`.

Archive survival and historical seriality need separate fields.

## 5. Drawing identifier and physical sheet are different ontologies

The later Hodgson collection summary in `Adobe Scan 2025年3月28日.pdf_by_PaddleOCR-VL-1.6.json`, Appendix C, counts zoological drawings by **sheets**:

- Birds: 1,241 sheets;
- Mammals: 557 sheets;
- Reptiles etc.: 55 sheets;
- total: 1,863 sheets.

Its footnote states that the drawings are on folio-size sheets and **many sheets contain several subjects**.

This blocks an easy merger with HOD/1/3:

`drawing identifier != necessarily sheet number`

`notebook entry number != necessarily one sheet`

`one sheet != one represented subject`

`1,241 bird sheets != 1,241 behavioural-description identifiers`.

Mechanism:

`IDENTIFIER_UNIT_SHEET_UNIT_SEPARATION`.

This is a paper ontology problem rather than a generic counting error. An identifier is a relational address; a sheet is a material support. Their cardinalities can diverge by design.

## 6. Distributed modal evidence package

The zoological object is distributed across media:

`specimen -> bodily/material trace`

`drawing -> selected visual/anatomical representation`

`numbered memorandum -> behavioural description`

`number -> relation key across those modalities`.

A dead specimen cannot itself transport `manners and habits`. The notebook is therefore a paper memory for event-like behavioural knowledge.

Mechanism:

`DISTRIBUTED_MODAL_EVIDENCE_PACKAGE`.

This is a concrete reason why Hodgson's science required several media: different supports preserve different epistemic properties.

## 7. Paper seriality makes distributed labour auditable

The architecture permits socially and materially distinct operations to remain reconnectable:

- observation away from Hodgson;
- translation by a writer distinct from the observer;
- drawing on separate sheets;
- serial accumulation in notebooks;
- number-based joins between surfaces.

The result is a distributed documentary witness rather than a single authored paper.

Mechanism:

`PAPER_MEDIATED_DISTRIBUTED_ZOOLOGICAL_AUTHORSHIP`.

`Authorship` is used only in the documentary/material sense established in Wave 36. It does not imply equal semantic or publication authorship.

## 8. Long operational life of the visual paper corpus

Appendix C reports that 1,115 bird sheets were lent to A. Hume in 1870 for a projected work, with eventual delivery to the Zoological Society required when Hume had finished; the drawings were transferred to ZSL in 1874.

Wave 34 reconstructs this as a custody/user/destination sequence. The paper-centred implication is that a visual corpus generated in Hodgson's research system remained an active research interface decades later while possession and institutional destination changed around it.

Mechanism:

`SERIAL_PAPER_CORPUS_REUSED_ACROSS_RESEARCH_GENERATIONS`.

Identifier continuity between HOD/1/3 and the Hume sheets remains to be tested directly.

## 9. Zoological research establishment as paper office

Wave 32 reconstructed a coordinated local research establishment. HOD/1/3 now supplies a specific internal workflow:

`field observer -> translation -> serial notebook -> numbered drawing relation`.

Article-ready formulation:

**Hodgson's zoological establishment operated partly as a paper office: local observations were converted into serial, numbered and cross-referenced documentary states that could travel independently of their original observers and later be joined to drawings, specimens, catalogues and institutional lists.**

Mechanism:

`ZOOLOGICAL_RESEARCH_ESTABLISHMENT_AS_PAPER_OFFICE`.

This links the Hodgson case to histories of paper technology as seriality, bookkeeping, administration and labour organization rather than only to specialized scientific instruments.

## 10. Article scene

### Numbering behaviour: the zoological paper office

Narrative sequence:

1. open with Hodgson's explicit HOD/1/3 title;
2. reconstruct `shikaree observation -> writer translation -> numbered notebook -> numbered drawing`;
3. show why behavioural evidence requires a separate paper memory from specimen/drawing evidence;
4. introduce Appendix C's warning that many represented subjects can occupy one folio sheet;
5. separate relation-key numbering from sheet cardinality;
6. close with the 1870 Hume reuse and 1874 ZSL destination as evidence of the long operational life of the paper corpus.

The scene carries three article-level claims:

- distributed documentary labour is materially recoverable;
- translation is constitutive scientific infrastructure before metropolitan publication;
- paper identifiers preserve relations across evidence media while physical sheets constitute a distinct counting ontology.

## 11. Mechanism codes

- `OBSERVATION_TRANSLATION_SERIALIZATION_CHAIN`
- `ROLE_SPECIFIC_LOCAL_KNOWLEDGE_PIPELINE`
- `TRANSLATION_AS_PRE_CIRCULATION_INFRASTRUCTURE`
- `NUMBER_AS_CROSS_MEDIA_RELATION_KEY`
- `SURVIVING_SERIAL_RANGE_NOT_ORIGINAL_COMPLETENESS`
- `IDENTIFIER_UNIT_SHEET_UNIT_SEPARATION`
- `PAPER_MEDIATED_DISTRIBUTED_ZOOLOGICAL_AUTHORSHIP`
- `DISTRIBUTED_MODAL_EVIDENCE_PACKAGE`
- `SERIAL_PAPER_CORPUS_REUSED_ACROSS_RESEARCH_GENERATIONS`
- `ZOOLOGICAL_RESEARCH_ESTABLISHMENT_AS_PAPER_OFFICE`

## 12. Direct archival checks required

1. Inspect surviving HOD/1/3 pages for hand(s), ruling, paper type, watermark/countermark, corrections, insertions, page/leaf numbers and repeated entry fields.
2. Determine whether the writer, Hodgson or another person physically inscribed translated entries.
3. Recover the entry schema: identifier, local/scientific name, locality, sex/age, behaviour, seasonality, measurement and other recurring fields.
4. Determine whether local-language terms survive within the translated English state.
5. Compare a controlled sample of HOD/1/3 numbers directly with surviving bird drawings.
6. Establish whether drawing identifiers are subject numbers, sheet numbers or a historically mixed system.
7. Investigate missing Vols.2, 4 and 5 as an archive-survival problem rather than assuming original loss.
8. Check the 20 July 1867 Günther correspondence concerning `printing of memorandum` and test whether it refers to this behavioural corpus.
9. Compare the 1870 Hume-used bird sheets with HOD/1/3 identifiers where possible.
10. Keep sheet, represented subject, notebook entry, drawing identifier and specimen totals separate until a historical conversion relation is demonstrated.

## 13. Source references

- Zoological Society of London, `NZSL/HOD/1/3`, archive catalogue record, `Memoranda of manners and habits of birds of my Collection (according to the numbers attached to the drawings). Done by my native sportsmen or Shikarees and translated by my writer`, dated 1846–1857.
- Zoological Society of London, `NZSL/HOD/1/1`, lists of drawings and specimens sent to various recipients, with dated count/custody states, 1842–1874.
- Zoological Society of London, `NZSL/HOD/5/3`, correspondence concerning printing/publication/use/donation of drawings and memoranda, 1858–1874.
- Local archive scan: `Adobe Scan 2025年3月28日.pdf_by_PaddleOCR-VL-1.6.json`, Appendix C, current digital pages c.156–157: drawing-sheet totals, folio-sheet/multiple-subject footnote, Hume loan and ZSL destination.

## Bottom line

The high-value object is not merely a bird notebook. It is a surviving node in a distributed paper system that separates and reconnects observation, translation, behavioural description and visual representation. Its numbers function as relation keys. The later sheet-count evidence simultaneously blocks a false quantitative merger: identifier series and physical paper units belong to different ontologies. This gives the paper-centred article a direct bridge between local knowledge labour, translation, seriality and material counting.