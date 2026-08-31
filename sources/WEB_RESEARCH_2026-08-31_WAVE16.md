# Web research wave 16 — count-version conflict, B.5 re-segmentation, and the labour of institutional legibility

Date: 2026-08-31

Status: direct nineteenth-century printed-text reconstruction from Rajendralal Mitra, *The Sanskrit Buddhist Literature of Nepal* (1882). Exact page-image verification remains desirable; the Internet Archive PDF exceeds the current web PDF fetch limit, but the two numerical passages are independently reproduced by PAHAR/Google-digitized text and Wisdomlib page OCR.

Primary text:
https://archive.org/stream/cu31924007399342/cu31924007399342_djvu.txt

PAHAR scan search witness:
https://pahar.in/pahar/Books%20and%20Articles/Nepal/1882%20The%20Sanskrit%20Buddhist%20Literature%20of%20Nepal%20by%20Mitra%20s.pdf

Wisdomlib page renderings used as independent OCR controls:
- prefatory p. xxiv: https://www.wisdomlib.org/history/book/the-sanskrit-buddhist-literature-of-nepal/d/doc1897108.html
- prefatory p. xl: https://www.wisdomlib.org/history/book/the-sanskrit-buddhist-literature-of-nepal/d/doc1897123.html
- B.5/B.65 fuller contents: https://www.wisdomlib.org/history/book/the-sanskrit-buddhist-literature-of-nepal/d/doc1897424.html

---

## 1. Mitra's own preface preserves two different Asiatic Society counts

The same 1882 preface gives two non-identical descriptions of the Asiatic Society of Bengal Hodgson collection.

### Distribution statement, prefatory p. xxiv

Mitra says Hodgson's Sanskrit-Buddhist copies were distributed in **381 bundles**. For the Asiatic Society of Bengal he gives:

**85 bundles comprising 144 separate works.**

The distribution continues with 85 bundles to the Royal Asiatic Society, 30 to the India Office, 7 to the Bodleian, and 174 to the Société Asiatique / Burnouf.

### Immediate-object statement, prefatory p. xl

When Mitra turns from the general historical distribution to the collection he actually had to analyse, he says:

**86 bundles including 170 separate works.**

He adds that these represented nearly a million and a half verses by the Indian mode of reckoning.

### Rule

Preserve both statements.

Do not currently normalize them into a single `Asiatic Society total`.

The difference is:

- bundle count: 85 -> 86;
- textual-work count: 144 -> 170.

The source itself does not, in the passages inspected, explicitly explain the conversion.

Possible explanations include changed collection state, recount, inclusion criteria, or the consequences of deeper segmentation. These remain hypotheses until a connecting source is found.

---

## 2. Why 144 -> 170 is historically suggestive but not yet solved

Immediately before the section describing the 86-bundle analytical task, Mitra explains that the old Calcutta list was structurally corrupt:

- one work could appear under two or three different names;
- four, five or more works could be collapsed under one name;
- multiple works were sometimes written continuously in one physical volume without a pagination break;
- cursory cataloguing read only the first and last page of a codex.

This makes a later increase in `separate works` historically plausible as an effect of re-segmentation.

But because false splitting also operated in the opposite direction, and because the bundle count also changes by one, the **26-work increase cannot be assigned mechanically to correction of false lumping**.

### Correct status

`85 bundles / 144 works` and `86 bundles / 170 works` should be coded as a **count-version conflict with a plausible but unproven relation to reanalysis**.

---

## 3. B.5 is the concrete microcase: stable identifier, radically deeper internal count

Mitra's table of contents gives:

- `Dharani-mantra-sangraha ... B.5`, p. 80;
- later `Dharanis ... B.5 and B.65`, pp. 291–292.

At the later point Mitra explicitly says the earlier description of B.5 **did not convey a full idea of its contents**.

He then states:

**B.5 comprises 39 Dharanis.**

He individually enumerates the 39 texts/ritual units. They include Harahara-hridaya, Abhayankari, Sahasravarta, Sinhanada, Shadaksharita-mahavidya, Avalokitesvara materials, Amoghapasa, Tara, Marichi, Parnasavari, Grihamatrika, Dhvajagrakeyuri, Pratisara texts, Mahamayuri, Lankavatara and others.

B.65 contains **12 Dharanis**, and Mitra explicitly says some are also included in B.5.

### What this proves

The institutional identifier can remain stable while represented object cardinality changes with inspection depth.

At one descriptive level:

`B.5 = Dharani-mantra-sangraha`.

At a deeper analytical level:

`B.5 = container/codex/assemblage containing 39 distinguishable Dharanis`.

This is stronger than a generic warning about catalogue error because Mitra documents the **re-description of one identified object inside his own book**.

---

## 4. B.5 is not merely a false-lump error

Do not automatically label B.5 itself as an erroneous old catalogue entry.

A collection title such as `Dharani-mantra-sangraha` can legitimately describe an anthology/assemblage. The important historical variable is **granularity**:

- collection-level identity;
- internal textual-work identities;
- overlapping texts across B.5 and B.65.

The schema therefore needs to distinguish:

- `FALSE_LUMP` — several works wrongly assumed to be one;
- `LEGITIMATE_COMPOSITE` — one material/catalogue unit intentionally contains multiple textual works;
- `UNDERDESCRIBED_COMPOSITE` — composite known as such, but internal contents incompletely represented;
- `RESEGMENTED_COMPOSITE` — later inspection explicitly enumerates internal units.

B.5 is best coded provisionally as `UNDERDESCRIBED_COMPOSITE -> RESEGMENTED_COMPOSITE`, unless the earlier p.80 entry itself proves a false one-work assumption.

---

## 5. Overlap between B.5 and B.65 introduces another relation type

Mitra says some of B.65's twelve Dharanis are also included in B.5. The visible list confirms repeated titles such as Parnasavari and Vasundhara families among the two aggregates.

This means catalogue incorporation cannot be modelled only as:

`physical unit -> unique set of works`.

The same textual work or closely related textual identity can occur in more than one physical/catalogue aggregate.

Add relations:

- `text_instance_of`
- `same_work_as`
- `parallel_copy_of`
- `also_contained_in`
- `composite_overlaps_with`

Do not treat repeated title strings as proof of textual identity without comparison.

---

## 6. Institutional legibility required a funded division of scholarly labour

Mitra's preface gives unusually explicit evidence for the labour required to turn the 86 bundles into an analytical catalogue.

Arthur Grote, as President of the Asiatic Society, repeatedly urged Mitra to examine the Hodgson manuscripts. Mitra initially resisted because the task was too large. After Grote's retirement, a plan was proposed to **divide the work among two or more persons**, and the Society Council agreed to **defray the cost of preparing and printing the analysis**.

The work was then distributed:

- **Pandit Harinath Vidyaratna**: employed to read texts and prepare Sanskrit abstracts under Mitra's direction; read about **two-thirds of the total number of texts**;
- **Pandit Ramanath Tarkaratna**: read the large Prajnaparamita;
- **Pandit Kamakhyanath Tarkayagisa**: read three smaller works;
- **Rajendralal Mitra**: handled the remainder and repeatedly compared Pandits' abstracts against originals;
- **Haraprasad Sastri**: translated abstracts of **16 larger works** into English when Mitra needed assistance.

Mitra says this comparison involved a great deal of hard and tedious reading.

### Mechanism

Institutional legibility is produced through **paid, divided, supervised and checked reading labour**.

The catalogue is therefore not an information layer that appears after the objects arrive. It is a labour-intensive secondary production process.

---

## 7. Verification was selective even inside the reanalysis

Mitra states that he frequently compared the Pandits' abstracts with originals. But he also says he did **not** consider it necessary, and did not have the opportunity, to compare all of Haraprasad Sastri's English renderings with the originals.

This is extremely useful for the project's auditability vocabulary.

A sophisticated reanalysis can still contain multiple verification depths:

- original read directly;
- Sanskrit abstract produced by another scholar;
- abstract checked against original by supervisor;
- English rendering made from abstract;
- English rendering not uniformly checked against original.

### Schema consequence

Add:

- `derivation_depth`;
- `checked_against_original`;
- `checking_sample_or_extent`;
- `intermediate_representation`;
- `supervision_relation`;
- `translation_from_original_or_abstract`.

`catalogue entry` should not be treated as a single epistemic distance from the manuscript.

---

## 8. Difficulty changed the intellectual scope of the published analysis

Mitra describes the manuscripts as:

- written in a Newari script unfamiliar to him;
- full of errors;
- containing unfamiliar technical terms;
- including difficult dialect quotations.

He then says his Pandits could not always master the philosophical terminology or condense diffuse doctrinal discussions clearly enough for public presentation. As a result, the attempt to review dogmas was **abandoned**, and the project shifted mainly toward narratives and stories of Buddha's previous births.

### HPS importance

The published intellectual object was shaped by the affordances and limits of the **cataloguing/translation labour system**.

This is not merely bias at the level of interpretation. Material/textual difficulty + available expertise + condensation requirements + publication economy selected which kinds of knowledge became legible.

The chain is:

**manuscript difficulty -> labour bottleneck -> abstraction difficulty -> editorial scope change -> published representation of the collection.**

---

## 9. A downstream analogue to the 1827 manuscript-production economy

Wave 13 reconstructed the upstream production economy:

**paper purchase -> copying -> binding -> bundling -> carpentry/labour -> porterage -> shipment -> receipt.**

Mitra 1882 now gives a downstream analytical economy:

**physical collection -> funded reading labour -> Sanskrit abstracts -> supervisory comparison -> English translation -> selective verification -> editorial condensation -> printed analytical catalogue.**

These are structurally comparable without being identical.

The manuscript is made twice:

1. as a transportable copied material object;
2. later as an institutionally legible analytical object.

This may become one of the article's strongest long-duration structures.

---

## 10. Counting is itself an output of labour

The 144/170 work counts should therefore not be treated as passive discovery of a pre-existing number.

To count `works`, cataloguers/readers must:

- access the physical unit;
- inspect internal boundaries;
- read titles and/or colophons;
- distinguish anthology from separate work;
- resolve aliases and repeated titles;
- compare copies where necessary;
- decide what qualifies as a separate work for the current catalogue.

A textual-work count is an **achieved descriptive state**.

This does not make it arbitrary. It makes the count historically reconstructible.

---

## 11. New mechanism: catalogue labour economy

### Definition

**Catalogue labour economy** = the allocation of money, expert readers, languages, scripts, intermediate abstracts, checking time and publication space required to convert materially possessed objects into institutionally usable descriptions.

### Why the term is useful

It prevents `cataloguing` from becoming a black box. In Mitra's case, we can observe:

- institutional patronage and Council funding;
- division of labour;
- differentiated expertise;
- supervision;
- partial checking;
- translation stages;
- limits imposed by time and difficulty;
- resulting changes in the topical scope of the publication.

This mechanism should be tested against zoological cataloguing, especially Gray/Hodgson correspondence, before being promoted into a general cross-domain claim.

---

## 12. New count-version record

Store at least:

```json
{
  "source": "Mitra 1882 preface",
  "collection": "Asiatic Society of Bengal Hodgson Sanskrit-Buddhist collection",
  "versions": [
    {
      "context": "historical distribution statement",
      "bundle_count": 85,
      "work_count": 144,
      "printed_page": "xxiv"
    },
    {
      "context": "collection as immediate object of Mitra analysis",
      "bundle_count": 86,
      "work_count": 170,
      "printed_page": "xl"
    }
  ],
  "relation": "UNRESOLVED_COUNT_VERSION_CONFLICT",
  "possible_resegmentation_relation": "PLAUSIBLE_NOT_DEMONSTRATED"
}
```

---

## 13. New microcase record — B.5

```json
{
  "institutional_identifier": "B.5",
  "earlier_description": "Dharani-mantra-sangraha",
  "later_description": "comprises 39 Dharanis",
  "later_page": "291-292",
  "change_type": "UNDERDESCRIBED_COMPOSITE_TO_RESEGMENTED_COMPOSITE",
  "identifier_stable": true,
  "internal_count_after_deeper_inspection": 39,
  "overlap_with": "B.65",
  "overlap_status": "some Dharanis explicitly said to occur in both",
  "image_verified": false,
  "text_status": "DIRECT_1882_OCR_MULTIPLE_DIGITAL_WITNESSES"
}
```

---

## 14. Article-level consequence

A sharper formulation is now available:

> Institutions did not merely catalogue Hodgson's manuscripts after receiving them. They had to manufacture textual individuality through paid and supervised acts of reading. Mitra's 1882 reanalysis shows that shallow inspection could alter the number of works, while deeper inspection of a stable object such as B.5 disclosed thirty-nine internal Dharanis. Yet deeper cataloguing remained selectively verified and materially constrained: Newari script, textual errors, technical vocabulary, labour availability and the difficulty of condensation reshaped the very subjects that the published catalogue represented.

This makes catalogue production a knowledge-making operation in the same strong sense as copying, drawing, paper-making and specimen preparation.

---

## 15. Immediate next checks

1. Recover Hunter 1881 full text and determine whether the Asiatic Society list there explicitly carries the **85/144** state.
2. Compare Hunter 1881 with Hunter 1896 to establish which titles Mrs Hodgson or Hunter revised after Mitra's 1882 criticism.
3. Inspect Mitra p.80 `Dharani-mantra-sangraha B.5` in page image to establish exactly how shallow the earlier description was.
4. Trace B.5/B.65 physical descendants in current Asiatic Society catalogues if accessible.
5. Search Asiatic Society Proceedings for the Council decision funding Mitra's analysis and any payments to Pandits/printers; this could quantify the catalogue labour economy.
6. Compare Mitra's workflow with Cowell/Eggeling and with Gray's zoological catalogue labour before claiming a cross-domain institutional pattern.

## Bottom line

Wave 16 turns catalogue correction from an abstract afterlife into a labour and material process. The same Mitra preface preserves a 85-bundle/144-work distribution count and a 86-bundle/170-work analytical count, a conflict that must remain versioned rather than silently harmonised. B.5 supplies the object-level mechanism: a stable identifier whose fuller analysis exposed 39 internal Dharanis. Mitra then reveals what such re-segmentation cost institutionally — Council funding, multiple Pandits, supervised comparison, translation through intermediate abstracts, selective checking and editorial compromise. Institutional legibility was manufactured.