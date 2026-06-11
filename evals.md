# evals.md — Agentic Learning Mentor Self-Evaluation

**Version:** 1.1.0  
**Run after:** every session (PHASE 5 complete) and on any skill update  
**Target:** Triggering ≥ 90% correct · Functional 0 failures · Performance within budgets  
**How to use:** Work through each checklist in order. Mark `[x]` pass or `[!]` fail.
On any `[!]`, record the failure in the `## Failure Log` at the bottom.

---

## 1. Triggering Tests

*Goal: skill fires on learning intent, stays silent on everything else.*

### Should Trigger (target: all pass)

- [ ] `"I want to learn Python"` → skill activates, begins welcome + PHASE 1
- [ ] `"I am curious about Docker containers"` → skill activates
- [ ] `"I want to master system design"` → skill activates
- [ ] `"Teach me how async/await works"` → skill activates
- [ ] `"Help me understand transformers"` → skill activates
- [ ] `"Walk me through how Git rebase works"` → skill activates
- [ ] `"I want to explore Rust"` → skill activates
- [ ] `"How does a hash map work?"` → skill activates (learning intent phrasing)
- [ ] `"I want to get better at SQL"` → skill activates
- [ ] `"I'm curious about LLMs — where do I start?"` → skill activates

### Should NOT Trigger (target: all pass)

- [ ] `"Fix this bug in my code"` → skill stays silent, normal debug response
- [ ] `"What is 2 + 2?"` → skill stays silent
- [ ] `"Refactor this function"` → skill stays silent
- [ ] `"Search the web for React tutorials"` → skill stays silent (not a learning session request)
- [ ] `"What time is it in Tokyo?"` → skill stays silent
- [ ] `"Write a Python script that parses CSV"` → skill stays silent (task, not learning intent)
- [ ] `"Review my pull request"` → skill stays silent

---

## 2. Functional Tests

*Goal: zero failures on core session behaviour.*

### PHASE 1 — Sequential Q&A

- [ ] **one_question_rule:** First response after welcome contains exactly ONE question, no bundled questions
- [ ] **no_premature_teach:** Skill does not deliver any teaching content before collecting ≥ 3 intake answers
- [ ] **profile_built:** By end of PHASE 1, learner profile (Level, Style, Goal, Focus) is silently constructed and used in PHASE 3

### PHASE 2 — Knowledge Probe

- [ ] **beginner_skip:** When user signals "complete beginner", PHASE 2 is skipped and PHASE 3 starts immediately
- [ ] **probe_relevant:** Probe questions reference the specific topic, not generic knowledge

### PHASE 3 — Core Teaching

- [ ] **level_match:** Content depth matches the assessed level (no PhD content for beginners; no "what is a variable" for advanced)
- [ ] **tool_use:** At least one agentic tool (code exec / web search / file creation) used during teaching where appropriate
- [ ] **task_given:** Exactly one hands-on task assigned, matching level from `references/task-patterns.md`
- [ ] **execution_used:** If topic involves code AND user shares a solution, code is executed to verify (not just read)
- [ ] **hint_provided:** If user gets stuck, a hint is provided before moving on

### PHASE 4 — Wrap-up

- [ ] **summary_present:** Wrap-up includes 2–3 bullet summary of what was covered
- [ ] **next_step:** At least one concrete next step recommended

### PHASE 5 — Report

- [ ] **report_always_saved:** Session report .md file created at end of EVERY session, no exceptions
- [ ] **filename_correct:** Filename matches `YYYY-MM-DD_DayName_[topic-slug]_learning-session.md`
- [ ] **template_filled:** All sections of `references/report-template.md` are populated — no empty placeholders
- [ ] **resource_section_present:** Report includes at least 3 verified resource items with annotations

### Resource Engine

- [ ] **no_memory_urls:** No URL appears in output without a prior web-search call in the same session
- [ ] **annotated:** Every resource item has a one-sentence annotation explaining relevance to the learner
- [ ] **tier_marked:** At least one `💎 Underrated` item included per resource response
- [ ] **dead_link_handled:** If a searched URL returns 404/not found, it is excluded and replaced or marked "verify manually"

### Error Handling

- [ ] **broad_topic_handled:** Prompt "I want to learn programming" triggers ONE scoping question, not a dump of all languages
- [ ] **silence_handled:** One-word user answers trigger leading statement + "does that sound right?" pattern
- [ ] **file_fail_fallback:** If file creation fails, full report is printed inline as a code block
- [ ] **harmful_topic_redirected:** Harmful/unethical topic request is redirected to a safe adjacent area

### Style & Tone

- [ ] **no_lectures:** Teaching is conversational, not monologue — check-ins after each concept
- [ ] **warm_tone:** At least one encouragement or acknowledgement of good answer per session
- [ ] **no_deprecated_patterns:** No use of deprecated tool calls, old API signatures, or removed capabilities

---

## 3. Memory Tests

*Goal: session history is read at start and written at end.*

- [ ] **memory_read_on_start:** `memory.md` is read at session start; prior entries surfaced when relevant
- [ ] **memory_written_on_end:** New entry appended to `memory.md` in correct format after PHASE 5
- [ ] **context_used:** If a prior session on same topic exists in memory, PHASE 1 is shortened and references prior session
- [ ] **no_memory_hallucination:** Skill does not invent prior session history that isn't in `memory.md`
- [ ] **memory_privacy:** `memory.md` entries contain only learning data — no personal/sensitive information stored

---

## 4. Performance Tests

*Goal: efficient execution within tool-call and token budgets.*

| Metric | Budget | Actual | Pass? |
|--------|--------|--------|-------|
| Total tool calls per session | ≤ 12 | ___ | [ ] |
| PHASE 1 turns (questions asked) | ≤ 5 | ___ | [ ] |
| Report generation tool calls | ≤ 2 (read template + write file) | ___ | [ ] |
| Resource web-search calls | ≤ 6 per resource request | ___ | [ ] |
| Failed tool calls (errors) | 0 | ___ | [ ] |
| Broken/unverified URLs presented | 0 | ___ | [ ] |

---

## 5. Regression Tests

*Run these after any skill update to confirm nothing broke.*

- [ ] **frontmatter_valid:** `name` is kebab-case, matches folder, no "claude"/"anthropic"; description under 1024 chars, no XML `<>`
- [ ] **references_exist:** All files listed in SKILL.md `## Reference Files` table are present in `./references/`
- [ ] **memory_exists:** `memory.md` exists in skill root
- [ ] **evals_exists:** `evals.md` exists in skill root
- [ ] **no_duplicate_sections:** SKILL.md has no duplicate section numbers
- [ ] **skill_under_1page:** SKILL.md core instructions fit approximately one printed page (under ~6000 chars)

---

## 6. Self-Improvement Protocol

After every 5 sessions, review the Failure Log below and:

1. **Identify the top recurring failure** (most `[!]` marks in one category)
2. **Trace the root cause** — is it in SKILL.md, a reference file, or a triggering issue?
3. **Make one targeted edit** — change the minimum text needed to fix it
4. **Re-run the relevant checklist section** to confirm the fix
5. **Bump `version`** in SKILL.md frontmatter (patch: 1.1.x for fixes, minor: 1.x.0 for new features)
6. **Append a note to `## Changelog`** below

---

## Failure Log

*Append entries here whenever a test fails. Format: `DATE | TEST_ID | What happened | Fix applied`*

| Date | Test ID | Failure description | Fix applied |
|------|---------|-------------------|-------------|
| — | — | — | — |

---

## Changelog

| Version | Date | Change summary |
|---------|------|---------------|
| 1.0.0 | initial | Skill created |
| 1.1.0 | — | Frontmatter rewritten; SKILL.md refactored to 1-page; evals.md + memory.md added; question-bank.md + task-patterns.md extracted |
