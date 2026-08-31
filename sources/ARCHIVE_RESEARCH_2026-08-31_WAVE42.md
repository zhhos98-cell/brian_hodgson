# Archive research wave 42 — from manuscript to sack to box: partial reconstruction of Hodgson's pre-archive shipment hierarchy

Date: 2026-08-31

Status: source-controlled partial reconstruction from the British Library Hodgson inventory. This wave distinguishes explicit historical container identifiers from modern catalogue terminology. Only joins supported by transcribed shipment/sack/box metadata are asserted.

## Executive result

The British Library inventory now supports a historical container hierarchy more specific than generic `bundle/package/box` language.

Evidence includes:

- pre-bound notebooks whose covers carry **original shipment numbers** in Nepali language/script;
- Newar notebooks whose **original sack numbers** are written in Nepali;
- a surviving contents sheet explicitly titled/described as **`Content of manuscripts from sack No. 8 of the original shipment`**;
- an individual Limbu manuscript whose own title description preserves **original sack number 8**;
- another documentary copy that preserves both an **original box and sack number** from the shipment;
- a separate surviving **content page of box No. 3 of original shipment**.

The resulting hierarchy is not yet fully reconstructed, but one historically grounded model is now available:

`document / notebook -> numbered sack -> numbered box -> shipment`.

The important mechanism is:

`NESTED_PAPER_CONTAINER_ADDRESSABILITY`.

Knowledge objects were made transportable not only by physical enclosure but by **nested identifiers written on paper boundary and contents surfaces**.

---

## 1. Distinguish modern catalogue words from historical identifiers

The BL inventory uses English descriptive terms such as:

- bundle;
- sack;
- box;
- shipment;
- cover page;
- title folio.

Some of these are modern translations/descriptions.

But the key evidence in this wave is stronger because the catalogue explicitly says original numbers occur **in Nepali language and script on historical covers**.

### Source-control rule

Use:

`original sack number` / `original shipment number` / `original box and sack number`

when the inventory says the historical surface carries that information.

Do not assume that every English `bundle` in the modern catalogue maps to the same historical Nepali container term.

---

## 2. MSS EUR HODGSON/4 — notebook cover joins title and original shipment number

Volume-level inventory statement:

all items are written in four pre-bound notebooks; in most cases the cover pages carry:

- a Nepali title;
- an original shipment number;
- both written in Nepali language/script.

### Mechanisms

- `NOTEBOOK_COVER_AS_SHIPMENT_IDENTITY_SURFACE`
- `LOCAL_SCRIPT_TRANSPORT_IDENTIFIER`.

### Relation

`textual identity + transport identity -> same cover surface`.

The cover is a join between semantic description and logistical address.

---

## 3. MSS EUR HODGSON/5 — shipment numbers are also described as original sack numbers

The volume contains six pre-bound notebooks whose covers normally carry Nepali titles and original shipment numbers.

For the `Jātamālā` / Newar caste-list notebooks, the catalogue is more specific:

- notebook titles are written in Nepali;
- **original sack numbers are written in Nepali**.

### Mechanism

`SACK_NUMBER_ON_NOTEBOOK_COVER`.

### Importance

The notebook is not merely inside a sack anonymously.

Its paper boundary carries a relation back to the transport container.

This makes later separation survivable at metadata level.

---

## 4. MSS EUR HODGSON/58 f.65 — sack No. 8 contents list survives

Shelfmark:

`MSS EUR HODGSON/58`, item 18, f.65.

Description:

`Content of manuscripts from sack No. 8 of the original shipment`.

Physical/documentary features:

- Nepali hand-made paper;
- Nepali language;
- list of manuscripts relating to customs and manners of different ethnic communities.

### Mechanisms

- `SACK_CONTENTS_LIST_SURVIVAL`
- `SACK_8_CONTENT_NODE`.

### Function

The sheet makes sack identity portable independently of the sack itself:

`sack No.8 -> paper contents list -> categories/items`.

This is a direct container checksum surface.

---

## 5. MSS EUR HODGSON/85 item 4 — an individual manuscript preserves sack number 8

Shelfmark:

`MSS EUR HODGSON/85`, item 4, ff.95–108.

Content:

Limbu traditional beliefs, rituals and prayers relating to agricultural cultivation, harvesting and marriage.

Material state:

- hand-made Nepali paper;
- small section mixed with slightly acidic paper;
- fine condition;
- fair writing;
- Nepali title description with Roman transliteration.

Crucial provenance field:

**original sack number (8) is mentioned in Nepali.**

### Mechanism

`INDIVIDUAL_ITEM_TO_SACK_8_JOIN`.

### Secure reconstruction

The item's subject — ritual/custom/agriculture/marriage — is compatible with the sack-8 contents sheet's broad `customs and manners of different ethnic communities` description.

More importantly, the **number itself** supplies the historical join.

Sequence:

`Limbu manuscript -> historical cover/title metadata = sack 8 -> sack-8 contents sheet`.

This is the first explicit item-to-container reconstruction in the current paper-centred pass.

---

## 6. The sack-8 reconstruction remains partial

Current online catalogue search has not exposed exact sack numbers for all candidate manuscripts.

Therefore do not infer that every ethnographic/customs manuscript in vols.56–60 or 83–85 belonged to sack 8.

### Evidence classes

- `EXPLICIT_JOIN`: historical sack number 8 recorded;
- `CONTENT_COMPATIBLE_ONLY`: subject resembles sack-8 contents description but no number transcribed;
- `UNKNOWN`.

### Rule

Only `EXPLICIT_JOIN` enters reconstructed membership.

---

## 7. MSS EUR HODGSON/1 item 8 — box and sack identifiers coexist

A second copy of a Nepalese narrative of Britain–Nepal relations survives on imported paper.

Its final page includes:

- Nepali title in Nagari;
- **original box and sack number at the time of shipment** in Nepali;
- additional Nepali words/numerals.

### Mechanisms

- `BOX_SACK_DUAL_IDENTIFIER`
- `NESTED_CONTAINER_METADATA_ON_ITEM`.

### Strong implication

At least one historical paper object was addressable simultaneously within two container levels.

This supports, without fully proving every intermediate relation, the model:

`item -> sack -> box -> shipment`.

---

## 8. MSS EUR HODGSON/55 f.129v supplies a box-level contents surface

Wave 41 established:

`f.129 verso: Content page of box No. 3 of original shipment`.

### Mechanism

`BOX_3_CONTENT_NODE`.

### Combined hierarchy

Evidence now exists for both:

- sack-level contents sheet;
- box-level contents page;
- item-level dual box+sack identifiers.

This is much stronger than treating container words as a flat list.

---

## 9. MSS EUR HODGSON/94 ff.40–44 supplies bundle-number/category metadata

This separated title/content set records:

- original shipment content;
- bundle numbers;
- categories;
- Nepali title description.

### Mechanism

`BUNDLE_NUMBER_CATEGORY_NODE`.

### Caution

Do not force `bundle = sack`.

The current catalogue may use different English words for historically distinct or overlapping container practices.

The relation between:

- bundle number;
- sack number;
- box number

must be solved from original wording/number joins, not English synonymy.

---

## 10. The hierarchy is paper-addressed at multiple levels

Potential address surfaces:

### Item/notebook level

- title;
- shipment number;
- sack number.

### Sack/bundle level

- cover page;
- contents list;
- number/category.

### Box level

- box contents page;
- box number.

### Shipment level

- aggregate list;
- destination/route documentation.

### Mechanism

`MULTILEVEL_PAPER_ADDRESS_SYSTEM`.

Physical containers become reconstructible because each level emits paper metadata.

---

## 11. Local-language metadata is structurally important

Repeated statements describe titles, shipment numbers and sack numbers written in:

- Nepali;
- Nagari script;
- sometimes mixed with other regional scripts/notations.

### Mechanism

`LOCAL_LANGUAGE_LOGISTICAL_METADATA`.

### HPS significance

Logistical addressability is not simply imposed later by English metropolitan cataloguing.

A local-script transport/index system already organizes parts of the research archive before institutional transfer.

This complicates any model of:

`local content -> metropolitan classification`.

The local production system itself contains classification and routing metadata.

---

## 12. Address systems accumulate rather than simply replace each other

One surviving item can now be represented as:

`historical title`

+ `historical sack number`

+ `historical box number`

+ `historical shipment relation`

+ `1921 volume/folio`

+ `modern catalogue item`.

### Mechanism

`LAYERED_DOCUMENT_ADDRESSABILITY`.

The paper does not carry one identity. It accumulates address systems produced by successive handling regimes.

---

## 13. Container numbering makes dispersal auditable

If an item is separated from its original sack or box but retains a sack/box number, a later actor can potentially reconstruct:

- former container membership;
- expected neighbors;
- missing items;
- shipment sequence;
- category relation.

### Mechanism

`CONTAINER_IDENTIFIER_AS_RECONSTRUCTION_KEY`.

This is the paper/logistics analogue of drawing-number joins in natural history, but paper remains the historical substrate carrying the identifier.

---

## 14. Partial reconstruction of sack No. 8

### Secure node A

`vol.58 f.65`:

sack No.8 contents list; customs/manners of different ethnic communities.

### Secure node B

`vol.85 item 4`:

Limbu ritual/agriculture/marriage manuscript; explicit original sack number 8 in Nepali.

### Relation

`A <-> B` by historical container number.

### Candidate nodes

Other manuscripts concerning customs/manners may prove to belong to sack 8, including material now dispersed across volumes 56–60 and 83–85, but they remain candidates until cover/sack numbers are read.

### Mechanism

`SACK_8_PARTIAL_RECONSTRUCTION`.

---

## 15. Why this matters for the paper article

The point is not merely that Hodgson used sacks and boxes.

The paper-history claim is:

**containers acquired durable epistemic identity because their numbers and contents were externalized onto paper surfaces that could survive the disappearance of the containers themselves.**

The paper surface converts a temporary transport relation into a potentially permanent provenance relation.

---

## 16. Cross-domain comparison, kept subordinate

### Zoological drawing number

joins drawing/specimen/behaviour note.

### Manuscript sack number

joins individual manuscript to container/shipment state.

### Shared operation

`identifier written on paper -> preserves relation after physical separation`.

### Paper-centred limit

The article need not turn this into a general information theory. It uses these comparisons only to show how paper marks make distributed scientific objects reconstructible.

---

## 17. New mechanism codes

- `NESTED_PAPER_CONTAINER_ADDRESSABILITY`
- `NOTEBOOK_COVER_AS_SHIPMENT_IDENTITY_SURFACE`
- `LOCAL_SCRIPT_TRANSPORT_IDENTIFIER`
- `SACK_NUMBER_ON_NOTEBOOK_COVER`
- `SACK_CONTENTS_LIST_SURVIVAL`
- `SACK_8_CONTENT_NODE`
- `INDIVIDUAL_ITEM_TO_SACK_8_JOIN`
- `BOX_SACK_DUAL_IDENTIFIER`
- `NESTED_CONTAINER_METADATA_ON_ITEM`
- `BOX_3_CONTENT_NODE`
- `BUNDLE_NUMBER_CATEGORY_NODE`
- `MULTILEVEL_PAPER_ADDRESS_SYSTEM`
- `LOCAL_LANGUAGE_LOGISTICAL_METADATA`
- `LAYERED_DOCUMENT_ADDRESSABILITY`
- `CONTAINER_IDENTIFIER_AS_RECONSTRUCTION_KEY`
- `SACK_8_PARTIAL_RECONSTRUCTION`

---

## 18. Immediate next tasks

1. Inspect/transcribe `vol.58 f.65` completely, preserving original Nepali wording for `sack` and category terms.
2. Inspect `vol.85 item 4` title/cover and capture exact historical sack-number notation.
3. Search all cover pages in vols.4–5, 56–60, 83–85 for sack number 8.
4. Reconstruct `box No.3` from vol.55 f.129v and identify whether its contents include numbered sacks/bundles.
5. Transcribe the original box+sack notation on vol.1 item 8.
6. Determine whether `sack`, `bundle`, and local historical container terms are equivalent or distinct.
7. Add hierarchy fields: `item_id`, `sack_id`, `bundle_id`, `box_id`, `shipment_id`, `historical_term`, `script`, `source_surface`.
8. Separate historical container number from modern folio/volume number in every dataset.
9. Do not infer sack membership from subject similarity without number/cover evidence.
10. Use the partial sack-8 reconstruction as a proof of method before attempting full shipment reconstruction.

## Bottom line

The Hodgson papers preserve enough pre-archive metadata to reconstruct at least one container relationship directly. A contents sheet identifies sack No.8 of an original shipment, and a surviving Limbu manuscript now bound elsewhere retains the same original sack number on its title metadata. Other records carry both box and sack numbers, while box No.3 has its own surviving contents page. The emerging architecture is a nested paper address system: manuscripts were not merely placed in sacks and boxes; their relationship to those containers was written onto covers and lists, allowing transport identity to survive later dispersal and rebinding.