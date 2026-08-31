# Web research 2026-08-31 — Wave 26
## Hodgson object-level imported paper marks: Kathmandu, Darjeeling and the mixed paper ecology

Date: 2026-08-31

Status: direct object-level follow-up to Waves 23–25. Scope remains paper itself. This wave asks whether imported-paper plurality can be demonstrated on objects produced within Hodgson's own research system rather than inferred only from Calcutta stationery supply or neighbouring institutions.

## Executive result

Yes. Published catalogue records for Hodgson-associated drawings now supply direct object-level evidence that his visual research system used multiple imported paper stocks and watermark families.

The strongest evidence currently located is:

1. a Christie's catalogue of more than four hundred Darjeeling/Nepalese-school bird studies, some dated 1849 and linked to Hodgson's Darjeeling period, records papers watermarked `MOINIER'S PATENT 1848`, `JOYNSON 1848`, `I NEWEY DARNFORD 1847`, `BRITANNIA`, and `1840`;
2. another Christie's Hodgson lot of Nepalese temple, deity and figure sketches records at least one sheet watermarked `WHATMAN`;
3. the Royal Asiatic Society's Raj Man Singh architectural series, drawn in Kathmandu in 1844, repeatedly records papers whose watermarks date them to 1841;
4. one RAS drawing attributed to c.1844 is explicitly on paper whose watermark dates it to 1821.

This shifts the paper argument from contextual plurality to **documented mixed-stock use within Hodgson's own working archive**.

The strongest formulation is now:

`Hodgson paper ecology != Nepali paper vs Whatman paper`

but:

`locally made Himalayan paper + multiple imported maker/proprietary papers + watermark motifs/grades + dated stocks + long-lived residual stock`.

Mechanisms:

- `HODGSON_OBJECT_LEVEL_IMPORTED_PAPER_PLURALITY`
- `MIXED_PAPER_STOCK_WITHIN_RESEARCH_WORKFLOW`
- `WATERMARK_DATE_NOT_USE_DATE`
- `PAPER_STOCK_RETENTION_OR_REUSE`
- `WATERMARK_SEMANTIC_TYPE_MUST_BE_CODED`
- `MAKER_MARK_NOT_PRODUCTION_TECHNOLOGY_WITHOUT_FORMATION_CHECK`

---

# 1. Darjeeling bird studies give direct multi-mark evidence

Primary catalogue evidence:

Christie's, `Darjeeling and Nepalese School, circa 1850, A Collection of over four hundred Studies of Nepalese Birds`.

URL:
https://www.christies.com/lot/lot-191301

The lot description states that the drawings are variously inscribed in Nepalese characters and numbered by Hodgson. The catalogue introduction notes that some are dated **1849**, when Hodgson was in Darjeeling.

The paper marks are transcribed as:

- `MOINIER'S PATENT 1848` — 5 occurrences;
- `JOYNSON 1848` — 2 occurrences;
- `I NEWEY DARNFORD 1847` — 11 occurrences;
- `BRITANNIA` — 17 occurrences;
- `1840` — 1 occurrence.

The catalogue reports 210 items in the lot, so these marked sheets are a subset of a larger visual-paper corpus rather than a complete paper census.

### Secure conclusion

Within one Hodgson-associated Darjeeling natural-history drawing corpus, at least five distinct watermark transcription classes occur.

This is direct evidence that the research operation did not depend on a single imported paper brand or maker.

Mechanism:

`HODGSON_OBJECT_LEVEL_IMPORTED_PAPER_PLURALITY`.

---

# 2. The Darjeeling marks include different kinds of watermark information

The five Christie's transcription classes should not all be coded as equivalent maker identities.

### Maker/proprietary-name candidates

- `JOYNSON 1848`
- `MOINIER'S PATENT 1848`
- `I NEWEY DARNFORD 1847`

### Motif/grade or generic watermark class

- `BRITANNIA`

### Date-only transcription

- `1840`

This distinction is methodologically important.

A watermark record can encode:

- maker name;
- mill/place name;
- proprietary brand;
- patent claim;
- paper size/grade convention;
- political/heraldic motif;
- date;
- or a countermark paired with another mark on the opposite half of a sheet.

Therefore the database should never store all watermark strings under a single `maker` field.

Required schema:

`watermark_transcription`

`watermark_semantic_type`

`candidate_maker`

`candidate_mill`

`date_in_mark`

`motif_or_grade`

`countermark_relation`

`formation_state`

`maker_confidence`.

Mechanism:

`WATERMARK_SEMANTIC_TYPE_MUST_BE_CODED`.

---

# 3. `BRITANNIA` is especially dangerous as a maker attribution

A Britannia watermark is not a unique maker signature.

Paper-history reference material describes Britannia as a widespread watermark form associated with paper size/grade conventions and with both British and Continental production for British markets.

Useful references:

National Gallery of Australia, Watermark and Countermark Library, `The Pro Patria watermark`:
https://nga.gov.au/art-artists/conservation/paper/listings-watermark-and-countermark-library/

British papermaking reference summary:
https://www.researchgate.net/publication/382764797_Studies_on_the_History_of_Papermaking_in_Britain

Therefore the 17 Christie's entries catalogued simply as `BRITANNIA` are important evidence for paper class/motif plurality, but they cannot presently be assigned to a named mill.

Rule:

`BRITANNIA watermark != British maker identity`.

And, more strongly:

`BRITANNIA motif != secure national production origin`.

Object inspection must recover:

- accompanying countermark;
- crown/legend form;
- whole-sheet relation;
- laid/wove/machine formation;
- dimensions;
- date;
- additional initials or names.

---

# 4. Joynson introduces an early machine-watermark context

The `JOYNSON 1848` sheets are particularly important because William Joynson's St Mary Cray mill belonged to a mechanised British paper regime.

Local paper-industry histories and later paper-object research agree that:

- William Joynson took over the St Mary Cray paper mill in 1834;
- the mill became known for high-quality paper;
- Joynson received a patent in **1839** for watermarking paper made by machine;
- surviving papers from the mill carry Joynson name marks.

References:

Kent History & Archaeology, `The Papermakers of Snodland c.1740-1854`:
https://www.kentarchaeology.org.uk/papers/the-papermakers-of-snodland-c1740-1854

Portsmouth Museums / NatSCA discussion of a later `JOYNSON 1860` watermark and St Mary Cray attribution:
https://natsca.blog/2023/02/02/flora-explorer-opening-the-cabinets-at-portsmouth-museums/

Corroborating object record, Northumberland Archives, cream laid paper watermarked `Joynson 1848`:
https://calmview.northumberland.gov.uk/Record.aspx?id=SANT%2FBEQ%2F5%2F4%2F1%2F42&src=CalmView.Catalog

### What is secure

The Joynson mark connects Hodgson's Darjeeling drawing paper to a named British paper-manufacturing enterprise active in machine production and machine watermarking.

### What is not yet secure

The catalogue transcription alone does not establish whether each Hodgson `JOYNSON 1848` sheet was:

- machine-made or handmade;
- laid or wove;
- which grade;
- which exact mill batch;
- supplied through Company stationery channels, private purchase, Calcutta stationers, or another route.

Thus:

`Joynson industrial context -> strong machine-production candidate`

but not yet:

`JOYNSON mark -> proven machine-made sheet`.

Required next observation:

`formation structure + watermark morphology + sheet edge/whole-sheet evidence`.

Mechanism:

`MAKER_MARK_NOT_PRODUCTION_TECHNOLOGY_WITHOUT_FORMATION_CHECK`.

---

# 5. `I NEWEY DARNFORD` needs transcription control before maker coding

Christie's transcribes eleven sheets as:

`I NEWEY DARNFORD 1847`.

A separate State Library of New South Wales archival watermark census records related strings including:

- `I. Newey / Dartford / 1841`;
- `I Newey / Darnford / 1844`.

Record:
https://archival.sl.nsw.gov.au/Details/archive/110321259

The coexistence of `Dartford` and `Darnford` in catalogue transcriptions means the place/name string requires physical verification rather than silent normalization.

This is a useful source-control case in its own right.

Possible explanations include:

- genuine variant marks;
- catalogue transcription error;
- difficult watermark letterforms;
- incomplete reading from a folded/cut sheet.

For the repo, retain the Christie's string exactly as published and add a normalized candidate only after a watermark image or independent maker directory confirms it.

Mechanism:

`WATERMARK_TRANSCRIPTION_UNCERTAINTY`.

---

# 6. `MOINIER'S PATENT 1848` is a proprietary-mark problem, not yet a resolved maker problem

The `MOINIER'S PATENT 1848` watermark is independently attested on nineteenth-century drawing paper outside the Hodgson corpus.

State Library of New South Wales archival records describe sketches with watermark:

`Moinier's / Patent / 1848`.

Example:
https://archival.sl.nsw.gov.au/Details/archive/110318870

A related journal/notes record also contains `Moinier's 1849` and `Moinier's Patent 1848` paper:
https://archival.sl.nsw.gov.au/Details/archive/110320933

This confirms that the Christie's transcription is not unique to the auction catalogue and represents a circulating paper mark.

At present, however, the exact maker/mill behind the mark remains unresolved in this research pass.

Code it as:

`watermark_semantic_type = proprietary_or_patent_mark`

not:

`maker = Moinier` with high confidence.

---

# 7. Hodgson temple/deity sketches directly attest Whatman but do not restore Whatman dominance

Primary catalogue evidence:

Christie's, `Brian Houghton Hodgson (1800-1896), A Collection of over eighty Sketches of mainly Buddhist Temples, Statues, Shrines and Figure Studies of Natives of Nepal from various Tribes`.

URL:
https://www.christies.com/en/lot/lot-191304

The lot is described as pencil, pen and ink on 41 loose pages, with:

`watermark 'WHATMAN' (1)`.

This is direct Hodgson-object evidence for Whatman-marked paper.

But the evidential consequence is the opposite of a Whatman default assumption.

The same broader Hodgson paper archive now contains:

- Whatman;
- Joynson;
- Newey/Darnford-transcribed paper;
- Moinier's Patent;
- Britannia-marked paper;
- date-only paper stocks;
- Nepalese country paper.

Therefore Whatman is securely **present** while remaining only one component of a mixed paper ecology.

Mechanism:

`WHATMAN_PRESENT_BUT_NOT_DEFAULT`.

---

# 8. Royal Asiatic Society architectural drawings show dated imported stock in Kathmandu

The Royal Asiatic Society online collection identifies the Hodgson architectural drawing corpus as mainly a series of 50 views of Nepalese architecture drawn by **Raj Man Singh Chitrakar in Kathmandu in 1844**.

Collection:
https://royalasiaticcollections.org/collection/hodgson-drawings/

Many individual records state:

`Watermark dates the paper to 1841`.

Examples include:

- RAS Hodgson 022.003, `Chaityas at Svayambunath, Kathmandu`;
- RAS Hodgson 022.009, `View of Svayambunath`;
- RAS Hodgson 022.011, `The Mahadeva temple, Patan`;
- RAS Hodgson 022.021, `Temple of Balkumari (?)`;
- RAS Hodgson 022.029, `Temple of Narayan at Narayanhitti`;
- RAS Hodgson 022.038, `The stupa at Bodhnath`;
- RAS Hodgson 022.041, `View of Chief Court of Justice, and palace, Bhatgaon`;
- RAS Hodgson 022.042, `The Golden Palace at Bhatgaon`;
- RAS Hodgson 022.043, `A Khas' house`;
- RAS Hodgson 022.045, `A Magar house`;
- RAS Hodgson 022.047, `The Dattaraya temple`.

The paper dimensions cluster around approximately 30 × 48.5 cm in many of these records.

### Strong paper-history implication

Imported or watermark-dated paper was not merely used after Hodgson left Nepal. It was already functioning as routine support for commissioned visual knowledge production in Kathmandu by 1844.

Thus the relevant local material environment was already mixed:

`Nepalese handmade paper + imported drawing/writing stocks`.

This coexistence is more historically precise than treating Nepal paper as an isolated indigenous technology facing an external European substitute.

Mechanism:

`COEXISTING_LOCAL_AND_IMPORTED_SUPPORT_REGIMES`.

---

# 9. The 1821 watermark on a c.1844 drawing exposes paper-stock time

The most analytically useful RAS record is:

`Temple of Krishna and Radha, Patan`, RAS Hodgson 022.026.

Royal Asiatic Society / Global Nepali Museum record:
https://globalnepalimuseum.com/objects/temple-of-krishna-and-radha-patan/

The record states:

- drawing date: `c. 1844`;
- artist: Raj Man Singh Chitrakar;
- location: Kathmandu;
- paper watermark date: `1821`;
- paper size: 31.6 × 43.8 cm.

If the drawing attribution and watermark reading are both correct, the watermark date predates the assigned drawing date by roughly **23 years**.

This matters because watermark date cannot be used as use-date identity.

The sheet may represent:

- long-lived stationery stock;
- stored imported paper;
- reuse or recirculation;
- an earlier support incorporated into a later drawing campaign;
- or a cataloguing/dating issue requiring object reinspection.

The evidence does not yet choose among these possibilities.

But it securely requires a new variable:

`paper_stock_age_at_use`.

And a rule:

`watermark date = paper-production/mark chronology evidence, not document-use date`.

Mechanism:

`WATERMARK_DATE_NOT_USE_DATE`.

Possible larger mechanism:

`PAPER_STOCK_RETENTION_OR_REUSE`.

---

# 10. This changes the Calcutta argument

Wave 25 established that Calcutta official/scientific paper supply was heterogeneous and could include multiple makers in a single institutional object.

Wave 26 moves the claim one evidential level closer to Hodgson.

The sequence is now:

### Supply environment

`London/Europe + Presidency redistribution + Calcutta stationery/scientific markets -> multiple imported paper types`.

### Hodgson working objects

`Kathmandu architectural drawings -> watermark-dated imported stocks`

`Darjeeling bird drawings -> multiple named/proprietary/motif watermark families`

`other Hodgson sketches -> Whatman present`

### Local production

`Nepalese handmade paper -> manuscripts, drawings, administrative and commercial uses`.

Therefore Hodgson's paper regime is best modelled as a **mixed-stock operational ecology** rather than a substitution sequence.

The paper question becomes:

**which paper stock was selected for which operation, at which place, through which procurement route, and with what lag between manufacture, purchase, storage and use?**

---

# 11. New article-level claim: paper choice is an allocation problem

The earlier article argument emphasised production history:

`paper properties = process history embodied in sheet`.

The object-level evidence adds a second layer:

`paper use = stock availability × procurement route × retained inventory × operation-specific selection`.

A useful combined model is:

`research-paper affordance = production history × supply history × stock history × intended operation`.

This avoids two simplifications:

1. national-material binary (`Nepali` vs `European`);
2. maker-brand binary (`local paper` vs `Whatman`).

The archive instead contains paper from different production regimes, circulating through different supply routes and remaining in stock for different durations before being assigned to particular operations.

Mechanisms:

- `PAPER_ALLOCATION_AS_RESEARCH_INFRASTRUCTURE`
- `STOCK_HISTORY_MODULATES_MATERIAL_USE`
- `MIXED_STOCK_OPERATIONAL_ECOLOGY`.

---

# 12. Immediate object census protocol

The next physical/digital inspection should record, per sheet/object:

1. collection and accession number;
2. object type;
3. attributed use/creation date;
4. use location;
5. maker/mark transcription exactly as visible;
6. watermark semantic type;
7. date in mark;
8. countermark;
9. laid/wove/machine formation;
10. chain-line spacing if laid;
11. paper dimensions and whether trimmed;
12. whole-sheet/half-sheet relation where reconstructible;
13. colour/tone;
14. thickness/caliper;
15. surface finish/sizing;
16. medium used: pencil, ink, wash, watercolour, writing ink;
17. evidence for stock age or reuse;
18. candidate procurement route;
19. confidence level for maker and production technology.

High-priority object groups:

- RAS Hodgson 022 architectural drawings, especially 022.026 and repeated 1841-watermark sheets;
- Christie's 1997 Darjeeling bird drawings if current locations can be traced;
- Christie's temple/deity sketch lot with `WHATMAN`;
- surviving ZSL Hodgson drawing sheets;
- British Museum/British Library Hodgson drawing and manuscript groups;
- Mss Eur Hodgson/6 paper-manufacture material and sample;
- Mss Eur Hodgson/1 ff.216–223 imported thick/thin papers already flagged in the repo.

---

# 13. Source-control rules added by this wave

1. `watermark date != use date`.
2. `watermark motif != maker`.
3. `maker name in watermark != production technology` without formation inspection.
4. `Whatman present != Whatman dominant`.
5. `Christie's transcription != verified physical reading`; retain exact published string and mark confidence.
6. `Darnford/Dartford` must remain unresolved until image/object inspection.
7. paper counts from auction lots describe the surviving/marketed lot, not necessarily Hodgson's original complete working set.
8. a paper-production date earlier than drawing date supports stock-history investigation but does not by itself prove continuous storage by Hodgson.

---

## Bottom line

The paper article has moved beyond a contextual claim that Calcutta imported multiple kinds of paper. Hodgson's own surviving visual materials directly document mixed imported paper stocks. A Darjeeling bird corpus contains several distinct watermark families; another Hodgson sketch group includes Whatman; Raj Man Singh's Kathmandu architectural drawings repeatedly use watermark-dated 1841 sheets, while one c.1844 drawing sits on paper dated 1821. These objects make paper supply and stock history experimentally visible. The article can therefore treat Hodgson's research environment as a mixed paper ecology in which locally made Himalayan sheets and imported stocks from multiple production regimes coexisted, aged, circulated and were allocated to different operations. Paper is not only process-retentive at manufacture; it is also **history-retentive in stock and use**.