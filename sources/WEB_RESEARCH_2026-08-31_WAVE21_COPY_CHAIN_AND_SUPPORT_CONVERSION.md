# Web research 2026-08-31 — Wave 21
## Copy chains, supply leaves, and directly observed support conversion

Date: 2026-08-31

Status: follow-up to the cross-support matrix. This wave changes the evidential target from `same work on different supports` to manuscript relations explicitly described as `copy`, `archetype`, `supply leaf`, or `copied to order`. The central result is a directly documented palm-leaf-to-paper conversion event at the level of a damaged final leaf.

## Executive result

The project now has direct evidence that support change can occur **inside a documented copy relation**, but the first secure case is a repair/surrogation event rather than wholesale recopying of a complete work.

Cambridge Add. 1644 is a palm-leaf `Pañcarakṣā`, dated Nepal Samvat 325 / A.D. 1205. Bendall states that its mutilated last palm leaf was `supplied by a paper leaf`. He further concludes that the paper supply appears to be a copy of the real last leaf made when the original was still in a more complete condition. The paper copy reproduces the old date even though its hand and paper are modern; Bendall interprets this copied date as deliberate testimony to the antiquity of the perishing original leaf, not as forgery or careless repetition.

This is therefore a securely observed chain:

`damaged palm-leaf final leaf -> transcription/surrogation -> modern paper supply leaf -> old date/textual ending preserved within same manuscript object`.

Mechanisms:

- `PALM_LEAF_DAMAGE_TO_PAPER_SUPPLY`
- `SUPPORT_CONVERSION_AS_PRESERVATION_REPAIR`
- `PAPER_SURROGATE_PRESERVES_PERISHING_LEAF`
- `COPIED_DATE_AS_MATERIAL_MEMORY`
- `PARTIAL_SUPPORT_CONVERSION_WITHIN_MANUSCRIPT_OBJECT`

The case proves that support conversion can be an operation of preservation and state transfer rather than a wholesale shift from one manuscript format to another.

---

## 1. Add. 1644: direct palm-leaf -> paper support conversion

Bendall describes Add. 1644 as:

- `Pañca-rakṣā`;
- palm leaf;
- 94 leaves (OCR typography uncertain in the scan, but chapter leaf counts total 94);
- five lines per page;
- approximately 21 × 2 in. in the OCR order; the printed scan typography should be checked before publication-level numerical use;
- dated Nepal Samvat 325 / A.D. 1205.

The physical event is explicit:

> `The last leaf is much mutilated, and is supplied by a paper leaf.`

Bendall then gives the stronger genealogical statement. The manuscript concludes with a paper supply leaf which `appears to be a copy of the real last leaf of our MS. when it was in a rather more perfect condition`, although he allows that another manuscript may also have been consulted because some forms differ.

The replacement therefore has a defensible source relation to the surviving palm-leaf original.

Source control:

- Cecil Bendall, *Catalogue of the Buddhist Sanskrit Manuscripts in the University Library, Cambridge* (1883), Add. 1644, pp. 152–153.
- Internet Archive full text, lines 10717–10768 in the parsed surrogate.

### Why this matters

This is stronger than an exact-work cross-support comparison because the catalogue explicitly joins the two supports within one object history.

The proper causal description is:

`material decay -> risk of information loss -> selective recopying -> support substitution -> continued composite object`.

The unit of conversion is one leaf, not the work.

Mechanism:

`LEAF_LEVEL_SUPPORT_CONVERSION`.

---

## 2. The copied date is not a dating error; it is part of the preservation operation

The paper supply leaf carries the old date and scribe name. Bendall notes that the hand and paper of the supply are modern, so the date is demonstrably copied rather than the production date of the paper leaf.

His interpretation is unusually explicit: the copied date is neither forgery nor thoughtless repetition, but was added as testimony to the antiquity of the damaged final leaf.

This produces two different temporal values on one paper leaf:

- **material/inscription time of the replacement paper**: modern relative to the 1205 palm leaf;
- **represented manuscript date**: N.S. 325 / A.D. 1205, transferred from the old leaf.

Mechanisms:

- `MATERIAL_DATE_VS_REPRESENTED_DATE`
- `COPIED_COLOPHON_AS_TEMPORAL_SURROGATE`
- `PAPER_AS_CARRIER_OF_PRIOR_SUPPORT_TIME`

This is directly relevant to the larger paper article because paper does not merely carry textual content. It can carry **metadata about an earlier material state**.

---

## 3. Bendall explicitly generalizes the phenomenon

In his palaeographical introduction Bendall says there are two real cases of copied dates in the Cambridge corpus. In each case, the last leaf of a palm-leaf manuscript had suffered through time and use, and a paper supply leaf recording the original date was preserved together with it. He singles out Add. 1644 as the especially clear case.

Thus the operation is not reconstructed only from one catalogue entry. Bendall himself treats it as a material-palaeographical class:

`perishing palm-leaf ending + paper supply + copied date`.

He also stresses that manuscript material itself provides chronological evidence and remarks that historical papers differ materially from modern Nepalese paper.

Mechanisms:

- `REPAIR_PRACTICE_AS_PALAEOGRAPHICAL_EVIDENCE`
- `SUPPORT_MATERIAL_AS_CHRONOLOGICAL_EVIDENCE`

---

## 4. Add. 1475: paper -> different paper replacement as a control

Add. 1475 is a seventeenth-century paper `Pañcarakṣā`:

- originally 114 leaves;
- five lines per page;
- 12 × 2 in.;
- seventeenth century.

Its last leaf is on **different paper** and in a slightly later hand. The replacement carries N.S. 802 / A.D. 1682, but Bendall again argues that it is simply a fresh copy of a damaged leaf and explicitly directs the reader to the introduction and Add. 1644.

This produces a useful same-support control:

`damaged paper leaf -> replacement on different paper -> copied old date`.

Mechanisms:

- `PAPER_TO_PAPER_REPLACEMENT_LEAF`
- `SUPPORT_STATE_CHANGE_WITHOUT_SUPPORT_CLASS_CHANGE`
- `COPIED_DATE_DOES_NOT_DATE_REPLACEMENT_SUPPORT`

The comparison with Add. 1644 shows that **copying and support conversion are analytically separable variables**:

- Add. 1644: copy relation + support class change (`palm leaf -> paper`);
- Add. 1475: copy relation + support class continuity (`paper -> paper`).

This distinction should now structure all further matched-witness work.

---

## 5. Add. 1478: explicit archetype -> Hodgson India Office manuscript

Bendall describes Cambridge Add. 1478 as:

- paper;
- 166 leaves;
- six to eight lines per page;
- approximately 13¾ × 2 in. according to the printed full-text surrogate; the fractional dimension should be checked against the page image before publication;
- chiefly Bengali hand;
- fourteenth–fifteenth century;
- catalogued by Bendall as `Śikṣā-samuccaya by Jayadeva` (retain this historical attribution as source wording; modern attribution is a separate historiographical matter).

He then states:

> `This MS. is the archetype of the Hodgson MS. (No. 15) in the India Office.`

This is the strongest explicit full-work genealogical relation currently located:

`Cambridge Add. 1478 -> archetype of -> Hodgson India Office MS No. 15`.

Mechanism:

`EXPLICIT_ARCHETYPE_TO_HODGSON_COPY_CHAIN`.

### Target-support status remains unresolved

The physical description of the India Office Hodgson MS No. 15 has **not yet been securely identified** in the later India Office catalogue numbering.

A tempting preliminary concordance (`General Collection No. 15 -> Catalogue No. 957`) must be rejected. Catalogue No. 957 in Eggeling’s general collection is Rayamukuṭa’s `Padacandrikā`, not the Buddhist `Śikṣāsamuccaya`. The shared number 15 is therefore a numbering collision, not an identification.

Mechanism:

`NUMBERING_COLLISION_REJECTED_BY_TITLE_CONTROL`.

The 1935 catalogue contains a separate `Hodgson Collection` concordance, confirming that general-collection numbers and Hodgson numbers must be kept distinct. The exact historical `Hodgson MS No. 15` used by Bendall still requires shelfmark resolution before its support can be coded.

Do not claim support conversion for this chain yet.

---

## 6. Wright/Cambridge: copying as an institutional procurement operation

Bendall’s preface supplies a second class of explicit copy relation. On Cowell’s suggestion, Daniel Wright was asked to procure specimens of copies that could be `made to order` from works still extant in Nepal. Those specimen transcripts became Cambridge Add. 1042. Wright subsequently discovered that originals were purchasable as well.

The catalogue then gives a concrete example, Add. 865 `Divyāvadāna`:

- paper;
- 258 leaves;
- 14–15 lines per page;
- 14 × 6½ in.;
- modern Nepalese hand;
- written 1873;
- explicitly `Copied to order for the University Library, through Dr D. Wright, from the only early copy known to exist, still preserved at Katmandu.`

This changes the meaning of nineteenth-century paper witnesses. Some are not merely later survivals on paper; they are **institutionally commissioned surrogate objects** manufactured because a European collection wanted textual access to an older Nepalese exemplar.

Mechanisms:

- `INSTITUTIONALLY_COMMISSIONED_MANUSCRIPT_SURROGATE`
- `COPY_TO_ORDER_AS_COLLECTION_TECHNOLOGY`
- `TEXTUAL_ACCESS_BY_NEW_PAPER_OBJECT`

The relation to Hodgson is structural rather than a direct Hodgson copy chain: Bendall explicitly frames Wright’s programme as a continuation of the manuscript access opened by Hodgson, but the individual Add. 865 commission belongs to Wright/Cambridge.

---

## 7. New analytical distinction: copy relation and support conversion are orthogonal

The evidence now supports a two-axis model.

### Axis A — textual/object genealogy

- no demonstrated relation;
- same named work;
- same textual portion;
- explicit copy;
- explicit archetype;
- commissioned transcript.

### Axis B — support relation

- same support, similar paper;
- same support, different paper;
- palm leaf -> paper;
- paper -> paper;
- unknown target support.

This prevents two recurrent errors:

1. assuming that different supports prove a copy transition;
2. assuming that an explicit copy relation necessarily involves support change.

Mechanism:

`COPY_GENEALOGY_ORTHOGONAL_TO_SUPPORT_TRANSITION`.

---

## 8. Article-level formulation

A stronger article paragraph can now be written:

**Paper entered Himalayan manuscript histories not only as a new support for complete copies but as a technology of selective survival. In Cambridge Add. 1644, a thirteenth-century palm-leaf Pañcarakṣā ends with a modern paper supply leaf made from its deteriorating final palm leaf. The replacement reproduces the old date, not as its own production date but as information about the earlier support whose disappearance it anticipates. Support conversion here is therefore a preservation operation: material decay produces a paper surrogate that transfers text, colophon and temporal metadata while remaining physically attached to the older object. A comparison with Add. 1475, where a damaged paper leaf is replaced by another paper leaf, shows that copying and support change must be treated as independent variables.**

Then connect to collection making:

**The same distinction scales upward. Bendall could identify Cambridge Add. 1478 as the archetype of a Hodgson manuscript in the India Office, while Wright’s later Cambridge programme commissioned paper copies to order from manuscripts still held in Nepal. Nineteenth-century manuscript collections were therefore assembled not only by acquiring old objects but by producing new paper surrogates whose genealogical relation to older witnesses could sometimes be explicitly recorded.**

---

## 9. Next research targets

1. Resolve the historical shelfmark and physical description of `Hodgson MS No. 15` in the India Office to complete the Add. 1478 archetype chain.
2. Mine the India Office Hodgson collection for phrases such as `copy of`, `another copy`, `transcript`, `from the original`, `copied for Hodgson`, and explicit source manuscripts.
3. Search Paris/Société Asiatique and Calcutta Hodgson destinations for reciprocal statements linking copies to Nepalese exemplars.
4. Separate full-work commissioned copies from leaf-level repairs and archival replacement leaves in the structured dataset.

## Bottom line

The paper project now has its first direct support-conversion event. It is not a hypothetical palm-leaf-to-paper transition inferred from dimensions: it is a catalogued damaged palm leaf whose content and old date were deliberately transferred to a modern paper supply leaf. This forces a more precise history of support change in which copying, repair, preservation, collection building and support substitution are related but non-identical operations.