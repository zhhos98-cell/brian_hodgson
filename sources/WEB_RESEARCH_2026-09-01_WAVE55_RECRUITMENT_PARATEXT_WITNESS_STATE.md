# Web research 2026-09-01 — Wave 55
## Recruitment paratext: direct marker, direct body, and unresolved reprint body

Date: 2026-09-01

Status: paper-centred paratext/versioning source-control wave following Waves 53–54.

## Executive result

The recruitment-policy addition to Hodgson's military-tribes paper can now be coded more precisely across print states without filling inaccessible text from inference.

### 1857 Selections

Direct full text shows:

- the recruitment sentence ending at `most highly prized.*`;
- the asterisk footnote marker;
- the full retrospective footnote body beginning `Since this paper was written (twenty-five years back)`.

Thus:

`1857 = FOOTNOTE_MARKER_DIRECT + FOOTNOTE_BODY_DIRECT`.

### 1874 Essays

Searchable 1874 text directly preserves the recruitment sentence ending `most highly prized.*` at the same argumentative location.

Thus:

`1874 = FOOTNOTE_MARKER_DIRECT`.

The currently accessible OCR/text interfaces have not yet yielded the associated footnote body.

Thus:

`1874 = FOOTNOTE_BODY_UNREAD`.

This is a narrower and more useful state than either `footnote absent` or generic `unknown`.

Mechanisms:

- `PARATEXT_WITNESS_STATE_MUST_SEPARATE_MARKER_FROM_BODY`
- `PARATEXTUAL_LAYER_PERSISTENCE_CANDIDATE`
- `ACCESS_FAILURE_NOT_TEXTUAL_ABSENCE`
- `PARATEXT_HAS_ITS_OWN_VERSION_HISTORY`.

## 1. Direct 1857 state

Primary searchable full text:
https://archive.org/stream/in.ernet.dli.2015.23938/2015.23938.Records-Of-The-Government-Of-Bengal-No27_djvu.txt

The body states that Gorkhali military services, if obtained, would become highly prized and places an asterisk after the sentence.

The note then retrospectively dates the paper to roughly twenty-five years earlier and reassesses the recruitment question in light of later experience.

This is the secure baseline for the paratext layer.

## 2. 1874 marker state

Bibliographic/full-view witnesses include:

- HathiTrust Harvard copy `hvd.32044060254646`;
- HathiTrust Michigan copy `mdp.39015029241042`;
- Internet Archive/Open Library edition `essaysonlanguage00hodg`;
- searchable OCR witnesses surfaced through web indexing.

HathiTrust Harvard text-only landing page:
https://babel.hathitrust.org/cgi/ssd?id=hvd.32044060254646

The searchable 1874 body preserves the recruitment sentence with `most highly prized.*`, demonstrating that a footnote call remains at the corresponding position.

However, current tool access to HathiTrust page-at-a-time OCR is blocked by semicolon-parameter encoding in section links, and other OCR surfaces have not returned the note body.

Therefore do **not** infer the body's presence, absence or exact wording from the marker alone.

## 3. Evidence state table

| State | Marker | Body | Reading status |
|---|---|---|---|
| 1833 JASB | requires separate check | not a 1857 retrospective addition | first-publication baseline |
| 1857 Selections | DIRECT | DIRECT | new retrospective recruitment paratext |
| 1872 Phoenix | UNREAD | UNREAD | serial transmission function known, page text unread |
| 1874 Essays | DIRECT | UNREAD | same-position footnote call survives; body unresolved |
| later secondary reception | n/a | cited/quoted as Hodgson's 1857 addition | secondary reception only |

## 4. What can be claimed now

Safe claim:

**the paratextual call survives into the 1874 base text at the same recruitment sentence.**

Not yet safe:

- that the complete 1857 footnote survives unchanged in 1874;
- that Phoenix retains it as a footnote;
- that Phoenix moves it into the running text;
- that 1874's star points to exactly the 1857 wording;
- that OCR failure means the note was omitted.

## 5. Why this matters for the paper argument

The paper article already shows asynchronous revision within the 1857 state:

`old descriptive body + new retrospective footnote`.

The later print history now raises a second operational question:

**what happens to a revision layer after it has been attached paratextually?**

Possible transformations are:

1. `footnote -> footnote continuity`;
2. `footnote -> revised footnote`;
3. `footnote -> body incorporation`;
4. `footnote -> omission`;
5. `footnote -> split between body and note`.

These are material/documentary transformations because typographic location controls the relation between old body text and later authorial intervention.

Working mechanism:

`PARATEXT_PLACEMENT_IS_A_VERSION_VARIABLE`.

## 6. Near-contemporary transmission context

The 1875 *Indian Antiquary* review independently states that the 1874 papers were reprinted from the Phoenix states and that Phoenix had introduced numerous marginal notes from Hodgson's own earlier printed copies into the text.

Source:
https://jainqq.org/booktext/Indian_Antiquary_Vol_04_Romanized/032496

This establishes a general mechanism of marginalia-to-running-text incorporation at Phoenix stage.

But it does not prove that this particular 1857 recruitment footnote was moved into the Phoenix body.

Keep:

`GENERAL_TRANSMISSION_MECHANISM_SECURE`

separate from:

`THIS_PARATEXT_PLACEMENT_UNRESOLVED`.

## 7. Later reception

Later scholarship explicitly identifies the recruitment passage as a footnote Hodgson added in 1857. Coleman, for example, quotes it as a revealing footnote added in that year.

This is useful for reception history but does not replace a direct 1874 page reading.

## Source-control rules

1. Footnote marker and footnote body are separate evidence fields.
2. A surviving marker does not prove unchanged body text.
3. OCR non-retrieval is not textual absence.
4. General Phoenix marginalia-incorporation evidence does not establish this particular footnote's location.
5. Secondary quotations may support reception/provenance but do not outrank direct edition witnesses.
6. Preserve 1857, Phoenix, 1874 and post-1874 copy-specific paratext states separately.

## Immediate next actions

1. Obtain a direct page-at-a-time HathiTrust/IA image or OCR of the 1874 asterisk note.
2. Read Phoenix No.26 pp.31–35 and determine whether the recruitment update remains paratext or has entered body text.
3. Compare exact wording of the recruitment update in 1857, Phoenix and 1874 if recovered.
4. Check whether the Alderley Oct 1874 p.37 annotation addresses the article's opening/recruitment framing.
5. Add paratext placement as a field in the publication-version graph.

## Bottom line

The 1857 recruitment update is directly recoverable as a new retrospective footnote attached to an older body text. The 1874 reprint directly preserves the footnote call at the same recruitment sentence, but its body is not yet directly recovered from accessible OCR. The correct historical state is therefore neither continuity nor omission but a controlled intermediate category: `marker survives; paratext body unread`. This keeps typographic placement itself available as a versioning variable rather than erasing it through inference.