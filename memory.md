# memory.md — Learner Session History

**Skill:** agentic-learning-mentor v1.1.0  
**Purpose:** Persistent cross-session memory that makes every session smarter than the last.  
**Format:** One entry per session, append-only. Never delete entries.

---

## HOW TO USE THIS FILE

### At session START (PHASE 0):
1. Read this entire file
2. Search for any prior entries matching the current topic (or closely related topics)
3. If a match exists:
   - Shorten PHASE 1 (skip questions already answered in prior sessions)
   - Reference the prior session: *"Last time we covered [X] — want to pick up from there or go somewhere new?"*
   - Adjust starting depth: never re-teach concepts already marked `✅ Understood`
4. If no match: proceed with full PHASE 1 as normal

### At session END (PHASE 5):
Append one new entry using the template below. Fill all fields — no blanks.

### Privacy rule:
Store ONLY learning data. No personal details, no names, no employer info, no health data.
If the user volunteers personal context during a session, use it in that session only — do not store it here.

---

## Entry Template

```
---
session: [auto-increment number, e.g. 001]
date: YYYY-MM-DD
day: [Monday / Tuesday / etc.]
topic: [exact topic slug, e.g. python-async, system-design, rust-ownership]
topic_display: [human-readable, e.g. "Python Async/Await", "System Design Fundamentals"]
level_assessed: [Beginner | Intermediate | Advanced]
goal: [one sentence — what the learner said they wanted to achieve]
report_file: [filename of the saved .md report]

concepts_covered:
  - [concept 1]
  - [concept 2]
  - [concept 3]

understood:
  - [concept or skill the learner clearly grasped]
  - [another]

needs_revisit:
  - [concept or skill that needs more work]
  - [another]

task_given: [one sentence describing the task]
task_outcome: [Completed | Partially completed | Not attempted] — [one sentence on what happened]

learner_signals:
  style: [Conceptual | Hands-on | Mixed — observed during session, may differ from stated preference]
  pace: [Slow | Moderate | Fast]
  engagement: [Low | Medium | High]
  notable: [one sentence — anything specific about how this learner thinks or communicates]

next_session_suggested_focus: [topic or concept to tackle next time]
continuation_prompt: "[Exact prompt the learner can paste to resume — make it specific]"

resources_given: [list 2-3 top resources shared]
  - [resource name + URL]
  - [resource name + URL]
---
```

---

## Session History

*Entries appear below in chronological order. Most recent is last.*

<!-- APPEND NEW ENTRIES BELOW THIS LINE -->

---
2026-06-10 | SKILL_FIXES | Added explicit report-template population check, required encouragement, enforced >=3 intake answers before teaching, memory read/append instructions, and performance budgets; bumped skill version to 1.1.1.


## Context Rules for Multi-Session Learners

When the learner has 2+ entries on the same topic:
- **Build a progress arc** — show them how far they've come: "In session 1 you were [beginner state], now you're [current state]"
- **Avoid repetition** — never re-explain a concept in `understood:` from a prior entry unless the learner explicitly asks
- **Escalate difficulty** — each session on the same topic should go one level deeper
- **Surface the gap** — prioritise `needs_revisit:` items from prior sessions before introducing new concepts

When the learner has entries on different but related topics:
- Connect the dots: "You've already worked with [topic A] — that'll actually help here because [reason]"
- Transfer knowledge: reference relevant concepts from prior sessions to accelerate learning

---

## Memory Health Checks

Run these periodically (or add to `evals.md` regression suite):

- [ ] All entries follow the template format
- [ ] No personal/sensitive data stored in any entry
- [ ] `continuation_prompt` in latest entry is specific enough to restore session context
- [ ] `needs_revisit` items from older entries are being addressed in newer entries (or explicitly deprioritised)
- [ ] No duplicate session numbers

---

## Pruning Policy

This file is **append-only** — do not delete entries.  
If the file grows beyond ~200 entries, create `memory-archive-YYYY.md` and move entries older than
12 months there, keeping the 20 most recent in this file.  
Update the archive reference at the top of this file.
