# State

> v0.4 | 2025-12-19
> Current operational truth. Layer 1 document.

---

## Current Phase

Iterating on Layer 1 infrastructure.

**Active focus:** Deduplication and consolidation of Layer 1 documents

**Next anticipated focus:** Continue Layer 1 refinement or begin Layer 2 design

---

## Document Inventory

| Document | Status | Layer | Last Updated | Notes |
|----------|--------|-------|--------------|-------|
| CLAUDE.md | v0.2 | 1 | 2025-12-19 | Lean loader file; points to other documents |
| PROTOCOL-SESSION.md | v0.4 | 1 | 2025-06-19 | Session lifecycle (start, working, handoff) |
| CLAUDE-OPERATING.md | v0.1 | 1 | 2025-06-19 | Claude's cognitive and behavioral protocols |
| STATE.md | v0.4 | 1 | 2025-12-19 | This document |
| GLOSSARY.md | v0.2 | 1 | 2025-12-19 | Quick-reference terminology |
| KNOWLEDGE-GAPS.md | v0.1 | 1 | 2025-06-19 | Research queue |
| ARCHIVE.md | v0.1 | 1 | 2025-06-19 | Cold storage; updated at session end only |
| PRINCIPLES.md | Not started | 2 | — | Foundation for Layer 2; highest authority |
| MODES.md | Not started | 2 | — | Operating modes for Claude Code workflow |

---

## Active Decisions

| ID | Decision | Date | Context |
|----|----------|------|---------|
| D001 | This is meta-work; we build the environment, not execute within it | 2025-06-19 | Fundamental distinction governing all current activity |
| D002 | Decision authority model: Flag and wait | 2025-06-19 | Claude recommends with confidence level; Human decides |
| D003 | ARCHIVE.md updated at session end only, never loaded at start | 2025-06-19 | Prevents context pollution |
| D004 | STATE.md stays lean—only active, relevant items | 2025-06-19 | Superseded items transition to ARCHIVE |
| D005 | Date format: YYYY-MM-DD | 2025-06-19 | Consistency across all documents |
| D006 | Confirmation required before capturing to persistent documents | 2025-06-19 | Prevents misrepresentation of intent |
| D007 | GLOSSARY.md loaded at every session start | 2025-06-19 | Prevents terminology drift across sessions |
| D008 | CLAUDE.md is a lean loader; authoritative content lives in source documents | 2025-12-19 | Prevents duplication; CLAUDE-OPERATING.md and PROTOCOL-SESSION.md hold details |
| D009 | GLOSSARY.md is quick-reference only; points to source documents | 2025-12-19 | Prevents maintenance burden of duplicated definitions |
| D010 | Documents contain their own version marker in header | 2025-12-19 | Version truth lives in document itself, not just STATE.md inventory |

---

## Open Items

| ID | Item | Urgency | Waiting On | Notes |
|----|------|---------|------------|-------|
| O001 | Begin Layer 2 design work | Medium | Layer 1 refinement | After Layer 1 is stable |

---

## Active Insights

| ID | Insight | Date | Implications |
|----|---------|------|--------------|
| I001 | Confidence level signaling improves recommendation quality | 2025-06-19 | Embedded in CLAUDE-OPERATING.md as standard practice |
| I002 | Curated persistence > exhaustive persistence | 2025-06-19 | Core tension; shapes all capture decisions |
| I003 | Small game-changing details can outweigh lengthy exposition | 2025-06-19 | Active extraction required during sessions |
| I004 | Layer 1 vs Layer 2 require explicit ongoing distinction; blur easily | 2025-06-19 | Must verify which layer we're operating on |
| I005 | Glossary prevents conceptual blur; defined terms persist across sessions | 2025-06-19 | Led to GLOSSARY.md creation |
| I006 | Document duplication creates maintenance burden and context waste | 2025-12-19 | Led to D008, D009 — single source of truth principle |

---

## Integrity Notes

- O002 (ROLES.md needed?) resolved: No. Roles defined in CLAUDE-OPERATING.md.
