# Archive ingestion wave 25 — Linnean, Kew, SOAS and self-archive batch

Date: 2026-08-31

Status: first-pass archive-side ingestion from newly uploaded OCR/vision JSONs. Claims below are kept at witness level. Low-confidence handwriting is quarantined for image-level transcription rather than silently normalized.

## Executive result

Public-source Waves 17–24 had already reconstructed a set of mechanisms around catalogues, reconciliation, copy states, receipt, distribution, manuscript production and retrospective self-archiving. The newly uploaded archival batch now supplies object-near witnesses for several of those mechanisms across distinct domains.

The strongest immediate findings are:

1. **1838 Linnean zoological catalogue as an active research state**, not a passive species list: Hodgson explicitly sends a classified catalogue through Wallich, inserts characters of new forms, marks some group distinctions as provisional, and frames further enquiry as capable of revising the grouping.
2. **Kew Inwards Book as a custody/receipt surface**: a register entry records material as received from Hodgson, with origin and botanical contents. This is an institutional conversion from moving material to locally addressable receipt metadata.
3. **Lepcha manuscript copies designed for future translation**: a later India Office description states that the Hodgson copies were physically laid out with blank space on the right for translation, with Nepalese translation already inserted in places. The page architecture itself therefore encodes a planned downstream operation.
4. **A later printed zoological checksum layer** preserves separate totals for specimens and drawings, explicitly distinguishes sheets from subjects, states that a British Museum reference series was retained while duplicates were distributed, and can now be compared against the 1844–45 ZSL reconciliation sequence from Wave 24.
5. **The 1868 Testimonials volume is a self-built reputation archive**: Hodgson labels a book as testimonials to the value of his labours in literature, science and education and gathers external assessments across Buddhism, zoology, ethnology and education.

Taken together, the archive batch strengthens the repo's central question: heterogeneous knowledge objects became usable after movement through deliberately constructed intermediate surfaces — catalogues, registers, layouts, numbering systems, copied texts, distribution tables and retrospective dossiers.

---

## A. Linnean DA-ENG-2-SP-514 — Classified Catalogue of Nipalese Mammals, 1838

### Witness

Shelfmark/file: `Linnean DA-ENG-2-SP-514 Hodgson B. H, 尼泊尔生物目录（林奈风）纸张、布局、地方知识、转交痕迹、折痕`

Visible archival metadata:

- Hodgson B. H.
- 1838
- SP 514
- letter heading: Resident at the Court of Nepal
- sent 20 Feb. 1838 to the Secretary, Linnean Society

### Direct content

Hodgson says he submits, **through his friend Dr. Wallich**, a **Classified Catalogue of all the mammals known to him as inhabitants of Nepal**. He states that he has inserted characters of the new forms.

Crucially, the document does not present classification as closed. Hodgson expresses doubt about the necessity and sufficiency of a separation within Cervidae while noting that the proposed forms help connect larger groups; he expects further enquiry to furnish better grounds of distinction.

The following page names five other new forms in OCR as:

- Cuon
- Urva
- Ursitaxus
- Bibos
- Pantholops

The catalogue pages then proceed through ordered taxonomic entries, repeatedly distinguishing established names, varieties and Hodgson's `nob.` forms.

### Mechanism

Code as:

`ACTIVE_CATALOGUE_STATE`

The catalogue is simultaneously:

- a descriptive inventory;
- a classification proposal;
- a record of uncertainty;
- a transmission object sent through Wallich;
- a consolidation surface for descriptions previously published piecemeal in the Asiatic Society's journal.

This matters because a catalogue can preserve a **versioned epistemic state** rather than merely a final list.

### Repo implications

Add to the article spine under object-making/auditability:

`field observation/publication fragments -> classified catalogue -> explicit provisional grouping -> institutional transmission -> later revision/comparison`

This is also a clean bridge between the pre-1845 zoological working regime and the later British Museum/ZSL reconciliation regime.

### Material follow-up

The uploaded file name indicates paper, layout, transfer traces and folds as research targets. OCR text alone cannot support claims about watermark, sheet manufacture, fold chronology or transfer annotations. Those require image-level inspection of recto/verso.

Priority: **P0 / direct article evidence**.

---

## B. Kew Inwards Book 1848–1858 — receipt from Hodgson

### Witness

File: `Adobe Scan 2025年3月26日 (1)`

Volume cover OCR:

- Royal Botanic Gardens, Kew
- Inwards Book
- 1848–1858
- `10-52`

A register page contains an entry OCRed approximately as:

`Received Jan. 27th from Mr. Hodgson. Sikkim. Seed[s] of 15 ... Rhododendron and of Hill Bamboo ...`

The exact species-count wording and elevation figure are not secure in OCR and must be checked against the image before quotation.

### Mechanism

Code as:

`INSTITUTIONAL_RECEIPT_REGISTER`

The register converts an incoming consignment into a local metadata tuple that appears to include:

- receipt date;
- sender;
- geographic origin;
- material form (`seeds`);
- taxonomic/plant identity;
- possibly altitude/elevation information.

This is a botanical analogue to the repo's `custody checksum` and `institutional legibility` mechanisms. The important act is not only shipment but institutional inscription at arrival.

### Repo implications

The Kew register gives an archive-side test for the distinction:

`physical arrival != complete scientific incorporation`

A received entry proves that Kew converted the arrival into a register state. It does not by itself prove germination, survival, identification, cultivation, redistribution or later accession continuity.

Priority: **P0**, with manual verification of the Hodgson entry.

---

## C. SOAS MS380882 — List of Lepcha Manuscripts in the Hodgson Collection

### Witness state

File: `SOAS MS380882 Papers of Dr. Rene Nevesky - Wojkowitz`

This is a later scholarly/institutional description of the Hodgson Collection preserved at the India Office Library, not an original Hodgson-era production list.

### Direct content

The list states that the Lepcha books in the India Office Library are, possibly with one exception, **copies prepared for Brian Hodgson with the view of future translation**.

The physical evidence cited by the describer is especially important:

- empty space to the **right side of the Lepcha text**;
- Nepalese translation already inserted **here and there**.

The describer also distinguishes at least two hands and notes that books written or dictated by `bong thing` or `mun` ritual specialists can show difficult handwriting and orthographic errors.

### Mechanism

Code as:

`TRANSLATION_READY_COPY_LAYOUT`

The manuscript copy was not simply a duplicate textual carrier. Its page architecture reserved a zone for a future transformation.

Operational sequence:

`local text / dictation -> prepared copy -> reserved translation field -> partial Nepalese gloss/translation -> anticipated fuller translation`

This is one of the strongest manuscript-side examples in the repo of **future work being materially designed into the object**.

### Caution

Because the statement comes from a later descriptive list, it should be coded as retrospective physical inference unless the original Lepcha manuscripts themselves are inspected.

The inference is still high-value because it is tied to observable page layout rather than biography alone.

Priority: **P0/P1**. Next target should be original manuscript images that show the blank translation column and partial Nepalese insertions.

---

## D. Later printed Hodgson collection tables — distribution and counting ontology

### Witness

File: `Adobe Scan 2025年3月28日`

This large printed source contains several appendices and retrospective lists relevant to the repo. It should not be treated as a primary 1840s distribution witness without identifying the exact publication and edition, but it supplies checksum targets for comparison with ZSL and British Museum records.

### Zoological totals and distribution

One table gives:

- birds: 9,512 specimens
- mammals: 903
- reptiles etc.: 84
- total specimens: 10,499

The accompanying text states that these were presented to the British Museum in 1843 and 1858; a series was reserved by the Museum, together with the reptiles, and the remaining duplicates were distributed to principal European and American societies.

A separate drawings table gives:

- bird drawings: 1,241 sheets
- mammal drawings: 557 sheets
- reptiles etc.: 55 sheets
- total drawings: 1,863 sheets

The printed note explicitly warns that **all drawings are on folio sheets and many sheets contain several subjects**.

### Mechanisms

Code as:

- `RETROSPECTIVE_DISTRIBUTION_CHECKSUM`
- `SHEET_SUBJECT_COUNT_ONTOLOGY`

The second is especially important. It independently confirms the repo rule that a physical support unit and a represented-object count are not interchangeable.

`1 sheet != 1 drawing subject`

This is directly analogous to manuscript work/volume/bundle count distinctions.

### Wave 24 comparison target

The later totals must be compared, not merged, with the 1844–45 ZSL copy-state counts and destination tables. Differences may reflect:

- different date states;
- 1843 vs 1858 cumulative gifts;
- sheet vs subject counts;
- retained vs distributed states;
- later reconstruction;
- counting or transcription error.

Do not normalize the figures into one master total before source-state reconciliation.

Priority: **P0 as checksum, P2 as direct evidential witness**.

---

## E. India Office manuscript gift and catalogue-copy infrastructure

The same printed file contains:

`LIST OF MSS. PRESENTED BY MR. HODGSON TO THE INDIA OFFICE LIBRARY, AUGUST, 1864.`

and an appendix headed:

`CATALOGUES OF HODGSON COLLECTION. (Copies distributed.)`

The India Office list preserves trunk/bundle organisation and a mixed-language manuscript donation structure. OCR elsewhere in the file records one grouping as 36 Sanskrit sastras, 17 Lepcha and 14 Limbu books.

The catalogue appendix identifies Hodgson manuscripts in the Royal Asiatic Society Library as catalogued by Cowell and Eggeling and published in 1876.

### Mechanisms

These sections give later cross-institutional checksum surfaces for:

- gift composition;
- trunk/bundle hierarchy;
- manuscript language/category counts;
- catalogue dissemination;
- divergence between transport/container identity and later bibliographic identity.

Priority: **P1**, especially for comparison against original India Office lists and SOAS/BL holdings.

---

## F. 1868 Testimonials volume — reputation as a constructed archive

### Witness

File: `Adobe Scan 2025年3月28日 (5)`

Hodgson's autograph title is OCRed clearly enough to establish the core act:

`Testimonials to the value of my labours in literature, science and education ... Mar. 12 1868. B. H. Hodgson`

The volume contains copied/collected endorsements from published and private assessments.

A related scanned printed source preserves, among others:

- Richard Owen, British Association report, May 1863, linking Hodgson's Buddhist research with his collection of skulls of different tribes as an ethnological contribution;
- Barnard Davis, British Association, May 1863, describing Hodgson's attention to human natural history through physical, philological, linguistic and intellectual aspects, and praising the Koch/Bodo/Dhimal work.

### Mechanism

Code as:

`SELF_CURATED_REPUTATION_DOSSIER`

This is stronger than the generic category `self-archive` because the operation is explicit:

`external testimony -> selection -> copying/collection -> disciplinary juxtaposition -> bound personal evidence dossier`

The volume turns distributed external judgments into a portable, internally ordered proof of value.

It should be analysed alongside later lists, corrected reprints and Hodgson's retrospective priority claims.

Priority: **P1 / article secondary spine**, potentially strong for a concluding section on recursive archive and reputation.

---

## G. Linnean certificate of recommendation, 1834

### Witness

File: `Linnean DA-EN-G-1-CR-48 Certificates of Recommendation including Brian Houghton Hodgson`

OCR securely catches:

- proposed in November 1834;
- a recommendation text describing Hodgson in connection with East India Company service / residence at the Nepal court and scientific/literary contribution;
- multiple signatures, including OCR-readable names such as Thomas Bell, N. B. Ward, S. B. Booth and W. A. Broderich, with several other signatures requiring manual transcription.

### Mechanism

Code provisionally as:

`INSTITUTIONAL_CREDENTIAL_ASSEMBLY`

The certificate is an institutional recognition surface: personal knowledge, offices, scientific work and signatory standing are compressed into a fellowship recommendation object.

Potential later comparison:

`1834 others certify Hodgson -> 1868 Hodgson curates others' certifications`

This creates a long arc from externally assembled credential to self-assembled reputation archive.

### Caution

Exact wording and full signatory list require image-level transcription. Do not quote the OCR text as prose.

Priority: **P1**.

---

## H. Linnean letter from The Rangers, Dursley, 15 May 1861

File: `Linnean DA-ENG-9-LL-8 ...`

The date and place are secure enough:

- The Rangers, Dursley
- 15 May 1861

The handwriting OCR is not reliable enough to establish the precise request/declination. It appears to concern attendance at a Linnean Society meeting on the 24th, but this remains unverified.

Code only as:

`NEEDS_IMAGE_TRANSCRIPTION`

Do not build a `late-career withdrawal`, `self-refusal` or attendance claim until the page is read directly.

Priority: **P0 transcription task, P2 argument**.

---

## I. Kew JDH-2-22-2 Hooker–Hodgson correspondence

The uploaded OCR is extensive but handwriting recognition is too unstable for claim extraction. Search surfaces possible late-career material on scientific networks, human antiquity/evolution, honours and Hodgson's public standing, but these phrases are currently contaminated by OCR substitutions.

This file should be treated as a **high-value transcription reservoir**, not a text source ready for synthesis.

Recommended protocol:

1. identify page/date/sender/recipient visually;
2. transcribe only passages containing archive-relevant operations or explicit scientific discussion;
3. mark uncertain readings;
4. separate Hooker voice from Hodgson voice;
5. then compare with printed correspondence or external dating aids.

Code:

`HANDWRITING_OCR_UNSAFE`

Priority: **P1 reservoir**, not yet evidence.

---

## J. Corrected autograph / Buddhist symbols material

File: `Adobe Scan 2025年3月28日 (3) (1)` includes a witness headed `NOTICE ON BUDDHIST SYMBOLS` with `corrected autograph` visible in OCR and a letter dated The Rangers, near Dursley, 26 Sept. 1860.

The text describes a compiled corpus of Buddhist symbols drawn from coins, temples, statues, pictures and illuminated manuscripts. Hodgson states that the Nepal symbols were copied and supervised by men of the Buddhist creed, while the intended explanatory project was displaced by other work and left without the planned explanations.

### Mechanism

Code as:

`ABANDONED_EXPLANATION_CORPUS` + `CORRECTED_PUBLICATION_STATE`

Operational sequence:

`distributed visual sources -> copied symbol corpus -> intended local explanation -> interruption/no completed explanations -> later corrected publication/autograph state`

This is useful because it preserves a failed or incomplete knowledge-making pipeline rather than only a finished publication.

Priority: **P1**.

---

## K. SOAS PPMS 77/2/2 Limbu texts

This file contains later translations/notes on Limbu material in the Hodgson Collection, including a historical text attributed in OCR to Joghan Singh Phago Limbu (1843) and later translation by I. S. Chemjong.

Its value is primarily:

- provenance of local-language material within the Hodgson Collection;
- evidence of later translation/re-description layers;
- possible recovery of named local textual authors/voices.

It is not yet a strong object-operation witness at the same level as the Lepcha copy-layout description.

Priority: **P2**, with provenance control.

---

## L. Items to hold back from the Hodgson corpus pending attribution

`Adobe Scan 2025年3月26日 (2)` includes later Kew Inwards Book material (1873–1877) and an OCR entry `From W. Hodgson`. Do not attribute this to Brian Houghton Hodgson without independent identification.

The 2016 Linnean programme on Nepalese biodiversity is useful orientation and explicitly highlights forgotten local collaborators and correspondence networks, but it is modern historiographical/contextual material rather than primary evidence for the mechanisms above.

---

## Cross-domain synthesis after first archive scan

The new archival batch suggests that the repo's strongest general claim can now be phrased more concretely:

**Hodgson's knowledge infrastructure repeatedly built intermediate representational surfaces that allowed a moving or incomplete collection to remain operable across distance and time.**

Those surfaces differ by domain:

- zoology: classified catalogue, number, specimen/drawing relation, distribution table;
- botany: inwards register;
- manuscripts: copy layout with translation reserve, trunk/bundle list, catalogue;
- Buddhist images: copied symbol corpus and corrected publication state;
- reputation: certificate and testimonial dossier.

They perform related operations:

- preserve expected relations;
- expose provisionality;
- stage future work;
- translate movement into institutional metadata;
- distinguish physical unit from semantic unit;
- enable later comparison or redistribution;
- permit retrospective reconstruction.

The strongest comparative formulation is therefore not simply `paper carried knowledge`. It is:

`paper/document surface -> makes a relation explicit -> relation survives separation -> later actor can compare, revise, route, translate or reconstruct`.

## Immediate next tasks

1. Manually transcribe the Kew Inwards Hodgson entry.
2. Image-read the 1861 Linnean letter before using the user's `self-refusal` interpretation.
3. Image-read the 1834 recommendation certificate for full wording, signatories, folds and watermark/material evidence.
4. Sample original Lepcha manuscript pages to verify the right-hand translation reserve described in the later list.
5. Reconcile later printed zoological totals (10,499 specimens; 1,863 sheets of drawings) against the 1844–45 ZSL states from Wave 24 rather than treating them as final truth.
6. Extract only date-secure, speaker-secure Hooker–Hodgson letters from JDH-2-22-2.
7. Add archive-side fields to the census schema: `witness_state`, `operation_encoded`, `future_operation_reserved`, `receipt_register_state`, `physical_unit`, `semantic_unit`, `retrospective_checksum`, `ocr_reliability`.

## Bottom line

The upload arrived at the right moment. Waves 17–24 created explicit tests; this archive batch immediately returns positive evidence for catalogue versioning, receipt inscription, translation-ready manuscript layout, count-unit separation and retrospective evidential assembly. The next phase should be controlled transcription and cross-witness reconciliation, not another broad public-web sweep.