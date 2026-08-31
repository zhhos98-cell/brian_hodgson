# Archive research wave 34 — negative receipts, recovery states, and provenance-preserving reintegration

Date: 2026-08-31

Status: custody-state reconstruction from ZSL/RAS/British Museum correspondence and list descriptions. This wave deliberately separates dispatch, intermediary arrival, institutional receipt, rediscovery, reintegration, metadata repair, and physical irrecoverability instead of treating all uncertain drawings as one category of `lost material`.

## Executive result

Waves 29–33 reconstructed the production relation graph, independent metadata failure channels, asynchronous catalogue/distribution processing, a local research office, and its hybrid fiscal/administrative status. Wave 34 follows drawings through custody failure and recovery and shows that `loss` itself had several historically distinguishable states.

At least four custody failures can now be separated:

1. **dispatch claimed / institutional receipt negative** — in 1837 Hodgson reported drawings and boxes sent toward the Royal Asiatic Society, while the RAS minutes recorded that none of the expected articles had been received;
2. **intermediary arrival known / onward state unexplained** — in 1843 Hodgson complained that 31 large sheets sent in May 1842 had effectively disappeared after their known arrival;
3. **material later found / delivery pending instruction** — in December 1844 Gray reported that 50 bird drawings had been found at the Zoological Society and were waiting for Hodgson's instructions for delivery;
4. **expected material known / physical recovery judged unrealistic** — in March 1845 the British Museum told Hodgson there was no realistic prospect of recovering mammal drawings from Mr Howard's receiver.

The archive also preserves a recovery/reintegration state. `HOD/1/1` contains a dedicated `List of Drawings (new series) received from the Zoological Society, March 1845`, while an undated working memo distinguishes `recent` drawings from those `first recd from Zool Socy`.

The stronger mechanism is therefore:

`custody uncertainty -> rediscovery/recovery -> route/provenance retained -> metadata checked/corrected -> reintegration`.

Auditability means not simply preventing loss, but preserving enough relations to distinguish **which kind of custody failure occurred** and how a recovered object re-entered the working collection.

---

## 1. Replace generic `lost drawings` with a custody-state ontology

Proposed states:

- `DESPATCH_CLAIMED`
- `INSTITUTIONAL_RECEIPT_NEGATIVE`
- `INTERMEDIARY_ARRIVAL_KNOWN`
- `ONWARD_STATE_UNKNOWN`
- `REDISCOVERED_AT_INSTITUTION`
- `DELIVERY_AWAITING_INSTRUCTION`
- `RECOVERED_FROM_PRIOR_CUSTODY`
- `REINTEGRATED_WITH_PROVENANCE`
- `METADATA_REPAIR_REQUIRED`
- `PHYSICAL_RECOVERY_UNLIKELY`
- `FINAL_RECOVERY_UNPROVEN`

General rule:

`despatched != received`

`received at intermediary != forwarded`

`found != delivered`

`recovered != correctly identified`

`historically identifiable != physically recoverable`.

---

## 2. 1837 — conditional routing and a negative receipt

### Source

`NZSL/HOD/5/2/24`, extracts from the Minutes of the Committee of Correspondence of the Royal Asiatic Society, 7 Nov. 1837.

Hodgson's communication reported material dispatched toward RAS custody, including **26 sheets of mammals and birds**. A second January consignment was entrusted to Captain Robinson with instructions conditioned on the existing location of Hodgson's stores at the Zoological Society.

The RAS minute records that **none of the above articles had been received**.

### Mechanisms

- `NEGATIVE_RECEIPT_EVENT`
- `CONDITIONAL_ROUTING_AMBIGUITY`
- `NEGATIVE_CUSTODY_CHECKSUM`

The route depended on a state check:

`Captain Robinson -> determine whether prior Hodgson stores remained with ZSL -> deposit with RAS if required`.

A later investigator can therefore know that Hodgson initiated a transfer without being able to localize exactly where the custody handoff failed.

### Count control

Public transcription surfaces disagree over the second consignment, reading it as five vs eight boxes/units. Preserve this as:

`PUBLIC_TRANSCRIPTION_COUNT_CONFLICT_5_VS_8`.

Do not project the conflict onto the original manuscript until the master image is inspected.

---

## 3. Negative receipt is a positive archival event

The RAS did not merely leave a silence. Its committee explicitly recorded non-receipt and carried the matter forward.

### Mechanism

`NEGATIVE_CUSTODY_CHECKSUM`

Sequence:

`expected transfer -> institutional check -> negative receipt recorded -> unresolved matter preserved`.

An absence becomes historically addressable because the receiving body records that an expected object is not present.

---

## 4. 1842–43 — known arrival followed by an accountability gap

### Source

`NZSL/HOD/5/2/4`, Hodgson to H. Torrens, 12 Jan. 1843.

Hodgson recalls transmitting **31 large sheets of drawings** on 13 May 1842, accompanied by a list, for Society inspection and then onward transmission to England if approved.

His complaint is unusually precise: the drawings had allegedly disappeared without explanation from the time of their **known arrival**.

### Mechanisms

- `KNOWN_INTERMEDIARY_ARRIVAL`
- `ONWARD_ACCOUNTABILITY_GAP`

State chain:

`dispatch -> intermediary arrival known -> inspection/forwarding expected -> later location/onward transfer unexplained`.

This differs fundamentally from 1837, where the institution explicitly recorded non-receipt.

### Data implication

Keep separate:

- `sender_dispatch_state`
- `intermediary_arrival_state`
- `institutional_receipt_state`
- `onward_transfer_state`
- `acknowledgment_state`
- `later_location_state`.

---

## 5. The 31-sheet package crossed later disciplinary boundaries

The May 1842 list begins with ethnographic/human figures and continues through mammals and birds.

### Mechanism

`CROSS_DOMAIN_TRANSFER_PACKAGE`

The transport unit did not respect later archive categories such as ethnography, mammalogy and ornithology.

`transport/package identity != later disciplinary identity`.

A recovery search restricted to one later discipline can therefore miss a historical shipment's unity.

---

## 6. December 1844 — 50 bird drawings are `found` at the Zoological Society

### Source

J. E. Gray to Hodgson, late Dec. 1844.

Gray reports hearing from Mr Rees that the Zoological Society had **found 50 drawings of birds**, but was waiting for Hodgson's instruction before delivering them. Gray urges Hodgson to write to the Society.

### Mechanisms

- `INSTITUTIONAL_REDISCOVERY`
- `DELIVERY_AWAITING_OWNER_INSTRUCTION`

Immediate state:

`object present at institution -> rediscovered/recognized as Hodgson material -> transfer paused pending routing instruction`.

### Caution

`found at ZSL` does not yet prove identity with:

- the missing 31 sheets of 1842;
- the uncertain 1837 consignments;
- any particular later total.

Code only:

`RECOVERY_CANDIDATE_NOT_IDENTIFIED`.

---

## 7. March 1845 — a dedicated recovery list exists

### Source

`NZSL/HOD/1/1 — Lists of drawings and specimens sent to various recipients`, 1842–1874.

The file description explicitly includes:

`List of Drawings (new series) received from the Zoological Society, March 1845`.

### Mechanism

`RECOVERY_LIST_SURFACE`

This is probably the highest-value next object for resolving the early drawing custody chain because it may encode:

`ZSL-held state -> recovered/returned state`.

### Required comparison

Collate against:

- Dec. 1844 `50 drawings found`;
- Hodgson master/original series;
- Jan. 1845 Gray/Gerrard receipt;
- May 1842 Torrens 31-sheet list;
- 1837 numbered drawing lists.

Chronology alone is insufficient for object identity.

---

## 8. Working memo preserves ZSL provenance after recovery

### Source

`NZSL/HOD/5/2/26`, undated memo sent to J. E. Gray regarding drawings, manuscripts and papers.

The memo refers to Gray holding a drawing list for correction and distinguishes:

- `recent`, meaning drawings given to Gray/Gerrard; and
- those **`first recd from Zool Socy`**.

### Mechanism

`PROVENANCE_PRESERVING_REINTEGRATION`

Recovered objects were not necessarily merged anonymously into the current collection. Their route/source state remained visible in the working list:

`current drawing -> current collection -> prior source/custody = ZSL`.

Reintegration can therefore preserve the recovery event as part of documentary identity.

---

## 9. Recovery and metadata repair are separate stages

### Source

`NZSL/HOD/5/2/27`, undated J. E. Gray letter.

Gray tells Hodgson that a list is **correct in the numbers** but that the names are `ludicrously wrong`, attributing the corruption to the ignorance of the copier. Hodgson is expected to recognize the intended objects and names are to be corrected when the list returns.

Wave 30 separately established Gray's concern that bird numbering itself could contain collisions/errors.

### Mechanisms

- `IDENTIFIER_SURVIVES_NAME_CORRUPTION`
- `COPYIST_METADATA_ERROR`
- `RECOVERY_CORRECTION_LOOP`

Sequence:

`material/list recovered or circulated -> copied names corrupted -> some identifiers remain usable -> Hodgson reviews/recognizes -> names corrected -> repaired list returns`.

Physical recovery and metadata recovery are different operations.

---

## 10. March 1845 — historically known material can be physically unrecoverable

### Source cluster

The ZSL `HOD/5/4` sequence records:

- Hodgson's Feb. 1845 request for help recovering a set of mammal drawings from Mr Howard;
- British Museum reply of 4 Mar. 1845 stating that there was no realistic chance of recovery from Mr Howard's receiver.

### Mechanism

`KNOWN_OBJECT_PHYSICAL_RECOVERY_FAILURE`

The archive can preserve knowledge that a drawing set existed, its expected relation to Hodgson's corpus, its former possessor, and the attempt to recover it, even when the physical copy is inaccessible.

`historically addressable != physically recoverable`.

---

## 11. Master originals preserve auditability after copy-custody failure

The Dec. 1844 correspondence establishes that Hodgson retained his own **original drawings**, from which transmitted drawings were copied.

### Mechanism

`MASTER_STATE_SURVIVES_COPY_CUSTODY_FAILURE`

The retained master can support reconstruction of:

- number;
- subject;
- expected transmitted state;
- series completeness.

It cannot automatically reconstruct the missing copy's exact route, later annotation or condition.

Redundancy preserves relations/expected states, not complete object biography.

---

## 12. Parallel recent and recovered drawing states coexist in 1845

A British Museum/Gerrard receipt around 1 Jan. 1845 records **81 drawings** delivered directly in the Canterbury/British Museum sequence.

At roughly the same time, older drawings were still being found and recovered through ZSL channels.

HOD/5/2/26 explicitly distinguishes recent Gray/Gerrard drawings from those first received from ZSL.

### Mechanism

`PARALLEL_RECENT_AND_RECOVERED_DRAWING_STATES`

A later total can combine components with different custody genealogies:

`recent delivery + recovered prior transmission + other earlier holdings`.

This may eventually help explain some 1844–45 count discrepancies, but no arithmetic reconciliation should occur until the March 1845 recovery list is transcribed.

---

## 13. `Received from ZSL` is itself an object state

The phrase `List of Drawings (new series) received from the Zoological Society, March 1845` is analytically significant.

The list is organized by a **custody event**, not merely by subject or taxon.

### Mechanism

`CUSTODY_EVENT_AS_LIST_IDENTITY`

Historical lists can be generated because a transfer occurred; the custody event creates the documentary surface.

---

## 14. Later collection records explicitly preserve dated count states

`NZSL/HOD/1/1` also contains mammal drawing lists described as:

- numbered by sheets according to the **Count of February 1870**;
- numbered by sheets according to the **Count of July 1874**.

### Mechanism

`DATED_COUNT_STATE_LIST`

The archive's own descriptive language treats counts as temporally situated states.

This validates the repo rule:

`count = observation at a particular date/operation`, not timeless collection cardinality.

The same logic should govern the bird 1,104 / 1,115 / 1,125 sequence.

---

## 15. Destination is a versioned state, not always an accomplished movement

The same HOD/1/1 file records ethnographic drawings whose intended destination changed:

- Jan. 1873: to Sir John Lubbock;
- May 1873: altered to the Christie Collection.

### Mechanism

`DESTINATION_REVISION_BEFORE_TRANSFER`

Rule:

`destination annotation != destination receipt`.

A routing note may represent intention, instruction, revision or completed transfer.

---

## 16. 1869 — posthumous destination is preassigned before the custody event exists

HOD/1/1 includes an August 1869 memo by Hodgson `in event of his death`, assigning portfolios — two mammal and four bird portfolios — to the Zoological Society.

### Mechanism

`POSTHUMOUS_DESTINATION_PREASSIGNMENT`

Custody metadata can point forward:

`present private custody -> anticipated death -> future institutional destination`.

The archive therefore contains **prospective provenance**.

---

## 17. 1875 — present user and terminal destination are separated

A 30 Jan. 1875 letter from P. L. Sclater thanks Hodgson for information concerning bird drawings in Hume's hands and says Hume will receive a copy so that he has due notice of the drawings' destination.

### Mechanism

`TEMPORARY_USER_WITH_DEFERRED_DESTINATION`

State distinction:

`current user/custodian = Hume`

while

`future/terminal destination = ZSL`.

Ownership/intended destination, physical possession and active research use can occupy different nodes.

---

## 18. Custody-state graph for drawings

The natural-history relation graph should now carry explicit event/state nodes:

`PRODUCED`

`NUMBERED / LISTED`

`MASTER / WORKING STATE`

`COPIED FOR TRANSMISSION`

`DESPATCHED`

`INTERMEDIARY ARRIVAL`

`INSTITUTIONAL RECEIPT`

`NOT RECEIVED`

`ONWARD LOCATION UNKNOWN`

`FOUND / REDISCOVERED`

`DELIVERY PENDING INSTRUCTION`

`RECOVERED FROM PRIOR INSTITUTION`

`REINTEGRATED WITH PROVENANCE`

`METADATA REPAIR`

`TEMPORARY LOAN/USE`

`DESTINATION PREASSIGNED`

`DESTINATION REVISED`

`FINAL INSTITUTIONAL RECEIPT`

`PHYSICAL RECOVERY FAILED`.

Each transition requires its own witness.

Never infer:

`DESPATCHED -> RECEIVED`

or

`FOUND -> SAME AS EARLIER MISSING SET`

without explicit identifier/list comparison.

---

## 19. Cross-domain mechanism: physical preservation with relational repair

### Drawings

`object/copy exists -> route breaks -> later numbers/lists permit rediscovery -> provenance retained -> names/relations repaired`.

### Manuscripts

`physical volume exists -> catalogue segments/names incorrectly -> deeper inspection permits re-identification and correction`.

### Shared mechanism

`PHYSICAL_PRESERVATION_WITH_RELATIONAL_REPAIR`

Physical survival or recovery does not complete the epistemic task. A second operation must restore identity, relation, sequence, naming, destination or provenance.

---

## 20. Article-level refinement

**Hodgson's lists, numbers and retained originals did more than prevent loss. They made different kinds of loss distinguishable. A drawing could fail to arrive, arrive and then disappear institutionally, be rediscovered awaiting routing instructions, re-enter the collection with its prior custody still marked, require metadata repair after recovery, or remain historically identifiable while physically unrecoverable. Auditability consisted partly in preserving enough external relations to identify which failure had occurred.**

This is more precise than saying redundancy simply reduced error.

---

## 21. New mechanism codes

- `NEGATIVE_RECEIPT_EVENT`
- `CONDITIONAL_ROUTING_AMBIGUITY`
- `NEGATIVE_CUSTODY_CHECKSUM`
- `KNOWN_INTERMEDIARY_ARRIVAL`
- `ONWARD_ACCOUNTABILITY_GAP`
- `CROSS_DOMAIN_TRANSFER_PACKAGE`
- `INSTITUTIONAL_REDISCOVERY`
- `DELIVERY_AWAITING_OWNER_INSTRUCTION`
- `RECOVERY_CANDIDATE_NOT_IDENTIFIED`
- `RECOVERY_LIST_SURFACE`
- `PROVENANCE_PRESERVING_REINTEGRATION`
- `IDENTIFIER_SURVIVES_NAME_CORRUPTION`
- `COPYIST_METADATA_ERROR`
- `RECOVERY_CORRECTION_LOOP`
- `KNOWN_OBJECT_PHYSICAL_RECOVERY_FAILURE`
- `MASTER_STATE_SURVIVES_COPY_CUSTODY_FAILURE`
- `PARALLEL_RECENT_AND_RECOVERED_DRAWING_STATES`
- `CUSTODY_EVENT_AS_LIST_IDENTITY`
- `DATED_COUNT_STATE_LIST`
- `DESTINATION_REVISION_BEFORE_TRANSFER`
- `POSTHUMOUS_DESTINATION_PREASSIGNMENT`
- `TEMPORARY_USER_WITH_DEFERRED_DESTINATION`
- `PHYSICAL_PRESERVATION_WITH_RELATIONAL_REPAIR`

---

## 22. Immediate falsification targets

1. Obtain/transcribe the actual `List of Drawings (new series) received from the Zoological Society, March 1845`.
2. Compare that list against Gray's Dec. 1844 `50 drawings found` statement.
3. Compare both against Hodgson's master originals/numerical catalogue to identify the recovered series.
4. Compare the March 1845 list with the 31-sheet May 1842 Torrens list; reject or confirm overlap species-by-species rather than by chronology.
5. Resolve the 1837 5/8 second-consignment transcription conflict from the master image.
6. Identify Mr Rees and the ZSL administrative event that led to rediscovery of the 50 drawings.
7. Reconstruct the Howard custody chain and receiver context to establish where physical recoverability ended.
8. Date HOD/5/2/26–27 by their distribution counts/correspondence sequence.
9. Test copyist-corrupted names against surviving numbered lists/objects.
10. Add custody-state nodes and `intended_destination` vs `actual_receipt` edges to the zoological relation graph.
11. Compare February 1870 and July 1874 mammal drawing count lists at item level.
12. Trace the bird drawings from Hume's research custody through the 1875 destination notice to final ZSL receipt.

## Bottom line

Wave 34 shows that Hodgson's archive did not merely survive episodes of loss and dispersal. Its numbers, lists, master states, receipts and correction loops made **custody failure itself classifiable**. The same drawing could be known as sent, not received, arrived but unaccounted for, found, waiting for routing, recovered with prior source still marked, or historically identifiable yet physically unrecoverable. That differentiation is a central part of what `auditability after separation` meant in practice.