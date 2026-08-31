# Quick-win queue — 2026-08-31

Purpose: sources or checks that can be advanced with one or a few clicks and should be batched later rather than interrupting the main research run.

## Highest priority

- [ ] **Cambridge Hodgson inventory image-host recovery — paper census pilot.** The live `hodgson.socanth.cam.ac.uk` item pages still expose individual folio-image links, but the old thumbnail/media host `catalogue2.socanth.cam.ac.uk/eXistdata/media/thumbs/` currently returns a 502/DNS-style failure. Recover a migrated/static/archived media path before treating these images as unavailable. Start with BL pilot cases that already have explicit folio images: vol. 12 item 3 (`f.117`, 1843 Nepali-paper bill), item 15 (`f.147`, seven-box receipt), item 20, and item 25. Search exact image filenames in Wayback/new Cambridge hosts if necessary. Once recovered, use full recto/verso images for edge/fold/seal/support observation and request transmitted-light only where the ordinary image cannot answer formation/watermark questions.
  - live metadata page: https://hodgson.socanth.cam.ac.uk/chunkhtml/vol012.html
  - historical media prefix: `http://catalogue2.socanth.cam.ac.uk/eXistdata/media/thumbs/`

- [ ] **ZSL `NZSL/HOD/5/4/38` — list of boxes/crates of skins, horns, skulls and osteological specimens.** A 16.5 MiB digital PDF is exposed directly in the ZSL catalogue. Inspect for box numbers, crate structure, destinations, packing vocabulary and any preservation instructions.
  - https://zsl-archive.maxarchiveservices.co.uk/index.php/list-of-boxes-crates-etc-of-skins-horns-skulls-osteological-specimens-of-birds-and-mammals-sent-to-england?sf_culture=en

- [ ] **Saint-Hilaire, February 1863, RAS `BHH/19/3`.** Hodgson's retained printed copy is catalogued as annotated. Photograph/scan request or direct inspection would give the first half of the contemporary description of the Institut drawings/paintings.
  - https://www.royalasiaticarchives.org/index.php/informationobject/browse?page=7&showAdvanced=1&sort=identifier&sortDir=asc&subjects=643&topLod=0

- [ ] **Saint-Hilaire, March 1863, RAS `BHH/19/4`.** Second and final article; inspect alongside February issue for material vocabulary and Hodgson's annotations.
  - same RAS browse page as above.

- [ ] **Foucher catalogue, pp. 1–6.** Verify directly the `note found in the case` / 1866 chronology statement and the separation of explanatory manuscripts from paintings. Persée has the full article.
  - https://www.persee.fr/doc/mesav_0398-3587_1902_num_11_1_1080

- [ ] **JRAS `The Hodgson Drawings at Paris` note.** Save local copy / full citation. It gives the cleanest explicit diagnosis of Foucher's container-derived 1866 error.
  - https://www.cambridge.org/core/services/aop-cambridge-core/content/view/DE9E75AAC85D8EA69B2A44A7E84A71AB/S0035869X00146805a.pdf/iii_notes_and_news.pdf

## Direct-text confirmations

- [ ] **1857 Hodgson commerce passage.** Record exact printed page number, section heading and line context around the two-bazaar-maund load-unit passage. This is already a direct Hodgson source, but page-level citation should be fixed before article drafting.
  - https://pahar.in/pahar/Books%20and%20Articles/Nepal/1857%20Papers%20on%20Colonization%20Commerce%20Physical%20Geography%20%26c.%20%26c.%20to%20Himalaya%20Mountains%20and%20Nepal%20by%20Hodgson%20s.pdf

- [ ] **1831 manuscript / Government of Bengal publication genealogy.** Match the 1857 printed passage back to BL `Mss Eur Hodgson/6` and the Government of Bengal *Selections* publication so the article can distinguish original report, official print, 1857 compilation and 1874 reprint.
  - BL inventory lead: https://hodgson.socanth.cam.ac.uk/chunkhtml/vol006.html

- [ ] **1870 Marshall box, `NZSL/HOD/5/3/9`.** Download/retain the digital object and transcribe the exact memorandum layout. Important because `big deal box → four portfolios → 1,104 sheets + manuscript/printed apparatus` is one of the strongest nested-container cases.
  - https://zsl-archive.maxarchiveservices.co.uk/index.php/informationobject/browse?collection=12410&mediatypes=137&names=4543&places=61275&sf_culture=pt&showAdvanced=1&sort=referenceCode&sortDir=desc&topLod=0&view=table

## Medium-priority quick checks

- [ ] Search ZSL digital items adjacent to `NZSL/HOD/5/4/38` for `box`, `crate`, `case`, `package`, `label`, `ticket`, `preserve`, `dry`, `oil`, `spirit`, `arsenic`, `soap`, `insect`.
- [ ] Pull the 15 July 1837 Burnouf and 29 July 1837 Mohl receipt letters together as a paired `safe arrival` case.
- [ ] Check whether the 1858 Institut `roll` and `other box` are mentioned by dimensions or number in Foucher/Saint-Hilaire.
- [ ] Record whether Foucher's `liasses de dessins` still preserve Sanskrit notes physically attached to individual sheets or only associated at bundle level.
- [ ] Check whether current Institut/Bibliothèque inventories preserve any original Hodgson case numbers, bundle labels or wrapper inscriptions.

## Rule for future runs

Items on this page are deliberately low-friction. When the user asks to `run quick wins`, process them as a batch, commit each resolved item into the relevant research wave/census, and tick the checkbox here rather than interrupting a deeper research branch one item at a time.
