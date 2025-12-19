# Session Protocol

## Purpose
Govern our methodology while designing the meta-workflow.
Ensure continuity, prevent context loss, and enable rigorous curation—without constraining exploration.

---

## Core Tension

Persistence requires documentation.  
Documentation without judgment creates pollution.  
**Goal: Curated persistence—capture what matters, discard what doesn't, archive what might.**

---

## Date Format Standard

All dates use `YYYY-MM-DD` format (e.g., 2025-01-15).

---

## Document Authority Hierarchy

When conflicts arise between documents, precedence follows this order:

1. **PRINCIPLES.md** — Foundational, highest authority, rarely changes
2. **CLAUDE-OPERATING.md** — Claude's behavioral/cognitive protocols
3. **STATE.md** — Current operational truth
4. **Latest session handoff** — Most recent, but provisional until STATE.md is updated
5. **Other working documents** — Subordinate to the above

**Rule:** Conflicts get flagged immediately, not silently resolved. Claude surfaces the inconsistency; Human decides resolution.

---

## Document Loading Rules

**Always load at session start:**
- PRINCIPLES.md (when it exists)
- CLAUDE-OPERATING.md
- STATE.md
- GLOSSARY.md
- Focus-relevant documents for the session

**Never load at session start:**
- ARCHIVE.md (retrieve only when specifically needed)

---

## Session Lifecycle

### 1. SESSION START — Bootstrap

**Human responsibilities:**
- Load core documents into context
- State session goal or focus area
- Flag any external changes: shifted priorities, new constraints, updated thinking

**Claude responsibilities:**
- Confirm documents received and understood
- Summarize current state as understood
- Surface relevant open items and knowledge gaps
- Ask: "Anything to correct or add before we proceed?"

**Integrity check:**
- If documents seem incomplete or inconsistent, flag before proceeding
- If uncertain whether context is complete, ask explicitly

---

### 2. DURING SESSION — Working

**Capture Rules:**
- Decisions logged immediately (even provisional)
- New terms/concepts defined on first use
- Disagreements documented, not just resolved
- Game-changing details flagged regardless of size
- Knowledge gaps logged with urgency

**Confirmation Before Capture:**
- Before logging any DECISION or INSIGHT to persistent documents:
  - Claude states: "Capturing this as [X]. Correct?"
  - Human confirms, corrects, or rejects
- This applies to anything destined for STATE.md, DECISIONS, or KNOWLEDGE-GAPS
- Does NOT apply to working notes or exploratory discussion

**Signal Words:**

| Signal | Meaning |
|--------|---------|
| **DECISION:** | A choice has been made |
| **OPEN:** | Unresolved, needs future attention |
| **PARKED:** | Valid but not now; archive candidate |
| **DRAFT:** | Proposed, not yet agreed |
| **GAP:** | Knowledge needed, research required |
| **ASSUMED:** | Proceeding on assumption (note confidence + risk) |
| **INSIGHT:** | Small but significant realization |

---

### 3. SESSION END — Handoff

**Claude produces:**

1. **Session Summary** — Distilled discussion
2. **Decisions Made** — With DECISION markers (confirmed during session)
3. **Insights Captured** — Game-changers, including small ones
4. **Knowledge Gaps Identified** — What needs research
5. **Open Items** — Unresolved matters
6. **Archive Transitions** — Items moving from STATE to ARCHIVE; confirm before moving
7. **Document Updates** — What was created/modified
8. **Next Session Suggested Focus**

**Human responsibilities:**
- Confirm summary accuracy
- Approve archive transitions
- Save/export documents to Claude Code environment
- Note any corrections for next session

**Archive Update Rule:**
- ARCHIVE.md is updated only at session end
- Superseded decisions, parked ideas, and discarded items transition here
- This keeps STATE.md lean and prevents archive pollution during working sessions

---

## Error Recovery

### Detecting Problems

| Symptom | Likely Cause |
|---------|--------------|
| Claude's state summary doesn't match Human's understanding | STATE.md outdated or session handoff was incomplete |
| Repeated discussion of settled topics | Decision not captured or document not loaded |
| Contradictory information across documents | Update missed or conflict introduced |
| Claude references unknown decisions/concepts | Document failed to load or was never created |

### Recovery Actions

**Minor drift (caught within session):**
- Pause, identify discrepancy
- Clarify correct state verbally
- Update documents immediately before proceeding

**Major drift (discovered across sessions):**
- Stop substantive work
- Conduct explicit reconciliation:
  - What does STATE.md say?
  - What does Human recall as true?
  - What evidence exists (prior documents)?
- Produce corrected STATE.md before resuming

**Uncertain integrity:**
- If Claude suspects incomplete context but isn't sure, ask:
  - "I may be missing context. Can you confirm [X] is still current?"
- Do not proceed on uncertain foundations for consequential decisions

---

## Patterns and Anti-Patterns

### PATTERNS (Do)

| Pattern | Description |
|---------|-------------|
| **Distill wisely** | Capture essence, not volume. A three-word insight may outweigh three paragraphs. |
| **Ground what matters** | Research high-stakes decisions. Mark assumptions explicitly with confidence. |
| **Flag game-changers immediately** | Small realizations that shift perspective get surfaced, not buried. |
| **Archive with intent** | Preserve potential value with clear tags and reasoning. |
| **Update atomically** | STATE.md changes should be coherent, traceable, defensible. |
| **Confirm before committing** | Verify understanding before anything becomes persistent. |
| **Surface conflicts immediately** | Don't silently resolve—flag and escalate. |

### ANTI-PATTERNS (Don't)

| Anti-Pattern | Description |
|--------------|-------------|
| **Do not pollute** | Context is expensive. Noise costs future-us clarity. |
| **Do not lose gold in rubble** | Long discussions bury insights. Extract actively. |
| **Do not assume blindly** | Safe assumptions are fine. High-stakes assumptions need grounding. |
| **Do not archive everything** | Archive is not a junk drawer. Confirm value first. |
| **Do not update speculatively** | STATE.md reflects decisions and facts, not possibilities. |
| **Do not proceed on shaky ground** | Uncertain context + consequential decisions = flag and verify. |

---

## Supporting Documents

| Document | Purpose | Load at Start? |
|----------|---------|----------------|
| **CLAUDE-OPERATING.md** | Claude's cognitive and behavioral protocols | Yes |
| **STATE.md** | Living anchor. Current truth. | Yes |
| **GLOSSARY.md** | Shared terminology. Prevents drift. | Yes |
| **KNOWLEDGE-GAPS.md** | Research queue. What we need to know and why. | Yes |
| **ARCHIVE.md** | Cold storage for parked ideas. | No—retrieve only when needed |

---

## Versioning

- **Snapshots:** Major milestones get versioned copies (v1.0, v2.0)
- **Evolving:** Working documents update in place; significant changes get date stamps
