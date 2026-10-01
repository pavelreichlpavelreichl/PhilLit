# Literature Review Outline: Kant Scholarship 2010-2026, Year by Year

**Research Project**: A chronological, year-by-year review of selected significant Kant scholarship (books, edited volumes, editions/translations, journal articles), 2010 through 2026-09-30
**Date**: 2026-10-01
**Total Literature Base**: 251 verified entries across 6 domain files (literature-domain-1.bib to -6.bib; 43 / 45 / 45 / 45 / 45 / 28 entries), listed in `intermediate_files/entries_digest.tsv`
**Format**: Introduction, 17 year sections, Conclusion. Organised BY YEAR, not thematically. Every year section lists ALL digest entries of that year (no omissions, no additions). Every entry is one bullet with a 1-3 sentence summary.

---

## 0. Entry counts by year (verified against the digest)

Verification method: the digest has 251 data rows (file lines 2-252); rows were counted per year and per domain; the sums below equal 251 and the per-year numbers equal the numbers in the task brief and in the domain @comment headers (D2-D6 report the same per-year counts; the D1 file has no @comment header, see Notes).

| Year | N | Domain file | Year | N | Domain file |
|---|---|---|---|---|---|
| 2010 | 13 | 1 | 2019 | 15 | 4 |
| 2011 | 15 | 1 | 2020 | 15 | 4 |
| 2012 | 15 | 1 | 2021 | 15 | 4 |
| 2013 | 15 | 2 | 2022 | 15 | 5 |
| 2014 | 15 | 2 | 2023 | 15 | 5 |
| 2015 | 15 | 2 | 2024 | 15 | 5 |
| 2016 | 14 | 3 | 2025 | 15 | 6 |
| 2017 | 16 | 3 | 2026 | 13 | 6 |
| 2018 | 15 | 3 | **Total** | **251** | |

Block sums: 2010-12 = 43; 2013-15 = 45; 2016-18 = 45; 2019-21 = 45; 2022-24 = 45; 2025-26 = 28; total 251.
Entries flagged INCOMPLETE in the digest: 26 (2010: 1; 2011: 2; 2012: 2; 2013: 1; 2014: 4; 2015: 5; 2018: 1; 2019: 4; 2020: 1; 2021: 1; 2023: 1; 2025: 2; 2026: 1). They are marked `INC` in the key tables of Part C.

---

## Part A. Writer allocation (writers run SEQUENTIALLY; the Conclusion writer runs LAST)

| Order | Output file | Exact heading(s) to write | Years | Entries | .bib file(s) to read |
|---|---|---|---|---|---|
| 1 | synthesis-section-1.md | `## Introduction` | none | 0 | headers (first ~55 lines) of literature-domain-2..6.bib; digest |
| 2 | synthesis-section-2.md | `## 2010`, `## 2011`, `## 2012` | 2010-2012 | 43 | literature-domain-1.bib |
| 3 | synthesis-section-3.md | `## 2013`, `## 2014`, `## 2015` | 2013-2015 | 45 | literature-domain-2.bib |
| 4 | synthesis-section-4.md | `## 2016`, `## 2017`, `## 2018` | 2016-2018 | 45 | literature-domain-3.bib |
| 5 | synthesis-section-5.md | `## 2019`, `## 2020`, `## 2021` | 2019-2021 | 45 | literature-domain-4.bib |
| 6 | synthesis-section-6.md | `## 2022`, `## 2023`, `## 2024` | 2022-2024 | 45 | literature-domain-5.bib |
| 7 | synthesis-section-7.md | `## 2025`, `## 2026` | 2025-2026 | 28 | literature-domain-6.bib |
| 8 | synthesis-section-8.md | `## Conclusion` | all | 0 (cites digest works only) | digest; synthesis-section-2..7.md (read to stay consistent) |

All paths are under `reviews/kant-2010-2026/`. The orchestrator passes: working directory, the exact heading text(s), this outline path, the .bib file(s), and the output filename. Headings are reproduced verbatim; no `###` subheadings inside year sections.

---

## Part B. Writing rules (apply to writers 2-7; the Introduction and Conclusion writers follow rules 1, 2, 3 (as to quotation), 10, 11 and 12)

These rules OVERRIDE the generic synthesis-writer defaults where they conflict (the project is a bullet list, not an analytic essay).

1. **Source discipline.** Use ONLY information in the entry's `SUMMARY`, `SUBFIELD AND DEBATE`, `SIGNIFICANCE INDICATORS` and `YEAR NOTE` note text (and the keywords tags). The `abstract` field may be used only to check wording. No outside knowledge: no biography, no facts about contents, reception or impact that the notes do not state.
2. **No evaluation.** No evaluative adjectives or superlatives: no "seminal", "landmark", "groundbreaking", "important", "influential", "major", "leading", "pioneering", "classic", "definitive", "most", "best", "first of its kind". Strip such words, and publisher self-praise ("new and complete reading", "first English-language book"), when copying from SUMMARY. A fact such as an award, review or citation count may be reported only if the SIGNIFICANCE note states it (see the award list below), in neutral wording ("won the North American Kant Society Book Prize 2015, per the prize-winners page").
3. **Length.** Summary at most 3 sentences, descriptive verbs (argues, reads, examines, collects, translates, reconstructs). Paraphrase; no direct quotations. Whole bullet (citation, title, summary, optional cross-reference, optional flag) about 35-90 words.
4. **Bullet form (exact).** One bullet per entry, in the ORDER given in the key tables:
   `- Author (Year), *Title as in the digest*. Summary sentence(s). [optional cross-reference] [optional flag]`
   - The citation string is the "Cite as" column, exactly as given (surnames as in the digest, with diacritics: "de Boer", "van Mazijk", "Lu-Adler", "O'Neill", "Møller", "Abacı", "Förster"). The bibliography script (generate_bibliography.py) matches entries by FIRST author or editor surname within 60 characters of the year, so surname and year must stand together in the bullet.
   - Editors: `Surname (ed.) (Year)` / `Surname and Surname (eds.) (Year)`; three or more names: `Surname et al. (Year)` or `Surname et al. (eds.) (Year)` (conventions.md).
   - Title: copied from the digest, in italics; clean typesetting artefacts (``` ``X'' ``` and `` `X' `` become "X"; for example kleingeld2026strikingsimilarity is *The "Striking Similarity" Between Kant's Prolegomena and the Groundwork* and rosefeldt2024initself is *"In Itself": A New Investigation of Kant's Adverbial Wording of Transcendental Idealism*; the title is copied as it stands, while the summary itself must not call a work "new").
   - Same author and year need letters: Kant (2012a) = *Lectures on Anthropology*, Kant (2012b) = *Natural Science*; Merritt (2018a) = *Kant on Reflection and Virtue*, Merritt (2018b) = *The Sublime*; Guyer (2024a) = *Kant's Impact on Moral Philosophy*, Guyer (2024b) = *The Moral Foundation of Right*. (Letters follow Chicago title order. The bibliography script does not add letters; the orchestrator should check this at Phase 6.)
5. **Year overview.** Each `## YEAR` heading is followed by a one- or two-sentence overview (25-60 words) naming that year's most visible threads, taken ONLY from the "Threads" line in Part C for that year (derived from tags and notes). It may cite 2-4 entries of that year as `Author (Year)`. No claims of "turn", "consolidation", "shift" or ranking beyond what the Threads line states.
6. **Order.** Follow the key table order exactly. The order is by subfield: theoretical (CPR, mind, science/math/logic), practical (ethics, Metaphysics of Morals/virtue), political/legal, aesthetics/teleology, religion/anthropology/race/gender/animals, pre-critical/Opus postumum, reception, editions/reference. No subheadings and no visible group labels.
7. **Cross-references.** Add a cross-reference ONLY where the "Continues" line in Part C lists one. Form: a short parenthetical at the end of the bullet, e.g. `(Continues the nonconceptualism debate of 2011: Hanna (2011), McLear (2011).)`. Cite only the digest entries listed. Do not add other cross-references. Names that a note mentions but that are not digest entries (e.g. Mills, Strawson) may appear as surnames WITHOUT a year, only as the note states them.
8. **Entry types.** Say so when an entry is an edition or translation (flag `ED`: "an edition/translation of ..."; give an original date only if the YEAR NOTE states it); for edited volumes and reference works use the note's own label (Critical Guide, Companion, congress proceedings, lexicon, Handbook, Cambridge Element) when it is stated. The `(ed.)` marks in the digest are authoritative; for `baiasu2023kantianmind` and `basile2022opus` the digest shows no `(ed.)` although both are tagged edited volumes: check whether the .bib has `editor =` and use `(eds.)` only if it does.
9. **INCOMPLETE entries are INCLUDED** (project decision, Phase 4; this overrides the generic rule that skips INCOMPLETE entries). Source flags in the key tables: `PUB` = summary rests on a publisher description; `NDPR` = on an NDPR review; `REV` = on review text; `SNIP` = on a PhilPapers or publisher-page snippet. For flagged entries end the bullet with a short parenthetical, e.g. `(Summary based on the NDPR review.)`. Entries marked `INC` without such a flag have a summary based on an abstract retrieved from a journal or archive page; no flag needed. For 2010-2012 (D1 has no summary-source tags), also add the parenthetical when the SUMMARY note itself says it rests on a publisher description, NDPR or snippet instead of an abstract. Entries marked `DATE` get the parenthetical `(Dated by its CrossRef print or online date; see YEAR NOTE.)` when the YEAR NOTE shows a differing conventional or online date (denis2014ethics, ginsborg2014normativity, maliks2014politics, palmquist2015religion, thorndike2017, baiasu2023kantianmind, kinzel2024neokantian, luadler2026colonialslavery).
10. **Citations.** Chicago author-date, in-text only. Do NOT write a References section (generated later by script from literature-all.bib), no word-count line, no notes to the orchestrator inside the file. Cite only digest works.
11. **Accuracy first.** If a note is silent on something, leave it out. If a summary cannot be written from the notes without adding facts, write the shorter summary the notes support and report the problem to the orchestrator. Do not discover or add works. Every key of the writer's years must appear exactly once.
12. **How to read the .bib (efficient).** Do not read whole files. For each year use Grep with pattern `^@[a-z]+\{(key1|key2|...),` on the relevant .bib, `output_mode: content`, `-A 14`; the `note` field holds SUMMARY, SUBFIELD AND DEBATE, SIGNIFICANCE INDICATORS and YEAR NOTE on one line, and `keywords` shows INCOMPLETE and summary-source tags.

**Awards stated in SIGNIFICANCE notes (may be mentioned neutrally, once):** kleingeld2011cosmopolitanism (North American Kant Society Book Prize, listed for 2014 on the prize-winners page); wuerth2014mind (NAKS Book Prize 2015); allais2015manifest (NAKS Book Prize 2016, per web search); mcnulty2015regulative (NAKS Markus Herz Student Essay Prize 2014); guyer2026selectedessays (publisher abstract states the author won the 2024 International Kant Prize).

---

## Introduction (writer 1; heading `## Introduction`; 250-350 words)

**Purpose**: Tell the reader what the list is, how entries were chosen, how to read it, and where it is thin.

**Content, in this order (each point only from the facts given here):**
1. Scope: selected scholarship on Kant published 2010 through 2026 (2026 through 30 September): books, edited volumes, editions/translations and journal articles, mainly English-language with a few German-language reference works, proceedings and editions. Organised by year; each entry has a short summary.
2. Selection rule ("most significant works, verified through API searches"): an entry had to be verified in tool output (Semantic Scholar, CrossRef, PhilPapers via Brave search, CORE, NDPR, SEP/IEP; arXiv where relevant), be centred on Kant (or, for reception works, have Kant as one of the principal interlocutors), carry a publication year within the block (the API year, CrossRef print year preferred), not duplicate another entry, and meet at least one recorded significance indicator.
3. Significance judged by non-evaluative indicators recorded as data: citation counts relative to year and subfield (retrieved 2026-09-30/10-01), publisher or series and venue, NDPR and journal reviews, prizes (only where a source page confirms), mention in SEP/IEP Kant entries, status as a new edition/translation, and documented role in a debate.
4. Selective, not exhaustive: roughly ten to fifteen entries per year; many other works were screened out on indicators or on the per-year cap.
5. Total: 251 entries; year counts: 2010: 13; 2011: 15; 2012: 15; 2013: 15; 2014: 15; 2015: 15; 2016: 14; 2017: 16; 2018: 15; 2019: 15; 2020: 15; 2021: 15; 2022: 15; 2023: 15; 2024: 15; 2025: 15; 2026: 13 (to 30 September).
6. How to read a year section: a short overview, then entries ordered by subfield; "continues the debate of" notes link entries only where the annotations support it.
7. Honest limits: (a) 26 entries lack a retrievable abstract (mostly books), so their summaries rest on NDPR reviews, publisher or journal pages or snippets, flagged where it matters; (b) citation lag for 2024-2026: S2 and CrossRef counts for most 2025-2026 entries are between 0 and 6 (D6 header), so significance there rests on publisher, venue, reviews and author record, and no NDPR reviews dated 2026 were found in the NDPR sitemap; (c) OpenAlex returned 503 during the search and was not used for discovery (some abstracts nonetheless came from the abstract resolver's OpenAlex-backed records); (d) thin or empty subfields recorded in the domain headers' NOTABLE_GAPS: education and pedagogy (no entry), disability (no entry), animals (three entries: McLear 2011, Korsgaard 2018, Callanan and Allais (eds.) 2020), the Opus postumum (eight entries, none in 2010-2013, 2015, 2018, 2020, 2021, 2026), editions/translations (13 entries; none in 2010, 2014, 2020, 2021, 2023 or 2026; no new Cambridge Edition volume was found for 2022-2024); (e) dates follow the CrossRef print date, so a few works appear a year earlier than conventional citation (e.g. Denis and Sensen (eds.) 2014).

**Key papers**: none required. If any are named, use "Author (Year)" and digest entries only.
**Word target**: 250-350 words, one to three paragraphs, no bullets except an optional compact year-count line.

---

## Part C. Year sections

Legend for the key tables: `key | Cite as | flags`. Group letters: T theoretical, P practical, L political/legal, A aesthetics/teleology, R religion/anthropology/race/gender/animals, X pre-critical/Opus postumum, C reception, E editions/reference (orientation only; do not print them). Flags: `ED` edition/translation; `REF` reference work/proceedings; `INC` INCOMPLETE; `PUB`, `NDPR`, `REV`, `SNIP` summary source (Part B rule 9); `DATE`; `AWARD` (Part B list).

### Year 2010 (13 entries; writer 2; domain 1)
**Threads**: commentary on the Critique of Pure Reason and arguments for transcendental idealism (Guyer (ed.) 2010, Proops 2010, Allais 2010); Metaphysics of Morals, virtue and Right (Baxley 2010, Denis (ed.) 2010, Byrd and Hruschka 2010); a Critical Guide on the second Critique (Reath and Timmermann (eds.) 2010).
**Continues**: none (first year).
1. guyer2010companion | Guyer (ed.) (2010) | T
2. proops2010paralogism | Proops (2010) | T
3. allais2010transcendental | Allais (2010) | T
4. sturm2010consciousness | Sturm and Wunderlich (2010) | T
5. baxley2010virtue | Baxley (2010) | P
6. reath2010practical | Reath and Timmermann (eds.) (2010) | P
7. denis2010metaphysics | Denis (ed.) (2010) | P
8. pallikkathayil2010deriving | Pallikkathayil (2010) | P
9. byrd2010doctrine | Byrd and Hruschka (2010) | L
10. flikschuh2010sovereignty | Flikschuh (2010) | L; INC; SNIP (Wiley page snippet)
11. crowther2010kantian | Crowther (2010) | A
12. papadaki2010marriage | Papadaki (2010) | R (gender)
13. heis2010cassirer | Heis (2010) | C

### Year 2011 (15 entries; writer 2; domain 1)
**Threads**: nonconceptual content and animal consciousness (Hanna 2011, McLear 2011); Groundwork commentary, dignity and a German-English edition (Allison 2011, Sensen 2011, Kant 2011); Kant, race, geography and cosmopolitanism (Kleingeld 2011, Louden 2011, Elden and Mendieta (eds.) 2011); constructivism against realism (Stern 2011).
**Continues**: none required (the earliest entries on these debates in the digest).
1. kitcher2011thinker | Kitcher (2011) | T
2. hanna2011nonconceptual | Hanna (2011) | T
3. mclear2011animal | McLear (2011) | T
4. schulting2011idealism | Schulting and Verburgt (eds.) (2011) | T; INC; PUB
5. allison2011groundwork | Allison (2011) | P
6. sensen2011dignity | Sensen (2011) | P
7. stern2011obligation | Stern (2011) | P
8. kleingeld2011cosmopolitanism | Kleingeld (2011) | L; AWARD
9. ginsborg2011normativity | Ginsborg (2011) | A
10. dicenso2011religion | DiCenso (2011) | R
11. louden2011human | Louden (2011) | R
12. eldenmendieta2011geography | Elden and Mendieta (eds.) (2011) | R; INC; PUB
13. massimi2011dynamical | Massimi (2011) | X
14. rockmore2011phenomenology | Rockmore (2011) | C
15. kant2011groundwork | Kant (2011) | E; ED

### Year 2012 (15 entries; writer 2; domain 1)
**Threads**: conceptualist and two-aspect readings (Griffith 2012, Allison 2012); the Cambridge Edition volumes *Natural Science* and *Lectures on Anthropology* (Kant 2012a, 2012b); reception in German idealism and early analytic philosophy (Förster 2012, Sedgwick 2012, Parsons 2012); political and moral essays (Ellis (ed.) 2012, Hill 2012, Sensen (ed.) 2012).
**Continues**: griffith2012categories continues the conceptualism/nonconceptualism debate of 2011 (Hanna (2011), McLear (2011)); allison2012essays continues the two-aspect line of 2011 (Schulting and Verburgt (eds.) (2011)); gray2012race continues the Kant-and-race discussion of 2011 (Kleingeld (2011), Louden (2011), Elden and Mendieta (eds.) (2011)).
1. ameriks2012elliptical | Ameriks (2012) | T
2. allison2012essays | Allison (2012) | T
3. chignell2012spinoza | Chignell (2012) | T
4. griffith2012categories | Griffith (2012) | T
5. friedman2012geometry | Friedman (2012) | T; INC; SNIP (PhilPapers snippet)
6. hill2012virtue | Hill (2012) | P
7. sensen2012autonomy | Sensen (ed.) (2012) | P
8. ellis2012political | Ellis (ed.) (2012) | L; INC; NDPR
9. teufel2012judgement | Teufel (2012) | A
10. gray2012race | Gray (2012) | R
11. parsons2012husserl | Parsons (2012) | C
12. forster2012twentyfive | Förster (2012) | C
13. sedgwick2012hegel | Sedgwick (2012) | C
14. kant2012anthropology | Kant (2012a) | E; ED
15. kant2012natural | Kant (2012b) | E; ED

### Year 2013 (15 entries; writer 3; domain 2)
**Threads**: one-world (two-aspect) against two-world readings and nonconceptualism in journal articles (Marshall 2013, Tolley 2013); the empirical and scientific side of Kant (Friedman 2013, Frierson 2013, Mensch 2013); source texts on race (Mikkelsen (ed.) 2013); the Doctrine of Virtue commentary (Trampota et al. (eds.) 2013); Kant-Kongress proceedings (Bacin et al. (eds.) 2013).
**Continues**: marshall2013quaobjects continues the two-aspect line (Schulting and Verburgt (eds.) (2011), Allison (2012)); tolley2013nonconceptuality continues the conceptualism debate (Hanna (2011), McLear (2011), Griffith (2012)); mikkelsen2013race continues the Kant-and-race discussion (Kleingeld (2011), Elden and Mendieta (eds.) (2011), Gray (2012)); hay2013feminism continues the gender discussion (Papadaki (2010)); frierson2013human relates to Louden (2011) and Kant (2012a) (anthropology and human nature); trampota2013tugendlehre relates to Baxley (2010) and Denis (ed.) (2010) (Doctrine of Virtue).
1. marshall2013quaobjects | Marshall (2013) | T
2. tolley2013nonconceptuality | Tolley (2013) | T
3. friedman2013construction | Friedman (2013) | T
4. grenberg2013common | Grenberg (2013) | P
5. wuerth2013sense | Wuerth (2013) | P
6. trampota2013tugendlehre | Trampota et al. (eds.) (2013) | P
7. hay2013feminism | Hay (2013) | L (gender)
8. mensch2013organicism | Mensch (2013) | A; INC; PUB
9. matherne2013aesthetic | Matherne (2013) | A
10. insole2013creation | Insole (2013) | R
11. frierson2013human | Frierson (2013) | R
12. mikkelsen2013race | Mikkelsen (ed.) (2013) | R; ED
13. watkins2013newtonianism | Watkins (2013) | X
14. golob2013heidegger | Golob (2013) | C
15. bacin2013kongress | Bacin et al. (eds.) (2013) | E; REF

### Year 2014 (15 entries; writer 3; domain 2)
**Threads**: anthropology and empirical psychology (Frierson 2014, Cohen (ed.) 2014); the life sciences (Goy and Watkins (eds.) 2014); Kant and colonialism and the race debate (Flikschuh and Ypi (eds.) 2014, Mills 2014); one-object against two-object readings and naive-realist perception (Stang 2014, Gomes 2014); moral realism against constructivist readings (Wuerth 2014); the Opus postumum (Hall 2014) and a genealogy of neo-Kantianism (Beiser 2014).
**Continues**: stang2014nonidentity continues the two-aspect line (Marshall (2013), Allison (2012)); gomes2014naive continues the conceptualism debate (Tolley (2013), Griffith (2012), McLear (2011)); dyck2014rational returns to the Paralogisms (Proops (2010)); frierson2014empirical follows Frierson (2013); wuerth2014mind continues the constructivism-realism debate (Stern (2011)); cohen2014anthropology is the companion to Kant (2012a) (stated in the note); flikschuh2014colonialism and mills2014race continue the race/colonialism discussion (Elden and Mendieta (eds.) (2011), Mikkelsen (ed.) (2013), Kleingeld (2011), Gray (2012)); goy2014biology continues the life-sciences strand (Mensch (2013)); ginsborg2014normativity follows Ginsborg (2011) (normativity); beiser2014neokantianism relates to Heis (2010) (Marburg neo-Kantianism).
1. stang2014nonidentity | Stang (2014) | T
2. gomes2014naive | Gomes (2014) | T
3. dyck2014rational | Dyck (2014) | T; INC; PUB
4. frierson2014empirical | Frierson (2014) | T
5. wuerth2014mind | Wuerth (2014) | P; AWARD
6. ware2014sensibility | Ware (2014) | P; INC
7. denis2014ethics | Denis and Sensen (eds.) (2014) | P; DATE
8. maliks2014politics | Maliks (2014) | L; DATE
9. flikschuh2014colonialism | Flikschuh and Ypi (eds.) (2014) | L
10. goy2014biology | Goy and Watkins (eds.) (2014) | A
11. ginsborg2014normativity | Ginsborg (2014) | A; DATE
12. cohen2014anthropology | Cohen (ed.) (2014) | R
13. mills2014race | Mills (2014) | R; INC
14. hall2014postcritical | Hall (2014) | X
15. beiser2014neokantianism | Beiser (2014) | C; INC; NDPR

### Year 2015 (15 entries; writer 3; domain 2)
**Threads**: book-length treatments of transcendental idealism and the Deduction (Allais 2015, Allison 2015); naive-realist and conceptualism-related articles (Stephenson 2015, Onof and Schulting 2015); a constructivist reading of reason (O'Neill 2015) and a Groundwork commentary (Schönecker and Wood 2015); reference and edition work (Kant-Lexikon, the revised *Critique of Practical Reason*, *Reading Kant's Lectures*).
**Continues**: allais2015manifest continues the two-aspect line (Marshall (2013), Stang (2014)); stephenson2015hallucination continues the naive-realist reading (Gomes (2014)); onof2015space continues the conceptualism debate (Tolley (2013), Gomes (2014)); oneill2015authorities continues the constructivism debate (Stern (2011), Wuerth (2014)); schonecker2015groundwork is a Groundwork commentary like Allison (2011), and Kant (2015) is the Cambridge Texts edition of the text treated in Reath and Timmermann (eds.) (2010); palmquist2015religion relates to DiCenso (2011) and Insole (2013) (Religion).
1. allais2015manifest | Allais (2015) | T; AWARD
2. allison2015deduction | Allison (2015) | T; INC; PUB
3. ferrarin2015powers | Ferrarin (2015) | T; INC; NDPR
4. anderson2015poverty | Anderson (2015) | T
5. stephenson2015hallucination | Stephenson (2015) | T
6. onof2015space | Onof and Schulting (2015) | T
7. mcnulty2015regulative | McNulty (2015) | T; INC; AWARD
8. schonecker2015groundwork | Schönecker and Wood (2015) | P
9. oneill2015authorities | O'Neill (2015) | P
10. friedlander2015expressions | Friedlander (2015) | A
11. palmquist2015religion | Palmquist (2015) | R; INC; PUB; DATE
12. gardner2015turn | Gardner and Grist (eds.) (2015) | C; INC; NDPR
13. reath2015practical | Kant (2015) | E; ED
14. kantlexikon2015 | Willaschek et al. (eds.) (2015) | E; REF
15. clewis2015lectures | Clewis (ed.) (2015) | E

### Year 2016 (14 entries; writer 4; domain 3)
**Threads**: modal metaphysics (Stang 2016); the conceptualism and perception debate (Schulting (ed.) 2016, Conant 2016, McLear 2016); Kant's racism (Allais 2016); the highest good (Höwing (ed.) 2016); the Cambridge Edition *Lectures and Drafts on Political Philosophy* (Kant 2016); Opus postumum and pre-critical work (McNulty 2016, Dyck 2016).
**Continues**: stang2016modal relates to Chignell (2012) (modal metaphysics); mclear2016perceptual follows McLear (2011) and joins the naive-realist discussion (Gomes (2014), Stephenson (2015)); schulting2016nonconceptualism continues the conceptualism debate (Hanna (2011), Tolley (2013), Onof and Schulting (2015)); conant2016kantian states a conceptualist reading (cf. Griffith (2012)); westphal2016natlaw continues the constructivism debate (Stern (2011), O'Neill (2015)); allais2016racism continues the race debate and answers Mills (see Mills (2014)); nassar2016analogical continues the life-sciences strand (Mensch (2013), Goy and Watkins (eds.) (2014)); mcnulty2016chemistry relates to Hall (2014) (Opus postumum) and McNulty (2015) (chemistry); dyck2016spontaneity relates to Dyck (2014).
1. stang2016modal | Stang (2016) | T
2. mclear2016perceptual | McLear (2016) | T
3. schulting2016nonconceptualism | Schulting (ed.) (2016) | T
4. conant2016kantian | Conant (2016) | T
5. guyer2016virtues | Guyer (2016) | P
6. hoewing2016highest | Höwing (ed.) (2016) | P
7. westphal2016natlaw | Westphal (2016) | L
8. nassar2016analogical | Nassar (2016) | A
9. allais2016racism | Allais (2016) | R
10. dyck2016spontaneity | Dyck (2016) | X
11. mcnulty2016chemistry | McNulty (2016) | X
12. matherne2016merleau | Matherne (2016) | C
13. rauscher2016lectures | Kant (2016) | E; ED
14. fugate2016eberhard | Eberhard (2016) | E; ED

### Year 2017 (16 entries; writer 4; domain 3)
**Threads**: cognition, perception and the self (Watkins and Willaschek 2017, Gomes and Stephenson (eds.) 2017, Longuenesse 2017, O'Shea (ed.) 2017); normativity (Pollok 2017); laws of nature and mathematics (Massimi and Breitenbach (eds.) 2017, Sutherland 2017); global justice and colonialism (Flikschuh 2017, Valdez 2017); Kant and women (Varden 2017); the late transition project (Thorndike 2017).
**Continues**: watkinswillaschek2017 and gomesstephenson2017 continue the conceptualism and naive-realist discussion (Gomes (2014), Stephenson (2015), McLear (2016)); oshea2017 is a volume-length survey of the first Critique like Guyer (ed.) (2010); longuenesse2017 relates to Kitcher (2011) (apperception) and to the Paralogisms (Proops (2010), Dyck (2014)); pollok2017 relates to Ginsborg (2014) (normativity); sutherland2017number continues the Kant-and-mathematics strand (Friedman (2012)); flikschuh2017 and valdez2017 continue the colonialism discussion (Flikschuh and Ypi (eds.) (2014)); varden2017women continues the gender discussion (Papadaki (2010), Hay (2013)); thorndike2017 relates to Hall (2014) and McNulty (2016) (late work); huneman2017organism relates to Nassar (2016) and Goy and Watkins (eds.) (2014); engelland2017 relates to Golob (2013) (Heidegger on Kant).
1. longuenesse2017 | Longuenesse (2017) | T
2. pollok2017 | Pollok (2017) | T
3. watkinswillaschek2017 | Watkins and Willaschek (2017) | T
4. gomesstephenson2017 | Gomes and Stephenson (eds.) (2017) | T
5. oshea2017 | O'Shea (ed.) (2017) | T
6. massimibreitenbach2017 | Massimi and Breitenbach (eds.) (2017) | T
7. sutherland2017number | Sutherland (2017) | T
8. kleingeld2017 | Kleingeld (2017) | P
9. flikschuh2017 | Flikschuh (2017) | L
10. valdez2017 | Valdez (2017) | L
11. chaouli2017 | Chaouli (2017) | A
12. huneman2017organism | Huneman (2017) | A
13. varden2017women | Varden (2017) | R
14. thorndike2017 | Thorndike (2017) | X; NDPR; DATE
15. engelland2017 | Engelland (2017) | C
16. denis2017mm | Kant (2017) | E; ED

### Year 2018 (15 entries; writer 4; domain 3)
**Threads**: the Transcendental Dialectic (Willaschek 2018); Kant and animals (Korsgaard 2018); the race debate (Mills 2018, Sandford 2018); several Cambridge Elements (Horstmann 2018, Holtman 2018, Merritt 2018b); Baumgarten and Kant (Fugate and Hymers (eds.) 2018); a new edition of the *Religion* (Kant 2018) and the XII Kant-Kongress proceedings (Waibel et al. (eds.) 2018).
**Continues**: korsgaard2018fellow joins the animals discussion (McLear (2011)); mills2018radical continues the race debate (the note states that Allais (2016) answers Mills's earlier proposal; cf. Mills (2014)); sandford2018 takes the "systematic link" side of the race debate (cf. Mills (2014), Allais (2016)); naturfreiheit2018 belongs to the Kant-Kongress series (Bacin et al. (eds.) (2013)).
1. willaschek2018 | Willaschek (2018) | T
2. horstmann2018 | Horstmann (2018) | T
3. luadler2018 | Lu-Adler (2018) | T
4. merritt2018 | Merritt (2018a) | P; NDPR (summary source is the NDPR review)
5. sorensen2018 | Sorensen and Williamson (eds.) (2018) | P
6. papish2018 | Papish (2018) | P
7. holtman2018 | Holtman (2018) | L
8. merrittsublime2018 | Merritt (2018b) | A
9. korsgaard2018fellow | Korsgaard (2018) | R
10. mills2018radical | Mills (2018) | R; INC; SNIP
11. sandford2018 | Sandford (2018) | R
12. fugatehymers2018 | Fugate and Hymers (eds.) (2018) | X
13. nisenbaum2018 | Nisenbaum (2018) | C
14. kantreligion2018 | Kant (2018) | E; ED
15. naturfreiheit2018 | Waibel et al. (eds.) (2018) | E; REF

### Year 2019 (15 entries; writer 5; domain 4)
**Threads**: autonomy, constructivism and constitutivism (Kleingeld and Willaschek 2019, Schafer 2019); laws of nature (Watkins 2019); modality and the metaphysics lectures (Abacı 2019, Fugate (ed.) 2019); nonideal theory and cosmopolitanism (Huseyinzadegan 2019, Valdez 2019); how to deal with Kant's sexism and racism (Kleingeld 2019); the Yale Groundwork edition (Kant 2019).
**Continues**: abaci2019modality follows Stang (2016) (stated in the NDPR note); kleingeldwillaschek2019autonomy and schafer2019constitutivism continue the constructivism/realism debate (Stern (2011), Wuerth (2014), O'Neill (2015), Westphal (2016)); watkins2019laws relates to Massimi and Breitenbach (eds.) (2017) (laws of nature); ameriks2019subjects continues Ameriks (2012) (the note says it continues his line of interpretation); valdez2019transnational continues Valdez (2017) and Flikschuh and Ypi (eds.) (2014); kleingeld2019sexismracism joins the race and gender debates (Mills (2018), Sandford (2018), Varden (2017)); insole2019freebelief relates to Insole (2013); howard2019transition relates to Hall (2014) and Thorndike (2017) (transition project); kant2019groundwork relates to Kant (2011), Allison (2011) and Schönecker and Wood (2015) (Groundwork editions and commentaries).
1. watkins2019laws | Watkins (2019) | T; NDPR (summary source is the NDPR review)
2. abaci2019modality | Abacı (2019) | T
3. kraus2019inner | Kraus (2019) | T
4. kleingeldwillaschek2019autonomy | Kleingeld and Willaschek (2019) | P; INC
5. schafer2019constitutivism | Schafer (2019) | P
6. formosasticker2019beneficence | Formosa and Sticker (2019) | P
7. ameriks2019subjects | Ameriks (2019) | P
8. huseyinzadegan2019nonideal | Huseyinzadegan (2019) | L; REV
9. valdez2019transnational | Valdez (2019) | L
10. fisher2019organisms | Fisher (2019) | A; INC
11. insole2019freebelief | Insole (2019) | R
12. kleingeld2019sexismracism | Kleingeld (2019) | R; INC
13. howard2019transition | Howard (2019) | X
14. kant2019groundwork | Kant (2019) | E; ED; INC; PUB
15. fugate2019lectures | Fugate (ed.) (2019) | E

### Year 2020 (15 entries; writer 5; domain 4)
**Threads**: Kant and animals (Callanan and Allais (eds.) 2020); sex, love and gender (Varden 2020); inner sense and self-knowledge (Kraus 2020); the philosophy of mathematics (Posy and Rechter (eds.) 2020); freedom (Allison 2020); religion (Wood 2020); race and nonideal theory (Basevich 2020); reception through Cassirer, Husserl and McDowell (Biagioli 2020, van Mazijk 2020).
**Continues**: kraus2020selfknowledge follows Kraus (2019); allaiscallanan2020animals continues the animals discussion (McLear (2011), Korsgaard (2018)); varden2020sex continues the gender discussion (Papadaki (2010), Hay (2013), Varden (2017)); basevich2020race continues the race debate (Mills (2018), Kleingeld (2019)) and the nonideal-theory strand (Huseyinzadegan (2019)); kleingeld2020meremeans continues the humanity-formula discussion (Pallikkathayil (2010)); wood2020religion relates to DiCenso (2011), Palmquist (2015) (Religion); posyrechter2020mathematics relates to Friedman (2012), Sutherland (2017); biagioli2020cassirer relates to Heis (2010) (Cassirer); vanmazijk2020perception continues the conceptualism debate (Matherne (2016)); moller2020tribunal relates to Pollok (2017) (normativity).
1. kraus2020selfknowledge | Kraus (2020) | T
2. cohen2020emotions | Cohen (2020) | T; INC
3. deboer2020reform | de Boer (2020) | T
4. moller2020tribunal | Møller (2020) | T
5. posyrechter2020mathematics | Posy and Rechter (eds.) (2020) | T; PUB
6. allison2020freedom | Allison (2020) | P
7. kleingeld2020meremeans | Kleingeld (2020) | P
8. loriaux2020distributive | Loriaux (2020) | L
9. halper2020artnature | Halper (2020) | A
10. wood2020religion | Wood (2020) | R
11. varden2020sex | Varden (2020) | R
12. allaiscallanan2020animals | Callanan and Allais (eds.) (2020) | R (cite the editors in the digest order)
13. basevich2020race | Basevich (2020) | R
14. biagioli2020cassirer | Biagioli (2020) | C
15. vanmazijk2020perception | van Mazijk (2020) | C

### Year 2021 (15 entries; writer 5; domain 4)
**Threads**: the two-world/two-aspect debate and the Dialectic (Jauernig 2021, Proops 2021); the philosophy of mathematics (Sutherland 2021); the law of war (Ripstein 2021); women, enlightenment and race (Sabourin 2021, Yab 2021); the *Cambridge Kant Lexicon* and the 13th Kant Congress proceedings (Wuerth (ed.) 2021, Himmelmann and Serck-Hanssen (eds.) 2021).
**Continues**: jauernig2021world continues the two-world versus two-aspect debate (Marshall (2013), Stang (2014), Allais (2015)); proops2021fiery relates to Proops (2010) and Willaschek (2018) (Dialectic); schafer2021capacitiesfirst follows Schafer (2019); sutherland2021mathematical relates to Sutherland (2017) and Posy and Rechter (eds.) (2020); ware2021justification relates to Ware (2014); sabourin2021enlightenment continues the gender discussion (Varden (2017)); yab2021racism continues the race and cosmopolitan-right discussion (Kleingeld (2011), Valdez (2019)); merritt2021stoic relates to Papish (2018) (radical evil); ripstein2021war relates to Byrd and Hruschka (2010) (Doctrine of Right); wuerth2021lexicon relates to Willaschek et al. (eds.) (2015) (reference works); himmelmannserckhanssen2021court belongs to the Kant-Kongress series (Waibel et al. (eds.) (2018)).
1. jauernig2021world | Jauernig (2021) | T
2. proops2021fiery | Proops (2021) | T
3. ypi2021architectonic | Ypi (2021) | T
4. sutherland2021mathematical | Sutherland (2021) | T
5. hogan2021handedness | Hogan (2021) | T
6. schafer2021capacitiesfirst | Schafer (2021) | T
7. schulting2021apperception | Schulting (2021) | T
8. ware2021justification | Ware (2021) | P
9. ripstein2021war | Ripstein (2021) | L
10. makkai2021taste | Makkai (2021) | A
11. merritt2021stoic | Merritt (2021) | R
12. sabourin2021enlightenment | Sabourin (2021) | R
13. yab2021racism | Yab (2021) | R; INC; PUB
14. wuerth2021lexicon | Wuerth (ed.) (2021) | E; REF
15. himmelmannserckhanssen2021court | Himmelmann and Serck-Hanssen (eds.) (2021) | E; REF

### Year 2022 (15 entries; writer 6; domain 5)
**Threads**: metaphysical readings of Kant's idealism (Schafer and Stang (eds.) 2022); a Critical Guide to the *Metaphysical Foundations* (McNulty (ed.) 2022); the Opus postumum (Basile and Lyssy 2022); Kant and race and labour (Lu-Adler 2022, Pascoe 2022); Kant and artificial intelligence (Kim and Schönecker (eds.) 2022); a critical edition of the *Träume* (Kant 2022).
**Continues**: schaferstang2022sensible continues the metaphysical-reading line (Jauernig (2021), Willaschek (2018)); pendlebury2022mind continues the conceptualism debate (McLear (2016), Conant (2016), Watkins and Willaschek (2017)); mcnulty2022mfnw relates to Friedman (2013); timmons2022virtue relates to Trampota et al. (eds.) (2013) (Doctrine of Virtue); pascoe2022labour continues the gender-and-citizenship discussion (Sabourin (2021)); stone2022provisional relates to Byrd and Hruschka (2010) (private right); geiger2022empirical relates to Ypi (2021) (purposiveness); luadler2022savagery continues the race debate (Allais (2016), Sandford (2018)); basile2022opus continues the transition-project discussion (Hall (2014), Thorndike (2017), Howard (2019)).
1. schaferstang2022sensible | Schafer and Stang (eds.) (2022) | T
2. gomes2022categories | Gomes et al. (2022) | T
3. pendlebury2022mind | Pendlebury (2022) | T
4. mcnulty2022mfnw | McNulty (ed.) (2022) | T
5. wilson2022naturalistic | Wilson (2022) | T
6. timmons2022virtue | Timmons (2022) | P
7. herman2022commitments | Herman (2022) | P
8. kimschoenecker2022ai | Kim and Schönecker (eds.) (2022) | P
9. pascoe2022labour | Pascoe (2022) | L
10. stone2022provisional | Stone and Hasan (2022) | L
11. geiger2022empirical | Geiger (2022) | A
12. luadler2022savagery | Lu-Adler (2022) | R
13. rosen2022shadow | Rosen (2022) | R
14. basile2022opus | Basile and Lyssy (2022) | X (check editor field, Part B rule 8)
15. kant2022traume | Kant (2022) | E; ED (German-language critical edition)

### Year 2023 (15 entries; writer 6; domain 5)
**Threads**: a book-length treatment of Kant, race and racism (Lu-Adler 2023); freedom and rational agency (Kohl 2023); the formulas of the categorical imperative (Fahmy 2023, Kleingeld 2023); the unity of the third Critique and natural history (Sweet 2023, Cooper 2023); the late philosophy of nature (Howard 2023); sex, love and friendship (Rinne and Brecher (eds.) 2023); Heidegger's reading of Kant (Lambeth 2023).
**Continues**: luadler2023race continues Lu-Adler (2022) (stated in the note) and the race debate; schafer2023reason follows Schafer (2019) and Schafer (2021); kohl2023freedom relates to Allison (2020) (freedom); howard2023latenature follows Howard (2019) and relates to Basile and Lyssy (2022); fahmy2023merely continues the humanity-formula discussion (Kleingeld (2020), Pallikkathayil (2010)); kleingeld2023volitional follows Kleingeld (2017); rinne2023sex relates to Papadaki (2010) and Varden (2020); davies2023selfsufficiency relates to Pascoe (2022) (passive citizenship); sweet2023territory relates to Geiger (2022) (unity of the third Critique); cooper2023naturalhistory has links to the race debate (Sandford (2018)); chignell2023hope relates to Höwing (ed.) (2016) (moral faith); lambeth2023heidegger relates to Golob (2013), Engelland (2017); baiasu2023kantianmind relates to Wuerth (ed.) (2021) (reference works).
1. schafer2023reason | Schafer (2023) | T
2. stang2023schematism | Stang (2023) | T
3. cooper2023naturalhistory | Cooper (2023) | T
4. kohl2023freedom | Kohl (2023) | P
5. fahmy2023merely | Fahmy (2023) | P
6. kleingeld2023volitional | Kleingeld (2023) | P
7. davies2023selfsufficiency | Davies (2023) | L
8. sweet2023territory | Sweet (2023) | A
9. clewis2023origins | Clewis (2023) | A
10. chignell2023hope | Chignell (2023) | R
11. luadler2023race | Lu-Adler (2023) | R
12. rinne2023sex | Rinne and Brecher (eds.) (2023) | R
13. howard2023latenature | Howard (2023) | X
14. lambeth2023heidegger | Lambeth (2023) | C
15. baiasu2023kantianmind | Baiasu and Timmons (2023) | E; REF; INC; PUB; DATE (check editor field, Part B rule 8)

### Year 2024 (15 entries; writer 6; domain 5)
**Threads**: the tercentenary year of Kant's birth (22 April 2024), with the *Oxford Handbook of Kant* (Gomes and Stephenson (eds.) 2024); imagination and intuition (Matherne 2024, Smyth 2024, Russell 2024); dignity and Kant's racism (Ameriks 2024); race, radical evil and the Haitian Revolution (Papish 2024, Huseyinzadegan 2024); Baumgarten and the foundations of practical philosophy (Fugate and Hymers (eds.) 2024); two-aspect arguments from Kant's language (Rosefeldt 2024); a source-materials volume for the second Critique (Walschots 2024).
**Continues**: rosefeldt2024initself continues the two-aspect versus two-object debate (Stang (2014), Marshall (2013)); matherne2024seeing relates to Horstmann (2018) (imagination); smyth2024intuition relates to Allais (2010) (Transcendental Aesthetic); ameriks2024dignity relates to Sensen (2011) (dignity); vilhauer2024sympathy relates to Ware (2014) and Sorensen and Williamson (eds.) (2018) (moral feeling); papish2024race relates to Papish (2018), Merritt (2021) (radical evil) and Sandford (2018) (race and natural history); huseyinzadegan2024haiti takes the negative side of the systematic-link question (Sandford (2018), Mills (2014)); fugate2024baumgarten follows Fugate and Hymers (eds.) (2018); kinzel2024neokantian relates to Heis (2010), Biagioli (2020) (Marburg neo-Kantianism) and Pendlebury (2022) (conceptualism); aigner2024technics relates to Kim and Schönecker (eds.) (2022) (technology) and Howard (2023) (late work); walschots2024cpr relates to Kant (2015).
1. smyth2024intuition | Smyth (2024) | T
2. rosefeldt2024initself | Rosefeldt (2024) | T
3. matherne2024seeing | Matherne (2024) | T
4. russell2024fantasy | Russell (2024) | T
5. guyer2024impact | Guyer (2024a) | P
6. ameriks2024dignity | Ameriks (2024) | P
7. vilhauer2024sympathy | Vilhauer (2024) | P
8. guyer2024right | Guyer (2024b) | L
9. papish2024race | Papish (2024) | R
10. huseyinzadegan2024haiti | Huseyinzadegan (2024) | R
11. fugate2024baumgarten | Fugate and Hymers (eds.) (2024) | X
12. aigner2024technics | Aigner (2024) | X
13. kinzel2024neokantian | Kinzel (2024) | C; DATE
14. walschots2024cpr | Walschots (2024) | E; ED (an edition of source materials by Kant's contemporaries; say only what the note says)
15. gomes2024handbook | Gomes and Stephenson (eds.) (2024) | E; REF

### Year 2025 (15 entries; writer 7; domain 6)
**Threads**: the origins and structure of the first Critique (Anderson 2025, Stang 2025, Hogan 2025); the Metaphysics of Morals applied (Timmermann 2025, Sabourin 2025, Williams 2025); the race debate (Kleingeld 2025, a critical notice of Lu-Adler 2023); Kantian ethics and the environment (Heneghan 2025); the Opus postumum (Thomson 2025); an edition of student transcripts of the logic lectures (Kant 2025). The overview may also state that the indicators for 2025 entries are early (citation counts near zero, per the D6 header).
**Continues**: anderson2025skeptical relates to Proops (2021) (Antinomies); hogan2025nutshell follows Hogan (2021) and joins the two-aspect line (Jauernig (2021), Rosefeldt (2024)); stan2025natural relates to Friedman (2013) and McNulty (ed.) (2022); cureton2025sovereign continues the constructivism debate (Schafer (2023), Kleingeld and Willaschek (2019)); sabourin2025marriage follows Sabourin (2021) and relates to Varden (2020), Papadaki (2010); teufel2025teleology follows Teufel (2012); kleingeld2025antiracism is a critical notice of Lu-Adler (2023) (stated in the note); thomson2025opus continues the Opus postumum discussion (Howard (2023), Basile and Lyssy (2022), Hall (2014)); kant2025logicvolckmann relates to Lu-Adler (2018) (Kant's logic).
1. anderson2025skeptical | Anderson (2025) | T
2. stang2025obsolete | Stang (2025) | T
3. hogan2025nutshell | Hogan (2025) | T
4. stan2025natural | Stan (2025) | T
5. cureton2025sovereign | Cureton (2025) | P
6. kain2025goodwill | Kain (2025) | P
7. timmermann2025lie | Timmermann (2025) | P
8. heneghan2025environmental | Heneghan (2025) | P
9. williams2025incorporated | Williams (2025) | L
10. sabourin2025marriage | Sabourin (2025) | L (gender)
11. teufel2025teleology | Teufel (2025) | A
12. kleingeld2025antiracism | Kleingeld (2025) | R; INC; PUB
13. thomson2025opus | Thomson (2025) | X
14. bruno2025facticity | Bruno (2025) | C
15. kant2025logicvolckmann | Kant (2025) | E; ED; INC; PUB (German-language edition)

### Year 2026, through 2026-09-30 (13 entries; writer 7; domain 6)
**Threads**: a historicist, religion-centred reading of the critical project (Hunter 2026); collected essays on transcendental idealism and method (Guyer 2026); Kant and Freud, and predictive processing (Longuenesse 2026, Schlicht 2026); law and morality in the Doctrine of Right (Brecher and Hirsch (eds.) 2026); moral feeling (Noller 2026); Kant and colonial slavery (Lu-Adler 2026, online first). The overview may also state that 2026 indicators are early and that no NDPR review dated 2026 was found (D6 header).
**Continues**: wolf2026conclusions relates to Allais (2010) and Smyth (2024) (Transcendental Aesthetic); schnieder2026psr relates to Schafer (2023) (principle of sufficient reason); guyer2026selectedessays relates to the two-aspect line (Jauernig (2021)); carson2026mathematics relates to Posy and Rechter (eds.) (2020) and Sutherland (2021); longuenesse2026organization relates to Longuenesse (2017); schlicht2026predictive relates to Sturm and Wunderlich (2010) (Kant and the scientific study of the mind); brecher2026lawmorality relates to Guyer (2024b) and Williams (2025) (law and morality); khurana2026lifefreedom relates to Cureton (2025) and Kleingeld and Willaschek (2019) (autonomy; the note says it argues against the self-legislation model); noller2026respect relates to Ware (2014) and Vilhauer (2024) (moral feeling); luadler2026colonialslavery continues Lu-Adler (2022), Lu-Adler (2023) and Kleingeld (2025) (race and colonialism).
1. wolf2026conclusions | Wolf (2026) | T
2. kleingeld2026strikingsimilarity | Kleingeld (2026) | T
3. guyer2026selectedessays | Guyer (2026) | T; AWARD
4. carson2026mathematics | Carson (2026) | T
5. longuenesse2026organization | Longuenesse (2026) | T
6. schlicht2026predictive | Schlicht (2026) | T
7. noller2026respect | Noller (2026) | P
8. khurana2026lifefreedom | Khurana (2026) | P
9. brecher2026lawmorality | Brecher and Hirsch (eds.) (2026) | L
10. tuna2026artcriticism | Tuna (2026) | A
11. hunter2026kantianreligion | Hunter (2026) | R; INC; PUB
12. luadler2026colonialslavery | Lu-Adler (2026) | R; DATE
13. schnieder2026psr | Schnieder (2026) | X

---

## Conclusion (writer 8; heading `## Conclusion`; 300-450 words; runs last)

**Purpose**: Trace developments across years and the main debates, balanced, citing only digest works in the "Author (Year)" form of the bullets. Read synthesis-section-2..7.md first so every claim matches what the year sections say. No new works, no verdicts, no evaluative adjectives; use "the entries record", "the annotations describe", "remains contested in the entries".

**Content (one paragraph each, 4-6 paragraphs):**
1. *Transcendental idealism and perception.* Two-aspect (one-world) against two-world and two-object readings: Allais (2010), Schulting and Verburgt (eds.) (2011), Allison (2012), Marshall (2013), Stang (2014), Allais (2015), Jauernig (2021), Schafer and Stang (eds.) (2022), Rosefeldt (2024), Hogan (2025), Guyer (2026). Conceptualism and nonconceptualism, with naive-realist readings: Hanna (2011), McLear (2011), Griffith (2012), Tolley (2013), Gomes (2014), Stephenson (2015), Conant (2016), Watkins and Willaschek (2017), van Mazijk (2020), Pendlebury (2022), Kinzel (2024). The 2016-2018 and 2019-2022 annotations describe book-length reconstructions of Kant's metaphysics and Dialectic: Stang (2016), Willaschek (2018), Proops (2021), Schafer and Stang (eds.) (2022).
2. *Constructivism and the formulas.* Stern (2011), Wuerth (2014), O'Neill (2015), Westphal (2016), Kleingeld and Willaschek (2019), Schafer (2019), Schafer (2023), Cureton (2025), Khurana (2026); the humanity and universal-law formula discussions: Pallikkathayil (2010), Kleingeld (2017), Kleingeld (2020), Fahmy (2023), Kleingeld (2023). State that the entries present realist, constructivist and constitutivist readings side by side and do not record a settlement.
3. *Race, colonialism, gender, animals.* From Kleingeld (2011), Louden (2011), Elden and Mendieta (eds.) (2011), Gray (2012) and Mikkelsen (ed.) (2013), through Flikschuh and Ypi (eds.) (2014), Mills (2014), Allais (2016), Valdez (2017), Mills (2018), Sandford (2018), Kleingeld (2019), Basevich (2020), to Lu-Adler (2022; 2023; 2026), Huseyinzadegan (2024) and Kleingeld (2025). Describe the systematic-link question as the notes frame it (Sandford (2018) on the "systematic link" side, Huseyinzadegan (2024) on the negative side, Allais (2016) on the relation to universalist ethics, Kleingeld (2025) as a critical notice of Lu-Adler (2023)). Gender: Papadaki (2010), Hay (2013), Varden (2017), Varden (2020), Sabourin (2021), Rinne and Brecher (eds.) (2023), Sabourin (2025). Animals: McLear (2011), Korsgaard (2018), Callanan and Allais (eds.) (2020).
4. *Anthropology, science and mind.* Louden (2011), Kant (2012a), Frierson (2013), Frierson (2014), Cohen (ed.) (2014); Friedman (2013), Goy and Watkins (eds.) (2014), Massimi and Breitenbach (eds.) (2017), Watkins (2019), Posy and Rechter (eds.) (2020), McNulty (ed.) (2022); Kraus (2020), Longuenesse (2017), Longuenesse (2026), Schlicht (2026); Opus postumum: Hall (2014), Thorndike (2017), Howard (2019), Basile and Lyssy (2022), Howard (2023), Thomson (2025).
5. *Tercentenary and AI.* 2024 (tercentenary of Kant's birth) brings Gomes and Stephenson (eds.) (2024), Matherne (2024), Smyth (2024) and Ameriks (2024); the notes record no new Cambridge Edition volume for 2022-2024. Kant and AI or technology appears in Kim and Schönecker (eds.) (2022), Aigner (2024) and, for cognitive science, Schlicht (2026); the domain headers describe this strand as thin.
6. *Closing sentence(s).* The review is selective, tied to the recorded indicators, with early indicators for 2024-2026; the debates above remain open in the entries.

**Word target**: 300-450 words.

---

## Notes for Synthesis Writers and the Orchestrator

**Totals**: 17 year sections; 251 bullets (13/15/15/15/15/15/14/16/15/15/15/15/15/15/15/15/13). Introduction 250-350 words; Conclusion 300-450 words; year sections about 35-90 words per bullet plus a 25-60 word overview, so roughly 11,000-16,000 words in all.

**Checks the orchestrator can run after writing** (each is a count or search, no judgment): (a) per file, `## YEAR` headings are exactly those listed in Part A; (b) bullets (`- `) per year equal the N in section 0; (c) every "Cite as" string appears once as a bullet start; (d) none of the banned words of Part B rule 2 appears; (e) no `## References` heading; (f) the Conclusion cites only works whose Author (Year) occurs in the bullets.

**Digest anomalies and cautions** (details also in the report to the orchestrator): author/key mismatches (reath2015practical, rauscher2016lectures, denis2017mm and kantreligion2018 carry Kant as author although the keys name editors or translators; fugate2016eberhard has Eberhard as author; allaiscallanan2020animals lists Callanan first); missing `(ed.)` marks for baiasu2023kantianmind and basile2022opus; same-author-same-year pairs (Kant 2012, Merritt 2018 with two name variants, Guyer 2024) that the bibliography script will not letter; the D1 file has no @comment header; title artefacts (kleingeld2026strikingsimilarity, rosefeldt2024initself); dating differences recorded in YEAR NOTEs (Part B rule 9, flag DATE).
