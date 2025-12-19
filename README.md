# Symbiotic Collaboration Workflow

A structured methodology for human-AI collaboration sessions using Claude Code.

## Purpose

This repository provides a complete workflow system for maintaining continuity, capturing decisions, and enabling productive collaboration between a human and Claude across multiple sessions.

**Core tension addressed:** Persistence requires documentation, but documentation without judgment creates pollution. This workflow enables *curated persistence* — capturing what matters, discarding what doesn't, archiving what might.

## Quick Start

### Starting a Session

Use the `/bootstrap` command to load context and confirm current state:

```
/bootstrap
```

This loads core documents and provides:
- Current phase and focus summary
- Active decisions
- Open items
- Knowledge gaps

### During a Session

- Work proceeds in one of five **modes**: Planning, Execution, Research, Review, Handoff
- Decisions are confirmed before capture: "Capturing this as [X]. Correct?"
- Use signal words: `DECISION`, `OPEN`, `PARKED`, `DRAFT`, `GAP`, `ASSUMED`, `INSIGHT`
- Use `/status` for quick orientation
- Use `/log-decision` or `/log-gap` to capture items

### Ending a Session

Use the `/handoff` command to properly close the session:

```
/handoff
```

This generates a session summary, updates STATE.md, and transitions items to ARCHIVE.md.

## Document Structure

### Core Documents (Load at Session Start)

| Document | Purpose |
|----------|---------|
| `PRINCIPLES.md` | Foundational truths; highest authority |
| `CLAUDE-OPERATING.md` | Claude's behavioral protocols |
| `STATE.md` | Current operational truth |
| `GLOSSARY.md` | Shared terminology |
| `MODES.md` | Operating modes |

### Supporting Documents

| Document | Purpose |
|----------|---------|
| `PROTOCOL-SESSION.md` | Session lifecycle procedures |
| `KNOWLEDGE-GAPS.md` | Research queue and assumptions |
| `ARCHIVE.md` | Cold storage (load only when needed) |

### Claude Code Configuration

| File | Command |
|------|---------|
| `.claude/commands/bootstrap.md` | `/bootstrap` |
| `.claude/commands/handoff.md` | `/handoff` |
| `.claude/commands/status.md` | `/status` |
| `.claude/commands/log-decision.md` | `/log-decision` |
| `.claude/commands/log-gap.md` | `/log-gap` |

## Authority Hierarchy

When conflicts arise between documents:

1. **PRINCIPLES.md** — Highest authority
2. **CLAUDE-OPERATING.md** — Behavioral protocols
3. **STATE.md** — Current operational truth
4. **Latest session handoff** — Provisional until STATE.md updated
5. **Other documents** — Subordinate

**Rule:** Conflicts are flagged immediately, not silently resolved.

## Key Concepts

- **Layer 1:** Design-process infrastructure (protocols, meta-work)
- **Layer 2:** The designed product (the actual workflow in use)
- **Curated persistence:** Capture essence, not volume
- **Flag and wait:** Claude recommends, human decides

## License

Private repository for personal workflow use.
