# Web/archive research 2026-09-02 — Wave 68
## Paper counting regimes and unit-translation risk: ream, quire, dasta, takhta, and the unresolved Nepali ḍhyāp

Date: 2026-09-02

Status: active paper-history mainline. This wave treats paper quantity units as material infrastructure. It does not equate European/Company units with South Asian local units and does not normalize the Cambridge catalogue's `ḍhyāp` reading until the original 1843 bill is recovered.

## Executive result

Paper quantity is not a neutral number attached to a sheet. It is produced inside a **counting and packaging regime**.

The evidence now allows three distinct cases.

### 1. English/Company paper trade: `ream -> quire -> sheet`, with package position built into quality

Moxon's period technical account states that a ream contains twenty quires and that the two outside quires are cording/cassie quires. Individual quires may contain twenty-four or twenty-five sheets depending on the stock. The 1725 Fort St George paper complaint shows this structure operating inside Company quality control: returned musters came from the poorer outside cording quires, so their position inside the ream distorted the assessment.

### 2. North Indian/Kashmiri paper trade: `dasta` is a local/regional unit whose internal definition is not universally fixed

A contemporary 1831 Kashmir observation reconstructed from Victor Jacquemont's notes describes twenty-four finished sheets rolled together as one `dastā`. Patrick Carnegy's North Indian official glossary, first published in 1853 and expanded in 1877, instead defines paper `dasta` as twenty-four `takhtas`, each takhta consisting of two, four or more sheets. The same lexical label therefore does not authorize a universal sheet conversion across region, period or trade practice.

### 3. Hodgson's 1843 Nepal bill: `ḍhyāp` remains a catalogue-attested but externally unverified unit

Cambridge transcribes f.117 as `1,012 bundles (ḍhyāp)` of Nepali paper and glosses one bundle as ten sheets. Searches of Nepali-script variants, romanized forms and general historical paper vocabulary have not produced an independent nineteenth-century source confirming `ḍhyāp` as a paper-count unit. The original image link currently returns 502, and the catalogue's quantity/rate/total arithmetic does not reconcile under a literal reading.

Therefore the correct state is:

`ḌHYĀP = CATALOGUE_TRANSCRIPTION/EDITORIAL_GLOSS_ONLY_PENDING_ORIGINAL_BILL`.

The paper-history consequence is methodological:

**do not translate historical paper units directly into sheet totals until their internal package structure, local meaning and source layout have been controlled.**

Core mechanisms:

- `PAPER_QUANTITY_IS_UNIT_SYSTEM_DEPENDENT`
- `COUNTING_REGIME_IS_PART_OF_SUPPLY_INFRASTRUCTURE`
- `PACKAGE_UNIT_AND_SHEET_COUNT_ARE_NOT_INTERCHANGEABLE`
- `SAME_UNIT_WORD_CAN_HAVE_REGIONALLY_VARIABLE_INTERNAL_STRUCTURE`
- `CATALOGUE_NORMALIZATION_CAN_HIDE_ACCOUNTING_STRUCTURE`
- `ARITHMETIC_CONTROL_IS_SOURCE_CRITICISM`
- `LOCAL_UNIT_REQUIRES_INDEPENDENT_LEXICAL_OR_OBJECT_CONTROL`.

---

## 1. Moxon: the ream is a package with internal structure, not only a sheet count

Joseph Moxon's *Mechanick Exercises* gives direct period technical evidence:

- each ream contains twenty quires;
- two of those twenty are the outside `Cording Quires` / `Cassie Quires`;
- cording quires serve as the cases/protective outsides of the ream;
- they are commonly made up from torn, wrinkled, stained or otherwise inferior sheets;
- when culling good sheets, Moxon allows twenty-four or twenty-five sheets to a quire depending on how the paper `holds out`.

Source:
https://www.gutenberg.org/cache/epub/78991/pg78991-images.html

This means the unit hierarchy is simultaneously quantitative and qualitative:

`REAM`
-> `QUIRE POSITION`
-> `SHEET QUALITY`.

A sheet count alone loses package position.

Mechanisms:

- `COUNTING_UNIT_HAS_MATERIAL_TOPOLOGY`
- `REAM_IS_A_QUALITY_STRUCTURED_PACKAGE`.

---

## 2. Fort St George: Company quality control depends on understanding the unit structure

Wave 67's direct Court despatch becomes more precise when read against Moxon's unit description.

Madras returned paper musters to demonstrate poor quality. The supplier responded that the samples all came from the outside `Corded Quires`, which the Court described as normally worse than the rest of the ream.

The complaint failed as representative sampling because the local evaluators treated:

`sample sheet`

as if it represented:

`whole ream`.

But the ream's internal structure made that inference unsafe.

Thus:

`PAPER_COUNTING_UNIT -> SAMPLE_FRAME`.

The Court's solution was not a new abstract paper grade but better package provenance: future complaints should identify chest marks and numbers so the consignment could be traced to one of the Company's two stationers.

Mechanisms:

- `UNIT_STRUCTURE_CONDITIONS_SAMPLING_VALIDITY`
- `COUNTING_AND_TRACEABILITY_ARE_LINKED`.

---

## 3. 1831 Kashmir: one dastā = twenty-four finished sheets in a directly observed manufacture context

Amélie Couvrat Desvergnes's study of nineteenth-century Kashmiri paper reconstructs Victor Jacquemont's observation of Srinagar papermaking on 4 June 1831.

After final burnishing:

- twenty-four sheets were rolled together to form a `dastā`;
- the dastā itself had a market price varying by grade;
- Jacquemont's manuscript/book-production calculation used multiple `dasteh` of paper alongside copyist and illumination costs.

Source:
COMSt Bulletin 9 (2023), `Nineteenth-century Kashmiri Paper`.

This is almost exactly contemporary with Hodgson's intensive Kathmandu paper/manuscript work.

But it is evidence for Kashmir, not Nepal.

Safe code:

`KASHMIR_1831_DASTA = 24 FINISHED SHEETS DIRECTLY OBSERVED_IN_RECONSTRUCTED_JACQUEMONT_ACCOUNT`.

Mechanisms:

- `LOCAL_PAPER_UNIT_CAN_BUNDLE_FINISHED_SHEETS_AFTER_PROCESSING`
- `COUNTING_UNIT_CAN_BE_PRICE_UNIT`.

---

## 4. Carnegy: `dasta` can also have a nested internal structure

Patrick Carnegy's *Kachahri Technicalities* was first published in 1853; the expanded second edition appeared at Allahabad in 1877.

Its entry on idiomatic classifiers states:

`Dasta` — paper, with one dasta containing twenty-four `takhtas`, and a takhta consisting of two, four or more sheets.

Direct searchable second-edition text:
https://tufs.repo.nii.ac.jp/record/11270/files/43552.pdf

Bibliographic control for first edition:
Carnegy, *Kutcherry Technicalities, or Vocabulary of Law Terms as used in the Mofussil Courts N.W.P.*, Allahabad, 1853.

The important point is not to choose between `24 sheets` and `24 takhtas` as the single correct Indian definition.

It is the opposite:

**the lexical label `dasta` could sit at different levels of the paper-count hierarchy in different documented practices.**

That makes dictionary translation insufficient for reconstructing an account book.

Mechanisms:

- `SAME_UNIT_LABEL_CAN_ENCODE_DIFFERENT_PACKAGE_DEPTH`
- `LEXICAL_EQUIVALENCE_NOT_QUANTITATIVE_EQUIVALENCE`.

---

## 5. Wider manuscript-paper evidence reinforces regional variability

Modern paper-history scholarship notes further variation in `dast/dasta/dastah` usage across Arabic/Persianate paper commerce and manuscript practice, often around twenty-four or twenty-five sheets but not with one universal value.

This should be used only as comparative control, not to reconstruct Nepal.

The relevant methodological lesson is already secure from Kashmir and Carnegy:

`local unit name -> local package convention`,
not
`unit name -> universal sheet number`.

---

## 6. Hodgson f.117: what the Cambridge catalogue actually proves

Direct catalogue text for `MSS EUR HODGSON/12 f.117` records:

- bill made out to Dr Nathaniel Wallich;
- Nepal Residency, 1843;
- bill itself on machine-made paper;
- Nepali paper and book-binding material;
- total Nepali Rupees 79.30, converted to Indian Rupees 61.12;
- `1,012 bundles (ḍhyāp)`;
- editorial gloss: ten sheets in one bundle;
- rates transcribed as Rupees 10/- and Rupees 14/- per bundle;
- wax cloth, thread and twine.

Source:
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol012.html

Current image endpoint:
`catalogue2.socanth.cam.ac.uk/eXistdata/media/thumbs/vol012item003_117R_L.jpg`

returns 502.

The catalogue proves that its editors read/normalized a local unit as `ḍhyāp` and understood it as a ten-sheet bundle.

It does **not** yet prove:

- how the unit is written on the bill;
- whether `ḍhyāp` is the exact original lexical form;
- whether `1,012` is a whole number, a compound/fractional figure or a flattened column value;
- whether the rate applies per ḍhyāp, per larger grouping, per hundred sheets or to different paper grades;
- whether the ten-sheet gloss comes from the document, cataloguer knowledge or another source.

Thus current evidence fields must remain separate:

`ORIGINAL_UNIT_READING = UNREAD`

`CATALOGUE_UNIT_TRANSCRIPTION = ḍhyāp`

`CATALOGUE_UNIT_GLOSS = 10 sheets`

`EXTERNAL_UNIT_VALIDATION = NOT_FOUND`

`ARITHMETIC_CONSISTENCY = FAILS_LITERAL_READING`.

---

## 7. External search for ḍhyāp is a controlled negative result

Searches were run for:

- `ḍhyāp`;
- `dhyap`;
- `ढ्याप`;
- `ध्याप`;
- `द्याप`;
- combinations with `paper`, `Nepali paper`, `kagaj / कागज`, `bundle` and `sheets`.

The only relevant historical-paper result returned is the Cambridge Hodgson catalogue itself.

Modern Nepali hits use phonetic/onomatopoeic or unrelated senses and do not validate the unit.

Therefore:

`NO_INDEPENDENT_LEXICAL_CONFIRMATION_FOUND_IN_CURRENT_WEB_SURVEY`.

This is not proof that the unit did not exist. It means the term cannot yet bear comparative weight outside the f.117 catalogue record.

Mechanism:

`SEARCH_FAILURE_LIMITS_NORMALIZATION_NOT_HISTORICAL_EXISTENCE`.

---

## 8. The f.117 arithmetic conflict is probably structural evidence, not merely a typo to fix casually

Literal catalogue normalization yields:

`1,012 ḍhyāp × 10 sheets = 10,120 sheets`.

That scale is difficult to reconcile with the catalogue's total NRs 79.30 and the rates transcribed as Rs 10/- and Rs 14/- per bundle, especially after wax cloth and thread/twine are included.

Do not solve this by choosing whichever number seems plausible.

Potential causes include:

- fractional notation flattened into `1,012`;
- multiple quantity columns concatenated;
- two grades of paper with separate rates;
- a rate applying to a larger count unit;
- unit hierarchy lost in prose transcription;
- catalogue transcription error.

Current state:

`ACCOUNT_STRUCTURE_LOST_IN_CATALOGUE_PROSE = HIGH_PROBABILITY_LEAD / CAUSE_UNRESOLVED`.

The original page layout is therefore indispensable evidence.

Mechanisms:

- `ACCOUNT_LAYOUT_ENCODES_UNIT_RELATIONS`
- `PROSE_CATALOGUING_CAN_DESTROY_TABULAR_ARITHMETIC`.

---

## 9. The paper-history article should compare counting regimes, not translate them into one another

Current controlled comparison:

### Company / English paper handling

`sheet`
-> `quire`
-> `ream`
-> `bundle/chest`.

Properties:

- package hierarchy explicit;
- cording-quire position affects quality;
- chest marks trace supply branches;
- quire sheet counts can themselves vary 24/25.

### Kashmir 1831

`sheet`
-> `dastā (24 finished sheets)`.

Properties:

- unit formed after finishing/burnishing;
- market/pricing unit.

### North Indian official glossary

`sheet`
-> `takhta (2, 4 or more sheets)`
-> `dasta (24 takhtas)`.

Properties:

- nested unit with variable sheet depth.

### Nepal Residency 1843

`sheet?`
-> `ḍhyāp?`
-> possible higher/parallel account unit.

Properties:

- catalogue gloss says ten sheets;
- original bill unread;
- arithmetic unresolved.

No horizontal conversion should be made across these systems without local evidence.

---

## 10. New census schema: quantity provenance

Add the following fields whenever paper quantities appear:

- `quantity_value_as_written`;
- `quantity_unit_as_written`;
- `catalogue_normalized_quantity`;
- `catalogue_unit_gloss`;
- `sheets_per_unit_direct_or_inferred`;
- `package_hierarchy`;
- `unit_region/institution`;
- `unit_date`;
- `price_unit`;
- `quality_grade`;
- `package_position`;
- `conversion_confidence`;
- `arithmetic_check`;
- `original_layout_read`.

This prevents historical local units from disappearing into a modern `number_of_sheets` column.

Mechanism:

`QUANTITY_PROVENANCE_IS_PART_OF_PAPER_PROVENANCE`.

---

## 11. Relation to Wave 64 and Wave 67

Wave 64 established that Nepali paper was a quantified input in a Residency bookmaking economy.

Wave 67 established that Company paper quality and supplier provenance were managed through reams, cording quires, marked chests and returned musters.

Wave 68 connects them through a stricter proposition:

**paper accounting units do not merely count material; they organize paper into packages that structure pricing, quality, handling, sampling and transport.**

Thus the article can compare:

`counting regime`
without claiming
`unit equivalence`.

---

## Source-control rules

1. Never publish `1,012 ḍhyāp = 10,120 sheets` as fact before direct inspection of f.117.
2. Keep `ḍhyāp` in romanized form exactly as Cambridge gives it and label it a catalogue transcription/editorial gloss.
3. Do not identify `ḍhyāp` with `dasta`, `quire`, `bundle` or any Nepali/Newar word from phonetic similarity.
4. Use Kashmir 1831 `dastā = 24 sheets` as a regional comparative case only.
5. Use Carnegy's `dasta = 24 takhtas` as evidence of unit variability, not as the Nepal definition.
6. Moxon's 20-quire ream is period technical control; actual Company supply counts must remain attached to direct Company evidence where possible.
7. Keep quantity, package hierarchy, price unit and quality grade as separate fields.
8. A catalogue prose sentence is not a substitute for reading columns, fractions and ditto marks in the original account.

## Immediate next actions

1. Recover f.117 recto through Wayback, migrated Cambridge media, BL imaging or direct archival request.
2. Recover ff.128–130 1827 bills and identify whether the same local paper unit recurs.
3. Search historical Nepali/Newar dictionaries, account manuals and paper-trade sources for the original unit form rather than only modern web pages.
4. Search other Hodgson bills for local quantity terms around paper, cloth, thread, books and manuscripts.
5. Directly inspect Jacquemont's published travel papers if a searchable edition exposes the 4 June 1831 Kashmir paper account.
6. Add quantity-provenance fields to the paper census protocol.
7. Compare paper package units with manuscript/package/box units only after maintaining stage-specific distinctions.

## Bottom line

The quantity of paper in Hodgson's archive cannot safely be reduced to modern sheet counts. English/Company paper moved in reams whose internal cording quires carried a quality gradient; Kashmir paper in 1831 was rolled into twenty-four-sheet dastās after finishing; North Indian official vocabulary later used `dasta` for a nested twenty-four-takhta unit; and Hodgson's 1843 Nepal bill survives only through a catalogue transcription of an unresolved `ḍhyāp` unit whose ten-sheet gloss and arithmetic still require the original page. **Counting paper was itself a material technology: the unit defined how sheets were bundled, priced, sampled, moved and audited.**