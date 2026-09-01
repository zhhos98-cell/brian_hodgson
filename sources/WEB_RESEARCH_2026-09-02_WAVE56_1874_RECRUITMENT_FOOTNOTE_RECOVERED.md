# Web research 2026-09-02 — Wave 56
## 1874 recruitment footnote recovered: direct presence, damaged OCR, selective paratext survival

Date: 2026-09-02

Status: paper-centred paratext/versioning correction to Wave 55.

## Executive result

Wave 55 coded the 1874 recruitment footnote as:

`MARKER_DIRECT + BODY_UNREAD`.

That state can now be narrowed materially.

Direct Internet Archive OCR of the 1874 *Essays on the Languages, Literature, and Religion of Nepal and Tibet* shows:

- printed p.41 retains the recruitment sentence ending `most highly prized.*`;
- the corresponding footnote body is present in the OCR stream, although badly damaged by the page/table layout;
- the recoverable tail includes `Brahman ... Kshatri Sipi-`, `mercenaries`, `earnestly dwelt ...`, and the date `(1857.)`.

The correct evidence state is therefore:

`1874 = FOOTNOTE_MARKER_DIRECT + FOOTNOTE_BODY_DIRECT_PRESENT_OCR_GARBLED + FOOTNOTE_PLACEMENT_DIRECT`.

This supersedes `FOOTNOTE_BODY_UNREAD`.

It does **not** yet establish exact token-for-token identity with the 1857 footnote because the 1874 OCR destroys much of the note's middle wording.

Mechanisms:

- `DIRECT_PRESENCE_DISTINCT_FROM_EXACT_WORDING`
- `OCR_LAYOUT_FAILURE_CAN_HIDE_PRESENT_PARATEXT`
- `PARATEXT_SURVIVES_SELECTIVE_TEXTUAL_INTEGRATION`
- `PARATEXT_PLACEMENT_IS_A_VERSION_VARIABLE`.

## 1. Direct 1874 locus

Primary witness:

https://archive.org/stream/essaysonlanguage00hodg/essaysonlanguage00hodg_djvu.txt

At printed p.41 the recruitment paragraph reads through the familiar prediction that Gorkhali military services, if obtained, would become `most highly prized.*`.

The asterisk is directly present at the same argumentative locus as in the 1857 *Selections*.

Further down the OCR stream, after the tabular material has disrupted reading order, the associated small-type note is partially recovered. The end is sufficiently legible to show the same retrospective recruitment-policy vocabulary and the explicit terminal date `(1857.)`.

Because the body is actually present in the edition-derived OCR, the following outcomes can now be excluded for the 1874 state at this locus:

- `PARATEXT_OMISSION`;
- `FULL_PARATEXT_TO_BODY_RECODING`.

The remaining exact textual alternatives are:

1. `FOOTNOTE_CONTINUITY` — 1857 wording retained substantially or exactly;
2. `FOOTNOTE_REVISION` — footnote retained but wording altered.

Current state:

`1874 = FOOTNOTE_CONTINUITY_OR_REVISION`.

## 2. Controlled comparison with 1857

Primary 1857 witness:

https://archive.org/stream/in.ernet.dli.2015.23938/2015.23938.Records-Of-The-Government-Of-Bengal-No27_djvu.txt

The 1857 footnote is directly readable as beginning:

`Since this paper was written (twenty-five years back)`

and continuing through:

- the tested `value and ... availability` of Gorkhali soldier tribes;
- Fane, Napier and Lawrence on recruitment;
- Hodgson's own attempts to press the subject on those in authority;
- the prejudice in favour of Brahman and Kshatri Sipahis;
- the danger of a homogeneous army of foreign mercenaries;
- terminal dating to 1857.

The 1874 damaged OCR directly preserves several late-note anchors in the same sequence, especially `Brahman ... Kshatri`, `mercenaries`, `earnestly dwelt`, and `(1857.)`.

This makes continuity highly probable, but source control requires retaining:

`WORDING_IDENTITY_TO_1857 = HIGH_ALIGNMENT_NOT_EXACTLY_VERIFIED`.

Do not silently repair the 1874 OCR by importing the 1857 wording.

## 3. 1874 NOTICE changes the transmission model

The 1874 volume's own NOTICE is stronger evidence for the editorial process than later secondary descriptions.

It states that Hodgson's improved and extended views existed in numerous marginal notes in his copy of the 1841 *Illustrations* and that, similarly, many manuscript additions had been made in his own copy of the 1857 *Selections*. It then states that these corrections and additions were introduced into the text of the reprint.

The same NOTICE identifies the Phoenix as the serial reprint project from which the collected publication developed and explains that publication stopped before the whole programme was completed.

This confirms a general material sequence:

`printed copy -> Hodgson handwriting on print -> editorial/typesetting incorporation -> Phoenix serial state -> 1874 collected state`.

But the directly surviving asterisk and footnote body at the recruitment locus show that `introduced into the text` did not mean typographic homogenization of every intervention into running prose.

The process was locus-specific:

`some handwritten additions -> running text`

while

`existing retrospective recruitment intervention -> remains paratext in 1874`.

This is a useful correction to any model that treats marginalia-to-print incorporation as a single global transform.

Mechanism:

`EDITORIAL_INCORPORATION_IS_LOCUS_SPECIFIC_NOT_DOCUMENT_GLOBAL`.

## 4. Why this matters for the paper argument

The military-tribes paper now supplies a stronger material example of asynchronous versioning.

By 1874 the same printed work can simultaneously contain:

- old body readings carried over from earlier print states;
- body readings changed through the Phoenix/collected-reprint process;
- an 1857 retrospective footnote still visibly marked as paratext;
- a printed correction apparatus proposing still later changes;
- physical copies that Hodgson subsequently annotates again by hand.

Thus the operational unit of revision is smaller than the document and smaller than the edition.

A better formulation is:

**revision attaches to loci and layers on particular paper/print surfaces; a new edition can integrate one intervention into running text, preserve another as footnote, and leave another for later handwritten correction.**

This preserves the article's paper-object argument rather than reducing the case to abstract textual variants.

## 5. Phoenix state remains the decisive missing breakpoint

Bibliography and Google Books metadata securely identify *The Phoenix*, vol. III (1872), with No.27 beginning at p.41. This is consistent with the military-tribes article's established placement in No.26, August 1872, pp.31–35.

The bound Volume 3 has now been located in Google Books, but current web-readable endpoints expose metadata/contents rather than the target page OCR.

Therefore Phoenix remains:

`MARKER_UNREAD + BODY_UNREAD + PLACEMENT_UNRESOLVED`.

Do not infer its exact state solely from the 1874 result.

The new 1874 evidence does, however, sharpen the Phoenix question:

**did Phoenix already preserve the recruitment update as a footnote, or did the collected 1874 typesetting restore paratextual separation?**

That is now the key transmission test.

## Source-control rules

1. Replace 1874 `BODY_UNREAD` with `BODY_DIRECT_PRESENT_OCR_GARBLED`.
2. Presence, placement and exact wording remain separate fields.
3. Do not reconstruct illegible 1874 words by copying 1857 text into the direct-witness field.
4. The `(1857.)` tail is direct evidence that the 1874 note preserves the retrospective dating layer.
5. General statements that corrections/additions were `introduced into the text` describe an editorial process, not the typographic placement of every individual locus.
6. Phoenix remains unread until its target pages are directly recovered.
7. Direct edition evidence outranks secondary quotation for wording and placement.

## Immediate next actions

1. Recover Phoenix vol.III no.26 pp.31–35 from a page-image/full-view endpoint.
2. Search Phoenix specifically for `most highly prized`, `Since this paper was written`, `Brahman and Kshatri`, and `foreign mercenaries`.
3. Recover a higher-quality 1874 page image/OCR for the footnote and compare exact wording with 1857.
4. Add a three-level evidence field to the publication graph: `presence`, `placement`, `wording fidelity`.
5. Revisit the chronology and caste/cast loci under the same locus-specific integration model.

## Bottom line

The 1874 recruitment footnote is no longer an unread body inferred from a surviving star. It is directly present in edition-derived OCR, remains paratextual, and ends with the retrospective `(1857.)` marker. Exact wording remains partly unread because OCR collapses the small-type note into the adjacent table. This changes the transformation problem from `continuity vs revision vs recoding vs omission` to the much narrower `footnote continuity vs footnote revision`, and it shows that the Phoenix/1874 incorporation process operated selectively at individual textual loci rather than synchronizing the whole document.