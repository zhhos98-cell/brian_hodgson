# Web research wave 24 — 1845 reconciliation loop, subset catalogues, and copy-state counting failure

Date: 2026-08-31

Status: object-near reconstruction from ZSL digital-object transcriptions, with direct page-image verification of `NZSL/HOD/5/4/9` (3 Jan. 1845). This wave is deliberately the last public-source calibration before the next archive upload.

Core public archive: Zoological Society of London, Brian Houghton Hodgson papers, `NZSL/HOD/5/4`.

---

## 1. A primary copy already contains an internal counting conflict

### Source

`NZSL/HOD/5/4/9` — copy of Hodgson to the Trustees of the British Museum, 3 Jan. 1845.

ZSL page:
https://zsl-archive.maxarchiveservices.co.uk/index.php/copy-of-a-letter-from-brian-houghton-hodgson-to-the-trustees-of-the-british-museum

The two-page master PDF was inspected directly in the digital archive.

### Counts as written in the surviving copy

The opening tabulation gives:

- Drawings of Mammals: **15**
- Drawings of Birds: **70**
- tabulated drawings total: **85**
- Mammal skins: **402**
- Bird skins: **4,444**
- skins total: **4,846**
- Mammal osteological specimens: **406**
- Bird osteological specimens: **663**
- osteological total: **1,069**
- stated grand total: **5,996**

But later on the same surviving copy Hodgson writes that the drawings now presented amount to **eighty one**.

### Arithmetic

`4,846 skins + 1,069 osteological specimens = 5,915`.

- with 85 drawings: `5,915 + 85 = 6,000`
- with 81 drawings: `5,915 + 81 = 5,996`

The stated grand total therefore closes exactly with the later prose count of **81**, not with the opening tabulated total of **85**.

### Source-control rule

This archive item is explicitly a **copy of a letter**. The conflict is therefore direct evidence that the surviving copy-state contains incompatible numerical states. It does **not** by itself prove that the original letter delivered to the British Museum contained the same discrepancy.

Code provisionally as:

`COPY_STATE_COUNTING_CONFLICT`

rather than silently choosing 81 or 85.

### HPS value

This is an unusually clean microcase in which arithmetic exposes a metadata inconsistency inside the primary archival witness itself. The object is not merely evidence for a collection count; it is evidence for how copying/tabulation could introduce or preserve incompatible counts.

---

## 2. Hodgson explicitly treats numbered catalogues as a checksum for missing drawings

The same 3 Jan. letter states that the drawings form a regularly numbered sequel and that earlier drawings had fallen into different hands and were not all forthcoming.

Hodgson then says that the **numbered catalogues according to which the drawings were prepared and despatched from India** would provide a ready clue to the number of drawings that ought to be forthcoming.

He supplies species counts:

- Mammals of Nepal: **126**
- Birds of Nepal: **656**
- Mammals of Tibet: **47**

He immediately warns that most species were separately delineated and that many had **several delineations**.

### Mechanism

The catalogue therefore functions as a historical **expected-state register**:

`numbered catalogue -> expected drawings -> present holdings -> missing/forthcoming exception`.

But species count is not drawing count. The source itself prevents a simplistic one-species/one-drawing reconciliation.

This is stronger than the repo's earlier analytic language `catalogue = checksum`: Hodgson describes the operational use directly.

---

## 3. The February request formalises a received / retained / distributed reconciliation protocol

### Source

`NZSL/HOD/5/4/13` — Hodgson to J. Forshall, 4 Feb. 1845.

Hodgson asks the Keeper of Zoology to submit a **summary statement** showing totals of:

- what the Museum had **received**;
- what it had **retained**;
- what had been **distributed elsewhere**;
- separately for skins, bones and drawings.

He also specifies the destination order for duplicate skins:

India House -> Leyden -> Paris -> Berlin -> Frankfurt -> Edinburgh -> Dublin -> Newcastle -> Canterbury -> Manchester -> Earl of Derby.

Duplicate bones were to go first to the Royal College of Surgeons and ZSL, then through the same destination list as material permitted.

Crucially, Hodgson says he had already prepared **letters to accompany these specimens**, but was waiting for two things before sending them:

1. the Keeper's report of what was available;
2. the catalogue the Keeper was engaged to furnish.

### Mechanism

This is a formal synchronization sequence:

`receipt -> institutional sorting -> retained/distributed totals -> availability report -> catalogue -> destination letters -> physical distribution`.

Distribution is therefore not a simple act of giving duplicates away. It requires a reconciled institutional state before destination-level documentation can be completed.

---

## 4. Destination catalogues carried an explicit subset mask

### Source

`NZSL/HOD/5/4/14` — Hodgson to Leyden Museum, 5 Feb. 1845; same form adapted for Paris, Berlin, Frankfurt, Edinburgh, Dublin, Newcastle, Canterbury, Manchester, Earl of Derby and Hugh Strickland.

For Leyden Hodgson writes that he presents:

- **536 birds**;
- **69 mammals**, with a pencilled amendment to **70** in the ZSL transcription.

He says the transmitted catalogue lists **all** the birds and mammals discovered by him in Nepal for the trustees' information, while the particular species physically transmitted to the destination are **distinguished in the annexed catalogue by a cross prefixed**.

### Mechanism

This is more precise than `catalogue accompanies specimens`.

The destination receives:

`global descriptive universe + local physical subset marker`.

A prefixed cross acts as a historical **subset mask** mapping a destination's physical series onto the larger Hodgson/British Museum reference catalogue.

This is one of the cleanest examples in the repo of relational addressability being materially encoded for a distributed collection.

### Dataset implication

Add fields:

- `catalogue_scope = GLOBAL_COLLECTION`
- `destination_subset_marker = PREFIXED_CROSS`
- `subset_marker_semantics = PHYSICALLY_TRANSMITTED_TO_THIS_DESTINATION`
- `destination_count`
- `catalogue_version`

Do not assume the same physical subset at every destination merely because the same catalogue form was reused.

---

## 5. The British Museum tabular statement becomes a correction surface

### Sources

`NZSL/HOD/5/4/16` — memo of zoological collections delivered to the British Museum, c. 10 Feb. 1845.

`NZSL/HOD/5/4/17` — Forshall to Hodgson, 4 Mar. 1845.

The February memo attempts to tabulate the collection by destination and material class, including bird skins, mammal skins, bird bones, and mammal bones/horns.

Forshall then tells Hodgson in March that the **tabular statement** of his collections sent by Gray was hoped to be satisfactory.

Hodgson's pencilled marginal response states of the distribution statement:

**“full of omissions and inaccuracies”**

and asks for a copy **when correct**, adding that he would pay for its being copied.

### Mechanism

The audit loop is now directly visible:

`Hodgson requests reconciliation table -> museum compiles/transmits table -> Hodgson audits table -> exceptions detected -> corrected copy requested`.

The table is therefore not passive metadata. It is a mutable working object in a negotiated reconciliation process.

### Important control

Do not normalize the February, February-destination-letter, and July distribution numbers into one final matrix without page-level comparison. The surviving ZSL transcriptions show some count differences and ambiguous column alignments. These are **version-comparison targets**, not arithmetic errors to be repaired in the dataset.

---

## 6. Cross-media numbering makes separated osteology identifiable

### Source

`NZSL/HOD/5/4/31` — Hodgson to the Royal College of Surgeons, 1845.

Hodgson says his osteological remains were for the most part **duly numbered with reference to the series of skins and drawings** presented to the British Museum, and that species could therefore, for the most part, be identified at once.

### Mechanism

The number is not merely an accession label attached to one object class. It is a **cross-media relation key** linking:

`osteological specimen <-> skin <-> drawing`.

This gives a direct nineteenth-century statement of **relational addressability after physical separation**.

It also clarifies the limits of identifier evidence: numbering can recover species-level relation among media without necessarily proving that one bone, skin and drawing were produced from the exact same biological individual.

---

## 7. Gray explains why catalogue synchronization was necessary for nomenclatural standing

### Source

J. E. Gray to Hodgson, British Museum, 25 Dec. 1844 (`NZSL/HOD/5/2/12`).

Gray says that after the collection had been sorted and duplicates distributed into sets, they would form the catalogue of specimens and drawings. He asks for a complete list of Hodgson's publications because Indian periodicals were scarce in Britain and even less accessible on the Continent.

The key operational point is explicit: if specimens were sent without such a catalogue/work, their names would risk being treated as **mere manuscript names** and be little or not at all recorded.

### Mechanism

The catalogue does at least three things simultaneously:

1. synchronizes distributed material;
2. points distant users toward otherwise hard-to-find prior descriptions;
3. stabilizes the published/nomenclatural status of names attached to specimens.

Thus `metadata synchronization` is also a mechanism of scholarly priority and recordability.

---

## 8. Gray's publication note makes corrected catalogues part of the distribution design

### Source

`NZSL/HOD/5/4/35` — note by J. E. Gray regarding publications.

The note records an undertaking to prepare a **corrected Catalogue of the whole** and explicitly says it was to be **distributed with the specimens**, with a copy also sent to Hodgson.

This connects the distribution architecture directly to version control:

`corrected catalogue version -> physical duplicate sets -> recipient institutions + collector`.

The corrected catalogue is therefore designed from the start as a synchronization device, not merely as a later printed description of the collection.

---

## 9. Distributed duplicates could retain contemporary “type” standing

### Sources

`NZSL/HOD/5/4/19` — H. E. Strickland to Hodgson, 23 May 1845.

Strickland thanks Hodgson for **205 specimens of birds** and calls them “original and authentic types” of the novelties Hodgson had described.

`NZSL/HOD/5/4/21` — Strickland to Hodgson, 14 Jun. 1845.

Strickland reports that Gray had forwarded the Nepalese bird collection to him and says it would be of great service in identifying Hodgson's new species.

### Analytical consequence

A distributed series was not necessarily epistemically secondary merely because it was selected as duplicate material. At least one contemporary recipient treated the received set as evidentially authoritative for identifying Hodgson's novelties.

This reinforces the rule:

**`duplicate` is a distribution status, not automatically a low-evidence status.**

Its epistemic role must be reconstructed from selection, identifiers, catalogue synchronization and recipient use.

---

## 10. A direct material-audit sequence can now be reconstructed for early 1845

The public archive exposes the following sequence:

1. **3 Jan** — Hodgson delivers a counted batch and states that numbered catalogues can reveal missing drawings.
2. **23 Jan** — British Museum acknowledges the gift and begins deciding which osteological material to retain.
3. **23 Jan** — Hodgson offers the East India Company a quantified duplicate series.
4. **4 Feb** — Hodgson requests a formal `received / retained / distributed` summary by material class and defines recipient order.
5. **5 Feb** — destination letters pair physical sets with catalogues in which the local subset is marked by prefixed crosses.
6. **c. 10 Feb** — a distribution memo tabulates institutional allocations.
7. **4 Mar** — Forshall reports transmission of the tabular statement; Hodgson annotates it as full of omissions/inaccuracies and requests a corrected copy.
8. **May–Jun** — recipient Strickland receives a distributed series and uses it as identification/type material.
9. **later catalogue production** — corrected catalogue is intended to travel with specimens and maintain synchronized names/descriptions across nodes.

This is a much denser audit cycle than `donation -> museum catalogue`.

---

## 11. New mechanism: reconciliation surface

### Definition

**Reconciliation surface** = a list, table, catalogue, receipt or annotated copy on which expected and observed collection states can be compared, exceptions recorded, and a corrected state requested or propagated.

Historical examples now include:

- Hodgson's numbered drawing catalogues used to infer what ought to be forthcoming;
- British Museum received/retained/distributed summary statement;
- Hodgson's marginal criticism of omissions/inaccuracies;
- destination catalogues whose prefixed crosses mark the locally transmitted subset.

This is narrower than `catalogue` and broader than `receipt`.

### Test

For each archival list/table ask:

- what state is it supposed to represent?
- what other state can be compared against it?
- what is the counting unit?
- does it encode expected, observed, retained, missing or distributed material?
- can corrections be written back?
- is a corrected version propagated to another node?

---

## 12. Distinguish three levels of addressability

Wave 20 separated addressability levels. Wave 24 gives direct historical controls:

### Level 1 — object addressability

Can an institution find/retain the physical item?

Example: received/retained/distributed table.

### Level 2 — relational addressability

Can the item be linked back to another representation/object class?

Example: numbered osteological remains keyed to skins and drawings.

### Level 3 — historical-event addressability

Can the surviving relations prove that this particular object participated in a specific event, such as description of a taxon or preparation of a drawing?

Numbers and catalogue marks strengthen but do not automatically establish this strongest relation.

The 1845 materials therefore support a graded model rather than a binary `identified/unidentified` field.

---

## 13. Immediate archive-upload tests generated by this wave

When new archive images enter the repo, highest-yield checks are now sharply defined:

1. **count-state test** — does a working copy disagree internally with its own totals or later copy?
2. **subset-marker test** — crosses, ticks, underlining, destination initials or other marks indicating a distributed subset within a global list;
3. **received/retained/distributed test** — can one list be assigned to one of these operational states?
4. **correction-surface test** — marginal corrections, totals, recalculation, requests for fair/corrected copies;
5. **cross-media-key test** — does one number explicitly bridge specimen/drawing/bone/list?
6. **expected-state test** — is a list being used to infer what ought to exist or arrive, rather than only what is present?
7. **version-propagation test** — was a corrected list/catalogue copied or sent to multiple physical recipients?
8. **copy-state test** — distinguish draft, retained copy, sent original, fair copy, printed catalogue and annotated printed copy before reconciling numerical differences.

---

## Bottom line

Wave 24 closes the pre-upload public-source run with a complete material audit loop. Hodgson did not simply send specimens and later receive a catalogue. He used numbered catalogues as expected-state checks for missing drawings; requested explicit tables of what the British Museum had received, retained and distributed; paired destination specimen sets with global catalogues whose locally transmitted species were marked by crosses; audited the Museum's distribution statement and rejected it as incomplete/inaccurate; and relied on shared numbers to reconnect separated bones, skins and drawings. Even the surviving 3 Jan. **copy** contains an internal 81/85 drawing-count conflict whose arithmetic can be diagnosed from the document itself. The history of the collection is therefore recoverable as repeated acts of reconciliation among physical objects, counts, identifiers, lists and copy states.