# Web research 2026-08-31 — Wave 29
## Christie's 10 June 1997 `Visions of India`: Hodgson lot mapping and source control

Date: 2026-08-31

Status: custody/provenance control follow-up to Waves 26–27. Scope remains paper objects and their later custody.

## Executive result

The public record now securely identifies two of the critical 1997 Hodgson natural-history lots and preserves one unresolved mapping rather than inferring it from webpage sequence.

### Secure

**Lot 170 — bird corpus**

Christie's current page for the collection of more than four hundred Nepalese bird studies is the corpus carrying the Wave 26 watermark classes:

- `MOINIER'S PATENT 1848` (5);
- `JOYNSON 1848` (2);
- `I NEWEY DARNFORD 1847` (11);
- `BRITANNIA` (17);
- `1840` (1).

Current Christie's page:
https://www.christies.com/en/lot/lot-191301

Independent searchable scholarship cites the Hodgson natural-history material at the 10 June 1997 `Visions of India` sale as lots 170–172, and the Christie's page places this corpus at the beginning of the Hodgson natural-history sequence. Treat the bird corpus as lot 170 in the working mapping, with a note that recovery of the printed catalogue remains the preferred primary control.

**Lot 172 — fish/reptile corpus**

Current Christie's page:
https://www.christies.com/en/lot/lot-191303

Title: collection of 14 watercolours of fish and reptiles.

More importantly, a later Christie's Linley Hall catalogue explicitly states that eight sheets of related reptile/fish studies were:

`Anonymous sale, Christie's, 10 June 1997, lot 172 (part)`

and were acquired there by Justin Coldwell.

2016 catalogue source:
https://electronicsandbooks.com/edt/manual/Art/Auction/Christies/2016/20160309%20CKS12451%20Linley%20Hall%2C%20Shropshire%20Property%20from%20The%20Collection%20of%20The%20Late%20Sir%20Jasper%20%26%20Lady%20More%20%5B7%5D.pdf

Thus `lot 172 = fish/reptile material` is secure.

### Still unresolved in this pass

**Lot 171**

Secondary scholarship associates lot 171 with a preliminary Hodgson natural-history drawing series and an old British Library/OIOC shelfmark, but the current BL catalogue state conflicts with that published identifier. Until the printed 1997 catalogue or BL accession/concordance record is inspected, keep lot 171 as `corpus mapping unresolved at primary-source level`.

Do not infer lot 171 solely because current Christie's object-page IDs appear sequential.

Mechanisms:

- `AUCTION_LOT_TO_CORPUS_MAPPING`
- `PRIMARY_LOT_CONTROL_OVER_WEBPAGE_SEQUENCE`
- `PARTIAL_LOT_CUSTODY_BRANCHING`
- `SHELFMARK_CATALOGUE_DRIFT`

---

## 1. Lot 170: the watermark-rich bird corpus

Christie's describes the bird material as more than four hundred studies, represented by 210 catalogued sheets/objects in the lot, variously inscribed in Nepali characters and numbered by Hodgson. Some drawings are dated 1849, Hodgson's Darjeeling period.

The support description is the core paper evidence:

`MOINIER'S PATENT 1848` (5)

`JOYNSON 1848` (2)

`I NEWEY DARNFORD 1847` (11)

`BRITANNIA` (17)

`1840` (1).

This lot is the principal object-level proof of imported-paper plurality in Hodgson's late natural-history visual production.

Source-control:

- counts are auction-catalogue counts;
- watermark strings are catalogue transcriptions, not transmitted-light verification;
- 210 is the lot count as catalogued and should not be silently equated with the phrase `over four hundred studies` without distinguishing studies from sheets/objects.

Mechanism:

`STUDY_COUNT_VS_SHEET_COUNT`.

---

## 2. Lot 172: fish/reptile corpus and later private branch

Christie's current page describes 14 watercolours of fish and reptiles, including named snakes and fish, executed in pencil, pen-and-ink and watercolour.

The 2016 Linley Hall catalogue later identifies eight sheets with ten snake studies, two eel studies and one lizard study as `lot 172 (part)` from the 1997 sale.

Therefore the 1997 lot was later subdivided or only part of it entered the documented Coldwell branch.

Custody sequence:

`Hodgson-associated corpus`
-> `Christie's 1997 lot 172`
-> `part acquired by Justin Coldwell / Linley Hall`
-> `Christie's 2016 lot 159`
-> `current public custody unresolved`.

Mechanism:

`PARTIAL_LOT_CUSTODY_BRANCHING`.

---

## 3. Lot 171 should remain a controlled gap

A previous repo wave recorded the conflict between a published old OIOC/BL shelfmark and the current British Library catalogue status.

This wave tightens the rule:

`neighbouring lot numbers + neighbouring Christie's web IDs != provenance proof`.

Required evidence for lot 171:

1. printed `Visions of India`, 10 June 1997 catalogue page;
2. Christie's sale archive with lot number/title;
3. BL accession record or old-to-new shelfmark concordance;
4. published source with enough object description to match sheets materially.

Until then:

`LOT171_CORPUS = unresolved_primary_mapping`.

---

## 4. Lot 173 / Buddhist sketch page should remain separate from the 170–172 natural-history citation

A current Christie's page preserves a Hodgson collection of over eighty Buddhist temples, statues, shrines and Nepal figure studies on 41 loose pages, including one `WHATMAN` watermark:

https://www.christies.com/en/lot/lot-191304

This corpus is already important to the paper article because it proves Whatman-mark presence in Hodgson-associated visual material.

However, the scholarship located in this pass explicitly cites Hodgson natural-history **lots 170–172**. The present page should not be assigned a specific 1997 lot number merely from numerical adjacency until the printed catalogue confirms it.

Rule:

`object-page sequence != auction-lot identity`.

---

## 5. Revised custody identifiers

For auction-origin material, store at least:

- sale house;
- sale title;
- sale date;
- lot number;
- current web object ID/URL;
- corpus description;
- sheet/study count distinction;
- later partial-lot events;
- current holder if known;
- confidence.

Do not use Christie's current `lot-19130x` web ID as though it were the historical lot number.

---

## Immediate targets

1. Obtain/inspect the printed 10 June 1997 `Visions of India` catalogue, pages covering lots 170–173.
2. Lock lot 171 title, dimensions, support/watermarks and buyer/provenance if printed.
3. Verify whether the Buddhist/figure-study corpus now at Christie's page `lot-191304` was historical lot 173.
4. Reconcile lot 171 against the BL/OIOC shelfmark conflict.
5. Trace the post-2016 location of the lot-172 Coldwell branch.

## Bottom line

The auction chain is now sufficiently controlled to separate fact from sequence inference. Lot 170 is the watermark-rich bird corpus used in the paper-plurality argument; lot 172 is the fish/reptile corpus, with a documented partial branch into Linley Hall and resale in 2016. Lot 171 remains an explicit primary-source mapping gap. This matters because the article's paper census depends on knowing which surviving sheets belong to which historical corpus before watermark, support and custody histories are recombined.