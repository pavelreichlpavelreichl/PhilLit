# Literature Review Progress Tracker

**Research Topic**: Historical materialism in Marx and, especially, after Marx — reception, interpretation, criticism, and defense
**Started**: 2026-09-11
**Last Updated**: 2026-09-12

## Progress Status

- [x] Phase 1: Verify environment and determine execution mode
- [x] Phase 2: Structure literature review domains
- [x] Phase 3: Research domains sequentially (11 domains, one at a time per user request)
- [x] Phase 4: Outline synthesis review across domains
- [x] Phase 5: Write review for each section (run sequentially per user request)
- [ ] Phase 6: Assemble final review files and move intermediate files

## Completed Tasks

[2026-09-11] Phase 1: Environment check ran with transient 429 rate-limit responses on Semantic Scholar/OpenAlex/CORE across repeated checks (all required env vars set; CrossRef, Brave, arXiv consistently reachable). Treated as transient rate limiting, not misconfiguration; proceeding with graceful per-source degradation as already designed into domain-literature-researcher agents.

[2026-09-11] Phase 2: literature-review-planner produced an 11-domain plan (lit-review-plan.md) covering Marx's own texts plus post-Marx reception: Engels/Second International orthodoxy, Western Marxism, Frankfurt School, structural Marxism, analytical Marxism (special emphasis), Political Marxism (special emphasis), external critiques, feminist historical materialism (special emphasis), world-systems/dependency theory (special emphasis), contemporary/ecological revivals.

[2026-09-11 to 2026-09-12] Phase 3: All 11 domains researched sequentially, one domain-literature-researcher agent at a time (per user request to avoid hitting limits). Two container restarts occurred mid-phase (during Domain 10 and Domain 11); in both cases the agent's .bib output had already finished writing to disk before the restart, verified by brace-balance and proper-termination checks, so no re-run was needed. Paper counts: D1=17, D2=16, D3=16, D4=18, D5=18, D6=22 (special emphasis), D7=17 (special emphasis), D8=17, D9=15 (special emphasis), D10=16 (special emphasis), D11=14. Total ~206 raw entries before Phase 6 deduplication. All files validated for brace balance; several agents caught and corrected mismatched/false-positive abstract enrichments (documented in each file's NOTABLE_GAPS section) rather than propagate incorrect data.

[2026-09-12] Phase 4: synthesis-planner produced synthesis-outline.md: Introduction + 8 sections (16 subsections) + Conclusion, organized dialectically (not domain-by-domain) tracing the theory's career from orthodoxy through humanist/structuralist/analytical/class-relational revisions, external critique, and extensions (feminist/world-systems/ecological) to contemporary defenses. ~110-115 distinct papers cited, ~85% of space to post-Marx material, target length ~6000-6500 words. Includes explicit redundancy-avoidance coordination notes for the Phase 5 writers (6 specific overlap points flagged).

[2026-09-12] Phase 5: All 10 sections written sequentially, one synthesis-writer agent at a time (Introduction, Sections 1-8, Conclusion). Word counts: Intro 525, S1 676, S2 1283, S3 658, S4 1086, S5 685, S6 993, S7 1098, S8 447, Conclusion 563 (~8000 words total). Writers consistently applied citation-integrity discipline: several INCOMPLETE/no-abstract .bib entries were either dropped or cited cautiously via note-field content only, never fabricated or quoted without verification. Coordination notes from the outline (avoiding redundant treatment of Brenner/neo-Smithian-Marxism, Habermas/post-Marxism, Chibber 2011, Poulantzas-Gramsci convergence, duplicate Wood/Ruben citations) were followed by each writer.

## Current Task

Phase 5 complete and committed. Starting Phase 6: assembly, dedup, bibliography, lint, cleanup.

## Next Steps

1. Run assemble_review.py to combine sections with YAML frontmatter.
2. Run normalize_headings.py.
3. Run dedupe_bib.py across all 11 domain .bib files -> literature-all.bib.
4. Run generate_bibliography.py to append References section.
5. Run lint_md.py and fix any issues.
6. Clean up intermediate files in reviews/historical-materialism/.
7. Copy final literature-review-final.md (+.docx if available) and literature-all.bib to artifacts/historical-materialism/, commit, push.

## Notes on deviations from default workflow (per user instruction)

- Working/scratch directory remains `reviews/historical-materialism/` (gitignored, local only), matching the skill's internal resume/active-review logic.
- Final AND intermediate deliverables are additionally copied to `artifacts/historical-materialism/` (git-tracked) at the end of every phase, followed by `git add`, `git commit`, `git push`.
- Phase 3 (domain research) and Phase 5 (section writing) are run sequentially (one subagent at a time) rather than in parallel, per explicit user request to avoid hitting rate/usage limits.
