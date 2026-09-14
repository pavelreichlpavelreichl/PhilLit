# Literature Review Progress Tracker

**Research Topic**: Historical materialism in Marx and, especially, after Marx — reception, interpretation, criticism, and defense
**Started**: 2026-09-11
**Last Updated**: 2026-09-14

## Progress Status

- [x] Phase 1: Verify environment and determine execution mode
- [x] Phase 2: Structure literature review domains
- [x] Phase 3: Research domains sequentially (11 domains, one at a time per user request)
- [x] Phase 4: Outline synthesis review across domains
- [x] Phase 5: Write review for each section (run sequentially per user request)
- [x] Phase 6: Assemble final review files and move intermediate files

## WORKFLOW COMPLETE

## Completed Tasks

[2026-09-11] Phase 1: Environment check ran with transient 429 rate-limit responses on Semantic Scholar/OpenAlex/CORE across repeated checks (all required env vars set; CrossRef, Brave, arXiv consistently reachable). Treated as transient rate limiting, not misconfiguration; proceeding with graceful per-source degradation as already designed into domain-literature-researcher agents.

[2026-09-11] Phase 2: literature-review-planner produced an 11-domain plan (lit-review-plan.md) covering Marx's own texts plus post-Marx reception: Engels/Second International orthodoxy, Western Marxism, Frankfurt School, structural Marxism, analytical Marxism (special emphasis), Political Marxism (special emphasis), external critiques, feminist historical materialism (special emphasis), world-systems/dependency theory (special emphasis), contemporary/ecological revivals.

[2026-09-11 to 2026-09-12] Phase 3: All 11 domains researched sequentially, one domain-literature-researcher agent at a time (per user request to avoid hitting limits). Two container restarts occurred mid-phase (during Domain 10 and Domain 11); in both cases the agent's .bib output had already finished writing to disk before the restart, verified by brace-balance and proper-termination checks, so no re-run was needed. Paper counts: D1=17, D2=16, D3=16, D4=18, D5=18, D6=22 (special emphasis), D7=17 (special emphasis), D8=17, D9=15 (special emphasis), D10=16 (special emphasis), D11=14. Total ~206 raw entries before Phase 6 deduplication. All files validated for brace balance; several agents caught and corrected mismatched/false-positive abstract enrichments (documented in each file's NOTABLE_GAPS section) rather than propagate incorrect data.

[2026-09-12] Phase 4: synthesis-planner produced synthesis-outline.md: Introduction + 8 sections (16 subsections) + Conclusion, organized dialectically (not domain-by-domain) tracing the theory's career from orthodoxy through humanist/structuralist/analytical/class-relational revisions, external critique, and extensions (feminist/world-systems/ecological) to contemporary defenses. ~110-115 distinct papers cited, ~85% of space to post-Marx material, target length ~6000-6500 words. Includes explicit redundancy-avoidance coordination notes for the Phase 5 writers (6 specific overlap points flagged).

[2026-09-12] Phase 5: All 10 sections written sequentially, one synthesis-writer agent at a time (Introduction, Sections 1-8, Conclusion). Word counts: Intro 525, S1 676, S2 1283, S3 658, S4 1086, S5 685, S6 993, S7 1098, S8 447, Conclusion 563 (~8000 words total). Writers consistently applied citation-integrity discipline: several INCOMPLETE/no-abstract .bib entries were either dropped or cited cautiously via note-field content only, never fabricated or quoted without verification. Coordination notes from the outline (avoiding redundant treatment of Brenner/neo-Smithian-Marxism, Habermas/post-Marxism, Chibber 2011, Poulantzas-Gramsci convergence, duplicate Wood/Ruben citations) were followed by each writer.

[2026-09-12 to 2026-09-14] Phase 6: Assembled 10 sections into literature-review-final.md with YAML frontmatter (assemble_review.py); normalized 15 headings (normalize_headings.py); deduplicated 11 domain .bib files into literature-all.bib (dedupe_bib.py caught 2 exact-key duplicates: ruben1981cohen, chibber2011living); generated References via generate_bibliography.py (131 entries matched).

Manual accuracy fixes beyond the automated pipeline (documented per project's accuracy-first priority):
- Caught a duplicate the automated dedupe could not catch: Wood's "Rational Choice Marxism" essay existed as two BibTeX entries (`wood1989rational`, the sparse original 1989 New Left Review printing; `woodellen1995rational`, the fuller 1995 book-reprint with verified abstract/DOI) under different keys with no shared DOI to key off. The outline had already flagged this as one essay to cite once. Merged the 1989 entry's SEP-context note into the surviving 1995 entry and removed the sparse duplicate from literature-all.bib.
- Caught a bibliography-generation false-positive: generate_bibliography.py's surname+year proximity matching pulled in two entries (`cohen1986walt`, `walt1986historical` — the 1986 Cohen-Walt Ethics exchange) that are never actually cited anywhere in the review's text (verified by grepping all synthesis-section-*.md for "Walt" and "Cohen 1986" — zero hits). Manually removed both from the rendered References section in literature-review-final.md to keep the bibliography limited to what is actually cited, per the project's accuracy priority. (Left them in literature-all.bib itself, since that file is the full aggregated research corpus, not a citations-only list.)
- Re-validated brace balance and lint_md.py (exit 0) after each manual edit.

Cleanup: moved all intermediate files (task-progress.md, lit-review-plan.md, synthesis-outline.md, synthesis-section-*.md, literature-domain-*.bib, stray JSON) into reviews/historical-materialism/intermediate_files/; removed reviews/.active-review pointer. Pandoc not installed in this environment, so DOCX conversion was skipped (final deliverable is literature-review-final.md + literature-all.bib).

Final review: ~10,085 words, 131 cited references, 11 research domains.

## Current Task

All 6 phases complete. Final literature-review-final.md and literature-all.bib copied to artifacts/historical-materialism/ and committed/pushed.

## Next Steps

None — workflow complete. reviews/historical-materialism/ retains the full local working copy (plan, outline, domain bibs, section drafts, intermediate JSON) as scratch/local-only per user instruction; artifacts/historical-materialism/ holds the git-tracked deliverables from every phase.

## Notes on deviations from default workflow (per user instruction)

- Working/scratch directory remains `reviews/historical-materialism/` (gitignored, local only), matching the skill's internal resume/active-review logic.
- Final AND intermediate deliverables are additionally copied to `artifacts/historical-materialism/` (git-tracked) at the end of every phase, followed by `git add`, `git commit`, `git push`.
- Phase 3 (domain research) and Phase 5 (section writing) are run sequentially (one subagent at a time) rather than in parallel, per explicit user request to avoid hitting rate/usage limits.
