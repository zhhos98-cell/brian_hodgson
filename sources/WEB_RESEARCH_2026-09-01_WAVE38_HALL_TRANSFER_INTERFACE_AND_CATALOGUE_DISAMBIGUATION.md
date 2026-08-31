# Web research 2026-09-01 — Wave 38
## FitzEdward Hall, bilingual control lists, and catalogue disambiguation at the 1864 transfer interface

Date: 2026-09-01

Status: paper-centred transfer-interface and source-control follow-up to Wave 37. This wave identifies the India Office librarian who inspected Hodgson's manuscript collection, reconstructs the layered descriptive surfaces already in circulation before formal donation, and separates an unrelated 1865 zoological `second edition catalogue` from the manuscript-transfer list chain.

## Executive result

Three points materially sharpen the 1864 transfer sequence.

1. `Mr Hall`, who inspected the manuscript collection before Hodgson formally tendered it to the India Office, can be securely identified as **FitzEdward Hall (1825–1901), Librarian of the India Office, 1864–1869**.
2. Hodgson's 2 August 1864 presentation letter says that **lists in English and Hindi of the contents of the MSS were already in the hands of the Librarian**. The later transfer manifest repeatedly refers downward to `Hindi` or `Nagri` lists for bundle-level detail. The transfer therefore used a layered descriptive system rather than one self-sufficient catalogue.
3. RAS `BHH/5/19`, Hodgson's 1 December 1865 letter to Hall sending a corrected copy of the `second edition of the catalogue`, belongs to the **zoological British Museum catalogue chain**, not the India Office manuscript-donation manifest. ZSL preserves three Hodgson-annotated copies of the 1863 *Catalogue of the Specimens and Drawings of Mammals, Birds, Reptiles, and Fishes of Nepal and Tibet ... Second Edition*; the 1865 RAS letter also discusses specimen numbers.

Thus Hall sits at the intersection of two Hodgson documentary networks — manuscript custody and zoological catalogue circulation — but their `catalogue` objects must remain separate.

Core mechanisms:

- `PRE_DEPOSIT_LIBRARIAN_INSPECTION`
- `BILINGUAL_CONTENT_LIST_AT_TRANSFER_INTERFACE`
- `LAYERED_TRANSFER_DESCRIPTION_SYSTEM`
- `SUBORDINATE_LISTS_INDEX_PHYSICAL_BUNDLES`
- `INSTITUTIONAL_EVALUATION_BEFORE_FORMAL_CUSTODY`
- `CATALOGUE_TERM_REQUIRES_OBJECT_DISAMBIGUATION`
- `HALL_CONNECTS_DISTINCT_DOCUMENTARY_NETWORKS`

---

## 1. `Mr Hall` is FitzEdward Hall, India Office Librarian 1864–1869

British Library visual-archives catalogue:

`Photo 322(1)`

`Portrait of Fitzedward Hall (1825–1901), Librarian, India Office, 1864–9.`

BL search result:
https://searcharchives.bl.uk/?f%5Bmaterial_type_si%5D%5B%5D=Photographs&f%5Brelated_places_ssim%5D%5B%5D=Westminster%2C+England&f%5Burl_non_blank_si%5D%5B%5D=No&per_page=100&search_field=all_fields&sort=date

The same BL sequence identifies:

- James Robert Ballantyne as Librarian 1861–64;
- FitzEdward Hall as Librarian 1864–69;
- Reinhold Rost as Librarian 1869–93.

This chronology fits Hodgson's August 1864 correspondence exactly.

Additional biographical control:

The *Dictionary of National Biography* supplement states that Hall settled in London after leaving India and served as librarian at the India Office, retiring in 1869. Hall was an experienced Sanskrit/Hindi scholar, not merely a clerical receiving officer.

Source:
https://en.wikisource.org/wiki/Dictionary_of_National_Biography%2C_1912_supplement/Hall%2C_Fitzedward

Mechanism:

`PRE_DEPOSIT_LIBRARIAN_INSPECTION`.

---

## 2. Hodgson describes Hall's inspection as epistemic evaluation before deposit

RAS `BHH/5/18`:

`Draft letter from Brian Houghton Hodgson to The Right Honorable Sir C Wood ... 2 August 1864`.

Reference:
`GB 891 BHH-BHH/5-BHH/5/18`.

RAS catalogue:
https://royalasiaticarchives.org/index.php/draft-letter-from-brian-houghton-hodgson-to-the-right-honorable-sir-c-wood-g-l-b-mp-secretary-of-state-for-india-2-august-1864

The catalogue says Hodgson's Kathmandu collection concerning civil/natural history and Buddhism had been inspected by Hall before Hodgson tendered it for India Office deposit.

Hunter's later reproduction of the letter preserves more of Hodgson's wording. Hodgson says he had submitted the collection to Hall's `summary inspection`; Hall concurred that the materials, despite their crude state, were capable of serving the purposes for which Hodgson had accumulated them and were likely to be useful if deposited in the India Office Library.

The transfer sequence is therefore not simply:

`private owner -> Secretary of State -> library`.

It includes a prior library-side evaluation:

`private store`
-> `librarian inspection`
-> `librarian judgement of usability`
-> `formal tender to Secretary of State`
-> `institutional custody`.

Mechanism:

`INSTITUTIONAL_EVALUATION_BEFORE_FORMAL_CUSTODY`.

Source-control:

Hunter 1896 is downstream of surviving RAS event-near states; use it for wording/navigation until `BHH/5/18` is directly transcribed.

---

## 3. English and Hindi contents lists already circulated before the formal donation

Hodgson's 2 August 1864 letter states that:

`lists in English and Hindi of the contents of the MSS are in the hands of the Librarian`.

Hunter reproduction:
William Wilson Hunter, *Life of Brian Houghton Hodgson* (1896), Appendix B, p.357.

Digital scan:
https://dspace.gipe.ac.in/xmlui/bitstream/handle/10973/24484/GIPE-000910-Contents.pdf?isAllowed=y&sequence=2

This means descriptive control material had already separated from the manuscript collection and reached Hall before formal acceptance was closed.

The list itself was therefore a circulating custody object.

Mechanisms:

- `BILINGUAL_CONTENT_LIST_AT_TRANSFER_INTERFACE`
- `CONTROL_LIST_PRECEDES_FORMAL_CUSTODY`.

High-priority archival target:

Locate both the English and Hindi contents lists that Hall held. They may be distinct from:

- `BHH/11/14` private store/donation list;
- `BHH/19/5` printed August 1864 list;
- the Hindi/Nagri subordinate lists named inside the printed manifest.

Do not assume identity among these list classes until compared.

---

## 4. The 1864 manifest is not a self-contained inventory: it points to subordinate vernacular lists

Hunter's reproduction repeatedly delegates item-level detail to other lists.

Examples:

### Newar institutions / Buddhism

Under Trunk 1, second large bundle, Buddhist papers are described as:

- thirty-six papers `as detailed in the Nagri list hereto appended`;
- twenty-two further Buddhist papers `as per list just named`.

### Bhatgaon revenue

Trunk 2, fourth large bundle contains twenty-seven lesser bundles of Bhatgaon land-revenue papers, with details `given in the subjoined Hindi list`.

### Kathmandu revenue

The fifth large bundle contains twenty-one lesser bundles of Kathmandu land-revenue papers, with particulars `given in the Hindi list`.

### Jumla revenue

The sixth large bundle contains the Jumla revenue statement in Khas and English `as per details in Hindi list`.

Therefore descriptive architecture is hierarchical:

`presentation letter / summary`
-> `master trunk-and-bundle manifest`
-> `Hindi/Nagri subordinate lists`
-> `lesser bundles / manuscripts`.

Mechanism:

`LAYERED_TRANSFER_DESCRIPTION_SYSTEM`.

The subordinate lists function as relational indexes between broad custody units and lower-level paper objects.

Mechanism:

`SUBORDINATE_LISTS_INDEX_PHYSICAL_BUNDLES`.

---

## 5. The bilingual/list hierarchy complicates the phrase `the 1864 list`

There is no longer one analytically sufficient object called `the 1864 list`.

At minimum the transfer system currently contains:

1. `BHH/11/14` — handwritten 1858 store list becoming 1864 donation list;
2. `BHH/5/18` — draft presentation letter to Sir Charles Wood;
3. English contents list in Hall's hands — not yet located;
4. Hindi contents list in Hall's hands — not yet located;
5. one or more Hindi/Nagri subordinate lists referenced inside the master manifest — exact identity with item 4 unresolved;
6. `BHH/19/5` — printed August 1864 manifest with annotations;
7. India Office institutional accession/receipt copies — not yet located;
8. Hunter 1896 reproduction.

Thus:

`transfer description = multi-document control system`.

Mechanism:

`TRANSFER_DESCRIPTION_IS_DISTRIBUTED_ACROSS_CONTROL_SURFACES`.

---

## 6. BHH/5/19: the 1865 `second edition catalogue` is zoological, not the manuscript donation catalogue

RAS `BHH/5/19`:

`Draft letter from Brian Houghton Hodgson to Mr Hall, 1 December 1865`.

Reference:
`GB 891 BHH-BHH/5-BHH/5/19`.

RAS browse/citation:
https://royalasiaticarchives.org/index.php/informationobject/browse?levels=241&media=print&names=2296&sf_culture=nl&sort=lastUpdated&sortDir=asc&topLod=0

The catalogue says Hodgson:

- had been sorting through his papers since returning home;
- sent Hall a corrected copy of the `second edition of the catalogue`;
- wrote about the numbers of specimens he had collected.

This wording alone makes a zoological identification likely. Independent ZSL evidence makes it strong.

ZSL `NZSL/HOD/1/4`, `Annotated British Museum Catalogues`, preserves:

- three copies annotated by Hodgson of the 1863 **Second Edition** of the British Museum `Catalogue of the Specimens and Drawings of Mammals, Birds, Reptiles, and Fishes of Nepal and Tibet, presented by B.H. Hodgson`.

ZSL catalogue:
https://zsl-archive.maxarchiveservices.co.uk/index.php/informationobject/browse?media=print&names=8774&sf_culture=en&showAdvanced=1&sort=startDate&sortDir=asc&subjects=10546&topLod=0&view=table

The British Museum's history of its natural-history collections likewise says Hodgson's collections were important enough to generate special catalogues in 1846 and 1863.

Therefore the best current identification is:

`BHH/5/19 second edition catalogue = 1863 zoological British Museum catalogue`.

Confidence:

high, but page-level transcription of `BHH/5/19` remains desirable.

Mechanism:

`CATALOGUE_TERM_REQUIRES_OBJECT_DISAMBIGUATION`.

---

## 7. Hall participates in two distinct Hodgson documentary networks

This source-control correction produces a useful historical observation.

Hall is involved in:

### Manuscript-custody network, 1864

- summary inspection of Kathmandu manuscript collection;
- holding English/Hindi contents lists;
- advising that the India Office Library was an appropriate place for use;
- transfer interface before Hodgson's formal offer to Wood.

### Zoological-catalogue network, 1865

- recipient of Hodgson's corrected copy of the 1863 second-edition zoological catalogue;
- correspondence includes specimen-number accounting.

Thus one institutional actor participates in multiple paper systems.

But that overlap is **not evidence that the catalogues are one object family**.

Mechanism:

`HALL_CONNECTS_DISTINCT_DOCUMENTARY_NETWORKS`.

This is a useful warning against entity-based archival reconstruction: following a person alone can collapse different document ontologies.

---

## 8. Hall's linguistic expertise matters, but should not be overinterpreted

Hall was a Sanskritist and scholar of Hindi/Hindustani as well as India Office librarian. The English/Hindi list pair therefore reached an institutional reader capable of engaging directly with Indian-language descriptive material.

The secure institutional claim is:

`bilingual descriptive surfaces were held at the transfer interface by a linguistically competent librarian`.

Do not yet claim:

- that Hall authored or edited the Hindi lists;
- that Hall personally verified every manuscript;
- that Hindi was selected specifically for Hall;
- that his summary inspection was equivalent to full cataloguing.

Mechanism:

`LINGUISTICALLY_COMPETENT_TRANSFER_READER` — contextual, not yet causal.

---

## 9. Acceptance/receipt remains an open archival edge

Current public searching has not yet located a secure reply from Sir Charles Wood accepting the donation or a formal India Office accession receipt for the 1864 Hodgson collection.

RAS `BHH/11/14` contains a copy of Hodgson's letter concerning acceptance of his donation, but the catalogue description alone does not supply the Secretary of State's response text.

The Charles Wood papers are now held at the Borthwick Institute, University of York; the British Library catalogue notes that the former India Office private-papers collection `Mss Eur F78` was transferred there in 2011, with some microfilm retained at BL.

BL fonds reference:
https://searcharchives.bl.uk/?f%5Brelated_places_ssim%5D%5B%5D=Bombay%2C+India&f%5Brelated_places_ssim%5D%5B%5D=India%2C+Asia&f%5Burl_non_blank_si%5D%5B%5D=No&per_page=100&search_field=all_fields&sort=date

Next archival search target:

`Wood papers / India Office Library correspondence / August 1864 / Hodgson manuscripts / Hall`.

Source-control status:

`formal acceptance/receipt = not yet recovered`.

---

## 10. Article consequence

The 1864 transfer now appears as an institutional interface composed of multiple paper control surfaces:

`private store order`
-> `Hall inspection`
-> `English + Hindi contents lists already circulated`
-> `formal presentation letter`
-> `master trunk/bundle manifest`
-> `Hindi/Nagri subordinate lists`
-> `physical bundles`
-> `institutional accession/receipt [still to locate]`.

This matters because archival transfer does not merely move objects. It requires relations to become legible to a new custodian.

The descriptive system is itself versioned, multilingual and hierarchical.

Strong formulation:

**Before Hodgson's manuscripts formally entered India Office custody, their contents had already been detached into English and Hindi control lists and subjected to a librarian's summary inspection. The printed transfer manifest then delegated lower-level detail to Hindi and Nagri lists tied to physical bundles. Institutional incorporation was therefore mediated by a layered paper interface whose control documents circulated ahead of, alongside and within the manuscript containers.**

---

## Source-control rules

1. `BHH/5/19 second edition catalogue` must not be inserted into the India Office manuscript-manifest version chain; current evidence identifies it as the 1863 British Museum zoological catalogue.
2. Hall's presence in both networks does not merge their document objects.
3. English/Hindi lists in Hall's hands may or may not be identical to the subordinate Hindi/Nagri lists referenced inside the printed manifest; identity remains unresolved.
4. `summary inspection` is not full cataloguing.
5. Hunter 1896 remains downstream of RAS event-near objects; direct RAS page transcription should supersede Hunter wording when available.
6. Formal acceptance/receipt of the 1864 donation remains an open edge until response/accession evidence is located.
7. Hall's linguistic expertise is contextual evidence, not proof of his authorship or detailed verification of the lists.

## Immediate next actions

1. Search Borthwick Institute Charles Wood papers for Hodgson correspondence/acceptance in August 1864.
2. Search India Office Library administrative records for Hall's inspection, receipt and accession handling.
3. Locate the English and Hindi contents lists Hodgson says were already in Hall's hands.
4. Determine whether the subordinate Hindi/Nagri lists referenced by the printed manifest survive among `Mss Eur Hodgson`, RAS `BHH/11`, or India Office catalogue records.
5. Image-transcribe `BHH/5/18`, `BHH/11/14`, and `BHH/19/5` to reconstruct the exact list/control-document stemma.
6. Page-transcribe `BHH/5/19` only to close the zoological-catalogue identification; keep it outside the manuscript-transfer chain.
7. Search later Hall/Hodgson correspondence for receipt, reclassification, requests for corrected lists or institutional use of the transferred papers.

## Bottom line

Wave 38 identifies the 1864 transfer as a multilayered descriptive interface rather than a single manifest. FitzEdward Hall, India Office Librarian from 1864 to 1869, inspected Hodgson's manuscript collection before formal tender and already held English and Hindi contents lists. The eventual master manifest repeatedly points to subordinate Hindi/Nagri lists for physical bundle detail. At the same time, a superficially tempting 1865 `second edition catalogue` reference is demonstrably part of Hodgson's zoological British Museum catalogue network, not the manuscript donation. The result is both a stronger custody mechanism and a cleaner source ontology.