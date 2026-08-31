# Web research 2026-09-01 — Wave 41
## Historical shipment identifiers across supports, languages and document states

Date: 2026-09-01

Status: follow-up to Wave 40. This wave tests whether surviving shipment/container identifiers belong mainly to local-language handmade manuscripts or instead function as a cross-material archival key.

## Executive result

The simple model is falsified.

Historical shipment metadata survives on:

- Nepali hand-made paper contents lists;
- Limbu/Nepali local manuscripts;
- English copies on imported paper;
- English working notebooks on machine-made paper.

The strongest case is `MSS EUR HODGSON/1 item 8`.

It is an English copy written by Campbell on imported paper, but its final page preserves in Nepali the **original box and sack number at the time of shipment**.

Thus:

`shipment identity != support identity`

and

`shipment identity != language identity`.

The old container identifier is a relational key capable of crossing both.

Mechanisms:

- `SHIPMENT_IDENTIFIER_CROSSES_SUPPORT_AND_LANGUAGE`
- `OLD_SHIPMENT_METADATA_ON_MACHINE_PAPER_DERIVATIVE`
- `CONTAINER_IDENTITY_ORTHOGONAL_TO_SUPPORT_IDENTITY`
- `PAPER_IDENTIFIER_AS_RELATIONAL_CHECKSUM`.

---

## 1. Imported-paper English derivative with Nepali box/sack metadata

Cambridge `vol.1 item 8, ff.281–290` is:

- an English second copy of a Nepalese narrative of Britain–Nepal relations;
- written by Campbell;
- on imported paper, 33.7 × 20.5 cm;
- materially a derivative/copy state rather than the original Nepali record.

Yet the catalogue states that the final page contains:

- a Nepali title description;
- the **original box and sack number at the time of shipment**, written in Nepali;
- other Nepali words and numerals.

Source:
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol001.html

This is decisive for the container argument.

An English/imported-paper derivative can retain a local-script archival identity layer.

The shipment number therefore does not classify the document by language, maker or paper origin. It links a material version to a historical custody unit.

---

## 2. Machine-paper English notebooks also preserve original shipment numbers

Cambridge describes `vol.4` as four pre-bound notebooks. In most cases, the notebook covers retain:

- Nepali title;
- original shipment number in Nepali language/script.

The notebooks themselves are English working documents on machine-made paper, including ethnography, Buddhist scripture lists, geography and routes to Tibet/Peking.

Source:
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol004.html

Likewise `vol.5` consists of six pre-bound machine-paper notebooks. Their cover pages normally carry Nepali titles and original shipment numbers. The Jatamala notebooks explicitly retain original sack numbers.

Source:
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol005.html

This gives a recurring object form:

`machine/imported-paper English work state`
+
`Nepali historical shipment metadata`.

Mechanism:

`MULTILAYER_DOCUMENT_IDENTITY_ON_SINGLE_SUPPORT`.

---

## 3. Sack 8 shows the same system on a handmade local manuscript

By contrast, the sack-8 control system also survives on Nepali handmade supports:

- `vol.58/18 f.65`: sack No.8 contents list, Nepali handmade, Nepali;
- `vol.85/4 ff.95–108`: Limbu text on handmade Nepali paper, title explicitly preserving original sack number 8.

Sources:
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol058.html
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol085.html

The same archival technology therefore crosses:

`local source manuscript`

and

`English derivative notebook/copy`.

The operative variable is custody identity, not document language or support class.

---

## 4. A modern archival graph must separate four identities

The evidence now requires at least four independent fields:

1. **support identity** — Nepali handmade / machine-made / imported / mixed;
2. **documentary version identity** — source / copy / translation / abstract / notebook / chart;
3. **historical custody identity** — box / sack / bundle / trunk / shipment number;
4. **modern archival identity** — MSS EUR HODGSON volume/item/folio.

These fields can recombine in multiple ways.

For example:

`vol.1/8`

= imported paper
+ English copy
+ Nepali box/sack identifier
+ modern vol.1 shelfmark.

Therefore none of the four identities can substitute for another.

Mechanism:

`MULTIAXIAL_DOCUMENT_IDENTITY`.

---

## 5. Why this strengthens the paper argument

The paper article can now avoid two common simplifications.

First, the material archive cannot be reconstructed through a local/European paper binary.

Second, paper inscriptions cannot be treated merely as textual content added after material selection.

The same support can carry multiple operational layers:

- translated/analytical content;
- corrections;
- title;
- historical custody number;
- later catalogue/binding identity.

A sheet therefore participates simultaneously in knowledge work and archive control.

The strongest formulation is:

**paper is both an epistemic working surface and an addressable relational surface.**

Mechanism:

`PAPER_AS_ADDRESSABLE_RELATIONAL_SURFACE`.

---

## 6. Source-control consequence

Because old identifiers cross material/language categories, reconstruction must proceed by explicit identifier matching rather than thematic or material clustering.

Required graph rule:

`edge(old container -> modern object)`

is admitted only when supported by:

- explicit same historical number;
- legible content-list match;
- or another direct historical custody statement.

Do not infer edges merely because:

- two documents share subject;
- both are Nepali handmade;
- both are translations;
- or both now sit in adjacent modern volumes.

---

## Immediate next operations

1. Physically/image-read the actual box/sack numerals on `vol.1 item 8`.
2. Recover original shipment numbers from the covers of the four `vol.4` notebooks.
3. Recover original shipment/sack numbers from all six `vol.5` notebooks.
4. Use recovered numbers to query the surviving control leaves in vols.55, 58 and 94.
5. Build a bipartite historical-container ↔ modern-shelfmark graph.
6. Preserve support/language/version fields as attributes rather than using them as identity keys.

## Bottom line

Surviving shipment metadata is not confined to Nepali handmade local-source papers. An English Campbell copy on imported paper and machine-made English notebooks retain Nepali box, sack or shipment numbers alongside local handmade manuscripts that carry the same kind of identifiers. Historical container identity therefore operated across material and linguistic classes. For the paper article, this makes the sheet not only a medium of translation and analysis but an addressable surface through which documentary versions could remain attached to a custody architecture even after that architecture was physically dismantled.