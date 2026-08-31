# Web research 2026-09-01 — Wave 50
## Phoenix 1872 as the decisive intermediate witness; 1857 readings locked

Date: 2026-09-01

Status: paper-centred microrevision follow-up to Wave 49. This wave narrows the change interval for two readings in Hodgson's `Origin and Classification of the Military Tribes of Nepal` and locates the August 1872 Phoenix witness without inventing unread text.

## Executive result

Two key readings are now directly recoverable in the 1857 `Selections from the Records of the Government of Bengal, No. XXVII` full text:

1. physiognomic phrase: `general caste and character`;
2. Gorkha/Khas chronology: `seventy years ago`.

Therefore both later changes occur **after 1857**.

The next surviving publication witness is now securely located:

`The Phoenix`, vol. III, no. 26, August 1872, pp. 31–35,

which Boulnois explicitly identifies as a reprint of the military-tribes paper.

Google Books contains multiple full-view digitizations of vol. III. One 1872 copy exposes No. 26 in the table of contents. However, during this wave the Google Books `text-only` endpoint returned 403 and full PDF download required CAPTCHA. Thus the two target readings in Phoenix remain unread.

The correct current interval is:

`1857 [caste; seventy]`
→ `Phoenix Aug 1872 [LOCATED, READINGS UNRECOVERED]`
→ `1874 base [caste; some]`
→ `1874 correction apparatus [cast; about 100]`.

Mechanisms:

- `INTERMEDIATE_WITNESS_LOCATED_TEXT_UNREAD`
- `REVISION_INTERVAL_NARROWED_AFTER_1857`
- `PRINTED_PAGE_REOPENED_BETWEEN_EDITION_STATES`
- `SOURCE_CONTROL_PREVENTS_BACK_PROJECTION`.

---

## 1. 1857 chronology is explicitly `seventy years ago`

The Internet Archive full-text representation of `Records Of The Government Of Bengal, No.27` contains the military-tribes essay.

At the Khas/Gorkha passage it reads:

`because it was thence immediately that they issued, seventy years ago, under the guidance of Prithvi Narayan ...`

Source:
https://archive.org/stream/in.ernet.dli.2015.23938/2015.23938.Records-Of-The-Government-Of-Bengal-No27_djvu.txt

This directly resolves the previously open 1857 chronological state.

Thus:

`1833: 70 years`
→ `1857: seventy years`.

The `70 -> some` change did **not** occur between the JASB print and the 1857 Selections.

Mechanism:

`EARLY_PRINT_READING_PERSISTS_TO_1857`.

---

## 2. 1857 physiognomic phrase is explicitly `general caste and character`

The same Internet Archive full text reads:

`Their physiognomies, too, have peculiarities proper to each, but with the general caste and character fully developed in both.`

This upgrades the earlier indexed-text evidence to a directly searchable full-text witness.

Thus at minimum:

`1857: caste`
→ `1874 base: caste`
→ `1874 correction apparatus: cast`.

The `caste -> cast` intervention is therefore a post-1857 correction unless the October 1832 manuscript proves `cast` was an older manuscript reading later lost in print.

Mechanism:

`POST1857_SEMANTIC_CORRECTION_INTERVAL`.

---

## 3. Phoenix military-tribes reprint is bibliographically secure

Boulnois, `Bibliographie du Népal`, entry 3282, gives the publication history of the military-tribes essay and explicitly lists:

- JASB II, 17 (1833), pp.217–224;
- `Selections`, XXVII, pp.141–149;
- `Phoenix`, III, 26, August 1872, pp.31–35;
- `Essays` (1874).

Source:
https://pahar.in/pahar/Books%20and%20Articles/Nepal/1969%20Bibliographie%20Du%20Nepal%20Volume%201%20Sciences%20Humaines%20by%20Boulnois%20s.pdf

This establishes Phoenix as a real intermediate publication state, not an inferred or merely proposed reprint.

---

## 4. Phoenix vol. III has multiple surviving digital witnesses

Bibliotheca Sinica points to three Google Books digitizations of vol. III:

- Oxford University copy;
- National Library of the Netherlands copy;
- Biblioteca Nazionale Centrale di Roma copy.

Source:
https://china-bibliographie.univie.ac.at/2017/06/21/summers-ed-the-phoenix-a-monthly-magazine-for-china-japan-and-eastern-asia/

The Rome-derived Google Books copy exposes a table-of-contents entry:

`VOL III No 26 AUGUST 1872`.

Google Books volume ID:
`0eaqUKm_xQIC`.

The Netherlands-derived copy is volume ID:
`LXlRAAAAcAAJ`.

These are useful independent scan witnesses for later page-level collation.

---

## 5. Phoenix readings remain explicitly unresolved

Attempts during this wave:

- Google Books full-view volume located;
- No.26 located in table of contents;
- page-level HTML endpoint reached;
- `text-only` endpoint returned HTTP 403;
- PDF download endpoint required CAPTCHA.

Therefore do **not** write:

`Phoenix = some years`

or

`Phoenix = seventy years`.

Likewise do not assign `cast` or `caste` to Phoenix until the actual page is read.

Mechanism:

`INTERMEDIATE_WITNESS_LOCATED_TEXT_UNREAD`.

This is a source-control state, not a research failure.

---

## 6. Revised two-variable microrevision table

### Chronological phrase

| state | reading |
|---|---|
| Oct 1832 fair manuscript | UNREAD |
| 1833 JASB | `70 years ago` |
| 1857 Selections | `seventy years ago` |
| Aug 1872 Phoenix | UNREAD / located witness |
| 1874 base | `some years ago` |
| 1874 correction apparatus | `about 100 years ago` |

The change `seventy -> some` occurred somewhere in the interval:

`1857 < change <= 1874 base`.

Phoenix can reduce that interval further once read.

### Physiognomic phrase

| state | reading |
|---|---|
| Oct 1832 fair manuscript | UNREAD |
| 1833 JASB | requires direct check |
| 1857 Selections | `general caste and character` |
| Aug 1872 Phoenix | UNREAD / located witness |
| 1874 base | `caste` implied by correction apparatus and searchable body |
| 1874 correction apparatus | `cast` |

The intended `cast` correction is demonstrably later than the 1857 printed state, though its relation to 1832 remains open.

---

## 7. Phoenix matters because the 1874 Notice describes manuscript-on-print revision

The 1874 `NOTICE` states that Hodgson made many manuscript additions in his own copy of the 1857 `Selections`, and that corrections/additions were incorporated into the new reprint.

It also says Phoenix began reprints from the `Selections` at vol. II p.96 and that the serial programme was interrupted when Summers left for Japan.

Thus the historically relevant conversion path is not merely:

`1857 print -> 1874 print`.

It includes a material working state:

`1857 printed copy`
→ `Hodgson manuscript additions on print`
→ `Phoenix serial and/or 1874 editorial setting`
→ `1874 collected print`.

Exactly which manuscript additions entered Phoenix before 1874 must be determined by direct Phoenix collation.

Mechanism:

`PRINTED_COPY_AS_MANUSCRIPT_WORKING_SURFACE`.

---

## 8. Falsifiable outcomes once Phoenix is read

### Outcome A
Phoenix has `some`.

Then:

`seventy -> some` occurred by August 1872.

The strongest candidate mechanism becomes manuscript revision incorporated into the Phoenix serial state.

### Outcome B
Phoenix retains `seventy`.

Then:

`seventy -> some` occurred after Phoenix, during preparation of the 1874 collected edition or another intermediate editorial state.

### Outcome C
Phoenix has `cast`.

Then the semantic correction predates the 1874 correction list, raising the possibility that the list registers a correction incompletely applied to the collected setting.

### Outcome D
Phoenix retains `caste`.

Then `cast` is a 1874-apparatus-level intended correction unless the manuscript witnesses show an older reading.

---

## 9. Paper-history payoff

This microrevision chain makes printed paper itself an observable historical instrument.

The key object is not a sequence of abstract texts but a sequence of material states:

`fair manuscript`
→ `journal print`
→ `government-record reprint`
→ `printed copy reopened by handwriting`
→ `serial reprint`
→ `collected reprint + correction apparatus`
→ `copy-specific handwritten annotations`
→ `1972 selective editorial extraction`.

The same claim can acquire, lose, and regain precision across these surfaces.

The documentary operation is therefore recursive:

`print can become manuscript substrate`.

---

## Immediate next actions

1. Obtain/read Phoenix III no.26 pp.31–35 from a library/full-view export and record the two target readings.
2. Inspect MSS EUR HODGSON/6 item 1 for `cast/caste` and the Gorkha date phrase.
3. Inspect vol.9/10 at the same loci.
4. Recover the 1972 Saha supplement's entries for Part II pp.37–44.
5. Recover Alderley Oct 1874 copy p.37 marginalia.
6. Compare the three Phoenix digital scan witnesses if OCR or typesetting ambiguity appears.

## Bottom line

The 1857 `Selections` now fixes both target readings: `general caste and character` and `seventy years ago`. Therefore both important late changes occur after 1857. Phoenix III no.26 (August 1872, pp.31–35) is now securely located as the decisive intermediate publication witness, but its target readings remain unread because Google Books blocked text-only access and download during this wave. The correct scholarly state is therefore to narrow the revision interval without back-projecting the 1874 readings into Phoenix.