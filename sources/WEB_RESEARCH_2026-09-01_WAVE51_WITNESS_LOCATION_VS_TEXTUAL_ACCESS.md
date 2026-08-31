# Web research 2026-09-01 — Wave 51
## Witness location is not textual access: Phoenix multiplicity and 1833 source control

Date: 2026-09-01

Status: source-control follow-up to Waves 49–50. This wave formalizes evidence states across manuscript, print, digitization and OCR witnesses.

## Executive result

The military-tribes microrevision chain now has enough witnesses that a new error becomes possible: treating a located digitization as though its target reading had been recovered.

Phoenix vol. III currently has at least four separately identifiable Google Books scan witnesses, including Oxford, National Library of the Netherlands, Biblioteca Nazionale Centrale di Roma, and New York Public Library copies. Yet the August 1872 no.26 target pages remain unread because available text/export interfaces are blocked or do not surface the required phrases.

Thus:

`witness located != target text read`.

Mechanisms:

- `DIGITAL_WITNESS_MULTIPLICITY_DOES_NOT_EQUAL_TEXTUAL_ACCESS`
- `READING_STATE_SEPARATE_FROM_WITNESS_LOCATION`
- `OCR_STATE_SEPARATE_FROM_IMAGE_VERIFICATION`.

## 1. Phoenix publication identity is secure

Boulnois entry 3282 explicitly places `Origin and classification of the Military tribes of Nepal` in:

`Phoenix III, no.26, August 1872, pp.31–35`.

Source:
https://pahar.in/pahar/Books%20and%20Articles/Nepal/1969%20Bibliographie%20Du%20Nepal%20Volume%201%20Sciences%20Humaines%20by%20Boulnois%20s.pdf

This establishes bibliographic existence and position, not the target readings.

## 2. Four digital Phoenix witnesses are now located

### Oxford University scan
Google Books ID: `aTBBAQAAMAAJ`.

### National Library of the Netherlands scan
Google Books ID: `LXlRAAAAcAAJ`.

### Biblioteca Nazionale Centrale di Roma scan
Google Books ID: `0eaqUKm_xQIC`.

The table of contents exposes `VOL III No 26 AUGUST 1872`.

### New York Public Library scan
Google Books ID: `pYIrO0HAJMoC`.

Google's search result identifies this as an NYPL copy digitized in 2023.

Bibliotheca Sinica independently records several vol.III Google digitizations:
https://china-bibliographie.univie.ac.at/2017/06/21/summers-ed-the-phoenix-a-monthly-magazine-for-china-japan-and-eastern-asia/

## 3. Four scans do not yet yield one target reading

During Waves 50–51:

- text-only Google Books endpoints returned 403;
- full export required CAPTCHA;
- search snippets did not surface the target sentences;
- no alternate public transcription of no.26 pp.31–35 was located.

Therefore Phoenix remains:

`BIBLIOGRAPHICALLY_SECURE`
+
`DIGITALLY_LOCATED_MULTIPLE_TIMES`
+
`TEXTUALLY_UNREAD_AT_TARGET_LOCI`.

Do not fill the gaps using 1857 or 1874 readings.

## 4. The two revision questions Phoenix can decide

### Chronology

Known states:

- 1833: `70 years ago`;
- 1857: `seventy years ago`;
- 1872 Phoenix: unread;
- 1874 base: `some years ago`;
- 1874 correction: `about 100 years ago`.

If Phoenix reads `seventy`, the change to `some` occurred after August 1872.

If Phoenix reads `some`, the change had entered the serial state by August 1872.

### Physiognomic phrase

Known states:

- Oct 1832 manuscript: unread;
- 1833 print: direct cast/caste reading not yet secured;
- 1857: `general caste and character`;
- 1872 Phoenix: unread;
- 1874 base: `caste`;
- 1874 correction: `cast`.

Phoenix can reveal whether the intended `cast` correction appeared in the serial before the 1874 collected edition.

## 5. 1833 source-control state

The 1833 chronological reading `70 years ago` is recoverable from the original JASB text and is independently consistent with later reprint history.

A complete JASB vol.II public-domain scan has also been located through Wikisource/Wikimedia/Internet Archive, providing a stronger future image witness than a topic-extracted PDF alone.

However, the specific 1833 `cast/caste` line remains unresolved because:

- available OCR at the target line is garbled;
- page-image access attempts failed during this wave.

Therefore code:

`1833 chronology = LOCKED`

`1833 cast/caste = UNRESOLVED`.

This asymmetry must remain visible.

## 6. Evidence-state schema

Each witness now needs at least four separate fields:

1. `existence_state` — is the physical/publication witness bibliographically secure?
2. `location_state` — is a physical/digital exemplar located?
3. `access_state` — can the target page/text currently be inspected?
4. `reading_state` — is the exact target reading recovered, and by OCR or image?

A fifth field is useful:

5. `material_state` — manuscript, journal print, reprint, serial, corrected print, manuscript-on-print, editorial extraction.

This prevents false certainty produced by digital abundance.

Mechanism:

`WITNESS_CONTROL_REQUIRES_ACCESS_AND_READING_STATES`.

## 7. Article consequence

The source-control method itself reinforces the paper argument.

The same abstract text may survive as multiple material witnesses, but the epistemic accessibility of a reading depends on the state of those witnesses and their digital interfaces.

Digital reproduction therefore does not eliminate material witness problems. It creates another layer:

`physical print`
→ `scan exemplar`
→ `platform access state`
→ `OCR/text layer`
→ `research reading`.

A digitized page can exist and remain practically unread.

This is not the article's main historical claim, but it is a necessary methodological control on the publication stemma.

## Immediate next actions

1. Obtain Phoenix III no.26 pp.31–35 via library scan, HathiTrust, institutional Google access or another exportable witness.
2. Read the two target loci before updating any Phoenix reading.
3. Image-verify the 1833 `cast/caste` line from the complete JASB vol.II scan.
4. Inspect the October 1832 fair manuscript at both microrevision loci.
5. Recover the Saha 1972 Part II supplement and Alderley p.37 marginalia.

## Bottom line

Phoenix is no longer a bibliographic uncertainty: at least four distinct digital vol.III witnesses are located, and its no.26 August 1872 publication slot is secure. But its two decisive readings remain unread. The correct research object is therefore not merely a textual stemma but a **witness-state matrix** in which existence, location, access, material form and actual reading are separately controlled.