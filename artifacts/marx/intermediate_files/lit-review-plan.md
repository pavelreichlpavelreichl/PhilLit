# Literature Review Plan: Marx Scholarship Since 1990

## Research Idea Summary

A chronological overview (by decade: 1990s, 2000s, 2010s, 2020s; then by year) of English-language peer-reviewed articles and scholarly monographs published since 1990 in which Marx appears in the title and/or Marx's own work is the main topic. Because the final review is chronological, not thematic, the domains below are SEARCH PARTITIONS (by area of Marx scholarship, each swept across the whole 1990-2026 period), plus a final title-based decade sweep to close coverage gaps.

## Key Research Questions

1. Which articles and books since 1990 take Marx (his texts, concepts, or legacy) as their main subject?
2. How is this literature distributed across years, so each year can receive a short entry?
3. Which works are landmarks in each decade (e.g., post-1989 "Marx after communism" literature, the 2008 crisis revival, the 2018 bicentenary)?

## Inclusion / Exclusion Criteria (apply in every domain)

- Include: peer-reviewed journal articles, scholarly monographs, edited volumes (chapters only if Marx is the chapter's main topic), in English, 1990 to present (2026), where "Marx" (or Marx's Capital, Grundrisse, Manuscripts, etc.) is in the title or is clearly the primary subject.
- Exclude: works that only mention Marx in passing, general Marxist theory not centered on Marx's own work (unless the title names Marx), textbooks and encyclopedia entries (use SEP/IEP for orientation only), popular journalism, and works about later figures (Lenin, Gramsci, Althusser) unless Marx is the main topic.
- Record for each item: author, year, title, venue, a one-to-two sentence description of the main topic and thesis (needed for the short per-item overviews). Year accuracy is essential, since output is ordered by year.
- Assignment rule for overlaps: assign each work to the domain of its primary topic; if found in another domain, still record it (deduplication happens in Phase 6).

## Literature Review Domains

### Domain 1: Marx's Philosophy and Its Interpretation (Anthropology, Alienation, Ideology, Dialectic, Ethics and Justice)

**Focus**: Marx as a philosopher: early writings and human nature, alienation and species-being, freedom, ideology and fetishism as philosophical concepts, dialectic and the Hegel-Marx relation, materialism, and the moral/normative debate (Marx and justice, exploitation, ethics), including analytical Marxism's aftermath.

**Key Questions**:
- How have interpretations of Marx's philosophical anthropology and theory of alienation developed since 1990?
- Did Marx have a theory of justice or a moral critique of capitalism (the Wood/Cohen/Geras line and later responses)?
- How is the Hegel-Marx relation and the status of dialectic treated?

**Search Strategy**:
- Primary sources: SEP (Karl Marx; Marxism; Alienation; Analytical Marxism; Marx's Theory of Ideology, Exploitation), then PhilPapers categories on Marx.
- Skill scripts: `search_sep.py`, `search_philpapers.py`, `s2_search.py`, `search_openalex.py`.
- Key terms: "Marx alienation", "Marx human nature", "Marx and justice", "Marx morality", "Marx freedom", "Marx Hegel dialectic", "Marx ideology fetishism", "Marx exploitation", "young Marx", "Economic and Philosophic Manuscripts", "Marx humanism".
- Expected items: 40-60 (journals: Philosophy & Public Affairs, Ethics, Historical Materialism, Science & Society, Radical Philosophy, Inquiry, Rethinking Marxism, European Journal of Philosophy, Journal of the History of Philosophy; presses: Cambridge, Oxford, Brill, Verso, Palgrave).

**Relevance to Project**: Core of "Marx as philosopher"; yields many titled-Marx items across all decades.

---

### Domain 2: Capital, Value Theory and Marx's Political Economy

**Focus**: Marx's economic theory: labor theory of value, money, abstract labor, the transformation problem (TSSI, Okishio, and other debates), the falling rate of profit and crisis theory, the "new dialectic"/systematic dialectic reading of Capital, the "new reading of Marx" (Neue Marx-Lektüre), Grundrisse, reproduction schemes, and Marx's economics after the 2008 crisis.

**Key Questions**:
- How have value theory and the transformation problem debates evolved since 1990?
- How is Capital read methodologically (Hegelian logic, systematic dialectics, Marx's method)?
- What Marx-titled work on crisis, finance and rent appeared after 2008?

**Search Strategy**:
- Primary sources: SEP (Marxism; Marx), OpenAlex/Semantic Scholar for economics journals, PhilPapers (Marx: economics).
- Key terms: "Marx's Capital", "Marx value theory", "Marx labour theory of value", "transformation problem Marx", "Marx crisis theory", "Marx falling rate of profit", "Marx money", "Marx Grundrisse", "Marx method Capital", "new dialectic Marx", "Marx abstract labour", "Marx fictitious capital".
- Expected items: 50-70 (journals: Cambridge Journal of Economics, Review of Radical Political Economics, Capital & Class, Historical Materialism, Science & Society, Review of Political Economy, Journal of Economic Perspectives; monographs from Brill's Historical Materialism series, Palgrave, Routledge, Cambridge).

**Relevance to Project**: The largest single body of Marx-centered work; needed for year-by-year coverage, especially 2008 onward and Capital's 150th anniversary (2017).

---

### Domain 3: Historical Materialism, Politics, Class, State and Marx's Historical Writings

**Focus**: Theory of history and historical materialism (Cohen's Karl Marx's Theory of History and its critics), class, state, democracy, revolution, communism, and Marx's political/journalistic writings (Eighteenth Brumaire, Civil War in France, Critique of the Gotha Programme, Jewish Question, writings on Paris Commune); Marx's relation to liberalism, republicanism, and rights; post-1989 "Marx after communism" literature.

**Key Questions**:
- How was historical materialism defended, reconstructed or rejected after 1990?
- What has been said about Marx's politics: democracy, state, revolution, the transition to communism?
- How did the fall of the Soviet bloc shape Marx's reception in the 1990s?

**Search Strategy**:
- Primary sources: SEP (Marx; Historical Materialism; Marxist Political Philosophy), PhilPapers, JSTOR-indexed via OpenAlex.
- Key terms: "Marx theory of history", "historical materialism Marx", "Marx state", "Marx democracy", "Marx communism", "Marx Eighteenth Brumaire", "Marx Paris Commune", "Marx class", "Marx political thought", "Marx rights liberalism", "Marx after communism", "Marx and republicanism".
- Expected items: 35-50.

**Relevance to Project**: Covers the political and historical Marx and the 1990s post-Soviet reassessment, a key opening period of the chronological review.

---

### Domain 4: Marx and Contemporary Topics (Ecology, Gender and Social Reproduction, Race and Colonialism, Non-Western Societies, Technology and Digital Capitalism)

**Focus**: Works with Marx in the title or as main subject applying or re-examining Marx on: ecology and metabolic rift (Foster, Burkett, Saito's "Karl Marx's Ecosocialism"), degrowth; feminism/social reproduction; race, slavery, colonialism, India/China/Ireland writings, Eurocentrism (Anderson's "Marx at the Margins"); technology, machinery, automation, AI, platform/digital labor, "Marx and the general intellect".

**Key Questions**:
- What did Marx actually say on nature, gender, race, colonialism and technology, according to this literature?
- How did these subfields emerge or grow across decades (ecology from the 1990s; colonialism and technology mainly 2010s-2020s)?
- What critical positions exist (e.g., Marx as Promethean or Eurocentric)?

**Search Strategy**:
- Primary sources: SEP (Marx; Feminist Perspectives; Environmental Ethics), PhilPapers, `s2_search.py --recent` for 2020-2026, `search_openalex.py`.
- Key terms: "Marx ecology", "Marx metabolic rift", "Marx and nature", "Marx ecosocialism", "Marx feminism", "Marx social reproduction", "Marx race slavery", "Marx colonialism", "Marx Eurocentrism", "Marx non-Western", "Marx technology machinery", "Marx automation", "Marx digital labour", "Marx artificial intelligence", "Marx degrowth".
- Expected items: 40-60. Balance the four subareas (do not let ecology crowd out others).

**Relevance to Project**: Supplies the bulk of 2010s-2020s entries and shows the expansion of Marx scholarship.

---

### Domain 5: Intellectual History, Biography, Textual Scholarship and Marx in Dialogue with Other Thinkers

**Focus**: Biographies (Sperber, Stedman Jones, Musto, Wheen and others), the MEGA edition and philology, Marx-Engels relationship, Marx's sources and reading (Aristotle, Epicurus, Spinoza, Hegel, Smith and Ricardo, Darwin, ethnological notebooks), Marx's reception and comparison with other thinkers (Marx and Nietzsche, Weber, Durkheim, Foucault, Derrida's Specters of Marx, Heidegger, Keynes, Arendt), and anniversary volumes (Manifesto 150th in 1998, Capital 150th in 2017, bicentenary in 2018, Marx-Engels-related retrospectives).

**Key Questions**:
- How has the picture of Marx's life, texts and sources changed with new archives and MEGA?
- Which comparative "Marx and X" studies define the field?
- What are the notable retrospectives and anniversary-driven publications?

**Search Strategy**:
- Primary sources: PhilPapers, NDPR (`search_ndpr.py`) for book reviews to locate monographs, SEP, Semantic Scholar, OpenAlex.
- Key terms: "Marx biography", "Karl Marx: A Nineteenth-Century Life", "Karl Marx: Greatness and Illusion", "MEGA Marx Engels", "Marx Engels relationship", "Marx Aristotle", "Marx Spinoza", "Marx Epicurus", "Marx Nietzsche", "Marx Weber", "Specters of Marx", "Communist Manifesto anniversary", "Marx bicentenary", "Marx Darwin", "Marx ethnological notebooks".
- Expected items: 30-45.

**Relevance to Project**: Captures monographs and landmarks (e.g., Derrida 1993/94, Sperber 2013, Stedman Jones 2016) that anchor specific years.

---

### Domain 6: Chronological Gap-Fill Sweep (Title-Based, by Decade) and Critical/Skeptical Literature

**Focus**: A systematic sweep by period (1990-1999, 2000-2009, 2010-2019, 2020-2026) for items with "Marx"/"Marx's"/"Marxian" in the title, restricted by year filters, to catch works missed by topical domains (e.g., Marx and religion, Marx and law, Marx and education, Marx and aesthetics/literature, Marx and psychology, Marx and India/Asia, Marx and anthropology, Marx and sociology). Also targeted search for critics and skeptics: "Marx refuted/critique/obsolete", "Marx's errors", Popperian, Austrian, and liberal critiques of Marx's economics, totalitarianism debates, and "failure of Marx" literature.

**Key Questions**:
- Which titled-Marx works are not captured by Domains 1-5, and how are they distributed per year?
- What are the main critiques of Marx published since 1990 and how were they answered?
- Are any years or decades thin due to search bias, and how can they be filled (especially 2024-2026)?

**Search Strategy**:
- Primary sources: OpenAlex and Semantic Scholar with year-range and title filters (run each decade separately, then by year in thin years), CORE, Crossref via verification scripts; `--recent` for 2023-2026.
- Key terms: "Marx" in title with "religion", "law", "education", "aesthetics", "literature", "psychology", "anthropology", "sociology", "Marx critique", "against Marx", "Marx obsolete", "Marx relevance", "Marx today", "reading Marx", "rereading Marx".
- Expected items: 30-50, plus a per-year count table showing coverage. Researcher should flag years with fewer than 3 entries and run supplementary searches.

**Relevance to Project**: Ensures the chronological review has no gaps by year and includes non-confirmatory and critical works.

---

## Coverage Rationale

Domains 1-5 partition Marx scholarship by subject (philosophy, economics, history/politics, contemporary applications, intellectual history/textual work), which minimizes overlap and mirrors how databases index the field. Domain 6 is orthogonal (time-based and title-based), directly serving the final chronological structure and compensating for topical searches that skew toward well-known themes. Six domains is within the requested 4-6 range; each is sized to about 30-70 items for one researcher.

## Expected Gaps

- Scholarship that treats Marx via Marxist tradition (Frankfurt School, Althusser, autonomism) without naming Marx in the title will be excluded by design.
- Non-English scholarship (German Neue Marx-Lektüre, MEGA philology, French, Chinese, Japanese) enters only via English translations; note this limitation in the review.
- Sociological and economics journals may be under-indexed in philosophy sources; use OpenAlex and Semantic Scholar.
- Very recent (2025-2026) items are likely under-indexed; verify dates carefully.

## Estimated Scope

- **Total domains**: 6
- **Estimated papers**: 200-300 raw, roughly 150-250 after deduplication and exclusion (larger than the default 40-80 because the chronological-catalogue format requires broad coverage; the synthesis phase should be told this)
- **Key positions/debates to be represented**: analytical Marxism and the justice debate; value-form/new dialectic vs. TSSI vs. traditional value theory; historical materialism reconstruction vs. critique; ecological Marx (metabolic rift) vs. Promethean Marx; Eurocentric vs. late-Marx multilinear reading; post-1989 "end of Marx" vs. revival after 2008.

## Search Priorities

1. Landmark and highly cited works per decade (use citation counts to rank within each year).
2. Recent developments 2020-2026 (`--recent`), especially ecology, technology/AI, and post-bicentenary work.
3. Critical responses and works skeptical of Marx (Domain 6), so the survey is not merely sympathetic.
4. Balanced distribution across years; record year counts per domain.

## Notes for Researchers

- Use the `philosophy-research` skill scripts for all searches; verify every entry (title, author, year, venue) via Crossref or another source before including it in the BibTeX. Never fabricate or infer years.
- Publication year matters for ordering: use the version-of-record year and note reprint or translation dates in the annotation only where relevant.
- Each BibTeX annotation should state the item's main topic in one to two sentences suitable for a short chronological entry, and note Marx-centrality (title or main topic).
- Exclude passing-mention works; when unsure, include only if Marx's own texts or thought are the primary subject.
- Since researchers run sequentially, later researchers (especially Domain 6) should consult earlier BibTeX files to avoid duplicates and to target thin years.
- Prioritize SEP/IEP only for orientation and identification of literature, not as items for the final review.
