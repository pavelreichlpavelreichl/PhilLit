# Literature Review Plan: Kant Scholarship 2010-2026, a Chronological Review by Year

## Research Idea Summary

A chronological literature review of the most significant scholarship on Immanuel Kant (books and journal articles, primarily in English, plus German/French works with international impact) published from 2010 through 2026 (2026 partial; today is 2026-09-30). The final review is organised BY YEAR (2010, 2011, ..., 2026), NOT thematically. Each year lists roughly 10-20 of the most significant works (fewer for 2026), each with a 1-3 sentence summary, and must span all major areas of Kant scholarship: theoretical philosophy, practical philosophy, aesthetics and teleology, political and legal philosophy, religion, anthropology/education/history, the Opus postumum and pre-critical work, Kant's reception, and the main interpretive debates.

## Key Research Questions

1. Which works, in each year 2010-2026, were the most significant in each major subfield of Kant scholarship, judged by prominent monographs, widely cited or influential articles, major edited volumes, new editions and translations, prizes, and works that shifted a debate?
2. How did the major interpretive debates develop across the period (two-world vs. two-aspect readings of transcendental idealism; conceptualism vs. nonconceptualism; constructivism vs. realism in Kantian ethics; Kant on race, gender, colonialism and animals; the status of the Opus postumum and the pre-critical work), and which works mark turning points?
3. How did the balance among subfields and traditions change (for example, the anthropology/empirical-psychology turn, the philosophy-of-science and mathematics revival, the political and legal turn, the growth of Kant-and-race scholarship, the 2024 tercentenary, Kant and AI)?
4. Which critical or dissenting works (critics of Kant, critics of dominant readings, decolonial/feminist/critical-race work, naturalist and speculative-realist reception) shaped the field, so that the review does not reflect only the mainstream Anglophone consensus?

## Selection Rule (applies to every domain)

**Include only the most significant works.** A work qualifies only if all of the following hold:

1. **Verified**: found and confirmed through the skill scripts (S2, CrossRef, PhilPapers via Brave, CORE, arXiv, NDPR). No entry may rest on the researcher's memory.
2. **Kant-central**: Kant's texts, concepts or arguments are the primary subject (or, for reception works, Kant is one of the two or three principal interlocutors). General "Kantian" moral or political theory qualifies only when it is a major, widely engaged Kant-interpretation (e.g., a constructivist reading of the Groundwork).
3. **Publication year within the block**, using the year the APIs return (see Year Assignment Rules).
4. **Significant by at least one recorded indicator** (see Significance Indicators): citation count relative to year and subfield, top-tier venue or series, prominent review coverage (NDPR, Mind, Philosophical Review, JHP, Kantian Review, Kant-Studien), prize or award, cited in SEP/IEP Kant entries, new edition/translation of a Kant text (e.g., Cambridge Edition), or documented role in shifting a debate.
5. **Non-duplicative**: not already recorded in an earlier block's .bib file.

## Constraints on Tooling (OpenAlex is unavailable)

- **OpenAlex currently returns 503. Do NOT use `search_openalex.py`**; do not treat its failure as a source failure. `enrich_bibliography.py` falls back from S2 to CORE automatically.
- **Use instead**: Semantic Scholar (`s2_search.py`, `s2_citations.py`, `s2_batch.py`, `s2_recommend.py`), CrossRef (`verify_paper.py`, plus the CrossRef REST API via `curl` for discovery and citation counts), PhilPapers via Brave (`search_philpapers.py`), Brave/WebSearch and WebFetch for publisher pages, prize lists and review pages, CORE (`search_core.py --year`), NDPR (`search_ndpr.py`, `fetch_ndpr.py`), SEP/IEP (`search_sep.py`, `fetch_sep.py`, `fetch_iep.py`), and arXiv only where relevant (Kant and AI/machine ethics, Kant and physics/logic/cognitive science, mainly 2022-2026).
- `search_philpapers.py` has no year filter (`--recent` means past year only). Put the year and a publisher or venue term in the query text and filter the results afterwards.
- `s2_search.py` supports `--year`, `--field Philosophy`, `--min-citations`, `--bulk` and `--limit`. It has no venue filter, so add the venue name to the query or post-filter by the returned venue.
- Save every raw script output as `.json` under `reviews/kant-2010-2026/intermediate_files/json/` (not just `reviews/kant-2010-2026/`). The metadata-provenance hook validates .bib fields against JSON files in that directory.

## Literature Review Domains (six sequential year-blocks)

Run Domain 1 through Domain 6 strictly in order (never in parallel). Each researcher should first read the citation keys and the @comment header of the preceding block's .bib file (to avoid duplicates and keep tags consistent), but must not copy entries. Output files: `reviews/kant-2010-2026/literature-domain-1.bib` through `literature-domain-6.bib`.

### Domain 1: 2010-2012

**Focus**: The most significant Kant scholarship published in 2010, 2011 and 2012, across all subfields. Aim for 10-15 entries per year (30-45 total), in balance across subfields (see Coverage Minimums).

**Period signature (a hypothesis to test, not a finding)**: A mature Anglophone commentary tradition (Allison, Guyer, Longuenesse, Ameriks). Debates on two-aspect vs. two-world readings and on nonconceptualism are active (Allais, Langton, Hanna, Ginsborg, Griffith, Gomes). Kantian constructivism and realism are contested in ethics (Korsgaard, Reath, O'Neill, Engstrom, Wood, Guyer, Schafer). Dignity, virtue and the Metaphysics of Morals receive book-length treatment. The Doctrine of Right and cosmopolitanism are in focus. Kant on race is being recovered as a topic. The Cambridge Edition is nearing completion (2012 volumes). The neo-Kantian and historicist reception is being revived (Beiser, Makkreel and Luft, Friedman).

**Key Questions**:
- Which 2010-2012 commentaries and monographs became reference points on the Groundwork, the Critique of Practical Reason, the Metaphysics of Morals (Right and Virtue) and the Critique of Pure Reason?
- Which articles defined the early-2010s state of the two-aspect/two-world and conceptualism/nonconceptualism debates?
- What new editions and translations appeared (Cambridge Edition volumes, revised Groundwork, Lectures on Anthropology, Natural Science), and what were the Kant-Kongress and reference-work outputs?
- How was Kant's reception treated (Kant and Hegel/German idealism, neo-Kantianism, Kant and phenomenology, Kant and analytic philosophy)?
- Which works began the Kant-and-race/anthropology/colonialism discussion, and which critical responses to dominant readings appeared?

**Search Strategy**:
- Primary sources: SEP/IEP Kant entries (bibliographies as a completeness check for 2010-2012); PhilPapers via Brave with the year in the query text; S2 with `--year 2010-2010`, `--year 2011-2011`, `--year 2012-2012` run separately for the generic queries (see Query Bank), and `--year 2010-2012` for the specific ones; CrossRef REST discovery for Kant-Studien, Kantian Review, JHP, Philosophical Review, Mind, Nous, Ethics, Philosophers' Imprint, EJP, AGPh (sorted by `is-referenced-by-count`); NDPR search for 2011-2013 reviews of 2010-2012 books (reviews lag publication by up to a year or two).
- Key terms: see Query Bank (all subfields, A through M), plus the block-specific ones: "Kant Groundwork commentary", "Kant's Doctrine of Right", "Kantian autonomy", "Kant dignity", "Kant nonconceptual content", "Kant transcendental idealism two aspects", "neo-Kantianism", "Kant cosmopolitanism", "Kant anthropology".
- Publishers to sweep: Cambridge UP (Critical Guides, Cambridge Companions, Cambridge Edition), Oxford UP, Harvard UP, Routledge, Palgrave, Springer, De Gruyter (Kant-Studien Ergaenzungshefte, Kant Yearbook), Indiana UP, SUNY, Chicago UP, Bloomsbury.
- Seed candidates (UNVERIFIED, from the planner's memory: locate through scripts; year and publisher may be wrong; do not include unless found): Byrd and Hruschka, *Kant's Doctrine of Right: A Commentary* (CUP); Baxley, *Kant's Theory of Virtue* (CUP); Uleman, *An Introduction to Kant's Moral Philosophy* (CUP); Guyer (ed.), *Cambridge Companion to Kant's Critique of Pure Reason*; Reath and Timmermann (eds.), *Kant's Critique of Practical Reason: A Critical Guide*; Denis (ed.), *Kant's Metaphysics of Morals: A Critical Guide*; Makkreel and Luft (eds.), *Neo-Kantianism in Contemporary Philosophy*; Allison, *Kant's Groundwork for the Metaphysics of Morals: A Commentary* and *Essays on Kant*; Kitcher, *Kant's Thinker*; Sensen, *Kant on Human Dignity*; Louden, *Kant's Human Being*; Schulting and Verburgt (eds.), *Kant's Idealism*; Elden and Mendieta (eds.), *Reading Kant's Geography*; Beiser, *The German Historicist Tradition*; Foerster, *The Twenty-Five Years of Philosophy*; Ameriks, *Kant's Elliptical Path*; Kleingeld, *Kant and Cosmopolitanism*; T. Hill, *Virtue, Rules, and Justice*; Sedgwick, *Hegel's Critique of Kant*; Stern, *Understanding Moral Obligation*; Parsons, *From Kant to Husserl*; Cambridge Edition volumes (revised *Groundwork*, *Lectures on Anthropology*, *Natural Science*). For articles, use author-based seeds only (Allais, Ginsborg, Hanna, Langton, Korsgaard, Reath, Engstrom, Guyer, Bernasconi, Kleingeld, Mills) and let S2 citation counts decide.
- Expected papers: 30-45 entries (from roughly 120-180 screened candidates).

**Relevance to Project**: Opens the chronology by fixing the baseline debates that later blocks extend or overturn, and records the last Cambridge Edition volumes.

---

### Domain 2: 2013-2015

**Focus**: The most significant Kant scholarship published in 2013, 2014 and 2015, across all subfields. Aim for 10-15 entries per year (30-45 total).

**Period signature (a hypothesis to test)**: An anthropology and empirical-psychology turn (Louden, Frierson, Cohen); Kant and the life sciences (Goy and Watkins, Mensch, Zammito, Ginsborg on organisms); Kant and the exact sciences (Friedman on the Metaphysical Foundations). Naive-realist and object-dependent readings of the Deduction and of transcendental idealism (Gomes, Stephenson, Allais 2015, Allison's Deduction commentary, McLear). Moral psychology, autonomy and constructivism (Grenberg, Sensen, Bagnoli, O'Neill, Stern). Kant and colonialism (Flikschuh and Ypi) and Kant's politics in context (Maliks). Guyer's multi-volume aesthetics history. Neo-Kantian genealogy (Beiser). Kant-Lexikon and revised Critique of Practical Reason (Reath).

**Key Questions**:
- Which monographs and articles from 2013-2015 defined the empirical (psychology, anthropology, biology, physics) side of Kant scholarship, and how did they change the reading of the critical system?
- How did the perception/intuition debates (nonconceptualism, naive realism, hallucination) develop after 2012?
- What book-length treatments of the Deduction, transcendental idealism (Allais, Allison) and judgment (Ginsborg) appeared, and how were they received (NDPR)?
- How did moral philosophy develop (moral psychology, dignity and autonomy, humanity formula, beneficence, constructivism), including the Lectures on Ethics and the revised Cambridge Critical Guides?
- Which works advanced critical perspectives on Kant (colonialism, race, gender, disability), and how were they answered?

**Search Strategy**:
- Primary sources: as in Domain 1, with the year ranges 2013-2013, 2014-2014, 2015-2015 for generic queries; NDPR for 2014-2017 reviews; SEP entries revised after 2013 (bibliographies).
- Key terms: Query Bank plus "Kant empirical psychology", "Kant anthropology lectures", "Kant biology teleology organism", "Kant Metaphysical Foundations natural science", "Kant naive realism", "Kant perception hallucination", "Kant colonialism", "Kant race Mills", "Kant beneficence", "Kant moral motivation", "Kant constructivism", "Kant Lectures on Ethics", "neo-Kantianism genesis", "Opus postumum".
- Publishers to sweep: as in Domain 1, plus Bloomsbury and University of Wales Press.
- Seed candidates (UNVERIFIED): Friedman, *Kant's Construction of Nature* (CUP); Mensch, *Kant's Organicism* (Chicago); Frierson, *What Is the Human Being?* and *Kant's Empirical Psychology*; Grenberg, *Kant's Defense of Common Moral Experience*; Kerstein, *How to Treat Persons*; Sweet, *Kant on Practical Life*; Sensen (ed.), *Kant on Moral Autonomy*; Bagnoli (ed.), *Constructivism in Ethics*; Wood, *The Free Development of Each*; Guyer, *A History of Modern Aesthetics*; Beiser, *The Genesis of Neo-Kantianism*; Maliks, *Kant's Politics in Context*; Flikschuh and Ypi (eds.), *Kant and Colonialism*; Goy and Watkins (eds.), *Kant's Theory of Biology*; Cohen (ed.), *Kant's Lectures on Anthropology: A Critical Guide*; Michalson (ed.), *Kant's Religion within the Boundaries of Mere Reason: A Critical Guide*; Pasternack, *Kant on Religion within the Boundaries of Mere Reason*; Golob, *Heidegger on Concepts, Freedom and Normativity*; Waxman, *Kant's Anatomy of the Intelligent Mind*; Allais, *Manifest Reality*; Allison, *Kant's Transcendental Deduction*; Ginsborg, *The Normativity of Nature*; Stern, *Kantian Ethics*; O'Neill, *Constructing Authorities*; Hall, *The Post-Critical Kant*; Denis and Sensen (eds.), *Kant's Lectures on Ethics*; Gardner and Grist (eds.), *The Transcendental Turn*; *Kant-Lexikon* (De Gruyter); Reath's revised Cambridge Edition *Critique of Practical Reason*; the 2013 proceedings of the Pisa Kant-Kongress (De Gruyter). Article author seeds: Gomes, Stephenson, McLear, Mills, Kleingeld, Bernasconi, Golob, Schafer, Stan, Breitenbach.
- Expected papers: 30-45 entries.

**Relevance to Project**: Records the empirical-science and moral-psychology turns and the first major critical-race and colonialism interventions in the mainstream literature.

---

### Domain 3: 2016-2018

**Focus**: The most significant Kant scholarship published in 2016, 2017 and 2018, across all subfields. Aim for 10-15 entries per year (30-45 total).

**Period signature (a hypothesis to test)**: Kant's modal metaphysics and the Dialectic (Stang, Willaschek, Chignell); laws of nature and scientific practice (Massimi and Breitenbach); persons, agency and mind (Watkins, Gomes and Stephenson, Longuenesse); normativity (Pollok); Kantian political and global thought (Rauscher's Cambridge Edition volume, Flikschuh, Holtman, Krasnoff et al.); animal ethics (Korsgaard); Kant's later work (Opus postumum studies); Kant's biology (Zammito, Goy); further Cambridge Critical Guides and handbooks (O'Shea, Altman); XII International Kant Congress proceedings.

**Key Questions**:
- Which 2016-2018 works reshaped readings of transcendental idealism, the Dialectic, modality and Kant's metaphysics?
- How did Kant on persons, agency, freedom and self-consciousness develop (including the philosophy-of-mind interpretations)?
- What were the main advances in Kant's philosophy of science, laws of nature, and biology?
- Which new work covered the Metaphysics of Morals (Right, welfare, civil society, global justice, virtue), Kant's ethics (highest good, humanity formula, Korsgaard), religion and evil?
- What was the state of the race/gender/colonialism and animal-ethics discussions?

**Search Strategy**:
- Primary sources: S2 with per-year ranges 2016-2016, 2017-2017, 2018-2018; CrossRef discovery per venue; NDPR for 2017-2019 reviews; SEP/IEP updates; Brave queries for Cambridge Critical Guides and Oxford volumes of 2016-2018.
- Key terms: Query Bank plus "Kant modality metaphysics", "Kant Dialectic transcendental illusion", "Kant laws of nature", "Kant persons agency", "Kant normativity", "Kant highest good", "Kant civil society welfare", "Kant global justice orientation", "Kant animals Korsgaard", "Kant Opus postumum transition", "Kant biology".
- Publishers: as above, plus Palgrave (Palgrave Kant Handbook), University of Wales Press, De Gruyter (congress volumes).
- Seed candidates (UNVERIFIED): Stang, *Kant's Modal Metaphysics* (OUP); Rauscher (ed.), Cambridge Edition *Lectures and Drafts on Political Philosophy*; Hoewing (ed.), *The Highest Good in Kant's Philosophy*; Longuenesse, *I, Me, Mine*; Watkins (ed.), *Kant on Persons and Agency*; Massimi and Breitenbach (eds.), *Kant and the Laws of Nature*; O'Shea (ed.), *Kant's Critique of Pure Reason: A Critical Guide*; Gomes and Stephenson (eds.), *Kant and the Philosophy of Mind*; Pollok, *Kant's Theory of Normativity*; Flikschuh, *What Is Orientation in Global Thinking?*; Altman (ed.), *The Palgrave Kant Handbook*; Korsgaard, *Fellow Creatures*; Willaschek, *Kant on the Sources of Metaphysics*; Schulting, *Kant's Radical Subjectivism*; Holtman, *Kant on Civil Society and Welfare*; Thorndike, *Kant's Transition Project and Late Philosophy*; Zammito, *The Gestation of German Biology*; Krasnoff, Sanchez Madrid and Satne (eds.), *Kant's Doctrine of Right in the Twenty-first Century*; Waibel et al. (eds.), *Natur und Freiheit* (Kant-Kongress 2015 proceedings, 2018); Nisenbaum, *For the Love of Metaphysics*. Article author seeds: Chignell, Stang, Schafer, McLear, Golob, Kleingeld, Lu-Adler, Allais, Watkins, Rosefeldt, Engstrom, Reath, Sensen.
- Expected papers: 30-45 entries.

**Relevance to Project**: Documents the shift from commentary on the Critiques toward systematic reconstruction of Kant's metaphysics, science, and agency, while cross-tracking the political and animal-ethics turns.

---

### Domain 4: 2019-2021

**Focus**: The most significant Kant scholarship published in 2019, 2020 and 2021, across all subfields. Aim for 10-15 entries per year (30-45 total).

**Period signature (a hypothesis to test)**: Kant on laws and metaphysics of nature (Watkins); philosophy of mathematics (Posy and Rechter's volumes); Kant and animals; a Kantian theory of sex, love and gender (Varden); a sustained book-length treatment of transcendental idealism (Jauernig 2021); intensified debates about Kant's racism and its place in his system; Kantian constructivism revisited (Schafer); Kant in Brandom-style Hegel/pragmatist reception; the Kantian Mind volume; continued growth of open-access and online-first journals (Ergo, Journal of Modern Philosophy, Journal of Transcendental Philosophy).

**Key Questions**:
- Which 2019-2021 works defined the mainstream interpretation of transcendental idealism and the systematic structure of the critical philosophy (Jauernig, Watkins, Willaschek, Allais)?
- How did Kant's philosophy of mathematics and physical science advance (Posy and Rechter, Massimi, Stan, McNulty)?
- How did Kant on gender, sex, marriage, animals and non-rational nature, race and colonial thought develop, and what were the principal disagreements (defenders vs. critics)?
- Which works advanced Kant's ethics and moral psychology (constructivism, emotions, virtue, self-cultivation, the Formula of Universal Law debates)?
- What reception work (German idealism, phenomenology, neo-Kantianism, analytic pragmatism) reshaped how Kant is read?

**Search Strategy**:
- Primary sources: S2 per-year ranges (2019-2019, 2020-2020, 2021-2021); CrossRef discovery; NDPR for 2020-2022 reviews; Kantian Review and Kant-Studien reviews; PhilPapers via Brave with year terms; CORE for open-access items (CORE `--year 2019-2021`).
- Key terms: Query Bank plus "Kant transcendental idealism appearances things in themselves", "Kant laws of nature", "Kant philosophy of mathematics", "Kant animals", "Kant sex gender marriage", "Kant race racism anthropology", "Kant constructivism realism", "Kant emotion feeling", "Kant self-cultivation", "Kant freedom determinism", "Kant Hegel pragmatism".
- Publishers: OUP, CUP, Routledge, Harvard UP, Bloomsbury, Palgrave, De Gruyter, Springer, Cambridge Elements (a newer format: check).
- Seed candidates (UNVERIFIED): Watkins, *Kant on Laws* (CUP); Schafer, "Realism and Constructivism in Kant's Metaphysics of Morals" (Philosophers' Imprint); Brandom, *A Spirit of Trust* (Harvard UP); Varden, *Sex, Love, and Gender: A Kantian Theory* (OUP); Allais and Callanan (eds.), *Kant and Animals* (OUP); Posy and Rechter (eds.), *Kant's Philosophy of Mathematics, Vol. 1* (CUP); Jauernig, *The World According to Kant* (OUP); Baiasu and Timmons (eds.), *The Kantian Mind* (Routledge). The planner's memory of 2019-2021 is thin: discovery must be search-driven.
- Expected papers: 30-45 entries.

**Relevance to Project**: Records the consolidation around systematic interpretations of transcendental idealism and the widening of the field to animals, sex/gender, mathematics and race.

---

### Domain 5: 2022-2024

**Focus**: The most significant Kant scholarship published in 2022, 2023 and 2024 (the 300th anniversary year of Kant's birth was 22 April 2024), across all subfields. Aim for 10-15 entries per year (30-45 total).

**Period signature (a hypothesis to test)**: Book-length treatments of Kant's logic and of race and racism (Lu-Adler, two 2023 books); Kant's mathematics (Sutherland); Critical Guide to the Metaphysical Foundations (McNulty); Kantian perspectival realism in philosophy of science (Massimi); the tercentenary wave of handbooks, anniversary volumes, special issues, biographies and exhibitions; new editions and translations; Kant and technology/AI; renewed argument over how to teach and read Kant given his racism.

**Key Questions**:
- Which 2022-2024 monographs and articles are the most significant in each subfield, and which were prompted by or published for the tercentenary?
- How did the Kant-and-race debate develop (Lu-Adler, Kleingeld, Bernasconi, Mills, Eze, others), including responses that defend or reject a systematic link between racism and the critical philosophy?
- What happened in Kant's logic, mathematics, science and mind (Lu-Adler, Sutherland, McNulty, Massimi, Golob, McLear)?
- What were the new directions in practical philosophy (Kantian ethics of technology/AI, ecological and animal ethics, disability, feminist work, political philosophy)?
- Which handbooks and reference works (Oxford Handbook of Kant if verified, congress proceedings, new Cambridge Edition or translation projects) shaped the field?

**Search Strategy**:
- Primary sources: S2 per-year ranges (2022-2022, 2023-2023, 2024-2024; citation counts will be modest, so use lower thresholds and other signals); CrossRef discovery; NDPR 2022-2025 reviews; PhilPapers via Brave; publisher catalogues (CUP, OUP, Routledge, De Gruyter, Bloomsbury, Springer, Palgrave) for 2022-2024; special-issue searches for the tercentenary (Kantian Review, Kant-Studien, JHP, BJHP, EJP, Journal of Modern Philosophy, Journal of Transcendental Philosophy, Kant Yearbook); arXiv and CORE for Kant and AI/machine ethics.
- Key terms: Query Bank plus "Kant 300th anniversary", "Kant tercentenary", "Kant logic", "Kant race racism", "Kant mathematics", "Kant perspectival realism", "Kant artificial intelligence", "Kant machine ethics", "Kantian ethics technology", "Kant environmental ethics", "Kant disability", "Kant feminist", "Kant decolonial", "Kant Oxford Handbook".
- Seed candidates (UNVERIFIED, low confidence): Lu-Adler, *Kant, Race, and Racism: Views from Somewhere* (OUP); Lu-Adler, *Kant and the Science of Logic* (OUP); Sutherland, *Kant's Mathematical World* (CUP); McNulty (ed.), *Kant's Metaphysical Foundations of Natural Science: A Critical Guide* (CUP); Massimi, *Perspectival Realism* (OUP); Gomes and Stephenson (eds.), *The Oxford Handbook of Kant* (verify existence and year).
- Expected papers: 30-45 entries.

**Relevance to Project**: Captures the tercentenary-driven output and the mature phase of the race debate, plus emerging technology/AI applications; it is the block most exposed to the citation-count lag, so non-citation indicators matter most.

---

### Domain 6: 2025-2026 (partial year; today 2026-09-30)

**Focus**: The most significant Kant scholarship published in 2025 (10-15 entries) and 2026 through 2026-09-30 (fewer, roughly 5-10). Target total: 20-30 entries.

**Period signature**: None assumed. The planner has no reliable knowledge of 2025-2026 output, so this block must be discovery-driven from tool results; no seeds are supplied.

**Key Questions**:
- Which monographs, edited volumes, editions/translations and articles published in 2025 and 2026 already show significance indicators (prominent publisher/venue, NDPR or journal reviews, early citations, prizes)?
- Which post-tercentenary trends are visible (consolidation, new editions and translations, Kant and AI/technology, ecological and animal ethics, race/decolonial work, cognitive-science and philosophy-of-science engagements)?
- Which 2025-2026 works respond critically to the dominant readings of the 2010s?

**Search Strategy**:
- Primary sources: S2 (`--year 2025-2026`, per-year runs; sort/screen by citations though counts are low; use `s2_recommend.py` from strong 2022-2025 seeds); CrossRef REST discovery with `from-pub-date:2025-01-01,until-pub-date:2026-09-30` filtered by venue ISSN; publisher catalogues and "forthcoming/new" pages (CUP, OUP, Harvard UP, Routledge, De Gruyter, Bloomsbury) via Brave/WebFetch; NDPR 2025-2026 reviews; Kantian Review, Kant-Studien, JHP, BJHP, EJP, Ergo, Philosophers' Imprint, Ethics, Mind, Nous issues for 2025 and 2026; CORE and arXiv (`--recent`) for Kant and AI/physics/logic/cognitive science; PhilPapers via Brave with "2025"/"2026" in the query.
- Key terms: Query Bank (all subfields), "Kant" with "2025" and "2026", "Kantian" AND "artificial intelligence"/"large language models", "Kant Critical Guide 2025", "Cambridge Edition new translation".
- Constraints: include only works with a verifiable 2025 or 2026 date. Announced-but-unpublished works are excluded. Online-first 2026 articles qualify only if CrossRef or S2 returns 2026 as the year. S2 coverage lags by months, so cross-check with CrossRef and publisher pages.
- Expected papers: 20-30 entries. Fewer is acceptable if verification fails; report the shortfall in NOTABLE_GAPS.

**Relevance to Project**: Completes the chronology up to the present and tests which recent works can already be called significant on non-citation evidence.

---

## Common Search Protocol (applies to every domain)

### Query Bank (run each with the block's year range; run generic ones per single year)

| Code | Subfield | Queries (prefix "Kant" or "Kantian" where not present) |
|---|---|---|
| A | Theoretical: Critique of Pure Reason, transcendental idealism, metaphysics | "transcendental idealism", "transcendental deduction", "categories judgment", "apperception self-consciousness", "space time transcendental aesthetic", "things in themselves appearances", "antinomies dialectic", "modality metaphysics", "causality Hume", "nonconceptual content", "conceptualism", "schematism imagination", "regulative principles reason", "transcendental argument skepticism", "refutation of idealism" |
| B | Philosophy of science and mathematics, logic | "Metaphysical Foundations natural science", "philosophy of mathematics geometry", "laws of nature", "Newton matter force", "chemistry physics", "logic general logic" |
| C | Mind and psychology | "empirical psychology", "perception", "self-knowledge", "cognition faculties" |
| D | Ethics: Groundwork, CPrR, autonomy | "categorical imperative", "formula of humanity", "autonomy", "Groundwork", "moral motivation respect", "freedom fact of reason", "highest good", "moral psychology", "constructivism realism", "dignity", "conscience" |
| E | Metaphysics of Morals, virtue | "Metaphysics of Morals", "doctrine of virtue", "duties to self", "beneficence", "lying", "marriage sex" |
| F | Political, legal, cosmopolitan | "Doctrine of Right", "property private right", "public right state", "cosmopolitan right", "perpetual peace", "international justice", "punishment", "republicanism", "colonialism" |
| G | Aesthetics and teleology (CPJ) | "judgment of taste beauty", "sublime", "genius art", "purposiveness", "teleology organisms", "reflective judgment", "biology" |
| H | Religion | "Religion within the Boundaries", "radical evil", "moral faith", "God postulates", "rational theology", "ethical community church" |
| I | Anthropology, history, education, race, gender, animals | "anthropology", "race racism", "gender women", "education pedagogy", "philosophy of history", "Enlightenment", "human nature", "animals" |
| J | Pre-critical, Opus postumum | "pre-critical", "Inaugural Dissertation 1770", "Only Possible Argument", "Opus postumum", "transition physics", "Leibniz Wolff" |
| K | Reception | "Fichte", "Hegel", "Schelling", "Schopenhauer", "neo-Kantian Marburg Cassirer Cohen", "Heidegger", "Husserl", "Sellars", "Strawson", "McDowell", "Rawls", "Habermas", "Arendt", "Foucault", "speculative realism Meillassoux", "naturalism" |
| L | Interpretive debates | "two-world two-aspect", "conceptualism nonconceptualism", "constructivism", "Kantian humility", "race gender critique" |
| M | Editions, translations, reference | "Cambridge Edition of the Works of Immanuel Kant", "translation", "Akademie edition", "Kant-Lexikon", "Kant Handbook", "Companion to Kant", "Critical Guide", "Kant-Kongress proceedings" |

### Discovery steps (per domain)

1. **Encyclopedia baseline**: `search_sep.py` and `search_iep.py` for Kant and each subfield; discover exact slugs (do not assume slugs); pull bibliographies with `fetch_sep.py --bibliography-only` and keep entries in the block's year range as candidates; save slugs to `intermediate_files/json/encyclopedia_entries.json`.
2. **S2 sweeps**: per Query Bank row, `s2_search.py "<query>" --field Philosophy --year <Y-Y> --limit 50`, saving each result set as JSON. Use `--min-citations` as the initial screen (heuristic, calibrate to what the results show): 2010-2012 about 40+, 2013-2015 about 30+, 2016-2018 about 20+, 2019-2021 about 10+, 2022-2024 about 3+, 2025-2026 none. Lower the threshold within a subfield when fewer than the quota survive (philosophy citation counts are low and books are under-indexed by S2).
3. **CrossRef discovery**: verify each journal's ISSN through the CrossRef `journals?query=` endpoint, then use `curl` on `https://api.crossref.org/works?query.bibliographic=Kant&filter=issn:<ISSN>,from-pub-date:<Y>-01-01,until-pub-date:<Y>-12-31&sort=is-referenced-by-count&order=desc&rows=50&mailto=$CROSSREF_MAILTO` per venue and per year, saving JSON in `intermediate_files/json/`. Core venues: Kant-Studien, Kantian Review, Journal of the History of Philosophy, British Journal for the History of Philosophy, Archiv fuer Geschichte der Philosophie, Philosophical Review, Mind, Nous, Ethics, Philosophers' Imprint, European Journal of Philosophy, Canadian Journal of Philosophy, Philosophy and Phenomenological Research, Philosophical Quarterly, Journal of Moral Philosophy, Philosophy and Public Affairs, Journal of Political Philosophy, Journal of Aesthetics and Art Criticism, British Journal of Aesthetics, Studies in History and Philosophy of Science, Oxford Studies in Early Modern Philosophy, Journal of the American Philosophical Association, Ergo, Kant Yearbook, Journal of Modern Philosophy, Journal for the History of Analytical Philosophy, Inquiry, Review of Metaphysics, Hegel Bulletin.
4. **PhilPapers via Brave**: `search_philpapers.py "Kant <topic> <year> <publisher>" --limit 40`; also WebSearch with `site:philpapers.org` patterns and PhilPapers Kant category pages (verify category names). Filter by year manually.
5. **Books, editions, edited volumes**: Brave/WebSearch and WebFetch for publisher series pages (Cambridge Critical Guides, Cambridge Companions, Cambridge Edition of the Works of Immanuel Kant, Oxford Handbooks, Oxford Kant titles, Harvard UP, Routledge Philosophy GuideBooks, De Gruyter Kant-Studien Ergaenzungshaefte); `search_ndpr.py "Kant"` (and per author/title) as a significance signal; review pages in Mind, JHP, Kantian Review, Philosophical Review, Kant-Studien Rezensionen.
6. **Prizes**: search for book and essay prizes announced by learned societies (verify that each prize exists before using it): North American Kant Society, Kant-Gesellschaft, British Society for the History of Philosophy, APA and similar; record an award only when a source page confirms it.
7. **Citation chaining**: `s2_citations.py --citations` on anchor works of the period (for example Allison, Guyer, Korsgaard, Longuenesse, O'Neill, Allais and other widely cited books found in the S2 results) to find in-window works with high citing counts; `s2_recommend.py` from confirmed seeds.
8. **Balance check**: after harvesting, tabulate candidates by year x subfield (see Coverage Minimums), then run targeted supplementary searches for any empty cell before finalising.

### Coverage Minimums (per year; ~10-15 entries per year)

Every year in every block should include, when verifiable works exist:
- Theoretical philosophy (CPR, transcendental idealism, metaphysics, epistemology, science/math/logic, mind): 3-4 entries, including at least one science/math/mind entry.
- Practical philosophy (Groundwork, CPrR, autonomy, moral psychology, Metaphysics of Morals, virtue): 3-4 entries.
- Political, legal and cosmopolitan philosophy or philosophy of history: 1-2 entries.
- Aesthetics and teleology/biology: 1-2 entries.
- At least one entry from religion, anthropology, education, race, gender, animals, pre-critical work or the Opus postumum (rotate so every block covers all of these).
- At least one reception entry (German idealism, phenomenology, neo-Kantianism, analytic philosophy, critical theory or other).
- At least one edited volume, edition/translation, or reference work when notable ones exist (these may double-count as a subfield entry).
- Cap: no more than about 15 per year and 48 per block (up to 20 in exceptionally rich years only when the extra works clear the significance rule). If a cell cannot be filled with a verifiable, significant work, leave it empty and record the gap; never pad.
- Non-Anglophone works: include German/French/Italian/Spanish works only when they have documented international impact (translated into English, widely cited in English-language scholarship, or major reference works such as *Kant-Lexikon* and Kant-Kongress proceedings); at most 2-4 per block.

### Significance Indicators (record for every entry; data only, no evaluative adjectives)

Record in the `note` field, on a line beginning `SIGNIFICANCE INDICATORS:`:
- S2 citation count with retrieval date (2026-09-30), and CrossRef `is-referenced-by-count` when available; compare within the same year and subfield, not across blocks (older works have accumulated more citations).
- Venue or publisher tier (for example journal name, Cambridge Critical Guide, Oxford Handbook, Cambridge Edition).
- Review evidence: NDPR review (yes/no), other prominent journal reviews (name them).
- Awards or prizes (with source).
- Encyclopedia evidence: appears in the SEP/IEP Kant bibliographies (name the entry slug), or `get_sep_context.py` output.
- Debate role: which debate it advances (use only what the abstract, review or encyclopedia text says).
- Importance tag in `keywords`: `High` (multiple strong indicators or a documented debate-shifting role), `Medium`, `Low` (included mainly to fill subfield or year coverage). Use tags honestly: most entries should not be `High`.

### Entry Note Template (adapted for this project; descriptive, no superlatives such as "seminal", "landmark" or "most important")

```
note = {
SUMMARY: [1-3 sentences on what the work argues or does, grounded in the abstract, NDPR review or publisher description.]

SUBFIELD AND DEBATE: [subfield in words; debate joined or shifted, e.g. "two-aspect reading", "nonconceptualism", "constructivism", "Kant and race"; earlier or later works it responds to or is answered by, if the sources say so.]

SIGNIFICANCE INDICATORS: [data only: citations (count, date), venue/publisher, reviews, awards, SEP/IEP mention.]

YEAR NOTE: [only if the online-first year and the print year differ, or an edition/translation year differs from the original.]
}
```

Keywords format: `kant, <subfield tag(s)>, <debate tag(s) if any>, <type tag>, <High|Medium|Low>`.
- Subfield tags: `tp-cpr`, `tp-science-math`, `tp-mind`, `pp-ethics`, `pp-mm-virtue`, `pp-right-politics`, `aes-teleo`, `religion`, `anthro-hist-edu`, `precritical`, `opus-postumum`, `recep-idealism`, `recep-phenom`, `recep-analytic`, `recep-neokantian`, `recep-other`, `edition-trans`, `reference`.
- Debate tags: `debate-two-aspect`, `debate-conceptualism`, `debate-constructivism`, `debate-race`, `debate-gender`, `debate-animals`, `debate-colonialism`, `debate-other-<word>`.
- Type tags: `type-monograph`, `type-article`, `type-edited-volume`, `type-chapter`, `type-translation-edition`, `type-reference-work`.

### Verification and Metadata Rules (critical for this project)

- **Never fabricate.** Seed candidates in this plan are memory-derived hints, not sources. An entry may appear only after it is found in tool output and its fields are grounded there. Prefer omitting an unverifiable work over including it; record it under NOTABLE_GAPS.
- **Books are the main risk.** S2 often lacks publisher data for books. Use `verify_paper.py --title ... --author ... --year ...` and `--doi` (most OUP, CUP, Harvard UP, Routledge, De Gruyter, Springer, Palgrave and Bloomsbury books have CrossRef DOIs) to obtain `publisher` and `suggested_bibtex_type`; save each verification output as JSON in `intermediate_files/json/`. If no tool output supplies a publisher, use `@misc` with a URL obtained from search results; do not write a publisher from memory.
- Edited volumes: use `editor`, not `author`, as CrossRef indicates. Book chapters: use `@incollection` only when CrossRef says so.
- Run `enrich_bibliography.py` on each finished .bib; for High/Medium books without abstracts the NDPR fallback runs automatically. Run encyclopedia context extraction (`get_sep_context.py`) for High-importance entries.

### Year Assignment Rules

- The BibTeX `year` must be the year returned by the API (CrossRef issue/print year preferred). If online-first and print years differ, use the API year and note both in YEAR NOTE; do not move an entry to another block silently.
- Editions/translations are dated by the edition year, not the original composition year; note "translation of Kant (17xx)" in YEAR NOTE.
- Reprints, second editions and paperback reissues are excluded unless substantively revised (for example, Cambridge Edition revised translations count as new editions).
- Collections of previously published essays are dated by the collection year; mention the original dates if known from sources.

### Reporting to the Orchestrator (each domain)

Report: entries per year, a year x subfield count table, number of High/Medium/Low, number of INCOMPLETE entries (no abstract) and which are books, any seed candidates that could not be verified, source failures (expect OpenAlex not used), and shortfalls against the coverage minimums. The @comment header should contain a per-year coverage table and NOTABLE_GAPS naming empty cells.

---

## Coverage Rationale

Six year-blocks of three years (the last block a two-year, partial-year block) give sequential, bounded searches of about 30-45 significant entries each, so each researcher can work year by year inside a block, verify every item, and stay within context. Requiring every block to cover all subfields (theoretical, practical, aesthetics/teleology, political/legal, religion, anthropology/history/education/race/gender/animals, pre-critical/Opus postumum, reception, editions/translations, interpretive debates) prevents the year lists from collapsing into one dominant area such as the Critique of Pure Reason. The multi-source significance criteria (citations, venue/series, reviews, prizes, encyclopedia mentions, debate role) compensate for the known weakness of citation counts in a humanities field, and the per-year tagging by subfield and debate lets the synthesis planner build year sections and, where useful, cross-references between years.

## Expected Gaps

- **Selection bias**: citation counts favour older works, Anglophone monographs, established authors and mainstream readings; work by feminist, critical-race, decolonial and non-Anglophone scholars may be under-indexed. The plan requires deliberate checks (NDPR, prize lists, SEP/IEP, targeted queries; Query Bank rows I and L) rather than citation ranking alone.
- **Book coverage**: S2 indexes books poorly and many will lack abstracts; expect a high INCOMPLETE rate for books, which by current workflow rules would exclude them from synthesis (see Notes for Orchestrator).
- **Recency lag**: 2024-2026 works have few citations; significance must rest on publisher/venue, reviews and author standing, and S2 coverage lags publication.
- **Genuine unevenness**: some years may have fewer than ten verifiable significant works in some subfields (Opus postumum, pre-critical, religion); the review should record this honestly.
- **Year ambiguity**: online-first vs. print, and translation vs. original dates, may move works between years.
- **Possible research contributions**: the finished review will show which subfields (for example the Opus postumum, pre-critical work, religion) were under-represented in high-impact venues, and how the race/gender/animal-ethics debates moved from margins to mainstream.

## Estimated Scope

- **Total domains**: 6 year-blocks, run sequentially.
- **Estimated entries**: about 170-255 in total (Domains 1-5 about 30-45 each; Domain 6 about 20-30), from roughly 700-1,100 screened candidates. This is deliberately larger than the generic 40-80 papers-per-review guideline because the deliverable is a year-by-year list.
- **Key positions and debates to cover**: two-world vs. two-aspect (and naive-realist) readings of transcendental idealism; conceptualism vs. nonconceptualism; constructivism vs. realism and formula-based interpretations in Kantian ethics; Kant's racism and colonial thought (indictment vs. defence, and the systematic-link question); Kant on gender, animals and non-rational nature; empirical-psychology and biology readings; Kant in relation to German idealism, phenomenology, neo-Kantianism and analytic philosophy; critical reception (naturalist, speculative-realist, decolonial, feminist).

## Search Priorities

1. **Foundational anchors of each year**: new Cambridge Edition volumes and other new editions/translations, major monographs (OUP, CUP, Harvard UP, Routledge) with NDPR or journal reviews, and encyclopedia-cited works.
2. **Widely cited articles per year and venue**: top-cited Kant-related articles in the core venue list (CrossRef and S2 sorted by citations), including Kant-Studien and Kantian Review.
3. **Debate-shifting works**: works that opened or resolved a named debate, identified via citation chaining and review essays.
4. **Critical and dissenting works**: critical-race, feminist, decolonial, naturalist, speculative-realist and Hegelian/pragmatist critiques, plus rejoinders and defences.
5. **Recent developments (2022-2026)**: tercentenary volumes, Kant and AI/technology, new translations; use non-citation indicators.

## Notes for Researchers

- Use the `philosophy-research` skill scripts extensively; do not rely on prior knowledge. Seed candidates are hints only and must be found by scripts before any use.
- **Do NOT use OpenAlex** (503). Use S2, CrossRef, PhilPapers via Brave, CORE, NDPR, SEP/IEP, and arXiv where relevant.
- **Override the default target**: the generic instruction to gather 10-20 papers per domain is replaced for this project by 30-45 entries (Domain 6: 20-30), at about 10-15 per year.
- Work year by year within the block: harvest candidates for a single year across all Query Bank rows, shortlist against the Coverage Minimums, verify, and only then move on; keep a scratch candidate list in `intermediate_files/` (not in the .bib). Compose the .bib in year order.
- Respect rate limits (S2, CORE 5 requests per 10 s, Brave); parallelise within one bash call using `&` and `wait` only for independent searches, never `run_in_background`.
- Descriptive annotations only; significance is recorded as data in SIGNIFICANCE INDICATORS, not as adjectives.
- Include German/French/Italian works only under the international-impact rule; do not exclude Anglophone works that are less cited if they are the field's standard treatment of a subfield.
- Give equal effort to critical and dissenting scholarship; explicitly include works that criticise Kant or the dominant readings, and responses to those criticisms.

## Notes for the Orchestrator (decisions and cautions before running)

1. **Sequential order**: run Domain 1 to 6 in order, passing each researcher the exact output path (`reviews/kant-2010-2026/literature-domain-N.bib`), the block's year range, and instructions to read the previous block's .bib (keys and @comment) first.
2. **Per-entry count override**: the domain-researcher default says 10-20 papers; tell each researcher that this project needs 30-45 entries (Domain 6: 20-30).
3. **INCOMPLETE-entry rule**: the standard workflow excludes entries with no abstract from synthesis. For a "most significant works" list, many important books may lack abstracts. Consider allowing entries whose summaries are grounded in an NDPR review, SEP/IEP context, or a publisher description retrieved in the session, and decide before Phase 4 how INCOMPLETE entries are handled.
4. **Metadata provenance hook**: `metadata_validator.py` checks publisher/journal/volume/pages against JSON in `intermediate_files/json/`. Remind researchers to save all script outputs there and to save `verify_paper.py` outputs for books. If the hook rejects CrossRef REST responses saved via `curl`, researchers should re-run `verify_paper.py --doi` on each selected item to produce compliant JSON.
5. **Synthesis format**: Phase 4/5 should structure the review into 17 year sections (2010-2026) with about 10-20 entries each (fewer for 2026), each entry with a 1-3 sentence summary; entry order within a year can follow the subfield tags. Cross-references between years (for example "continues the debate of [year]") should be drawn from the `debate-*` tags and SUBFIELD AND DEBATE lines.
6. **Seed lists are unverified**: they come from the planner's memory (thin for 2019 onwards, none for 2025-2026) and may contain wrong years or publishers; they are search aids only.
