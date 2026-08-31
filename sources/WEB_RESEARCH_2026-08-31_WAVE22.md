# Web research wave 22 — catalogue as checksum, correction surface, and metadata synchronization network

Date: 2026-08-31

Status: direct archival-transcription reconstruction from ZSL Hodgson correspondence and memos, especially 1844–1847. This wave supplies unusually explicit historical statements of mechanisms previously inferred from the broader archive.

## 1. Hodgson explicitly describes numbered catalogues as a completeness check

In his formal 3 January 1845 letter to the Trustees of the British Museum, Hodgson discusses the drawings being presented with the zoological collections.

He says the drawings form a **regularly numbered sequel** to the existing series and gives their physical format as approximately 20 by 12 inches. He urges the Museum to recover earlier drawings that had passed through various hands and were not all forthcoming.

Most importantly, he states that the **numbered catalogues according to which the drawings had been prepared and dispatched from India would provide a ready clue to the amount of drawings that ought to be forthcoming**.

He then gives species-count controls:

- Mammals of Nepal: 126;
- Birds of Nepal: 656;
- Mammals of Tibet: 47.

He notes that most species had individual delineations and some had several delineations.

Primary source:
ZSL `NZSL/HOD/5/4/9`, Hodgson to Trustees of British Museum, 3 Jan 1845.

### Mechanism: catalogue checksum

This is direct historical evidence that the numbered catalogue/list was designed to support **reconstruction after dispersal**.

The catalogue could answer:

- how many numbered representations should exist;
- which parts of a sequence were absent;
- what earlier distributed drawings ought to be recovered.

The repo's `custody checksum` concept can therefore be sharpened:

- a receipt checks arrival at transport-unit granularity;
- a numbered catalogue can check **expected relational completeness** of a distributed representation series.

This is not a retrospective analytic metaphor. Hodgson explicitly uses the catalogue as a clue to what ought to be present.

---

## 2. Correction was incorporated before publication

On 26 July 1844 J. E. Gray writes to Hodgson that a list had already been printed off. Gray says the list included **the corrections Hodgson made when he read the list over in London**.

Gray insists the list had been made out carefully and verified, and discusses nomenclatural changes made in response to Hodgson's prior naming.

Primary source:
ZSL `NZSL/HOD/5/2/10`, Gray to Hodgson, 26 Jul 1844.

### Mechanism: pre-publication correction loop

The sequence is directly visible:

**Hodgson list/names -> museum compilation -> Hodgson reads proof/list -> corrections -> printing.**

This is the zoological equivalent of a catalogue-production workflow with author/donor feedback before fixation in print.

### Important nuance

Gray's claim that the list was carefully verified does not make later error impossible. It records a **verification event and confidence claim** that can be compared against later corrections.

Store:

- `verification_claim_as_written`;
- `verification_actor`;
- `later_error_detected`;
- `correction_incorporated_before_print`.

---

## 3. Catalogue disagreement was treated as productive rather than merely erroneous

On 29 January 1847 Gray writes while copies of the completed catalogue were being sent to Hodgson. He says he hopes it will satisfy Hodgson, while acknowledging there are points on which they may differ. Gray explicitly frames such differences as capable of eliciting truth, in contrast to easy compliance perpetuating error.

Primary source:
ZSL `NZSL/HOD/5/2/20`, Gray to Hodgson, 29 Jan 1847.

### Mechanism

The printed catalogue is not presented as a final consensual metadata layer. It is a **published comparison surface on which disagreement remains legitimate and expected**.

This matters for Hodgson's later annotated copies: annotation can be read as continuation of an already acknowledged correction/disagreement regime rather than simply personal grievance.

---

## 4. The completed catalogue was tied to the distributed specimen network

On 29 April 1847 Hodgson acknowledges receipt in Darjeeling of **twelve copies** of the catalogue.

He describes it as founded on his own catalogues and corrected in synonymy by Gray under British Museum authority.

He then gives explicit distribution instructions for the remaining copies:

1. one copy should go to each public institution, abroad and in Britain, **to which duplicate specimens had been transmitted under the Trustees' auspices**;
2. remaining copies should go to prominent individual zoologists;
3. copies should carry a presentation inscription from Hodgson.

Named intended individual recipients include Temminck, Cuvier, Geoffroy Saint-Hilaire, H. Smith, Owen, Falconer, Yarrell, Ogilby and Sykes, with copies also reserved for Hodgson's father.

Primary source:
ZSL `NZSL/HOD/5/2/21`, Hodgson to J. Forshall, 29 Apr 1847.

### Mechanism: metadata synchronization network

The catalogue is deliberately sent along the same institutional topology created by duplicate specimen distribution.

The network becomes:

**master/reference collection -> duplicate specimen sets -> recipient institutions -> printed catalogue copies.**

The printed catalogue provides recipient nodes with a common descriptive/indexing surface for physically separated objects.

This is one of the strongest direct sources for the article's auditability argument.

### New claim

**Duplicate distribution and catalogue distribution are paired operations.**

Physical replication alone does not produce a usable distributed collection. A metadata copy must travel as well.

---

## 5. Catalogue copies themselves become distributed provenance objects

Because Hodgson instructed copies to follow duplicate specimens, a surviving institutional copy of the 1847 catalogue may preserve evidence of:

- intended specimen recipient status;
- institutional synchronization with British Museum nomenclature;
- Hodgson presentation inscription;
- later local annotations/corrections;
- divergence between local specimen holdings and catalogue state.

### Archive strategy

When possible, census institutional **copies of the catalogue**, not only editions.

Fields:

- `copy_id`;
- `recipient_institution_or_person`;
- `presentation_inscription`;
- `specimen_set_received`;
- `annotation_present`;
- `local_shelfmark`;
- `later_binding`;
- `provenance_chain`.

The catalogue copy is part of the distributed collection infrastructure.

---

## 6. Drawings could be added after catalogue work had already begun

On 23 April 1845 Gray tells Hodgson that mammal drawings had not yet arrived, but says this had not delayed work because they could be **added to the catalogues as soon as they arrived**. Bird examination and comparison were taking much longer than anticipated. Gray also planned a visit to Leiden to make comparisons.

Primary source:
ZSL `NZSL/HOD/5/2/18`, Gray to Hodgson, 23 Apr 1845.

### Mechanism: asynchronous incorporation

Catalogue production did not require every related medium to arrive simultaneously.

The working system could absorb:

- specimens first;
- drawings later;
- comparative results from another museum later still.

Thus the catalogue is an **asynchronously updated relational object**.

This also means that absence of a drawing at one production stage need not imply permanent separation or non-use.

---

## 7. Museum comparison extended beyond the receiving institution

Gray's planned Leiden visit shows that British Museum catalogue work itself depended on external comparison collections.

The relevant verification network therefore includes not only:

**Hodgson -> British Museum**

but:

**Hodgson material <-> British Museum material <-> Leiden comparison material <-> printed classification.**

Institutional cataloguing is geographically distributed even before duplicates and printed catalogues are redistributed outward.

---

## 8. Missing publication and missing acknowledgment were also custody problems

In his 28 February 1845 letter to H. Piddington at the Asiatic Society in Bengal, Hodgson complains that zoological papers and specimens sent in 1842–43 had not been properly acknowledged/published, even while their contents appeared in reports by the curator.

He explicitly links papers and specimens: some specimens had initially been lent for examination in relation to papers and were subsequently donated.

Primary source:
ZSL `NZSL/HOD/5/2/17`, Hodgson to Piddington, 28 Feb 1845.

### Mechanism

Custody includes **credit/publication state**, not only physical possession.

A specimen can:

- arrive;
- be examined;
- generate reported knowledge;
- remain formally unacknowledged;
- be associated with an unpublished paper.

This produces a priority/reputation failure without physical loss.

The archive should therefore separate:

- `physical_receipt_acknowledged`;
- `donation_acknowledged`;
- `paper_received`;
- `paper_published`;
- `information_used_in_report`;
- `credit_attribution`.

---

## 9. A stronger model of catalogue function

Wave 22 now identifies at least five historically demonstrated catalogue functions:

1. **expectation/checksum** — indicate what drawings ought to exist/be forthcoming;
2. **correction surface** — incorporate Hodgson's pre-print corrections;
3. **comparison surface** — preserve productive disagreement between Hodgson and Gray;
4. **synchronization device** — accompany duplicate specimen distributions to recipient institutions;
5. **asynchronous integration device** — accept drawings/comparative results after catalogue work has begun.

This is much stronger than treating catalogue as final description.

---

## 10. Catalogue synchronization versus catalogue versioning

Wave 21 established `version-purpose filtering`.

Wave 22 adds a second dimension:

### Versioning through time

Different catalogue states represent changing collections/classifications.

### Synchronization across space

Copies of a catalogue are distributed so multiple institutions can interpret separated objects against a shared descriptive state.

The analytical model therefore needs two axes:

- **diachronic version control**;
- **synchronic metadata synchronization**.

A distributed collection can fail on either axis:

- institutions may hold different catalogue versions;
- local annotations may diverge;
- specimen sets may change without metadata updates;
- catalogues may circulate without all intended specimens or vice versa.

---

## 11. Direct cross-domain payoff

The manuscript side has now yielded:

- government metadata forms;
- paid catalogue labour;
- work/volume segmentation;
- Hunter/Mitra version correction.

The zoological side yields:

- numbered catalogue as completeness check;
- proof corrections before printing;
- distribution of catalogue copies with duplicate specimens;
- later Hodgson annotated copies;
- asynchronous addition of drawings;
- external comparison visits.

### Shared mechanism

**Institutional knowledge objects require synchronized descriptive infrastructures, not only custody.**

### Domain difference

Manuscript synchronization emphasizes work identity and internal segmentation.

Zoological synchronization emphasizes specimen/representation/name relations and distribution state.

---

## 12. New preferred archive targets

Wave 22 changes archive priority slightly upward for:

1. presentation copies of the 1847 catalogue held at known duplicate-recipient institutions;
2. Hodgson's three annotated 1863 copies;
3. Gray working lists with Hodgson's 1844 corrections;
4. drawings lists showing expected versus forthcoming numbers;
5. recipient institutions' accession lists that can be compared with Hodgson's intended distribution;
6. Asiatic Society receipt/acknowledgment records for the 1842–44 papers/specimens.

## Bottom line

Wave 22 provides direct historical evidence for the strongest current thesis. Hodgson explicitly treated numbered catalogues as clues to drawings that ought to be forthcoming; Gray incorporated Hodgson's corrections before printing; the completed catalogue was deliberately distributed to institutions that had received duplicate specimens; and catalogue production continued asynchronously as drawings and external comparisons arrived. Catalogue infrastructure therefore performed both **version control through time** and **metadata synchronization across space**. This is the clearest evidence yet that nineteenth-century circulation required reconstructibility after separation, not movement alone.
