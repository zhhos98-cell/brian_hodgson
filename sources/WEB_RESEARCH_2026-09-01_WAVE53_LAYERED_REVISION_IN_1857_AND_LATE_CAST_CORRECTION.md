# Web research 2026-09-01 — Wave 53
## Layered revision: 1857 policy update, stable base readings, and the late `caste -> cast` correction

Date: 2026-09-01

Status: publication-versioning follow-up to Waves 49–52.

## Executive result

Direct 1857 full text now shows that Hodgson's reprint revised different layers of the military-tribes paper at different rates.

The 1857 *Selections* preserves two old base-text readings:

- `seventy years ago` for the Gorkha/Khas expansion chronology;
- `general caste and character` for Magar/Gurung physiognomy.

But the same 1857 reprint adds a new retrospective footnote after Hodgson's recruitment argument, beginning `Since this paper was written (twenty-five years back)` and updating the policy history in light of later Gorkhali military service.

Meanwhile the 1833 first publication is now directly readable as:

`general Calmak caste and character`.

Therefore the 1874 printed correction `caste -> cast` is **not a restoration of the 1833 printed reading**. `caste` persisted in print from 1833 through 1857 and remained the 1874 base reading before Hodgson's correction apparatus instructed `cast`.

Mechanisms:

- `REVISION_IS_LAYERED_NOT_WHOLE_DOCUMENT_SYNCHRONOUS`
- `PARATEXT_UPDATES_WHILE_BASE_TEXT_PERSISTS`
- `POLICY_LAYER_REVISED_BEFORE_DESCRIPTIVE_MICROREADINGS`
- `LATE_SEMANTIC_RECALIBRATION_AFTER_LONG_PRINT_STABILITY`
- `PRINTED_PAGE_CAN_HOST_DIFFERENT_VERSION_TIMES_SIMULTANEOUSLY`.

## 1. Direct 1833 reading: caste

Searchable JASB first-publication text:
https://pahar.in/pahar/Books%20and%20Articles/Nepal/1833%20Origin%20and%20Classification%20of%20Military%20Tribes%20of%20Nepal%20by%20Hodgson%20from%20JASBv2%20s.pdf

The Magar/Gurung physiognomy sentence reads in the first print:

`general Calmak caste and character in both`.

The exact typography/line-break form remains an image-level matter, but the word `caste` is directly recoverable from the searchable first-publication text.

Thus:

`1833 = caste`.

## 2. Direct 1857 readings: caste + seventy

Primary full text:
https://archive.org/stream/in.ernet.dli.2015.23938/2015.23938.Records-Of-The-Government-Of-Bengal-No27_djvu.txt

The 1857 reprint reads:

- `general caste and character fully developed in both`;
- Khas issued from Gorkha `seventy years ago` under Prithvi Narayan.

Thus both readings survive from the earlier publication tradition into 1857.

## 3. Direct 1857 retrospective recruitment footnote

The same 1857 text adds a footnote after Hodgson's claim that Gorkhali soldiers could be reliable British servants in arms.

The note explicitly says the paper had been written twenty-five years earlier and that subsequent experience had tested the value and availability of the Gorkhali soldier tribes. It regrets that recommendations by Fane, Napier and Lawrence for larger recruitment were not acted upon earlier and says Hodgson himself repeatedly pressed the policy while his voice carried weight.

This is a direct primary-source example of a later paper state carrying:

`older base text`
+
`new retrospective authorial paratext`.

The page therefore contains more than one temporal layer at once.

Mechanism:

`PARATEXTUAL_REVISION_WITH_BASE_TEXT_RETENTION`.

## 4. Revision rates differ by epistemic layer

The 1857 state demonstrates an asymmetry.

### Recruitment/policy layer

Updated in 1857 through a new retrospective footnote.

### Historical dating layer

Still preserves `seventy years ago`.

### Physiognomic wording layer

Still preserves `caste`.

Only later does the publication chain show:

`seventy -> some -> about 100`

and

`caste -> cast`.

Thus Hodgson did not periodically rewrite the entire paper into a single synchronized current state.

Different claims could be:

- left unchanged;
- supplemented in a footnote;
- later absorbed into serial running text;
- later corrected in an end apparatus;
- later reopened again through handwriting on a printed copy.

This is versioning by layer rather than by document replacement.

## 5. `caste -> cast` is a demonstrably late semantic intervention

Secure publication witnesses now give:

`1833 = caste`
-> `1857 = caste`
-> `Phoenix 1872 = unread; transmission predicts caste`
-> `1874 base = caste`
-> `1874 correction apparatus = cast`.

Therefore the correction cannot be described as recovering the 1833 printed wording.

Two possibilities remain:

1. `cast` restores an unpublished 1832 manuscript reading;
2. `cast` is a genuinely late authorial semantic revision.

Only MSS EUR HODGSON/6 item 1 and vol.9/10 can distinguish these.

Until then code:

`LATE_PRINTED_CORRECTION_SECURE; MANUSCRIPT_RESTORATION_STATUS_UNRESOLVED`.

## 6. `70 -> some -> about 100` is also layered

Secure state:

`1833 = 70 years`
-> `1857 = seventy years`
-> `Phoenix 1872 = unread, predicted some`
-> `1874 base = some years`
-> `1874 corrections = about 100`.

The 1857 recruitment footnote shows that Hodgson was already actively revisiting the paper in 1857, yet did not alter the `seventy years` sentence then.

Therefore the dating recalibration happened in a later revision layer, not simply because the paper was generally 'updated' in 1857.

## 7. Paper/material consequence

The relevant object is not merely a textual proposition but a layered printed support:

`older typeset body`
+
`new typeset footnote derived from later authorial reflection`
+
`later manuscript marginalia on a printed copy`
+
`new serial typesetting`
+
`new collected-edition base`
+
`new correction apparatus`.

A single work therefore has several coexisting material clocks.

Working formulation:

**paper preserves asynchronous revision.**

Mechanism:

`ASYNCHRONOUS_REVISION_PRESERVED_ON_PRINT_SURFACES`.

## 8. Consequence for problem genealogy vs textual stemma

The 1857 footnote strengthens the distinction established in Wave 46.

The military recruitment problem is continuous from Hodgson's early administrative work through 1833 and 1857.

But the classificatory text has its own version history.

Thus:

`problem continuity`
!=
`word-level textual continuity`.

The same policy problem can be retrospectively reinterpreted in paratext while older descriptive sentences remain unchanged.

## Source-control rules

1. The 1833 `caste` reading is now secure at searchable-text level; image-level diplomatic typography remains separately checkable.
2. Do not call 1874 `cast` a restoration until the 1832 manuscripts are read.
3. The 1857 footnote is a new paratextual layer; do not rewrite it as evidence that all 1857 base text was freshly revised.
4. Keep the Phoenix word-level target readings unresolved despite transmission evidence.
5. Distinguish policy revision, historical-dating revision, physiognomic wording revision and classificatory table revision as separate variables.

## Immediate next actions

1. Read `cast/caste` and chronology loci in MSS EUR HODGSON/6 item 1 and vol.9/10.
2. Read Phoenix No.26 pp.31–35 directly to locate the first printed appearance of `some` and test whether `caste` persisted.
3. Compare the 1857 added recruitment footnote against Phoenix and 1874: unchanged footnote, absorbed body text, or revised paratext?
4. Recover Alderley p.37 annotation and test whether it touches the paper's opening/recruitment framing.
5. Recover Saha 1972 military-tribes supplement entries.

## Bottom line

The military-tribes paper now provides direct evidence for asynchronous documentary revision. Hodgson could update the policy interpretation in a new 1857 footnote while leaving older historical and physiognomic wording untouched. The later `caste -> cast` correction came only after `caste` had persisted through at least the 1833 and 1857 print states. Paper did not simply transmit successive complete versions; it preserved overlapping temporal layers of revision.