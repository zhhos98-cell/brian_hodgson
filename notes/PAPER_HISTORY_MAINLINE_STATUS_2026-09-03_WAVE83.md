# Hodgson paper-history mainline — 2026-09-03, through Wave 83

Status: **current active guardrail**. Supersedes the Wave 82 active guardrail. Wave 83 adds an exact London Board's Collection file for Campbell's 1842 Darjeeling paper experiment while preserving the distinction between consultation identity and later London documentary derivatives.

## Current strongest documentary graph

### Campbell / Darjeeling, spring 1842

`25 Mar 1842 — Hodgson: 24 packages Nepalese paper pulp toward Calcutta`

parallel but not yet materially linked to:

`16 Apr 1842 — Campbell's Darjeeling factory reported closed under existing economics`
-> `21 Apr 1842 — Campbell -> G. A. Bushby paper letter/report`
-> `11 May 1842 — Political Original Consultation No.70`
-> `IOR/P/196/12 = high-confidence London consultation-volume target`
-> `[transmission/copy relation pending]`
-> `IOR/F/4/2006/89528 = direct Board's Collection file containing Campbell's result report on making paper from paper-tree bark`.

The last file is direct British Library catalogue evidence. The arrows from No.70 to `F/4/2006/89528` remain unproven until document-level cross-reference.

Encode:

`CAMPBELL_1842_PAPER_EXPERIMENT_HAS_AT_LEAST_THREE_DOCUMENTARY_STATES = SECURE`

where the three controlled states are:

1. underlying Campbell correspondence/report;
2. Political consultation processing;
3. London Board's Collection preservation.

Do not encode:

`OC_NO70 = F4_89528`

or

`F4_89528_CONTAINS_21_APR_LETTER`

until images/table of contents prove it.

---

## 1. Political O.C. semantics retained

For Abdul Ali's pre-Mutiny citations:

`Political O.C. = Political Original Consultation`.

Consultation date and underlying-letter date remain separate fields.

Calibration:

`8 Dec 1831 Hodgson letter`
-> `Political Consultation 13 Jan 1832, Nos.18–20`.

Target A:

`Political Consultation 29 Nov 1841, No.147`
=
O'Shaughnessy's report on the method of bleaching paper manufactured at Darjeeling, directly attested in the 1937 Imperial Record Department exhibition list.

Target B:

`21 Apr 1842 Campbell -> Bushby`
-> `Political Consultation 11 May 1842, No.70`.

Consultation numbers are date-local/sitting-local; adjacent numbers remain mandatory retrieval units.

---

## 2. Abdul Ali provenance retained

A. F. M. Abdul Ali was directly documented by National Archives of India as Keeper of Records / head of the Imperial Record Department and guided the 1925 pre-Mutiny records handbook. His 1937 Indian Historical Records Commission exhibition list directly names the Nepal-paper consultation clusters later used in his 1944 article.

Treat:

`ABDUL_ALI_ARCHIVAL_ADDRESS = HIGH_VALUE_REPOSITORY_NATIVE_FINDING_AID_TRACE`.

Still distinguish:

`archival address reliability`
from
`historical interpretation`.

---

## 3. 1832 calibration transaction is Nos.18–20, not No.19 alone

1937 exhibition control upgrades the paper-manufacture transaction to:

`Pol. Con. 13 Jan 1832, Nos.18–20`.

Abdul Ali's 1944 article cites No.19 for Hodgson's 8 Dec 1831 letter.

Thus:

`ONE_PAPER_TRANSACTION_CAN_SPAN_ADJACENT_CONSULTATION_NUMBERS = DIRECTLY_ATTESTED`.

Use this rule for No.147 and No.70 searches.

---

## 4. 1841 target remains exact at consultation level, London IOR/P volume unresolved

`29 Nov 1841 No.147`

Subject:

O'Shaughnessy report on bleaching paper manufactured at Darjeeling.

1937 IRD exhibition confirms the object remained separately identifiable.

Exact `IOR/P` volume remains unresolved.

Known boundary:

`IOR/P/196/4 = 13–30 Dec 1841`.

Do not infer `/2` or `/3` from sequence alone.

New Wave-83 search route:

search Board's Collections (`IOR/F/4`) by the exact report identity in parallel with the `IOR/P` volume search, because O'Shaughnessy's contemporary chemical/manufacturing reports demonstrably acquired F/4 documentary lives.

Do not confuse unrelated `IOR/F/4/1949/84712` with No.147; that file concerns manufacture of medicines.

---

## 5. 1842 consultation target remains `IOR/P/196/12` at high confidence

Independent documentary scholarship places 11 May 1842 India Political Consultation material in:

`IOR/P/196/12`.

Therefore:

`11_MAY_1842_NO70 -> IOR/P/196/12 = HIGH_CONFIDENCE_VOLUME_TARGET`.

Still pending:

- exact No.70 page/item image;
- adjacent-number transaction boundaries;
- Campbell 21 Apr letter image;
- internal order/minute/draft reply.

---

## 6. New direct London file: `IOR/F/4/2006/89528`

British Library catalogue directly states that this Board's Collection file contains:

`report by Dr Campbell of the result of his experiment in making paper from the bark of the paper tree`.

Date range:

`Mar 1842-Nov 1842`.

The file also contains other Darjeeling station proceedings concerning boundary marks, Birch Hill road and public works.

Encode:

`F4_2006_89528_CONTAINS_CAMPBELL_PAPER_EXPERIMENT_REPORT = DIRECT`

`F4_2006_89528 = SAME_PROGRAMME_LONDON_DERIVATIVE = HIGH_CONFIDENCE`

`F4_2006_89528 = OC_NO70 = UNPROVEN`.

Important retrieval implication:

Known subject-specific F/4 file now outranks generic `L/PS/6` searching for the Campbell experiment.

---

## 7. Board's Collections are no longer merely a fallback

Revised documentary retrieval order for Campbell 1842:

1. `Political Original Consultation 11 May 1842 No.70 ± adjacent numbers`;
2. `IOR/P/196/12` consultation witness;
3. `IOR/F/4/2006/89528` Campbell/Darjeeling Board's Collection file;
4. transmission index `IOR/Z/E/4/16`;
5. corresponding `IOR/E/4` India/Bengal despatch/letter;
6. `IOR/L/PS/6` only where a Political Letter transmission identity is established.

This is a document-identity workflow, not a repository-prestige workflow.

---

## 8. `IOR/Z/E/4/16` is the next transmission crosswalk

British Library:

`IOR/Z/E/4/16 — Index to India and Bengal Despatches, 1839–1842`.

This exact chronological index may identify the India/Bengal despatch under which Campbell's Darjeeling proceedings entered London correspondence.

Current state:

`CAMPBELL/DARJEELING/PAPER INDEX ENTRY = UNRECOVERED`.

Search spellings/heads:

- Campbell;
- Darjeeling / Darjiling;
- Paper;
- Paper tree;
- Manufactures;
- Experiments;
- Political / station locality headings.

Do not invent the transmission despatch number.

---

## 9. Material chain remains distinct from documentary convergence

Direct material anchor:

`25 Mar 1842 Hodgson -> 24 packages Nepalese paper pulp -> Champaran / Woodcock -> Patna by land OR Govind Gang by water -> Calcutta`.

Still missing:

- Halliday initiating directive;
- Woodcock route choice / carriage bill;
- intermediate receipt;
- Calcutta receipt;
- final experimental destination.

Wave 83's Campbell F/4 report increases documentary density around spring 1842 but does not identify the 24 packages as Campbell's feedstock.

Keep:

`HODGSON_24_PACKAGES -> CAMPBELL_FACTORY = UNPROVEN`.

---

## 10. 1837 sample/procurement line retained

Direct learned-society evidence:

- request for a small supply of each size and quality of Nepal paper for experimental purposes;
- Campbell promises supply;
- Campbell proposes samples to Chamber of Commerce;
- official correspondence copied into learned-society dossier/publication.

Keep:

`CHAMBER_FORWARDING = PROPOSED_DIRECT`

`CHAMBER_RECEIPT_OR_TEST = UNPROVEN`.

Finished-paper freight in 1837 remains distinct from the 1842 pulp-package freight.

---

## 11. Current multi-state paper-history proposition

The same broad material programme now has recoverable documentary states across:

`original technical/material event`
-> `incoming letter/report`
-> `Political Original Consultation packet`
-> `Political Proceedings / IOR/P consultation witness`
-> `Board's Collection F/4 subject file`
-> `India/Bengal despatch index / E/4 correspondence`
-> `other London departmental copies/enclosures`
-> `private copy / learned-society publication`
-> `later archivist extraction`.

These witnesses can preserve different information resolutions and dates.

---

## Immediate research order

1. Inspect/request `IOR/F/4/2006/89528`; extract table of contents, internal document dates, Campbell addressee(s), orders, enclosures and transmission references.
2. Test for Campbell -> G. A. Bushby, 21 Apr 1842.
3. Test for Political Consultation 11 May 1842 No.70 and adjacent numbers.
4. Recover No.70 in `IOR/P/196/12` at item/page level.
5. Search `IOR/Z/E/4/16` to recover the corresponding India/Bengal despatch reference.
6. Crosswalk the despatch to `IOR/E/4` and any relevant Political-letter derivative.
7. Search F/4 for the exact O'Shaughnessy 29 Nov 1841 Darjeeling bleaching report.
8. Continue exact `IOR/P` volume search for 29 Nov 1841 No.147.
9. Continue EAP880 Darjeeling/Sikkim consultation surrogate route when images are accessible.
10. Continue Halliday/Woodcock/Champaran material-logistics search independently.

---

## Guardrails

1. `Political O.C. = Political Original Consultation`.
2. Consultation date != underlying-letter date.
3. Adjacent consultation numbers can form one transaction.
4. 1832 paper transaction = Nos.18–20.
5. 1841 No.147 = O'Shaughnessy Darjeeling bleaching report; exact IOR/P volume unresolved.
6. 1842 No.70 -> `IOR/P/196/12` is high-confidence volume targeting, not page-level recovery.
7. `IOR/F/4/2006/89528` directly contains Campbell's paper-experiment result report.
8. `F4/89528 = No.70` remains unproven.
9. `F4/89528 contains 21 Apr letter` remains unproven.
10. Co-location with roads/public works does not prove shared budget or departmental classification.
11. `IOR/Z/E/4/16` is a finding-aid route; no despatch number is yet controlled.
12. `L/PS/6` remains a later transmission route, not the first consultation witness.
13. 25 Mar Hodgson pulp consignment remains materially unlinked to Campbell experiment.
14. Finished paper, pulp, classified sample, experimental feedstock and archival support remain distinct states.
15. 1831–42 remains recurrent programme continuity, not proven uninterrupted formal programme.

## Current strongest proposition

**Campbell's 1842 Darjeeling paper experiment can now be pursued across at least three discrete documentary states. Abdul Ali identifies an underlying 21 April letter to G. A. Bushby and its processing as Political Original Consultation No.70 on 11 May; independent evidence places that consultation date in `IOR/P/196/12`; and the British Library catalogue identifies a separate London Board's Collection file, `IOR/F/4/2006/89528`, containing Campbell's report on the result of making paper from the bark of the paper tree. These records are almost certainly documentary kin, but their exact derivational relation still requires inspection of dates, addressees, enclosures and transmission references. The immediate problem has therefore shifted from proving that Campbell's experiment reached London to reconstructing how one experiment was transformed from an India-side report and consultation into a Board's Collection file.**