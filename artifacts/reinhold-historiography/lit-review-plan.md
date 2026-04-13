# Literature Review Plan: Reinhold's Historiography of Philosophy

## Research Idea Summary

Reconstruct Karl Leonhard Reinhold's theory of the history of philosophy across his career phases, survey scholarly work on Reinhold's historiography, and situate it within the development of post-Kantian conceptions of philosophical history culminating in Hegel.

## Key Research Questions

1. How did Reinhold conceive of philosophy's history, progress, and the *Streit der Systeme*?
2. How did his historiographical views evolve (Elementary Philosophy → Rationalism → philological turn)?
3. How does Reinhold's approach compare to and influence Fichte, Schelling, the Romantics, and Hegel?

## Literature Review Domains

### Domain 1: Reinhold's Primary Texts on History of Philosophy
**Focus**: Reinhold's own writings—*Beyträge*, *Briefe über die Kantische Philosophie*, *Versuch einer neuen Theorie*, later *Beyträge zur leichteren Übersicht*, Bardili/Rationalism essays, philological-period works.
**Key Questions**: What does Reinhold say about philosophical progress, systemic strife, and method in history? How do his historiographical claims shift?
**Search Strategy**: `search_sep.py` (Reinhold); `search_philpapers.py` "Reinhold history philosophy"; `s2_search.py` terms: "Reinhold Beyträge", "Reinhold Elementarphilosophie history", "Reinhold Bardili", "Reinhold philological"; check Cambridge/SUNY translations.
**Relevance**: Foundation for (1).

---

### Domain 2: Scholarship on Reinhold's Historiography and Development
**Focus**: Secondary literature on Reinhold's conception of history of philosophy and his intellectual trajectory (Bondeli, Fabbianelli, di Giovanni, Ameriks, Frank, Breazeale, Onnasch, Stamm).
**Key Questions**: How do scholars interpret Reinhold's narrative of philosophical progress and *Streit*? How is his development periodized?
**Search Strategy**: `s2_search.py`/`search_openalex.py`: "Reinhold Elementarphilosophie", "Reinhold Streit der Systeme", "Reinhold rational realism", "Reinhold Bardili"; NDPR reviews of Ameriks *Kant and the Historical Turn*, Bondeli volumes; PhilPapers category "Karl Leonhard Reinhold".
**Relevance**: Core of (2).

---

### Domain 3: Post-Kantian Historiography — Fichte, Schelling, Romantics
**Focus**: How Fichte (*Vocation of Man*, Jena lectures), Schelling (*Vorlesungen über die Methode*, identity-philosophy histories), and early Romantics (F. Schlegel, Novalis, Schleiermacher) conceived philosophy's history after Kant.
**Key Questions**: What models of philosophical progress, system, and historical narrative emerge? How do they respond to or diverge from Reinhold?
**Search Strategy**: `search_sep.py` (Fichte, Schelling, Schlegel, German Romanticism); `s2_search.py`: "Fichte history of philosophy", "Schelling historiography", "Schlegel philosophy history", "post-Kantian historiography"; Beiser, Frank, Förster, Millán-Zaibert.
**Relevance**: Core of (3).

---

### Domain 4: Hegel's Historiography and Its Genesis
**Focus**: Hegel's *Lectures on the History of Philosophy*, its development, and its debts to Reinhold and post-Kantian predecessors.
**Key Questions**: How does Hegel's conception of philosophical history synthesize or supersede Reinhold-era approaches? What is the lineage from *Streit der Systeme* to Hegelian dialectical history?
**Search Strategy**: `search_sep.py` (Hegel); `s2_search.py`: "Hegel history of philosophy lectures", "Hegel Reinhold", "Hegel post-Kantian historiography"; Forster, Düsing, Houlgate, Pinkard.
**Relevance**: Terminus of (3); comparative anchor for (1)–(2).

---

### Domain 5: Context — Kant, Eclecticism, and 18th-c. Historia Philosophica
**Focus**: Kant on history of philosophy (*What Real Progress*), Brucker, Tiedemann, Tennemann, Meiners, Garve; the German *Historia Philosophica* tradition Reinhold inherited and transformed.
**Key Questions**: What historiographical resources did Reinhold draw on? How did Kantian/critical historiography reshape the genre?
**Search Strategy**: `s2_search.py`: "Brucker historia philosophica", "Tennemann Kantian history philosophy", "Kant Fortschritte Metaphysik", "18th century historiography philosophy"; Ameriks, Micheli, Catana, Piaia/Santinello volumes.
**Relevance**: Background essential for situating Reinhold and the post-Kantian turn.

---

## Coverage Rationale

Domains 1–2 address aims (1)–(2) directly; Domains 3–4 cover aim (3); Domain 5 supplies indispensable pre-Reinhold context. Sequential execution favors this compact structure.

## Expected Gaps

Reinhold's philological-period historiography and his mediating role between *Historia Philosophica* and Hegel are under-studied.

## Estimated Scope

- **Total domains**: 5
- **Estimated papers**: 50–70
- **Key positions**: critical/Kantian historiography; Reinholdian progress via *Streit*; Fichtean/Schellingian system-histories; Hegelian dialectical history; eclectic *Historia Philosophica*.

## Search Priorities

1. Reinhold primary texts + Ameriks, Bondeli, di Giovanni (foundational).
2. Recent scholarship (last 10 years) via `--recent` flag on `s2_search.py`.
3. Critical/revisionist readings and German-language sources (Onnasch, Stamm, Fabbianelli).

## Notes for Researchers

Use `philosophy-research` skill scripts extensively. Start with `search_sep.py` for Reinhold, Fichte, Schelling, Hegel, German Romanticism. Use `search_philpapers.py` and `s2_search.py` with German terms (*Streit der Systeme*, *Elementarphilosophie*, *Historia Philosophica*). Include NDPR reviews. Prioritize verified citations—many older German works need CrossRef/OpenAlex confirmation. Ensure balanced coverage including critics of Reinhold's historiographical claims.
