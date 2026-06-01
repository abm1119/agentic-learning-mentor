# 🎓 Agentic Learning Mentor

> **A revolutionary AI-powered learning and mentoring skill for Agentic IDEs**
>
> Transform the way you learn. Get personalized, interactive mentoring sessions that adapt to your level, teach you through hands-on challenges, and generate detailed learning reports — all in 15 minutes.

[![GitHub License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Status](https://img.shields.io/badge/status-Active-brightgreen)]()
[![Version](https://img.shields.io/badge/version-1.0-blue)]()

---

## 📌 Table of Contents

- [What is Agentic Learning Mentor?](#what-is-agentic-learning-mentor)
- [Key Features](#key-features)
- [Quick Start](#quick-start)
- [How It Works](#how-it-works)
- [Installation](#installation)
- [Complete User Guide](#complete-user-guide)
- [Examples & Use Cases](#examples--use-cases)
- [Understanding the Skill Architecture](#understanding-the-skill-architecture)
- [Session Report](#session-report)
- [Resource Engine](#resource-engine)
- [FAQ](#faq)
- [Contributing](#contributing)
- [License](#license)

---

## What is Agentic Learning Mentor?

**Agentic Learning Mentor** is an intelligent tutoring skill designed for Agentic IDEs (like VS Code with AI capabilities). It's a complete mentoring system that:

1. **Understands your learning intent** — Detects when you want to learn, explore, understand, or master ANY topic
2. **Assesses your current level** — Asks thoughtful, one-at-a-time questions to understand where you stand
3. **Delivers personalized learning** — Creates a custom lesson matched to your experience level and learning style
4. **Teaches through doing** — Gives you hands-on challenges and exercises tailored to your level
5. **Generates detailed reports** — Saves a comprehensive session report with everything covered, your progress, and next steps

The entire experience is designed to fit into a focused **15-minute session** while maintaining depth and quality.

---

## Key Features

### ✨ What Makes It Special

| Feature | Description |
|---------|-------------|
| **🎯 Intent Detection** | Automatically triggers when you mention learning goals like "teach me", "I want to learn", "explain", "help me understand" |
| **📊 Smart Assessment** | Asks sequential, one-at-a-time questions to understand your experience level, learning style, and specific goals |
| **🧠 Personalized Learning** | Adapts lesson depth and approach based on your profile (Beginner/Intermediate/Advanced) |
| **💻 Hands-on Challenges** | Every session includes a practical task matched to your level — code exercises, design problems, or guided walkthroughs |
| **📚 Resource Arsenal** | Curated, web-verified resources including official docs, research papers, books, GitHub repos, blogs, and more |
| **📄 Session Reports** | Automated markdown reports documenting what you learned, your strengths, areas to develop, and next steps |
| **🔗 Full Tool Integration** | Uses code execution, web search, file creation, and environment analysis for maximum learning impact |
| **🎮 Mentor Q&A** | After learning concepts, shift into open mentoring mode to ask follow-up questions and deepen understanding |
| **📚 Topic Playbooks** | Pre-built learning arcs for 16+ common topics (Python, React, SQL, System Design, etc.) |

---

## Quick Start

### For First-Time Users

1. **Open your Agentic IDE** (e.g., VS Code with AI capabilities)
2. **Express learning intent** — Use natural language like:
   - *"I want to learn Python"*
   - *"Teach me how React hooks work"*
   - *"I'm curious about SQL databases"*
   - *"Help me understand async/await in JavaScript"*
   - *"I want to get better at system design"*

3. **Answer assessment questions** — The mentor will ask 3–5 quick questions about your experience, style, and goals
4. **Learn through a personalized lesson** — Get concepts explained at your level + a hands-on task
5. **Ask questions** — Deep-dive into anything that comes up
6. **Receive your session report** — A complete `.md` file saved with everything you learned

**Total time:** ~15 minutes for a complete session.

---

## How It Works

### Session Architecture (5 Phases)

```
PHASE 0: Intent Detection & Welcome      (~1 min)
   ↓
PHASE 1: Intake Assessment Q&A           (~3 min)  [ONE question at a time]
   ↓
PHASE 2: Knowledge Probe (optional)      (~2 min)  [For intermediate+ learners]
   ↓
PHASE 3: Core Learning & Hands-on Task   (~7 min)  [Concepts + Challenge]
   ↓
PHASE 4: Reflection & Wrap-up            (~1 min)  [Summary + Next Steps]
   ↓
PHASE 5: Session Report Generation       (~1 min)  [Markdown file saved]
```

### Phase Breakdown

#### 🔍 **PHASE 0: Intent Detection & Welcome** (~1 min)

The mentor detects learning intent from phrases like:
- *"I want to learn [topic]"*
- *"Teach me about [topic]"*
- *"I'm curious about [topic]"*
- *"Help me understand [topic]"*
- *"How does [topic] work?"*

Upon detection, you'll receive:
- ✅ A warm welcome
- ✅ Clear expectations (3 questions → learning → hands-on task → report)
- ✅ Confirmation of the topic

---

#### 📋 **PHASE 1: Intake Assessment** (~3 min)

The mentor asks **ONE question at a time** to build your learner profile:

**Question Bank (adapted to your topic):**

| # | Focus | Example |
|---|-------|---------|
| Q1 | Prior Experience | *"Have you worked with [topic] before, or is this completely new?"* |
| Q2 | Current Level | *"How would you rate your understanding — complete beginner, dabbled, or solid foundation?"* |
| Q3 | Goal/Motivation | *"What's driving this — a project, career move, or pure curiosity?"* |
| Q4 | Specific Focus | *"Is there a specific aspect you want to focus on, or a broad overview?"* |
| Q5 | Learning Style | *"Do you prefer learning by doing (hands-on) or understanding concepts first?"* |
| Q6 | Blockers | *"Is there something specific about this that's confused you before?"* |

Your answers help the mentor build an **internal learner profile** (not shown to you):
- **Experience Level:** Beginner / Intermediate / Advanced
- **Learning Style:** Conceptual / Hands-on / Mixed
- **Focus Area:** Specific subtopic or broad overview
- **Goal:** What you want to achieve

---

#### 🧪 **PHASE 2: Knowledge Probe** (~2 min)

*Skipped for complete beginners or if you're in a hurry.*

For intermediate/advanced learners, the mentor asks 1–2 follow-up questions to pinpoint knowledge gaps:

- *"Let's test the water — what happens when [specific scenario]?"*
- *"Can you tell me the difference between [Concept A] and [Concept B]?"*

This helps the mentor adjust the depth of PHASE 3.

---

#### 🎓 **PHASE 3: Core Learning & Mentoring** (~7 min)

This is the heart of your session. Three parts:

##### 3a. Concept Delivery

**Based on your level:**
- **Beginner:** Start from first principles, use analogies, keep code simple
- **Intermediate:** Skip basics, go straight to interesting patterns
- **Advanced:** Discuss tradeoffs, edge cases, best practices — treat you as a peer

**The mentor uses agentic tools actively:**
- 💻 **For code topics:** Executes live examples showing actual output
- 🌐 **For frameworks/libraries:** Web-searches current docs and recent updates
- 📁 **For project structure:** Creates example files in your workspace
- 📐 **For conceptual topics:** Uses diagrams, pseudocode, and ASCII art

**Format:** Tight, focused explanations. Maximum 3–4 key concepts per session. After each concept:
> *"Does that make sense, or want me to go deeper on any part?"*

##### 3b. Personalized Task/Challenge

Every lesson includes **one concrete task** matched to your level:

| Your Level | Task Type | Example |
|-----------|-----------|---------|
| **Beginner** | Guided Exercise | *"Try writing a function that does X — here's the scaffold"* |
| **Intermediate** | Real Challenge | *"Build a module that does Y — here's the spec"* |
| **Advanced** | Design Problem | *"Given these constraints, how would you architect Z?"* |

You can:
- ✏️ Write code and share it for live execution
- 💭 Think through a design problem
- 🎯 Work through a guided walkthrough

The mentor provides hints if you get stuck — never leaves you stranded.

##### 3c. Open Mentor Q&A

After the core concepts and task, shift into mentoring mode:
- *"What questions came up while working through this?"*
- Answer questions with depth matched to your level
- Connect concepts to the bigger picture of your stated goal

---

#### 🎬 **PHASE 4: Reflection & Wrap-up** (~1 min)

Brief wrap-up summarizing:
- 2–3 bullet points of what was covered
- Your demonstrated strengths
- 1–2 areas to revisit or explore next
- A specific next step (resource, project idea, or concept to tackle)

---

#### 📄 **PHASE 5: Session Report** (~1 min)

**This is mandatory — every session generates a report.**

A detailed `.md` file is saved with the filename format:
```
YYYY-MM-DD_DayOfWeek_[topic-slug]_learning-session.md
```

Examples:
- `2025-07-18_Friday_python-async_learning-session.md`
- `2025-07-18_Friday_react-hooks_learning-session.md`

**Report includes:**
- Your learner profile (experience, style, goal)
- Where you stand right now (honest assessment)
- Concepts covered with summaries
- The task you completed
- Mentor observations about your learning
- Your next steps (immediate, short-term, long-term)
- **Complete resource arsenal:** Official docs, research papers, books, GitHub repos, blogs, newsletters, courses, and more — all web-verified and relevant to YOUR level and goal

---

## Installation

### Prerequisites

- **Agentic IDE:** VS Code with AI capabilities enabled (e.g., GitHub Copilot, Claude integration)
- **Skill Support:** Your IDE must support custom skills or extensions
- **No additional packages needed** — the skill uses built-in agentic capabilities

### Setup Steps

#### Option 1: Clone from GitHub (Recommended)

```bash
# Clone the repository
git clone https://github.com/abm1119/agentic-learning-mentor.git

# Navigate to the folder
cd agentic-learning-mentor

# Copy to your IDE's skills directory:
# For VS Code: Copy to ~/.vscode/extensions/copilot-skills/
# For other IDEs: Follow your IDE's custom skill installation path
```

#### Option 2: Manual Installation

1. Download the `SKILL.md` file from this repository
2. Place it in your IDE's skills directory
3. Ensure `references/` folder with supporting files is in the same directory:
   - `references/report-template.md`
   - `references/resource-engine.md`
   - `references/topic-playbooks.md`

#### Verify Installation

After installation:
1. Restart your IDE
2. Open the chat/assistant panel
3. Try a learning trigger phrase:
   - *"I want to learn Python"*
   - *"Teach me about React"*
   - *"Help me understand databases"*

If the skill is active, you'll see the welcome message and assessment questions begin.

---

## Complete User Guide

### Learning Trigger Phrases

Use **any** of these phrases to activate the skill:

| Intent | Example Phrases |
|--------|-----------------|
| **Learning** | "I want to learn X", "Teach me X", "Help me learn X" |
| **Understanding** | "Help me understand X", "Explain X to me", "How does X work?" |
| **Exploration** | "I'm curious about X", "Tell me about X", "I want to explore X" |
| **Mastery** | "I want to master X", "I want to get better at X" |
| **Study** | "I want to study X", "Walk me through X" |
| **Interest** | "I'm interested in X", "I want to know more about X" |

**The topic (X) can be anything:**
- Programming languages (Python, JavaScript, Rust, Go)
- Frameworks (React, Django, FastAPI, Next.js)
- Concepts (Databases, System Design, Machine Learning, Algorithms)
- Tools (Git, Docker, Kubernetes, SQL)
- Technologies (Cloud platforms, APIs, Microservices)
- Soft skills (Project management, communication, leadership)

---

### Assessment Questions Explained

During PHASE 1, you'll answer 3–5 questions like these:

#### Q: "Have you worked with [topic] before?"
**Why it matters:** Helps the mentor understand if you're starting from zero or building on existing knowledge.

**Your answer determines:**
- Whether to explain foundational concepts
- Pace of learning
- Complexity of examples

---

#### Q: "How would you rate your current understanding?"
**Why it matters:** Calibrates the lesson depth.

**Example scale:**
- **Complete beginner:** Never heard of it or no practical experience
- **Dabbled:** Played around or read about it, but not confident
- **Solid foundation:** Have worked with it or studied it extensively

---

#### Q: "What's driving you to learn this?"
**Why it matters:** Connects learning to your goals so examples are relevant.

**Your reasons might be:**
- 🚀 **Project:** You're building something that uses this
- 💼 **Career:** You want to level up professionally
- 🧠 **Curiosity:** You're exploring a new domain
- 🎯 **Skill development:** You want to become proficient

---

#### Q: "Do you prefer hands-on learning or understanding concepts first?"
**Why it matters:** Sets the learning style.

**Your preference determines:**
- Whether to start with theory or code/examples
- Whether the challenge comes early or late
- How much to explain vs. how much to let you discover

---

### Working Through the Hands-on Challenge

When the mentor gives you a task, you have several options:

#### Option 1: Code Submission
```python
# You write code and share it in the chat
def add_numbers(a, b):
    return a + b

# The mentor runs it with: 
# add_numbers(5, 3) → 8
```

The mentor will:
- ✅ Execute your code
- ✅ Show the actual output
- ✅ Provide feedback on correctness and style
- ✅ Suggest improvements

#### Option 2: Conceptual Discussion
For non-code topics (system design, architecture), you can:
- Describe your approach in writing
- Sketch a design on paper and describe it
- Walk through your thinking out loud

The mentor will:
- ✅ Evaluate your reasoning
- ✅ Ask probing questions
- ✅ Point out gaps or creative solutions
- ✅ Help refine your approach

#### Option 3: Guided Walkthrough
For complex topics, the mentor might:
- Walk you through a solution step-by-step
- Have you predict what happens next
- Let you fill in missing pieces

---

### Asking Follow-up Questions

After the main lesson, the mentor will ask:
> *"What questions came up while working through that?"*

This is your chance to **dig deeper:**
- ❓ "Why did we do it that way instead of [alternative]?"
- ❓ "How does this scale when [scenario]?"
- ❓ "What happens if [edge case]?"
- ❓ "How does this connect to [related concept]?"

The mentor will answer at your level with:
- ✅ Clear explanations
- ✅ Trade-off analysis (when relevant)
- ✅ Real-world examples
- ✅ Connections to the bigger picture

---

### Understanding Your Session Report

After every session, you'll receive a `.md` file. Here's what's in it:

#### 📋 Learner Profile Section
| Attribute | Example |
|-----------|---------|
| **Experience Level** | Beginner / Intermediate / Advanced |
| **Learning Style** | Hands-on / Conceptual / Mixed |
| **Primary Goal** | Build a Python app / Level up my React skills |
| **Focus Area** | Async functions / Hooks and state management |

---

#### 📍 Where You Stand Right Now
An honest assessment of your current understanding after the session:

```markdown
You're starting to grasp the fundamentals of async/await 
and can recognize when to use promises. You showed strong 
understanding of the event loop, but need practice with 
error handling in async chains.

**Strengths demonstrated:**
- Clear understanding of promise states
- Good intuition about when async is needed

**Areas to develop:**
- Error handling with async/await
- Debugging async code with dev tools
```

---

#### 📚 What We Covered Today
Detailed summaries of each concept taught:

```markdown
### Concepts Explored

1. **Promise Basics**
   Promises are objects representing future values in JavaScript. 
   They can be pending, resolved, or rejected.

2. **Async/Await Syntax**
   Async functions are syntactic sugar over promises that make 
   async code look and behave more like synchronous code.

### Key Takeaways
> **Async/await doesn't make code run in parallel — 
> it just makes sequential async operations easier to read.**
```

---

#### 🛠️ Task/Challenge Completed
Documents the hands-on work you did:

```markdown
**Task Given:** Build a function that fetches user data from 
an API and handles errors gracefully.

**Difficulty Level:** Intermediate

**Outcome:** You completed the task with minimal hints, 
properly using try/catch. You showed strong understanding 
of the happy path but initially missed handling network errors.

**Code Produced:**
[Your actual code here]
```

---

#### 💡 Insights & Observations
Personal mentor observations about YOUR learning:

```markdown
- You ask good clarifying questions and aren't afraid to probe edge cases
- You learn best through code examples rather than theory first
- You get frustrated quickly with errors — try debugging with dev tools first
```

---

#### 🗺️ Learning Journey Map
Visual representation of your progress:

```markdown
Async JavaScript — Intermediate
├─ ✅ Understood: Promises, async/await, .then() chains
├─ 🔄 Needs Practice: Error handling, debugging
└─ 🔜 Next: Promise.all() and concurrency patterns
```

---

#### 🚀 Your Next Steps
Actionable recommendations:

```markdown
### Immediate (Today/Tomorrow)
1. Practice error handling by refactoring one of your existing functions

### Short-term (This Week)
1. Build a real project using async code
2. Read the MDN guide on Promise.all()

### Long-term (This Month)
1. Understand event loop mechanics deeply
2. Learn about async generators
```

---

#### 📖 Your Complete Resource Arsenal
Web-verified, personalized resources including:
- 📄 Official Documentation
- 🔬 Research Papers (if applicable)
- 📚 Books
- 🐙 GitHub Repositories
- ✍️ Blogs & Long-form Writing
- 📬 Newsletters
- 🧪 Frontier Lab Guides
- 🏢 Major Organization Guides
- 🆓 Free Courses
- 💬 Twitter/Threads Influencers to Follow
- 🌐 Reddit Communities

**Every resource:**
- ✅ Is web-verified (not from memory)
- ✅ Has a direct link that works
- ✅ Includes one sentence explaining why it's useful FOR YOU specifically
- ✅ Is marked with a quality tier (⭐ Essential, 💎 Underrated, 🔬 Advanced, etc.)

---

## Examples & Use Cases

### Example 1: Learning Python (Beginner)

**Your message:**
> *"I want to learn Python, but I have no programming experience"*

**What happens:**

1. ✅ Welcome + expectations set
2. ✅ Assessment asks about your background, why you want to learn, hands-on vs. conceptual preference
3. ✅ Core lesson covers:
   - Variables and data types
   - Lists and loops
   - Writing your first function
4. ✅ Hands-on task: *"Write a script that counts the numbers in a list and prints the total"*
5. ✅ You write code, mentor runs it and gives feedback
6. ✅ Q&A: You ask about loops vs. list comprehensions
7. ✅ Session report saved with resources for continuing your Python journey

**Total time:** ~15 minutes | **Report file:** `2025-07-18_Friday_python-beginner_learning-session.md`

---

### Example 2: Learning React Hooks (Intermediate)

**Your message:**
> *"Help me understand React hooks — I know the basics but hooks confuse me"*

**What happens:**

1. ✅ Mentor skips beginner explanations
2. ✅ Assessment reveals you have React experience but hooks are the pain point
3. ✅ Core lesson covers:
   - Why hooks exist (replacing class component patterns)
   - useState: State in functional components
   - useEffect: Side effects and dependency arrays
4. ✅ Hands-on task: *"Refactor this class component to use hooks"* [you get a messy example]
5. ✅ You refactor it, mentor reviews for correctness and best practices
6. ✅ Q&A: You ask about custom hooks and how to extract logic
7. ✅ Session report with advanced resources on performance optimization

**Total time:** ~15 minutes | **Report file:** `2025-07-18_Friday_react-hooks_learning-session.md`

---

### Example 3: Learning System Design (Advanced)

**Your message:**
> *"I want to master system design — interviews are coming up"*

**What happens:**

1. ✅ Mentor skips basic explanations
2. ✅ Assessment reveals you have backend experience and goal is interview prep
3. ✅ Knowledge probe asks deeper questions about your weak areas
4. ✅ Core lesson covers a realistic design problem:
   - *"Design a scalable URL shortener that handles 100M requests/day"*
5. ✅ Hands-on challenge: You sketch the architecture and justify decisions
6. ✅ Mentor challenges your assumptions, asks about tradeoffs
7. ✅ Open discussion on failure modes, scaling strategies, and cost optimization
8. ✅ Session report with advanced resources on distributed systems and real interview prep guides

**Total time:** ~15 minutes | **Report file:** `2025-07-18_Friday_system-design_learning-session.md`

---

## Understanding the Skill Architecture

### File Structure

```
agentic-learning-mentor/
├── SKILL.md                          # Main skill definition (you're reading the guide version)
├── README.md                         # This file
├── references/
│   ├── report-template.md            # Session report template
│   ├── resource-engine.md            # Resource curation logic & search strategies
│   └── topic-playbooks.md            # Pre-built learning arcs for 16+ topics
└── [session reports generated here]  # YYYY-MM-DD_..._learning-session.md files
```

---

### Core Components

#### 🎓 SKILL.md (Main Definition)
The authoritative skill definition containing:
- Complete session architecture (5 phases)
- Intake assessment question bank
- Core mentoring strategies
- Tool usage guidelines
- Edge cases and handling
- Timing guidance

#### 📄 report-template.md
The template used to generate end-of-session reports. Includes:
- Learner profile section
- Where you stand assessment
- Concepts covered
- Task completed with code
- Mentor observations
- Next steps roadmap
- Resource arsenal template

#### 🔍 resource-engine.md
Comprehensive guide for the resource curation system:
- Verification protocol (web-search every URL)
- Quality tier system (⭐ Essential, 💎 Underrated, etc.)
- Search strategies for each resource category
- Relevance filtering rules
- Anti-patterns to avoid

#### 📚 topic-playbooks.md
Pre-built learning arcs for common topics:
- **Topics included:** Python, JavaScript/TypeScript, React, System Design, Machine Learning, Git, SQL, Docker, REST APIs, Data Structures, Rust, Cloud, Linux, LLMs, Web Scraping
- **For each:** Beginner path, Intermediate path, Advanced path
- **Each path:** Core concepts → hands-on task → live demo ideas

---

### How the Mentor Works

```
User Message
    ↓
[Does it match a learning trigger?]
    ├─ NO → Respond normally (not the mentor skill)
    └─ YES ↓
    
PHASE 0: Detect intent, welcome, confirm topic
    ↓
PHASE 1: Ask 3-5 assessment questions (one at a time)
    ├─ Analyze answers silently
    └─ Build learner profile (level, style, focus, goal)
    ↓
PHASE 2: Knowledge probe (optional, for intermediate+)
    ├─ Ask 1-2 probing questions
    └─ Adjust depth based on answers
    ↓
PHASE 3: Core learning + hands-on challenge
    ├─ Deliver concepts at learner's level
    ├─ Use agentic tools (code execution, web search, file creation)
    ├─ Give personalized task
    ├─ Open mentor Q&A mode
    └─ Answer follow-up questions
    ↓
PHASE 4: Reflection and wrap-up (1 min)
    ├─ Summarize what was covered
    ├─ Highlight strengths
    └─ Recommend next steps
    ↓
PHASE 5: Session report generation (MANDATORY)
    ├─ Generate markdown report
    ├─ Fill in report template completely
    ├─ Web-search and verify all resources
    ├─ Save file with naming convention
    └─ Confirm file saved to user
```

---

## Session Report

### Why Session Reports Matter

Every session generates a detailed markdown report that serves as:

1. **Learning Record** — Document of what you learned in this session
2. **Progress Tracker** — Track your growth across multiple sessions
3. **Action Plan** — Clear next steps for continued learning
4. **Resource Guide** — Curated, verified resources for deeper learning
5. **Personal Assessment** — Honest feedback on your strengths and areas to develop

### Using Your Reports

**After a session:**
1. 📖 **Read** your report to reinforce what you learned
2. 🔗 **Explore** the resource arsenal (start with ⭐ Essential items)
3. 🗺️ **Follow** the next steps roadmap
4. 📚 **Return** to the mentor for deeper dives on weak areas

**Across multiple sessions:**
1. 📊 **Build** a portfolio of learning reports
2. 🎯 **Track** your progression from beginner → intermediate → advanced
3. 🧠 **Review** mentor observations to understand your learning patterns
4. 🎓 **Celebrate** your growth and accomplishments

### Example Report Section: Resource Arsenal

Every report includes a comprehensive resource arsenal, web-verified and annotated:

```markdown
## 📖 Your Complete Resource Arsenal

### 📄 Official Documentation
| Resource | URL | Why it matters |
|----------|-----|----------------|
| ⭐ MDN Async/Await Guide | [URL] | The most authoritative reference for Promise/async syntax |
| JavaScript.info Promises | [URL] | Excellent visual explanations and interactive examples |

### 📚 Books
| Title | Author | Free/Paid | Why read it |
|-------|--------|-----------|-------------|
| ⭐ You Don't Know JS Yet: Async & Performance | Kyle Simpson | Paid | Deep dive into how async really works under the hood |
| 💎 Exploring Async JavaScript | Etienne Marais | Free PDF | Often overlooked but excellent on practical patterns |

### 🐙 GitHub Repositories
| Repo | Stars | Tag | Why it's great |
|------|-------|-----|----------------|
| ⭐ promises-aplus/promises-spec | ~7k | Essential | The standard that all Promise implementations follow |
| 💎 getify/You-Dont-Know-JS | ~180k | Underrated | Comprehensive book examples you can run locally |

### 📬 Newsletters & Sites
| Name | URL | Frequency | Best for |
|------|-----|-----------|---------|
| ⭐ JavaScript Weekly | [URL] | Weekly | Staying current with JS ecosystem news |
| 💎 Daily.dev | [URL] | Daily | Discovering underrated technical articles |
```

---

## Resource Engine

### What is the Resource Engine?

The Resource Engine is a sophisticated system for curating, verifying, and presenting learning resources. Every resource in your session report is:

✅ **Web-verified** — The URL is checked to be live and correct  
✅ **Level-matched** — Chosen specifically for your experience level  
✅ **Goal-aligned** — Selected to support YOUR stated learning goal  
✅ **Annotated** — Includes one sentence explaining WHY it's useful for you  
✅ **Quality-tiered** — Marked with ⭐ Essential, 💎 Underrated, 🔬 Advanced, etc.

### Resource Categories Included

1. **Official Documentation** — Authoritative docs for frameworks, libraries, standards
2. **Research Papers** — Latest academic papers from arXiv, Semantic Scholar, Google Scholar (with citations)
3. **Books** — Both free and paid books, with availability links
4. **GitHub Repositories** — Active projects, tutorials, and reference implementations
5. **Blogs & Long-form Writing** — In-depth technical articles from respected authors
6. **Newsletters & Sites** — Regular content feeds for staying current
7. **Frontier Lab Guides** — Whitepapers from OpenAI, Anthropic, Google, Meta, Microsoft Research
8. **Major Organization Guides** — Tutorials and guides from Google, AWS, Microsoft, and others
9. **Websites & Interactive Tools** — Playgrounds, visualizers, and interactive learning tools
10. **Free & Underrated Courses** — Full courses (many free), including fast.ai, MIT OpenCourseWare, Coursera audits
11. **Twitter/Threads Influencers** — People actively sharing insights on your topic
12. **Reddit Communities** — Active subreddits relevant to your learning goal
13. **Bonus/Miscellaneous** — Other genuinely valuable resources discovered during research

### How the Mentor Sources Resources

1. **Web-searches** before compiling any resource list
2. **Verifies links** are live and URLs are correct
3. **Checks recency** of publication (recent for fast-moving topics)
4. **Confirms relevance** to YOUR specific topic, level, and goal
5. **Avoids padding** — includes only genuinely useful items
6. **Surfaces underrated gems** — 💎 items you wouldn't find on "best of" lists

---

## FAQ

### ❓ How do I activate the skill?

Use any phrase expressing learning intent:
- *"I want to learn [topic]"*
- *"Teach me about [topic]"*
- *"Help me understand [topic]"*
- *"I'm curious about [topic]"*
- *"Explain [topic] to me"*

The skill will automatically detect your intent and begin the session.

---

### ❓ Can I use the skill for any topic?

**Yes!** The skill works for:
- ✅ Programming languages and frameworks
- ✅ Algorithms and data structures
- ✅ Databases and system design
- ✅ Cloud platforms and DevOps
- ✅ Machine learning and AI
- ✅ Web development
- ✅ Mobile development
- ✅ Soft skills (communication, leadership, project management)
- ✅ Any technology or concept

If a topic doesn't match a pre-built playbook, the mentor uses its general approach to structure the session.

---

### ❓ How long do sessions really take?

**~15 minutes** is the target for a complete session, but:
- ✅ Fast learners may finish in 10–12 minutes
- ⏱️ Deeper engagement may stretch to 18–20 minutes
- 📚 You can always extend and do follow-up sessions

The mentor will always complete the session report (PHASE 5) regardless of time.

---

### ❓ Can I ask for more resources?

**Absolutely!** Say:
- *"Can you give me more resources on [specific topic]?"*
- *"Find me research papers on [topic]"*
- *"What are the best [category] for [topic]?"*

The Resource Engine activates and provides a curated list of additional resources with web verification.

---

### ❓ What if I already know the topic?

The mentor will:
1. Detect your knowledge level during assessment
2. Skip beginner explanations
3. Jump straight to advanced concepts
4. Ask deeper probing questions
5. Engage you as a peer-level discussion

You can also tell the mentor directly: *"I already know the basics — focus on [advanced area]"*

---

### ❓ Can I do multiple sessions on the same topic?

**Yes!** Each session is independent and will:
- Generate a separate report
- Build on knowledge from previous sessions
- Go deeper or explore different aspects
- Help you progress from Beginner → Intermediate → Advanced

Your reports create a complete learning journey map.

---

### ❓ What if I get stuck during the hands-on task?

The mentor will:
1. 🤔 Ask clarifying questions about where you're stuck
2. 💡 Provide hints (not full solutions)
3. 🔍 Help you debug or think through the problem
4. 📚 Reference concepts covered earlier in the session
5. ✅ Guide you to the right approach

You're never left stranded — the mentor adapts support to get you unstuck.

---

### ❓ Can I see session reports from other people?

**No** — session reports are personalized to each learner. They:
- Reference your specific answers and goals
- Contain mentor observations about YOUR learning style
- Include resources chosen specifically for YOUR level

However, you can share reports if you want to!

---

### ❓ Where are my session reports saved?

Reports are saved to:
- Your **current working directory** by default
- Or a `/learning-reports/` folder if it exists in your project

Filename format:
```
YYYY-MM-DD_DayOfWeek_[topic-slug]_learning-session.md
```

Example: `2025-07-18_Friday_python-async_learning-session.md`

---

### ❓ What tools does the mentor use?

The mentor actively uses:

| Tool | When Used | Example |
|------|-----------|---------|
| **Code Execution** | Teaching programming | Run your code live, show output |
| **Web Search** | Current info needed | Find latest docs, research papers |
| **File Creation** | Saving reports | Generate markdown session reports |
| **Environment Analysis** | Context needed | Understand your workspace setup |

All tools enhance the learning experience without requiring setup from you.

---

### ❓ Can I give feedback on my session?

Session reports are snapshots in time, but you can:
1. 📝 Edit or annotate your own reports
2. 💬 Ask the mentor follow-up questions anytime
3. 🔄 Schedule another session to explore different aspects
4. 📧 Share feedback directly

---

### ❓ Is my data private?

Yes:
- ✅ Session reports are **stored locally** in your workspace
- ✅ No data is sent to external servers (beyond web searches for resources)
- ✅ You control access to your reports
- ✅ You can delete reports anytime

---

## Contributing

### How to Contribute

We welcome contributions! Ways you can help:

1. **📝 Add Topic Playbooks** — Expand `references/topic-playbooks.md` with new learning arcs
2. **🐛 Report Issues** — Find bugs? Open an issue with details
3. **💡 Suggest Features** — Ideas for improving sessions? We'd love to hear them
4. **✍️ Improve Documentation** — Help make guides clearer and more comprehensive
5. **🧪 Share Your Reports** — Real session reports help us improve (with your permission)
6. **🌍 Translate** — Help make the skill accessible in other languages

### Development Workflow

1. **Fork** this repository
2. **Create a feature branch:** `git checkout -b add/topic-playbook-rust`
3. **Make changes** and test in your Agentic IDE
4. **Commit with clear messages:** `git commit -m "Add Rust learning playbook"`
5. **Push** and open a **Pull Request**
6. **We'll review** and merge with feedback

### Code of Conduct

- Be respectful and inclusive
- Provide constructive feedback
- Give credit to contributors
- Follow the existing style and structure

---

## Frequently Asked Questions (Advanced)

### How are questions ordered during assessment?

The mentor **adapts question order** based on your topic:
- Questions are selected from the question bank (Q1–Q7)
- Order is optimized for natural conversation flow
- Follow-up probes dig deeper based on your answers
- NOT a rigid form — sounds conversational

---

### How does the mentor adapt to different learning styles?

**Conceptual learners:**
- Start with theory and high-level concepts
- Use analogies and comparisons
- Build to examples
- Task comes later, after concepts are solid

**Hands-on learners:**
- Jump into examples immediately
- Theory explained through code
- Concepts emerge from practice
- Task comes early, theory follows

**Mixed learners:**
- Balance both approaches
- Start with brief concept, then code example
- Cycle between theory and practice

---

### What happens if my topic is extremely niche?

The mentor will:
1. ✅ Use general mentoring structure even without a specific playbook
2. ✅ Web-search for current information on your niche topic
3. ✅ Adapt the core learning approach to your niche
4. ✅ Still deliver concepts + hands-on task + resources
5. ✅ Generate a complete session report

Niche topics are actually great opportunities for deep, focused learning!

---

### Can the mentor teach soft skills?

**Yes!** Try:
- *"Teach me how to give better presentations"*
- *"Help me understand effective leadership"*
- *"I want to get better at negotiation"*

The mentor will:
- ✅ Adapt the structure for soft skills
- ✅ Use real-world scenarios and examples
- ✅ Practice through role-play or analysis
- ✅ Provide resources on communication, psychology, business skills

---

### What's the difference between PHASE 2 and PHASE 3?

| PHASE 2 | PHASE 3 |
|---------|---------|
| **Knowledge probe** — test current understanding | **Core learning** — teach new concepts |
| Optional, skip for beginners | Mandatory, heart of session |
| Ask 1–2 diagnostic questions | Deliver 3–4 key concepts |
| Reveal knowledge gaps | Fill those gaps + hands-on task |
| 2 minutes | 7 minutes |

---

## License

This skill is released under the **MIT License** — feel free to use, modify, and share!

```
MIT License

Copyright (c) 2025 [Your Name / Organization]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
```

---

## Support & Community

- 🐛 **Found a bug?** [Open an issue](https://github.com/abm1119/agentic-learning-mentor/issues)
- 💡 **Have a feature request?** [Start a discussion](https://github.com/abm1119/agentic-learning-mentor/discussions)
- 🌟 **Like this skill?** [Star the repo](https://github.com/abm1119/agentic-learning-mentor)
- 👥 **Want to contribute?** [See CONTRIBUTING.md](CONTRIBUTING.md)

---

## Acknowledgments

- **Inspiration:** Best practices from Socratic mentoring, spaced repetition learning, and active recall
- **Structure:** Informed by educational psychology and adult learning principles
- **Tools:** Built on agentic AI capabilities (code execution, web search, file creation)

---

## Quick Links

| Link | Purpose |
|------|---------|
| [SKILL.md](SKILL.md) | Complete technical skill definition |
| [report-template.md](references/report-template.md) | Session report template |
| [resource-engine.md](references/resource-engine.md) | Resource curation logic |
| [topic-playbooks.md](references/topic-playbooks.md) | Pre-built learning arcs |
| [GitHub Issues](https://github.com/abm1119/agentic-learning-mentor/issues) | Report bugs & request features |

---

## What's Next?

1. ✅ **Install** the skill following the [Installation](#installation) section
2. 🎓 **Start your first session** with a learning trigger phrase
3. 📖 **Read your session report** to review what you learned
4. 🚀 **Follow the next steps** in your report
5. 🔁 **Schedule follow-up sessions** to deepen your knowledge

**Happy learning!** 🚀

---

<div align="center">

**Built with ❤️ for lifelong learners**

[GitHub](https://github.com/abm1119/agentic-learning-mentor) • [Issues](https://github.com/abm1119/agentic-learning-mentor/issues) • [Discussions](https://github.com/abm1119/agentic-learning-mentor/discussions)

</div>
