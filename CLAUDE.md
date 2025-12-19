# CLAUDE.md

> v0.3 | 2025-12-19
> Loader file for Claude Code. Points to authoritative documents.

---

## What This Repository Is

This is a **meta-workflow environment** for human-Claude collaboration. It defines protocols, documents, and structures that enable persistent, coherent work across Claude sessions.

**Current mode:** Meta-work — building the environment itself, not executing tasks within it.

### Two-Layer Architecture

| Layer | Purpose |
|-------|---------|
| **Layer 1** | Design-process infrastructure — protocols and documents used *while designing* |
| **Layer 2** | The designed product — the actual workflow that will live in Claude Code |

---

## Session Start

Auto-loaded documents:

- @CLAUDE-OPERATING.md — Claude's behavioral and cognitive protocols
- @STATE.md — Current operational truth
- @GLOSSARY.md — Shared terminology
- @KNOWLEDGE-GAPS.md — Research queue
- @PROTOCOL-SESSION.md — Session lifecycle (start, working, handoff)

**Never load at start:** ARCHIVE.md (retrieve only when needed)

After context loads, confirm state, surface open items, then ask: "Anything to correct or add before we proceed?"

---

## Document Authority

When conflicts arise: PRINCIPLES.md → CLAUDE-OPERATING.md → STATE.md → Latest handoff → Other documents

Conflicts get flagged immediately, not silently resolved.
