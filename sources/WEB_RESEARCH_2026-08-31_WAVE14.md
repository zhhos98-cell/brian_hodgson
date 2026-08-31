# Web research wave 14 — Fort William counting ontologies, catalogue conversion, and institutional legibility

Date: 2026-08-31

Status: mixed primary-catalogue / contemporary institutional-object / later-reconstruction wave. The core purpose is to stop forcing `work`, `bundle`, `volume`, and `catalogue entry` into a single count and instead reconstruct the conversions among them.

## 1. The immediate problem

The Fort William evidence now exposes at least three apparently incompatible counts around Hodgson's 1827 manuscript transfers:

- **109 bundles** received on 11 May 1827;
- **127 physical volumes**, described later in 1827 as `ponderous`, in a larger Hodgson collection at the College;
- **66 Sanskrit Buddhist works** later listed by W. W. Hunter as having been obtained from the Fort William library after having originally been forwarded there by Hodgson.

These figures should **not** be treated as failed versions of one underlying inventory.

They belong to different operational ontologies:

- `bundle` = transport / receipt / custody unit;
- `volume` = physical library unit;
- `work` = textual/title identity;
- `catalogue entry` = institutional descriptive unit.

The relevant historical question is how objects were converted from one unit system into another after arrival.

---

## 2. 11 May 1827 — 109 bundles: receipt verifies only the transport granularity

British Library `Mss Eur Hodgson/12 item 23, f.176`, as described by the Cambridge Hodgson inventory, is a receipt for the arrival of **109 bundles of Oriental manuscripts** sent by Hodgson to the College of Fort William for its library.

Catalogue:
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol012.html

The document gives a clean `custody checksum` at bundle level. It confirms that a counted transport aggregation reached the receiving institution. It does not by itself specify:

- how many textual works were inside;
- how many physical volumes or codices were represented;
- whether one work occupied multiple bundles;
- whether multiple works shared one bundle;
- whether every bundle was subsequently unpacked, identified and catalogued;
- whether later additions became merged with the May receipt corpus.

### Rule

Store `109 bundles` as `TRANSPORT_COUNT`, not as a manuscript-title count.

---

## 3. August 1827 — the corpus was still growing

The same Cambridge inventory describes `Mss Eur Hodgson/12 item 24, ff.177–178`:

- William Carey to Hodgson, 24 August 1827, expressing appreciation for manuscripts;
- copy of a Government letter dated 16 August 1827 concerning a **cash advance for further purchases**.

This matters chronologically. The 11 May receipt cannot automatically be equated with every Fort William Hodgson manuscript counted later in the year. The acquisition programme remained active after May.

Therefore a larger count in November need not indicate repacking, counting error or unexplained accretion. It may reflect a genuinely enlarged collection.

---

## 4. 12 November 1827 — 127 `ponderous` volumes and a competence bottleneck

G. S. A. Ranking's history of the College of Fort William, based on College proceedings, reports that on **12 November 1827** Lieutenant J. A. Ayton offered to ascertain the contents of a larger collection of manuscripts purchased for the College Library by Hodgson of the Nepal Residency.

Ranking reports:

- **127 volumes**;
- described by the College Secretary as **`ponderous`**;
- Ayton's offer was referred to Government;
- Captain Price and Dr Carey were consulted about his competence;
- Ayton was ultimately judged not competent and his offer was declined.

Ranking cites College proceedings: `Proc. XI, pp. 346–350`.

Digital search witness:
https://ignca.gov.in/Asi_data/31293.pdf

### Source-control warning

The IGNCA PDF is large and the present web interface exposed the passage through indexed search text but did not permit page-image inspection. The wording and proceeding citation should be checked against the PDF page image or archival `Proc. XI` before publication quotation.

### Why this is high-value

Institutional incorporation depended on more than physical custody. The College had a collection sufficiently materialised to count as 127 volumes, yet **the contents were not institutionally transparent**. Access to them was mediated by judgments about linguistic/scholarly competence.

This creates a new mechanism:

**receipt → physical library object → expert identification → catalogue legibility.**

The bottleneck is not transport but **competent description**.

---

## 5. 109 bundles and 127 volumes should not be arithmetically reconciled

The May and November figures differ both in date and counting unit.

Possible relations include:

1. some bundles contained more than one bound or bindable volume;
2. some physical volumes required multiple transport bundles;
3. items were rebound or assembled after receipt;
4. further manuscripts acquired after the August cash advance entered the November collection;
5. `bundle` and `volume` simply partitioned the material according to different institutional operations.

At present none should be selected as the explanation.

### Dataset rule

Do not calculate a `127 - 109 = 18 missing/added objects` field. The subtraction has no historical meaning until the unit conversion is demonstrated.

---

## 6. Hunter's 1896 list: 66 works is a retrospective title ontology

Sir William Wilson Hunter, *Life of Brian Houghton Hodgson* (1896), Appendix A, states that Hodgson's Sanskrit Buddhist works sent to Calcutta in 1827 and originally given to the Fort William Library comprised **66** items in its List VI.

Internet Archive full text:
https://archive.org/stream/lifeofbrianhough00hunt/lifeofbrianhough00hunt_djvu.txt

Hunter's heading is especially important. He describes List VI as:

> List of 66 Sanskrit Buddhist Works obtained from the Library of the College of Fort William, and forwarded thereto by B. H. Hodgson, Esq., from Nepal.

He immediately warns that **some titles are uncertain**, while others were **identified and corrected from manuscripts in the preceding five lists**.

### Consequence

Hunter's 66 is not a transparent survival of the 1827 receipt count. It is a later **work/title reconstruction**, already incorporating cross-list correction and re-identification.

That makes Hunter useful precisely because he exposes an evidential afterlife:

**physical custody did not freeze textual identity; later cataloguers reconstructed names by comparison across distributed witnesses.**

Store `66` as `RETROSPECTIVE_WORK_TITLE_COUNT`, not `1827_RECEIPT_COUNT`.

---

## 7. The Fort William catalogue itself survives as a material knowledge object

BULAC/BINA holds **MS.PERS.130**, `Catalogue of books in the library of the college of fort William`, dated broadly **1821/1836**.

Record:
https://bina.bulac.fr/s/fort-william-college/ark:/73193/bqrg86

BINA describes it as:

- anonymous;
- written in **Persian**;
- arranged by subject;
- organised in **four columns**:
  1. shelfmark;
  2. title;
  3. condition of the copy;
  4. quality of the handwriting;
- written in Nastaʿlīq;
- with marginal `balaġa` collation marks;
- on **Indian laid paper**;
- in a binding of about 1821 of a type associated with the College of Fort William;
- dating range 1821/1836.

The BINA JSON record exposes a large image/media sequence, so the catalogue appears to be digitally imaged even though the linked Internet Archive shortcut currently does not resolve cleanly.

### Analytical importance

This is not merely evidence that the College possessed a catalogue. It identifies the categories through which a book became institutionally legible:

**shelf location + textual title + physical condition + handwriting quality.**

Condition and hand are not marginal antiquarian observations; they are built into the catalogue's tabular grammar.

The catalogue therefore performs a conversion:

**physical book/volume → located, named, condition-assessed, script/hand-assessed institutional record.**

---

## 8. Catalogue language is itself an access technology

MS.PERS.130 is written in Persian, not English or Romanised title forms. The catalogue could therefore be perfectly functional for one institutional-linguistic regime while remaining difficult to use for another.

Ranking's later history reports a mid-1830s problem around Oriental manuscript catalogues: their contents had not been made institutionally legible through translation/Roman-character title representation to the satisfaction of the later administration. The exact Ranking passage still requires page-image verification.

### Working mechanism

**catalogue existence ≠ universal catalogue usability.**

A catalogue is an interface whose usability depends on language, script, classification practice and available expertise.

This gives a more precise formulation than saying that manuscripts were simply `catalogued` or `uncatalogued`.

---

## 9. Four transformations should now be distinguished

### A. Packing aggregation

Leaves/books are arranged into transport bundles, packages or boxes.

Typical count: `109 bundles`.

### B. Physical library individuation

Received matter is treated as physical volumes/books capable of shelf storage and handling.

Typical count: `127 volumes`.

### C. Textual identification

Contents are named as works; uncertain titles may be corrected through comparison.

Typical count: Hunter's `66 Sanskrit Buddhist works`.

### D. Catalogue inscription

The object receives an institutional entry containing selected attributes such as shelfmark, title, condition and handwriting quality.

Typical unit: `catalogue entry`.

None of these is ontologically prior for every operation. They are **different solutions to different institutional tasks**.

---

## 10. A stronger interpretation of `custody checksum`

The repo's earlier formulation separated `safe arrival` from item-level verification. Fort William now gives a concrete downstream chain:

**shipment count → receipt count → physical-volume count → expert inspection → title identification → catalogue entry → later re-identification.**

This means the checksum metaphor should remain narrow. The receipt verifies only the unit that the receipt counts.

A `109 bundles received` statement cannot verify:

- 66 title identities;
- 127 volume identities;
- completeness of a later catalogue;
- accuracy of textual naming.

Each stage requires another conversion and another verification practice.

---

## 11. Institutional legibility as a historical mechanism

The Ayton episode and MS.PERS.130 together suggest a precise mechanism:

> A knowledge object became institutionally usable only when a receiving institution could convert its transport and physical identities into a descriptive regime that available experts could read, trust and operate.

This makes institutional legibility materially and socially specific:

- objects have to be unpacked or accessed;
- physical units have to be delimited;
- titles have to be identified;
- condition/hand may be judged;
- shelfmarks have to be assigned;
- descriptions have to be written in a usable language/script;
- competent people have to be authorised to perform the work.

The institution is therefore not merely a destination node. It is a **conversion site**.

---

## 12. Why Hunter's corrected titles matter for the later archive

Hunter's explicit statement that titles were corrected from other manuscript lists is a miniature example of the larger article argument.

A later catalogue/list can:

- recover identities that an earlier institution could not securely establish;
- overwrite earlier names;
- make distributed collections mutually diagnostic;
- turn copies or parallels elsewhere into evidence for the identity of an object in Calcutta.

This is **recursive auditability** at work across decades.

It also means later lists should never be back-projected into 1827 as if the same titles were already stabilised at receipt.

---

## 13. Connection to the 1827 production bills

Wave 13 reconstructed the upstream production chain:

**paper/material purchase → copying → binding → bundling → packaging → porterage → shipment → receipt.**

Wave 14 now adds the downstream institutional chain:

**receipt → library-volume formation → content identification → competence adjudication → cataloguing → re-identification.**

Together they create a much longer object biography than `Hodgson collected manuscripts and gave them to Fort William`.

The production/custody object is repeatedly re-partitioned by changing unit systems.

---

## 14. Counting ontology — proposed provenance-schema addition

Add explicit fields:

- `count_value`
- `count_unit`
- `count_unit_class`
  - `TEXTUAL_WORK`
  - `PHYSICAL_VOLUME`
  - `LEAF`
  - `COPY`
  - `PACKAGE`
  - `BUNDLE`
  - `BOX`
  - `CATALOGUE_ENTRY`
- `count_operation`
  - production
  - packing
  - dispatch
  - receipt
  - shelving
  - cataloguing
  - retrospective reconstruction
- `count_date`
- `count_actor`
- `count_source`
- `unit_conversion_demonstrated` = true/false
- `conversion_relation`
- `same_corpus_status`
  - confirmed
  - partial_overlap
  - possible_overlap
  - unknown

### Hard rule

**Never subtract or reconcile counts across unit classes unless a primary or demonstrably reliable source supplies the conversion relation.**

---

## 15. New testable claims

### Counting-ontology claim

The numerical identity of a distributed collection changed legitimately as institutions counted different operational units; apparent count discrepancies can therefore document conversion between transport, physical, textual and catalogue regimes rather than loss or error.

### Institutional-legibility claim

Receipt made objects physically present but not necessarily institutionally usable. Identification and catalogue incorporation depended on material access, authorised expertise, language/script, classification and descriptive fields.

### Catalogue-interface claim

A catalogue was itself a historically specific interface, not a neutral mirror of holdings. Its tabular fields, language, script and judgments about condition and handwriting shaped what an institution could retrieve and compare.

---

## 16. Next high-value checks

1. Recover/image **Mss Eur Hodgson/12 f.176** to see exactly how `109 bundles` is phrased and whether the receipt contains internal breakdowns.
2. Recover/image **ff.179–182** to determine whether the 1827 itemised list is the ancestor of any portion of Hunter's later 66-work list.
3. Verify Ranking's 12 November 1827 passage against the actual page image and, ideally, College `Proc. XI, pp.346–350`.
4. Search MS.PERS.130 images for entries plausibly corresponding to Hodgson's Sanskrit Buddhist corpus; because the catalogue is Persian and subject-arranged, this may require page-by-page inspection rather than keyword search.
5. Recover the Fort William `Oriental manuscripts` catalogue/listing sequence around 1835 and determine whether Sanskrit/Buddhist holdings were recorded separately from Persian/Arabic collections.
6. Trace the 66 Fort William works into the Asiatic Society of Bengal catalogue and compare title changes one by one.
7. Check Arthur J. Arberry papers `Mss Eur B186` on disposal of the Fort William library and G. S. A. Ranking papers `Mss Eur B185` for the manuscript history behind the printed article.

---

## 17. Source-control hierarchy for this wave

### Level A — contemporary object/catalogue metadata

- Cambridge inventory of BL Hodgson papers for 1827 receipt, cash advance and itemised list.
- BULAC/BINA MS.PERS.130 record for the surviving Fort William manuscript catalogue.

### Level B — later source-based reconstruction

- Ranking, College history, using College proceedings; exact cited proceeding pages preserved, but PDF page-image verification still pending.

### Level C — retrospective scholarly reconstruction

- Hunter 1896 Appendix A. Particularly valuable because it explicitly admits uncertainty and cross-list correction.

Do not collapse these levels into one narrative voice.

---

## Bottom line

The new result is not that Hodgson sent `the wrong number` of manuscripts. It is that **the collection changed numerical identity as it crossed operational regimes**. In May 1827 the receiving institution could verify 109 transport bundles. Later in the year it confronted a larger collection as 127 physical volumes and had to decide who was competent even to ascertain their contents. By Hunter's retrospective reconstruction, one Fort William component could be named as 66 Sanskrit Buddhist works, with some titles corrected through comparison to other lists. Meanwhile the surviving Fort William catalogue shows a distinct institutional grammar of shelfmark, title, physical condition and handwriting quality, written in Persian on Indian laid paper. The epistemic problem after transport was therefore conversion into institutional legibility.