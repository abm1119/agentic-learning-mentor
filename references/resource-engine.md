# Resource Engine — Full Reference

This file governs how the Agentic Learning Mentor sources, verifies, curates, and presents
learning resources. Read it in full whenever Section 8 of SKILL.md activates.

---

## TABLE OF CONTENTS

1. Core Principles
2. Verification Protocol
3. Quality Tier System
4. Search Strategies (by category)
5. Category-by-Category Rules
   - R1: Official Documentation
   - R2: Research Papers
   - R3: Books
   - R4: GitHub Repositories
   - R5: Blogs & Long-form Writing
   - R6: Newsletters & Sites
   - R7: Frontier Lab Guides & Whitepapers
   - R8: Major Organisation Guides
   - R9: Websites & Interactive Tools
   - R10: Free & Underrated Courses
   - R11: Twitter / Threads Influencers
   - R12: Reddit Communities
   - R13: Bonus / Miscellaneous
6. Relevance & Context Rules
7. Anti-Patterns to Avoid
8. Output Format Reference

---

## 1. CORE PRINCIPLES

**P1 — Verify before you present.**
Every URL must be confirmed via web search before being shown. Never invent or assume a URL from
memory. If you can't confirm a link is live and correct, say so and provide the search query
instead: "Search: [query]"

**P2 — Relevance over volume.**
3 deeply relevant resources beat 15 generic ones. Cut anything that doesn't directly serve this
learner's topic, level, and goal.

**P3 — Annotate everything.**
Every item gets one sentence explaining WHY it's useful for THIS learner — not a generic
description of the resource. "This paper introduced the attention mechanism that powers the
transformers you'll use in your project" beats "A research paper on attention."

**P4 — Surface the underrated.**
Always include at least 1–2 items marked 💎 (underrated / hidden gem) per category. Popular
resources are easy to find. Your job is to surface the ones the learner wouldn't discover alone.

**P5 — Context-aware filtering.**
A resource that's excellent for one learner may be wrong for another. A beginner asking about
Python doesn't need a graduate-level research paper. An advanced ML researcher doesn't need
"Python for Dummies." Filter by: topic match, level match, goal match, recency.

**P6 — Respect the user's time.**
Don't dump everything. Lead with the top 2–3 items per category. Offer to go deeper if they want.

---

## 2. VERIFICATION PROTOCOL

Before presenting any resource, run this checklist:

```
[ ] Web-searched to confirm it exists and the URL is live
[ ] Publication/release date confirmed (for time-sensitive topics)
[ ] Author / creator confirmed as credible in this field
[ ] Content is relevant to the specific topic, not just loosely adjacent
[ ] Free/paid status is correct as of search date
[ ] No deprecated, archived, or abandoned resources presented as active
     (exception: if historically significant, label clearly as "historical reference")
```

**For research papers specifically:**
- Search arXiv, Semantic Scholar, or Google Scholar
- Use format: `[topic] [subtopic] site:arxiv.org` or `[topic] survey paper 2022 2023 2024`
- Confirm paper title, authors, and abstract match before presenting
- Always link to the abstract page, not just the PDF (more stable)

**For GitHub repos:**
- Confirm the repo is active (last commit within reasonable time, or clearly labelled as stable/archived)
- Check star count to inform quality tier
- Check README quality — a good README is a signal of a maintained project

---

## 3. QUALITY TIER SYSTEM

Use these markers consistently:

| Marker | Meaning | When to use |
|--------|---------|-------------|
| ⭐ Essential | Top-tier, widely respected, fundamental | The 1–2 items you'd recommend above all else |
| 💎 Underrated | Excellent but not widely known | Surface these deliberately — this is unique value |
| 🔬 Advanced | High depth, not for beginners | Label so learners know when to return |
| 🆓 Free | Completely free to access | Label all free resources explicitly |
| 🏛️ Classic | Older but foundational / timeless | For books/papers older than 5 years but still essential |
| ⚠️ Dated | Partially outdated — use with caution | Flag but don't omit if still conceptually valid |

---

## 4. SEARCH STRATEGIES BY CATEGORY

Use these search query patterns when web-searching for resources:

### Official Docs
```
[technology name] official documentation
[technology name] docs site:[official domain]
[technology name] getting started guide official
```

### Research Papers
```
[topic] arxiv 2023 2024 2025
[topic] survey paper recent
[topic] state of the art [year]
site:arxiv.org [topic keyword]
site:semanticscholar.org [topic]
[specific technique] paper [conference: NeurIPS ICML ICLR CVPR ACL etc]
```

### Books
```
best books [topic] [beginner/intermediate/advanced]
[topic] book free PDF github
[topic] book open source
[author name] [topic] book
```

### GitHub Repos
```
site:github.com [topic] awesome list
[topic] github stars tutorial
[topic] github implementation
[topic] github open source [year]
[topic] github underrated
```

### Blogs
```
best [topic] blog developers
[topic] in-depth technical blog
[topic] [specific subtopic] explained blog
[author/company] engineering blog [topic]
```

### Newsletters
```
[topic] newsletter subscription
best newsletters [topic] [year]
[topic] weekly digest email
```

### Frontier Lab Guides & Whitepapers
```
[topic] whitepaper [OpenAI OR Anthropic OR Google OR Meta OR Microsoft] [year]
[topic] technical report [lab name]
site:openai.com [topic]
site:anthropic.com [topic]
site:ai.google [topic]
site:research.facebook.com [topic]
site:microsoft.com research [topic]
[topic] position paper [year]
```

### Major Organisation Guides
```
[topic] guide Google developers
[topic] course Microsoft Learn
[topic] tutorial AWS
[topic] learning path official
```

### Websites & Interactive Tools
```
[topic] interactive playground online
[topic] visualiser tool
best websites learn [topic] interactively
[topic] sandbox online
```

### Free Courses
```
[topic] free course [year]
[topic] full course YouTube
[topic] free certification course
[topic] mooc free
[topic] course Coursera audit free
[topic] course fast.ai OR MIT OpenCourseWare OR Stanford Online
```

### Twitter / Threads Influencers
```
[topic] influencer twitter follow
who to follow [topic] twitter 2024
best [topic] accounts twitter
[topic] experts threads app
```

### Reddit
```
[topic] subreddit
best subreddit [topic] learn
reddit [topic] community
```

---

## 5. CATEGORY-BY-CATEGORY RULES

---

### R1: OFFICIAL DOCUMENTATION

**Always include.** This is the ground truth.

Rules:
- Link to the specific section most relevant to the learner's level/focus, not just the homepage
- If there are multiple versions, link to the stable/current release docs
- Note if the docs have interactive examples, playground, or tutorial built in
- For large docs, call out the 2–3 most useful sections for this learner specifically

Output format:
```
### 📄 Official Documentation

- ⭐ **[Technology] Docs** — [verified URL]
  *Start with the [Getting Started / Reference / Tutorial] section — it covers [specific thing
  relevant to this learner's focus]*

- **[Related official resource]** — [URL]
  *Useful for [specific aspect]*
```

---

### R2: RESEARCH PAPERS (LAST 5 YEARS PRIORITY)

**Include for technical, scientific, AI/ML, systems, security, and any research-adjacent topic.**
Skip for purely practical skills (e.g., "I want to learn git branching") unless the user specifically asks.

Rules:
- Prioritise papers from the last 5 years (2020–present)
- For foundational topics, ONE classic paper (pre-2020) is acceptable if marked 🏛️ Classic
- Always include the abstract-page URL, not just the raw PDF
- Conferences to prioritise: NeurIPS, ICML, ICLR, CVPR, ACL, EMNLP, SIGMOD, OSDI, SOSP, CCS, USENIX
- Include survey/review papers — they're the best entry point for learners
- Explain the contribution in plain language, not academic jargon

Output format:
```
### 🔬 Research Papers

| Paper | Authors | Venue/Year | Link |
|-------|---------|-----------|------|
| ⭐ [Title] | [Authors] | [NeurIPS 2023] | [arxiv or paper link] |
| 💎 [Title — underrated] | [Authors] | [Year] | [link] |
| 🏛️ [Classic title] | [Authors] | [Year] | [link] |

**Why these matter for you:** [2 sentences connecting papers to the learner's goal]
```

---

### R3: BOOKS

Rules:
- Always include at least one FREE option (free PDF, open-source, GitHub repo, or free web version)
- Note if a GitHub repo has the full book content
- Flag when a book has an online interactive version
- Include publication year — flag anything older than 7 years unless it's a timeless classic
- For beginners: practical, readable books over dense textbooks
- For advanced: include at least one textbook-level deep dive

Output format:
```
### 📚 Books

- ⭐ **[Title]** by [Author] ([Year]) — 🆓 Free at [URL] / Paid: [link]
  *[Why this book, specific to learner's level and goal]*

- 💎 **[Underrated title]** by [Author] ([Year]) — [Free/Paid]
  *[Why this hidden gem, what makes it different]*

- 🔬 **[Advanced title]** by [Author] ([Year])
  *[Return to this when you've got the basics — covers [specific advanced topic]]*
```

---

### R4: GITHUB REPOSITORIES

Rules:
- Include a mix: "awesome-[topic]" curated lists, reference implementations, project starters, and underrated gems
- Always note approximate star count (search to verify) — context for credibility
- Check that the repo has been active/maintained within a reasonable timeframe
- Include at least one underrated repo (< 2k stars but high quality)
- Explain what the user can DO with the repo, not just what it is

Output format:
```
### 🐙 GitHub Repositories

- ⭐ **[owner/repo]** (~Xk ⭐) — [URL]
  *[What to do with it — clone, study, use as reference, etc.]*

- 💎 **[owner/repo]** (~Xk ⭐) Underrated — [URL]
  *[Why this less-known repo is valuable for this learner]*

- **[owner/repo]** (~Xk ⭐) — [URL]
  *[One sentence practical use]*
```

---

### R5: BLOGS & LONG-FORM WRITING

Rules:
- Include individual authors/writers, not just publications
- Prioritise blogs with technical depth over surface-level content
- Note posting frequency — a blog inactive for 2 years should be flagged
- Company engineering blogs count (Netflix, Uber, Stripe, Cloudflare, etc.)
- Highlight 1–2 specific posts by name if they're particularly relevant

Output format:
```
### ✍️ Blogs & Long-form Writing

- ⭐ **[Blog/Author name]** — [URL]
  *[What makes it worth reading — depth, style, focus area]*
  → Must-read post: "[Post title]" — [URL]

- 💎 **[Blog/Author — underrated]** — [URL]
  *[Why this less-famous voice is worth following]*

- **[Company Engineering Blog]** — [URL]
  *[What they write about that's relevant]*
```

---

### R6: NEWSLETTERS & SITES

Rules:
- Include only newsletters that are actively published (verify via web search)
- Note format: curated links / original writing / mixed
- Note frequency: daily / weekly / bi-weekly
- Prefer newsletters with free tiers; note if paid-only

Output format:
```
### 📬 Newsletters & Sites

| Newsletter | URL | Frequency | Format | Best for |
|-----------|-----|-----------|--------|---------|
| ⭐ [Name] | [URL] | Weekly | Original + curated | [One sentence] |
| 💎 [Name] | [URL] | Bi-weekly | Deep dives | [One sentence — underrated gem] |
| [Name] | [URL] | Daily | Curated links | [One sentence] |
```

---

### R7: FRONTIER LAB GUIDES & WHITEPAPERS

**Include for AI, ML, LLMs, cloud, distributed systems, security, and any rapidly evolving technical field.**

Labs to search: OpenAI, Anthropic, Google DeepMind, Google Research, Meta AI (FAIR), Microsoft Research, Apple ML Research, Hugging Face, Mistral, Cohere, DeepSeek, Stability AI, EleutherAI.

Rules:
- These are authoritative but can be dense — note the target audience
- Include both technical reports AND more accessible guides/cookbooks
- Whitepapers should be from 2020–present unless foundational
- Always note if there's an accompanying blog post (easier entry point)

Output format:
```
### 🧪 Frontier Lab Resources

- ⭐ **[Title]** — [Lab Name], [Year] — [URL]
  *[One sentence on what it covers and why it's valuable for this learner]*
  → Easier entry point: [blog post URL if available]

- **[Title]** — [Lab Name], [Year] — [URL]
  *[One sentence]*
```

---

### R8: GUIDES FROM MAJOR ORGANISATIONS

Organisations to consider: Google (Developers, Research, Machine Learning), OpenAI (Cookbook, Docs), Anthropic (Docs, Guides), Microsoft (Learn, Azure Docs), AWS (Well-Architected, Training), Meta (AI Blog, PyTorch tutorials), NVIDIA (Deep Learning Institute), fast.ai, MIT OpenCourseWare, Stanford Online, freeCodeCamp, Mozilla Developer Network (MDN).

Rules:
- These are often high quality AND free — prioritise them
- Note if they come with certificates
- Flag interactive/sandbox versions when available
- Link to the specific guide, not just the organisation homepage

Output format:
```
### 🏢 Guides from Major Organisations

- ⭐ 🆓 **[Guide Name]** — [Organisation] — [URL]
  *[One sentence — what you'll learn, why it's trustworthy, what format it is]*

- 🆓 **[Guide Name]** — [Organisation] — [URL]
  *[One sentence]*
```

---

### R9: WEBSITES & INTERACTIVE TOOLS

Types to include: online playgrounds (e.g., CodePen, Replit, Jupyter notebooks), visualisers (e.g., algorithm visualisers, network simulators), reference sites (e.g., MDN, DevDocs, Devhints), community wikis, interactive tutorials (e.g., Rustlings, The Odin Project, Exercism).

Rules:
- Prioritise hands-on, interactive resources over passive reading
- Verify the site is actively maintained
- Note browser compatibility if relevant

Output format:
```
### 🌐 Websites & Interactive Tools

- ⭐ **[Site Name]** — [URL]
  *[What you can DO on this site — practice X, visualise Y, reference Z]*

- 💎 **[Underrated site]** — [URL]
  *[Why this less-known tool is great]*
```

---

### R10: FREE & UNDERRATED COURSES

Platforms to search: Coursera (audit), edX (audit), MIT OpenCourseWare, Stanford Online, fast.ai, freeCodeCamp, The Odin Project, Exercism, Kaggle Learn, Google Colab tutorials, YouTube (full course playlists), CS50, Brilliant, Scrimba, Codecademy (free tier), Khan Academy, Udemy (free courses), Hugging Face courses.

Rules:
- **Free is the filter** — include paid only if exceptionally high quality with no free equivalent
- Actively surface underrated courses, not just the famous ones (e.g., not just "Coursera ML by Andrew Ng")
- Note course length (hours/weeks) and time commitment
- Note if a certificate is included
- Flag courses that are self-paced vs cohort-based

Output format:
```
### 🎓 Free & Underrated Courses

- ⭐ 🆓 **[Course Name]** — [Platform] — [URL]
  *[Length] · [One sentence on why it's great and what you'll build/learn]*

- 💎 🆓 **[Underrated Course]** — [Platform] — [URL]
  *[Length] · [Why this lesser-known course is a hidden gem]*

- 🆓 **[Course Name]** — [Platform] — [URL]
  *[Length] · [One sentence]*
```

---

### R11: TWITTER / THREADS INFLUENCERS

Rules:
- Verify the account is active (recent posts) via web search
- Focus on people who post ORIGINAL insights, not just retweeters
- Include a mix: practitioners, researchers, educators, indie makers
- At least 1 person from Threads (separate platform, growing community)
- At least 1 underrated voice (< 10k followers but excellent content)
- Note their posting style: technical threads / quick tips / news commentary / tutorials

Output format:
```
### 🐦 Twitter / Threads: Who to Follow

| Handle | Platform | Focus | Why follow |
|--------|----------|-------|-----------|
| ⭐ @[handle] ([Name]) | Twitter/X | [Their niche] | [Posting style + what they share] |
| 💎 @[handle] ([Name]) | Twitter/X | [Niche] | Underrated — [Why they're worth following] |
| @[handle] ([Name]) | Threads | [Niche] | [One sentence] |
| @[handle] ([Name]) | Twitter/X | [Niche] | [One sentence] |
```

---

### R12: REDDIT COMMUNITIES

Rules:
- Always verify the subreddit is active (recent posts, not banned/private)
- Include subreddit size (members) as a quality signal
- Mix large (for quick help) and niche (for depth) communities
- Note the community culture: beginner-friendly, expert-heavy, news-focused, etc.
- Include at least one underrated or niche subreddit

Output format:
```
### 💬 Reddit Communities

| Subreddit | Members (approx) | Vibe | Best for |
|-----------|-----------------|------|---------|
| ⭐ r/[name] | [~Xk] | [Beginner-friendly / Expert-heavy] | [One sentence] |
| 💎 r/[name — niche/underrated] | [~Xk] | [Vibe] | [Why this smaller sub is valuable] |
| r/[name] | [~Xk] | [Vibe] | [One sentence] |
```

---

### R13: BONUS / MISCELLANEOUS

Anything that doesn't fit the above categories but is genuinely valuable:

- **Podcasts** — note episode length, frequency, guest quality
- **YouTube channels** — distinguish tutorial channels from lecture/talk channels
- **Discord / Slack communities** — note invite link or how to join
- **Cheat sheets** — one-page references (link to GitHub or official sources)
- **Playgrounds / Sandboxes** — e.g., Replit, CodeSandbox, StackBlitz
- **Roadmaps** — e.g., roadmap.sh entries
- **Conferences** — note if talks are free on YouTube
- **Podcasts** — note episode to start with

Output format: use judgment — table or list depending on volume.

---

## 6. RELEVANCE & CONTEXT RULES

Before including any resource, pass it through this filter:

```
TOPIC MATCH:     Is this resource about the SPECIFIC topic (not just adjacent)?
LEVEL MATCH:     Is this appropriate for the learner's assessed level?
GOAL MATCH:      Does this help them achieve what they said they wanted to achieve?
RECENCY:         For fast-moving fields (AI, cloud, security), is this from the last 2–3 years?
QUALITY SIGNAL:  Stars, citations, author reputation, publisher, or user recommendation?
ACTIONABILITY:   Can the learner start using this TODAY, or is it something to return to later?
```

If a resource fails any of these, either exclude it or clearly label its limitation.

**Special case — "anything they ask for":**
If the user asks for something unusual (e.g., "find me a documentary about this topic" or
"are there any games that teach this?"), use web search to find it. Apply the same relevance
check. Label it appropriately (🎬 Documentary / 🎮 Game / 🎵 Podcast / etc.) and include it.
Never refuse a resource request — find the best answer or explain why nothing good exists.

---

## 7. ANTI-PATTERNS TO AVOID

❌ **Hallucinated URLs** — Never invent a link. Always verify via web search.
❌ **Generic padding** — "Google it" or "Stack Overflow" without specifics is useless.
❌ **Level mismatch** — Sending a beginner to a PhD-level paper without warning.
❌ **Outdated resources without warning** — A 2016 React tutorial is actively harmful.
❌ **No annotation** — A list of bare links is lazy. Annotate every item.
❌ **Only famous resources** — If your list looks like the first Google result, dig deeper.
❌ **Broken/dead links** — If a URL is dead, say so and provide a search query instead.
❌ **Too many resources** — Don't overwhelm. Curate ruthlessly.
❌ **Ignoring the learner's level** — Resources must match where they ARE, not where you
     think they should be.
❌ **Presenting paid resources without noting free alternatives** — Always surface a free path.

---

## 8. OUTPUT FORMAT REFERENCE

When delivering resources in-session (not in the report), use this condensed format:

```markdown
## 📚 Your Resource Pack — [Topic]

### Start Here (Essential)
- ⭐ [Resource 1] — [URL] · [One sentence]
- ⭐ [Resource 2] — [URL] · [One sentence]

### Go Deeper
- 🔬 [Resource] — [URL] · [One sentence]
- 💎 [Underrated gem] — [URL] · [One sentence]

### Community & Follow
- r/[subreddit] — [URL]
- @[handle] on Twitter/X — [One sentence]

### Free Course to Continue
- 🆓 [Course] — [URL] · [Length] · [One sentence]

> Want the full resource arsenal (papers, books, newsletters, whitepapers, influencers)?
> Just say "give me the full resources" and I'll compile the complete list.
```

For the session report, use the full expanded format defined in `report-template.md`.
