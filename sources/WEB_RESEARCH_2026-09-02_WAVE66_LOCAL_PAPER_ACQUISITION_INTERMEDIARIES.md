# Web/archive research 2026-09-02 — Wave 66
## Local paper acquisition through research intermediaries: Rajmansingh, a Chitrakar, and non-market supply channels

Date: 2026-09-02

Status: active paper-history mainline. This wave follows the local supply side of Nepali handmade paper. It complements Wave 64's quantified/billed procurement by identifying direct catalogue evidence that paper also entered Hodgson's research through named or occupational intermediaries.

## Executive result

The current paper-supply model needs at least two distinct local acquisition channels.

### Channel A — billed procurement

Wave 64:

`local paper market/workshop`
-> `Residency bill / quantified unit`
-> `copying + binding + packaging + shipment`.

### Channel B — intermediary acquisition

Cambridge's inventory of `MSS EUR HODGSON/53` gives two unusually explicit notes:

- `vol.53 item 17, f.97` — Nepali handmade paper, 1831: **`paper acquired through Rajmansingh`**;
- `vol.53 item 19, f.99` — Nepali handmade paper, 1830: **`paper acquired from a Chitrakar`**.

These statements describe the support itself, not merely the information written on it.

Thus Hodgson's local paper supply cannot be reconstructed only through bills, markets or generic Residency stock. **Research assistants/artisanal collaborators could act as acquisition interfaces through which blank or usable local paper entered the working archive.**

Current mechanisms:

- `LOCAL_PAPER_ACQUISITION_HAS_MULTIPLE_CHANNELS`
- `RESEARCH_INTERMEDIARY_CAN_BE_PAPER_SUPPLY_INTERMEDIARY`
- `PAPER_PROVENANCE_CAN_ATTACH_TO_PERSONAL_NETWORK`
- `SUPPORT_ACQUISITION_AND_INFORMATION_ACQUISITION_MUST_BE_SEPARATED`
- `NAMED_ACQUISITION_AGENT_DOES_NOT_EQUAL_PAPERMAKER`.

---

## 1. Direct witness: f.97 acquired through Rajmansingh

Primary catalogue node:

`MSS EUR HODGSON/53 item 17, f.97`.

Cambridge records:

- date: 1831;
- subject: tenancy regulations relating to paddy fields and building houses by tenants;
- language: Nepali/Hindi mixed;
- support: **Nepali handmade paper**;
- Nepali and English title description;
- explicit note: **`paper acquired through Rajmansingh`**.

Source:
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol053.html

This phrasing is materially precise. It does not say merely that Rajmansingh supplied the information or wrote the text. The object description attaches the acquisition statement to **paper**.

Safe interpretation:

`Rajmansingh = documented acquisition intermediary for the support of this item`.

Unsafe interpretations without further evidence:

- Rajmansingh manufactured the paper;
- Rajmansingh owned a paper shop;
- Rajmansingh purchased it personally;
- all paper used in his research/drawing work came through him;
- the paper was newly manufactured when acquired.

The historical operation may have involved purchase, gift, retrieval from an existing household/office stock, or provision from another intermediary. Current evidence proves the acquisition route only at the person-mediated level.

Mechanism:

`PERSON_MEDIATED_SUPPORT_PROVENANCE`.

---

## 2. Direct witness: f.99 acquired from a Chitrakar

`MSS EUR HODGSON/53 item 19, f.99`:

- date: 1830;
- subject: different kinds of tax-free land (`virtā`);
- language: Nepali/Hindi mixed;
- support: **Nepali handmade paper**;
- Nepali and English title description;
- explicit note: **`paper acquired from a Chitrakar`**;
- English description/derivative cross-reference at vol.7/21 ff.138–139.

Source:
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol053.html

The occupational label `Chitrakar` is significant because Cambridge elsewhere identifies a `citrakār` as Hodgson's artist/assistant and repeatedly suggests Rajman Singh as the likely referent in research-collection contexts.

However, `paper acquired from a Chitrakar` must remain distinct from `paper acquired through Rajmansingh`.

Current identity state:

`F99_CHITRAKAR = POSSIBLY_RAJMAN_SINGH / NOT_PROVEN`.

Do not merge the two supply agents unless handwriting, original labels, correspondence or another direct catalogue statement resolves the identity.

Mechanism:

`OCCUPATIONAL_INTERMEDIARY_AS_SUPPORT_SOURCE`.

---

## 3. Rajman Singh's documented functions make paper acquisition part of a wider research-service ecology

The paper-supply evidence becomes more meaningful when placed beside Cambridge's descriptions of `citrakār` work elsewhere in the collection.

### vol.4 item 1

A Newar customs/manners account contains the note `mārphat Citrakāra` — literally `through a Chitrakar`. Cambridge explains that Hodgson's official painter was Rajman Singh and identifies him as the artist responsible for much of Hodgson's zoological, architectural and ethnographic drawing corpus.

### vol.59 item 18

Land-tenure/inheritance information is described as collected and written by a `citrakār`, presumed by the inventory to be Hodgson's artist and assistant Rajman Singh.

### vol.60 item 22

Newar customs material is described as information collected by `chitrakār (Rajman Sing?)`.

### vol.58 item 15

A later note records Rajman Chitrakar/Rajmansingh selecting/recommending birds for shipment and drawing them.

Sources:
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol004.html
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol059.html
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol060.html
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol058.html

This does not make every `Chitrakar` reference Rajman Singh. It does establish that the same occupational/research network performed multiple material operations:

- gathering information;
- writing/copying;
- drawing;
- selecting specimens;
- facilitating shipment;
- and, in at least one direct case, acquiring paper.

The assistant's role therefore cannot be reduced to `informant` or `artist` if the article is reconstructing paper infrastructure.

Working formulation:

**local collaborators could mediate not only knowledge and images but the material supports on which that knowledge entered Hodgson's archive.**

Mechanisms:

- `RESEARCH_ASSISTANT_AS_MATERIAL_INFRASTRUCTURE_AGENT`
- `KNOWLEDGE_NETWORK_AND_SUPPLY_NETWORK_PARTIALLY_OVERLAP`.

---

## 4. Support acquisition is not the same as information provenance

This distinction is now necessary in the paper census.

For f.97, the catalogue says:

`paper acquired through Rajmansingh`.

It does not by itself say:

`information collected by Rajmansingh`.

For f.99, similarly:

`paper acquired from a Chitrakar`.

The content concerns land tenure, but the support provenance and information provenance may have different paths.

Therefore every sheet-level record should separate:

- `information_source`;
- `writer/copyist`;
- `paper_acquisition_agent`;
- `paper_maker_or_origin`;
- `paper_stock_holder`; 
- `document_owner/provider`;
- `acquisition_mode`.

Current evidence often resolves only one or two of these.

Mechanism:

`SUPPORT_PROVENANCE_NOT_INFORMATION_PROVENANCE`.

---

## 5. Adjacent folios do not establish one stock batch

Modern vol.53 places:

- f.97 — Rajmansingh-acquired paper;
- f.98 — another Nepali handmade paper item;
- f.99 — Chitrakar-acquired paper.

This adjacency is suggestive but cannot currently support a same-stock claim.

The collection was reorganized and bound later; the Cambridge introduction states that the papers were bound into volumes in 1921, partly by physical dimensions.

Therefore:

`MODERN_FOLIO_ADJACENCY != ORIGINAL_STOCK_BATCH`.

Only direct physical examination can test whether f.97–99 share:

- fibre/formation;
- dimensions;
- chain/laid structure;
- colour/thickness/sizing;
- deckle/cut edges;
- watermark or countermark;
- original folds or attachment evidence.

Mechanisms:

- `BINDING_ADJACENCY_NOT_SUPPLY_IDENTITY`
- `STOCK_BATCH_REQUIRES_SHEET_LEVEL_PHYSICAL_CONTROL`.

---

## 6. Wave 64 + Wave 66 produce a two-channel local supply model

The article can now distinguish at least:

### Quantified commercial/Residency procurement

1843 f.117 and 1827 bills:

`paper as accounted material input`.

### Network-mediated acquisition

1830–31 f.97/f.99:

`paper as locally sourced support moving through named/occupational intermediaries`.

These are not mutually exclusive. Rajman Singh or a Chitrakar could have bought paper in a market, drawn it from workshop/household stock, obtained it through occupational networks, or simply conveyed it to Hodgson.

The distinction is evidential:

- one channel survives in **accounts**;
- the other survives in **provenance annotations/catalogue descriptions**.

Combined model:

`local manufacture`
-> `market / workshop / household / occupational stock`
-> `[billed purchase OR collaborator-mediated acquisition]`
-> `Residency working stock`
-> `allocation to writing/drawing/copying operation`.

The middle stages remain to be reconstructed.

---

## 7. Consequence for Raj Man Singh drawing-paper research

The RAS architectural programme is currently strongest on dimensional format and watermark date, not supply route.

The direct vol.53 evidence that paper could be acquired **through Rajmansingh** makes one new question legitimate:

**did Raj Man Singh also mediate the supply/allocation of papers used for visual research?**

Current answer:

`UNRESOLVED`.

Do not transfer the vol.53 support-provenance statement to the RAS drawing series.

What to test physically/documentarily:

- whether Raj Man Singh's drawings show recurrent local-paper stocks that can be linked to papers he supplied elsewhere;
- whether bills/accounts name paper supplied to draughtsmen or painters;
- whether correspondence uses `paper`, `drawing paper`, `sheet`, `book`, `citrakār` or Raj Man Singh in procurement contexts;
- whether finished English-paper drawing stock was centrally issued by Hodgson while local handmade paper was collaborator-provided.

This is now a research question, not a claim.

---

## Source-control rules

1. Treat `paper acquired through Rajmansingh` and `paper acquired from a Chitrakar` as direct catalogue statements about support provenance.
2. Do not identify the unnamed Chitrakar on f.99 as Raj Man Singh without further evidence.
3. Do not infer paper manufacture, ownership or commercial occupation from acquisition mediation.
4. Keep paper acquisition agent separate from information source and copyist.
5. Do not infer same stock from adjacency of f.97–99 in the modern bound volume.
6. Do not project the vol.53 paper-procurement role onto Raj Man Singh's drawing corpus without direct evidence.
7. Use 1921 binding history as a control against reading modern folio sequence as original material grouping.

## Immediate next actions

1. Recover ordinary-light images of vol.53 ff.97–99 and compare dimensions, texture, edges, ruling/folds and visible formation.
2. Search Hodgson correspondence/accounts for Rajman Singh/Chitrakar + paper/drawing-paper procurement language.
3. Search the full Cambridge inventory for other explicit `paper acquired/supplied/purchased through/by/from` statements.
4. Add `paper_acquisition_agent` and `acquisition_mode` to the paper census schema.
5. Compare vol.53 f.97/f.99 support against other Rajman Singh-associated writing/drawing objects only after sheet-level evidence is available.
6. Keep billed procurement and collaborator-mediated acquisition as separate edges in the paper supply graph.

## Bottom line

Hodgson's local paper supply was not exhausted by market purchase or Residency stationery stock. Two 1830–31 Nepali handmade-paper items preserve unusually explicit support provenance: one sheet was acquired through Rajmansingh and another from a Chitrakar. Elsewhere the same Chitrakar/Rajman Singh research network is documented collecting and writing information, drawing, selecting specimens and facilitating shipment. The safe paper-history conclusion is therefore narrow but important: **local research collaborators could function as material supply intermediaries, so the network that produced Hodgson's knowledge also partly mediated the paper on which that knowledge was written.**