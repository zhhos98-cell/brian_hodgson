# Web research 2026-08-31 — Wave 32
## Denominator missingness, relation-strength tiers and multi-version derivative families

Date: 2026-08-31

Status: methodological/source-control follow-up to Waves 30–31. Scope remains paper. This wave asks what would bias a denominator-complete conversion census and separates strict source→derivative edges from broader catalogue families.

## Executive result

The conversion corpus now has enough positive examples that the main risk is **selection bias**.

Two problems are visible.

1. Cambridge sometimes identifies a source/derivative relation while omitting paper support for the derivative, especially in some pre-bound notebook descriptions. Dropping those records would bias the observed corpus toward support-known cases.
2. Cambridge cross-references vary in semantic strength. `For original manuscript, see...` is stronger than `for similar manuscripts, see...`. A denominator must not count thematic similarity as direct documentary descent.

A third finding strengthens the substantive argument while also illustrating the second problem: the large Buddhist chronicle family around `vol.52/2` contains derivative/related states on both Nepali handmade and machine-made paper and in English and Farsi. It is a strong **version ecology**, but not every edge is equally secure as direct copying descent.

Mechanisms:

- `SUPPORT_MISSINGNESS_MUST_ENTER_DENOMINATOR`
- `RELATION_STRENGTH_TIERING`
- `DERIVATIVE_FAMILY_NOT_ALWAYS_DIRECT_STEMMA`
- `VERSION_ECOLOGY_ACROSS_SUPPORTS`
- `CATALOGUE_RELATION_SEMANTICS_ARE_HETEROGENEOUS`

---

## 1. Missing support is a data state, not an exclusion criterion

Several explicit relation targets have no paper class in their current Cambridge item description.

### Gorkhāvaṃśāvali English translation

`vol.17/1`, ff.1–167:

- four separate pre-bound notebooks;
- English translated from Nepali;
- Hodgson/Campbell handwriting;
- explicit original cross-reference;
- **paper support not stated**.

Source:
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol017.html

### Newar kings English chronicle

`vol.17/3`, ff.173–219:

- separate pre-bound notebook;
- English;
- original Nagari versions explicitly cross-referenced;
- **paper support not stated**.

The source-side cross-reference in `vol.55/9` gives ff.178–219, creating an additional folio-boundary discrepancy.

### Bhaktapur/Patan revenue summaries

`vol.13/3`, ff.139–178 and `vol.13/4`, ff.179–222:

- English;
- separate pre-bound notebooks;
- explicit Nepali-original cross-references;
- **paper support not stated**.

Source:
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol013.html

### Required code

`support = UNSPECIFIED_IN_CATALOGUE`

not:

- `MACHINE_MADE` inferred from binding;
- exclusion from denominator;
- or `unknown object`.

Mechanism:

`SUPPORT_MISSINGNESS_MUST_ENTER_DENOMINATOR`.

---

## 2. Why missingness could bias the conversion argument

If support-known English derivatives are disproportionately loose sheets or objects whose paper attracted cataloguer attention, while some bound notebooks lack support descriptions, then a census restricted to support-known items can misestimate support-switch frequency.

The safe denominator architecture is therefore:

`all explicit relation edges`

partitioned into:

- target support known;
- target support mixed;
- target support unspecified;
- target object unresolved.

Only the known-support subset can answer the narrow question `switch vs continuity`.

The full set is required to report the evidence base honestly.

Do not calculate:

`switches / known-support pairs`

without also publishing:

`known-support pairs / all explicit relation pairs`.

---

## 3. Relation-strength tiers

The Cambridge inventory uses cross-reference language with different meanings.

### Tier A — explicit documentary relation

Examples:

- `For original manuscript in Nepali, see...`
- `For English translation and summary, see...`
- `For Persian summary and translation, see...`
- reciprocal source and target cross-references.

These can enter the principal conversion denominator.

### Tier B — explicit source-family relation

Examples:

- multiple local ethnographic manuscripts collectively cross-referenced to `Hill tribes` English synthesis;
- multiple royal codes cross-referenced to one English comparative code notebook.

These support a synthesis relation but do not imply one-to-one scribal descent.

Code as:

`SOURCE_FAMILY_TO_SYNTHESIS`.

### Tier C — content-family / similar-manuscript relation

Phrases such as:

- `see also`;
- `similar manuscripts`;
- `similarities can be seen`;
- `can be compared with`.

These should not enter a direct source→derivative denominator unless another source establishes descent.

### Tier D — researcher-inferred thematic overlap

Exclude from the conversion denominator. Retain only as discovery leads.

Mechanism:

`RELATION_STRENGTH_TIERING`.

---

## 4. Buddhist chronicle vol.52/2 exposes a multi-support version ecology

Source:

`vol.52/2`, ff.7–52:

- Buddhist chronicle/account of Nepal;
- Nepali;
- Nepali hand-made paper;
- Cambridge says an English summary of the early part can be found across multiple referenced items.

Source:
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol052.html

The referenced/closely linked states include materially different objects.

### Nepali handmade English states

`vol.7/26`, ff.165–170:

- English genealogy/list;
- Nepali hand-made paper;
- catalogue links it to Nepali versions including vol.52/2.

`vol.21/6`, ff.25–57:

- English Buddhist account;
- Nepali hand-made paper;
- rough hand of a native writer;
- explicitly notes similarity to the early part of vol.52/2.

### Machine-made English states

`vol.18/5`, ff.27–99:

- English/Sanskrit historical-religious synthesis;
- machine-made paper.

`vol.18/10`, ff.158–175:

- English translation/mahatmya material;
- machine-made paper.

`vol.20/2`, ff.62–102:

- English working state related to Svayambhupurana/Nepal account;
- machine-made paper.

### Nepali handmade Farsi state

`vol.96/18`, ff.146–153:

- Farsi/Sanskrit;
- Buddhist account of Nepal;
- Nepali hand-made paper;
- catalogue cross-references the same family of English/Nepali account states.

Source:
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol096.html

### Interpretation

This is powerful evidence for a **version ecology across supports**, but the edge strength varies.

Some entries are described as summaries; others are explicitly only similar or related.

Therefore the family should support the article claim:

`one knowledge corpus exists in multiple material/version states`

but should not yet be drawn as a single direct stemma with every arrow from `vol.52/2`.

Mechanism:

`DERIVATIVE_FAMILY_NOT_ALWAYS_DIRECT_STEMMA`.

---

## 5. Actor signal inside the chronicle family

The family also reinforces an actor-level variable.

`vol.21/6`:

- English;
- Nepali handmade paper;
- rough hand of a native writer.

By contrast, several machine-paper English analytical states in vols.18 and 20 belong to Hodgson's English notebook/synthesis environment.

This parallels the Siddhinarasimha continuity case.

Working hypothesis:

`local assistant/writer English derivative -> increased probability of retained country-paper stock`

versus

`Hodgson/Campbell analytical/fair notebook state -> increased probability of machine/imported stock`.

This remains a hypothesis. It should be tested with actor-attributed pairs, not inferred from language alone.

Mechanism:

`ACTOR_WORKPLACE_AS_SUPPORT_SELECTION_VARIABLE`.

---

## 6. Jumla revenue gives the denominator's best Tier-A branching case

The Buddhist chronicle family is broad. The Jumla pair is much cleaner.

`vol.59/38` Nepali handmade source explicitly points to:

- `vol.8/1`: English machine-made 48.5 × 38 cm chart by Campbell;
- `vol.102/21`: Farsi Nepali-handmade very neat chart.

The target `vol.8/1` reciprocally points back to `vol.59/38` and to the Persian summary.

Sources:
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol008.html
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol102.html
https://hodgson.socanth.cam.ac.uk/chunkhtml/vol059.html

This is Tier A and should sit near the centre of the article.

It controls source content and general chart form while support diverges.

Mechanism:

`SAME_SOURCE_SAME_GENERAL_FORMAT_DIFFERENT_SUPPORT`.

---

## 7. A catalogue error already affects relation identity

The expanding corpus has exposed several reference discrepancies:

- `vol.59/6` currently cross-references `vol.3/16`, whereas the earlier working note had `vol.3/15`;
- `vol.26/19` refers to `vol.52/13 fol.165–171`, while the current vol.52 page places ff.165–171 under item 14;
- `vol.21/3` points to `vol.51/13 fol.183–185`, while the working source mapping has those folios under a neighbouring item;
- `vol.55/9` points to `vol.17/3 fol.178–219`, while current `vol.17/3` begins at f.173.

This is not merely clerical noise. It means a pair dataset that keys only on `volume/item` will silently corrupt relations.

Required primary key strategy:

`volume + folio range + content title + relation phrase`.

Item number remains a versioned catalogue field.

Mechanism:

`CATALOGUE_RELATION_REQUIRES_FOLIO_CONTROL`.

---

## 8. Denominator architecture v0.1

Each relation edge should now include:

- relation family ID;
- source volume/item;
- source folios;
- source support;
- target volume/item;
- target folios;
- target support;
- source relation phrase;
- target reciprocal phrase, if any;
- relation strength tier A/B/C/D;
- relation operation: copy/translation/summary/abstract/register/synthesis;
- source actor;
- target actor;
- language change;
- format change;
- binding change;
- support relation: switch/continuity/mixed/unspecified;
- catalogue-resolution status.

For denominator statistics:

`principal denominator = Tier A explicit edges`.

Tier B should be reported separately as source-family synthesis evidence.

Tier C/D should not inflate the transformation count.

---

## 9. Immediate targets

1. Build an edge-level denominator table from all v0.2 relation families.
2. Separate Tier A reciprocal pairs from Tier B source-family relations.
3. Add the support-unspecified targets rather than dropping them.
4. Search all current Cambridge volumes for explicit `For original`, `For English summary`, `For Persian/Farsi translation`, `For translation`, and reciprocal target wording.
5. Run an actor-coded subset to test the local-writer/country-paper hypothesis.
6. Physically inspect vol.8/1 and vol.102/21 first: same source and chart-like derivative state, different support.
7. Request/inspect paper support for vol.17 and vol.13 pre-bound derivative notebooks where Cambridge currently omits it.

## Bottom line

The conversion evidence is now strong enough that its main threat is methodological overcounting. A paper-centred article can already demonstrate switch, continuity and branching, but a quantitative claim requires an explicit missing-data denominator and relation-strength hierarchy. The most important result remains qualitative and robust: related Himalayan information was repeatedly versioned into materially different documentary states, yet the material pathway was not one-directional. Some derivatives moved onto machine/imported paper, others stayed on Nepalese handmade paper, and broad knowledge families persisted simultaneously across both.