# Web research wave 23 — manuscript redundancy as error control, collation, and distributed witness design

Date: 2026-08-31

Status: cross-domain calibration using Burnouf–Hodgson manuscript correspondence and later catalogue/provenance controls. The key request for multiple copies is preserved in later published transcription/citation of Burnouf's 15 July 1837 letter; direct manuscript image remains desirable.

## 1. Three cases arrive; receipt is immediately followed by textual use

Royal Asiatic Society archival descriptions preserve two Burnouf letters dated 15 July 1837:

- one acknowledges the safe arrival of **three cases of manuscripts** at the Société Asiatique;
- another acknowledges receipt of the Sanskrit Buddhist copies, names particular works including a fine `Rakṣābhagavatī`, and moves directly into textual discussion.

Jules Mohl independently writes on 29 July 1837 from the Société Asiatique Secretariat reporting arrival of the three crates.

### Mechanism

This is a clean manuscript custody sequence:

**three-case transport receipt -> item/work recognition -> scholarly reading/use.**

The two July acknowledgments already show that container-level receipt and work-level identification are distinct stages.

---

## 2. Burnouf deliberately requests duplicate textual witnesses

In his 15 July 1837 correspondence Burnouf asks Hodgson for further copies of selected texts.

The surviving published transcription/citation makes the rationale unusually explicit:

- many copies appeared to have been produced rapidly;
- they were therefore generally faulty;
- for difficult passages, one copy alone could not secure the sense;
- **two different copies were indispensable for comparison**.

Later scholarship reconstructs Burnouf as wanting two or three copies of the same texts so they could be collated.

### Mechanism: redundancy as error control

The extra copy is not primarily a dissemination duplicate.

It is an **independent witness used to diagnose scribal error**.

The operational sequence is:

**copy A ambiguous/faulty -> copy B/C requested -> variants compared -> reading stabilized.**

This is a direct manuscript analogue to the repo's broader `error-control redundancy` mechanism.

---

## 3. Duplicate does not mean interchangeable replica

Burnouf's request depends on difference between copies.

If two copies reproduced exactly the same scribal error, redundancy would provide little additional information. The value comes from partially independent copying histories.

### Consequence

For manuscript census work, distinguish:

- `duplicate_for_distribution`;
- `parallel_copy_for_collation`;
- `copy_from_same_exemplar`;
- `copy_from_independent_exemplar`;
- `copy_relationship_unknown`.

The word `copy` must not imply informational equivalence.

---

## 4. Copy multiplicity became geographically distributed

Later reconstruction shows repeated Hodgson copies of the same Buddhist works entering different institutional collections.

Examples include `Kāraṇḍavyūha` copies sent across multiple destinations, including the Asiatic Society of Bengal, Royal Asiatic Society, Bodleian, Société Asiatique and Burnouf's own holdings; `Guṇakāraṇḍavyūha` copies similarly entered several institutions.

The exact copy genealogy must be reconstructed title by title and should not be inferred solely from matching titles.

### Mechanism

A textual tradition becomes a **distributed witness network**.

The network can support later collation even when the original commissioning purpose differed across copies.

---

## 5. Burnouf's philological workflow exploited cross-institutional redundancy

Later accounts of Burnouf's *Saddharmapuṇḍarīka* work show him collating manuscripts from different holdings, including manuscripts associated with the Société Asiatique, Bibliothèque/BnF and British collections.

### HPS significance

The scholarly object is produced through comparison of physically separated witnesses.

This means textual authority can increase **after separation**, provided enough identity/provenance relations survive to reunite witnesses intellectually.

This is almost the inverse of the relation-loss cases elsewhere in the repo.

---

## 6. Comparison with zoological duplicates

The word `duplicate` now clearly covers different epistemic operations in the two domains.

### Manuscript duplicate

Typical high-value use:

- compare variants;
- diagnose scribal error;
- reconstruct a more secure reading;
- test ambiguous passages.

### Zoological duplicate

Typical 1845 British Museum use:

- retain a reference series;
- distribute comparative sets;
- exchange specimens;
- extend institutional coverage;
- provide multiple institutions with representative material.

### Shared infrastructure

Both depend on **controlled redundancy**.

### Different error model

Manuscript redundancy helps recover a text by comparing non-identical witnesses.

Zoological redundancy distributes multiple physical exemplars of a taxon while metadata must preserve which individual is which.

Do not collapse these into one generic `duplicate economy` without recording operation.

---

## 7. Redundancy has a cost structure

Burnouf's request for additional copies was not free. Later reconstruction places the July 1837 manuscript commission in a monetary range of roughly £25–30.

The project already has upstream evidence that copying could be priced by textual extent and that paper, scribal labour, binding and shipment were separately costed.

### Mechanism

Error-control redundancy is materially produced:

**paper + scribal labour + time + copying supervision + packaging + shipment -> comparative witness.**

This joins the 1827 manuscript-production economy directly to Burnouf's philological error-control strategy.

---

## 8. Receipt redundancy and witness redundancy are different

The 15 July Burnouf and 29 July Mohl acknowledgments provide two institutional statements that the same three crates arrived.

This is a different kind of redundancy from parallel manuscript copies.

### Custody redundancy

Multiple acknowledgments strengthen evidence that a transport event occurred.

### Witness redundancy

Multiple textual copies strengthen the capacity to resolve textual error.

### Rule

Record what redundancy is intended to verify:

- custody event;
- object count;
- textual reading;
- taxonomic identity;
- distribution state;
- publication/priority claim.

---

## 9. A new field: redundancy purpose

Add controlled values:

- `CUSTODY_CONFIRMATION`;
- `TEXTUAL_COLLATION`;
- `REFERENCE_SERIES`;
- `DISTRIBUTION_SET`;
- `EXCHANGE_DUPLICATE`;
- `BACKUP_COPY`;
- `PUBLICATION_SYNCHRONIZATION`;
- `UNKNOWN`.

For every apparent duplicate, ask:

**duplicate for what operation?**

---

## 10. Cross-domain claim now available

A stronger formulation is possible:

> Hodgson's infrastructures repeatedly used redundancy as a way to make distributed knowledge auditable, but redundancy was operation-specific. Burnouf requested multiple manuscript copies precisely because one rapidly made witness was not trustworthy enough to secure a reading; British Museum zoologists retained and redistributed duplicate specimens to create reference and comparative series. In both cases, multiplication did not eliminate identity problems. It created a new requirement to preserve relations among copies, specimens, lists and representations.

---

## 11. Archive tests

The next manuscript batch should test:

1. whether multiple copies show explicit shared or independent exemplars;
2. whether copyists, dates, paper stocks or colophons distinguish witness genealogy;
3. whether Hodgson lists mark requested duplicates or destinations;
4. whether Burnouf requests can be mapped to surviving BnF/Société/RAS shelfmarks;
5. whether textual variants are visibly corrected through comparison in marginalia or later copies;
6. whether packing/accounting records separately price duplicate copying.

## Bottom line

Wave 23 shows that manuscript multiplication was itself an epistemic technology. Burnouf requested two or more copies of difficult Buddhist texts because rapidly produced manuscripts were error-prone and one witness could not secure the sense. This creates a precise cross-domain comparison with Hodgson's zoological duplicate sets: both systems use redundancy to control uncertainty, but manuscripts use independent textual witnesses for collation while museums use duplicate physical specimens for reference, comparison and distribution. Redundancy therefore belongs in the repo as an operation-specific verification mechanism, not a generic property of abundance.
