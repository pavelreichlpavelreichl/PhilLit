# Literature Review Progress Tracker

**Research Topic**: Scholarship on Marx since 1990 (articles/books with Marx in the title or his work as main topic), presented chronologically by decade and year
**Started**: 2026-09-30
**Last Updated**: 2026-09-30
**Execution mode**: Full Autopilot, all agents run sequentially
**Output location**: artifacts/marx/ (reviews/ is scratch only); commit + push after each phase to claude/youthful-sagan-6usrl0

## Progress Status

- [x] Phase 1: Verify environment and determine execution mode
- [x] Phase 2: Structure literature review domains
- [x] Phase 3: Research 6 domains (sequentially)
- [x] Phase 4: Outline synthesis review (chronological by decade/year)
- [x] Phase 5: Write review sections (sequentially)
- [ ] Phase 6: Assemble final review files and move intermediate files

## Completed Tasks

2026-09-30 Phase 1: environment check. OpenAlex returned HTTP 429 on 3 consecutive checks; all other sources OK. User approved proceeding.

2026-09-30 Phase 2: created lit-review-plan.md (6 domains; search partitions, not thematic sections)

2026-09-30 Phase 3: 6 domain files, 447 entries (D1 59, D2 96, D3 75, D4 69, D5 46, D6 102); every year 1990-2026 has >=10 combined. Source issues: OpenAlex 429 for search (used only in enrichment); discovery mainly Semantic Scholar + CrossRef verification; SEP/IEP/PhilPapers/Brave/CORE mostly unused; ~100 entries INCOMPLETE (no abstract, title-based notes); 8 DOI-less books flagged unverified-crossref in D5.

2026-09-30 Phase 4: synthesis-outline.md + section-keys.md (12 writer chunks + Introduction + Conclusion). Orchestrator script-verified the key assignment (all years match) and removed 1 duplicate (wendling2009technology in d4); total now 446 entries.

2026-09-30 Phase 5: synthesis-section-1..14.md written sequentially (Introduction, 12 chronological chunks, Conclusion); 446 item lines verified against key lists; no dashes.

## Current Task

Phase 6: assemble into artifacts/marx/

## Next Steps

1. Fix data issues (McNeill 2021 misattached abstract; cheng2026state author order), then assemble, dedupe bib, generate bibliography, lint, output to artifacts/marx/
