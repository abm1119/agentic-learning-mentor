# Topic Playbooks

Pre-built learning arcs for the most commonly requested topics.
When a user's topic matches one of these, use the corresponding playbook to structure PHASE 3.
These are guides, not scripts — adapt freely based on the learner profile.

---

## TABLE OF CONTENTS

1. Python
2. JavaScript / TypeScript
3. React
4. System Design
5. Machine Learning / AI
6. Git & Version Control
7. SQL & Databases
8. Docker & Containers
9. REST APIs
10. Data Structures & Algorithms
11. Rust
12. Cloud (AWS / GCP / Azure)
13. Linux / Command Line
14. LLMs & Prompt Engineering
15. Web Scraping
16. [Generic Template — use for any other topic]

---

## 1. PYTHON

**Core arc:** Syntax → Data Types → Functions → OOP → Standard Library → Ecosystem

**Beginner path:**
- Variables, types, f-strings
- Lists, dicts, loops
- Functions and scope
- Task: "Write a script that reads a list of numbers, filters the odds, and prints the sum"

**Intermediate path:**
- List comprehensions, generators
- Decorators, context managers
- Error handling patterns
- Task: "Refactor this script to use generators and proper exception handling"

**Advanced path:**
- Async/await, concurrency models
- Type hints, dataclasses
- Performance profiling
- Task: "Profile this code and rewrite the bottleneck using asyncio or multiprocessing"

**Live demo ideas:** Run a quick script in the IDE, show `f-strings`, demonstrate `enumerate()` and `zip()`

---

## 2. JAVASCRIPT / TYPESCRIPT

**Core arc:** Types → Async → DOM/Node → Modules → TypeScript layer

**Beginner path:**
- `const`/`let`, arrow functions
- Array methods (`map`, `filter`, `reduce`)
- Promises basics
- Task: "Fetch data from a public API and log specific fields"

**Intermediate path:**
- `async/await`, error handling
- Closures and scope
- ES modules
- Task: "Build a small utility module with typed exports"

**Advanced path:**
- TypeScript generics, utility types
- Event loop mechanics
- Performance and memory patterns
- Task: "Type this JavaScript module fully and add a generic cache utility"

---

## 3. REACT

**Core arc:** Components → Props → State → Effects → Patterns

**Beginner path:**
- JSX, functional components
- Props and component composition
- useState basics
- Task: "Build a counter with increment/decrement buttons"

**Intermediate path:**
- useEffect, dependency arrays
- Lifting state, prop drilling vs context
- Custom hooks
- Task: "Extract a data-fetching custom hook from this component"

**Advanced path:**
- Performance (useMemo, useCallback, lazy)
- State management patterns
- Testing components
- Task: "Identify and fix the performance bottleneck in this component tree"

---

## 4. SYSTEM DESIGN

**Core arc:** Requirements → Components → Scaling → Trade-offs

**Beginner path:**
- What is a system? Clients, servers, databases
- HTTP and APIs at a high level
- Reading a simple architecture diagram
- Task: "Sketch the architecture for a URL shortener on paper / markdown"

**Intermediate path:**
- CAP theorem, consistency models
- Load balancing, caching layers
- SQL vs NoSQL choice
- Task: "Design the data layer for a social feed — justify your database choice"

**Advanced path:**
- Distributed systems patterns (sagas, CQRS, event sourcing)
- Failure modes and resilience
- Cost and latency tradeoffs
- Task: "Given these requirements and 10M DAU, design and critique the messaging service"

---

## 5. MACHINE LEARNING / AI

**Core arc:** Concepts → Data → Training → Evaluation → Deployment

**Beginner path:**
- What is ML? Supervised vs unsupervised
- Features, labels, training data
- What a model actually is
- Task: "Describe what data you'd collect to predict [simple scenario]"

**Intermediate path:**
- Overfitting, validation, cross-validation
- Common algorithms (decision trees, linear regression, neural nets at high level)
- Evaluation metrics
- Task: "Given this dataset description, pick a model and explain why"

**Advanced path:**
- Transformers architecture
- Fine-tuning vs RAG vs prompt engineering
- MLOps, model monitoring
- Task: "Design a RAG pipeline for this use case — what are the failure modes?"

---

## 6. GIT & VERSION CONTROL

**Core arc:** Init → Commit → Branch → Merge → Collaborate → Advanced

**Beginner path:**
- What is version control and why
- `init`, `add`, `commit`, `log`
- Task: "Init a repo, make 3 commits with meaningful messages, view the log"

**Intermediate path:**
- Branching strategy, `merge` vs `rebase`
- Resolving conflicts
- Task: "Create a feature branch, make changes, merge back, resolve a conflict"

**Advanced path:**
- `reflog`, `cherry-pick`, `bisect`
- Interactive rebase for clean history
- Git hooks and CI integration
- Task: "Use `git bisect` to find which commit introduced a bug in this history"

---

## 7. SQL & DATABASES

**Core arc:** Tables → Queries → Joins → Aggregates → Indexes → Design

**Beginner path:**
- What is a relational DB, tables, rows, columns
- `SELECT`, `WHERE`, `ORDER BY`
- Task: "Write a query to find all users who signed up in the last 30 days"

**Intermediate path:**
- JOINs (INNER, LEFT, RIGHT)
- Aggregates (`GROUP BY`, `HAVING`)
- Subqueries
- Task: "Write a query to get the top 5 products by revenue per category"

**Advanced path:**
- Query execution plans, `EXPLAIN`
- Index design and trade-offs
- Transactions and isolation levels
- Task: "Optimise this slow query — read the execution plan and add appropriate indexes"

---

## 8. DOCKER & CONTAINERS

**Core arc:** Why containers → Images → Containers → Compose → Production

**Beginner path:**
- VMs vs containers
- `pull`, `run`, `ps`, `stop`
- Task: "Run a PostgreSQL container and connect to it"

**Intermediate path:**
- Writing a Dockerfile
- Layers and caching
- docker-compose for multi-service apps
- Task: "Containerise this Node app and add a Postgres service with compose"

**Advanced path:**
- Multi-stage builds, image size optimisation
- Networking and volumes
- Kubernetes intro
- Task: "Reduce this Docker image from 800MB to under 150MB using multi-stage builds"

---

## 9. REST APIs

**Core arc:** HTTP → Resources → Methods → Status codes → Auth → Design

**Beginner path:**
- HTTP methods (GET, POST, PUT, DELETE)
- Status codes and what they mean
- JSON request/response
- Task: "Use curl or fetch to call a public API and parse the response"

**Intermediate path:**
- RESTful resource design
- Authentication (API keys, Bearer tokens, OAuth flow)
- Pagination patterns
- Task: "Design the REST API for a todo app — write out the endpoints and payloads"

**Advanced path:**
- Idempotency, versioning, rate limiting
- OpenAPI / Swagger documentation
- REST vs GraphQL vs gRPC trade-offs
- Task: "Review this API design and find 3 violations of REST principles — fix them"

---

## 10. DATA STRUCTURES & ALGORITHMS

**Core arc:** Complexity → Arrays/Lists → Hash Maps → Trees → Graphs → Patterns

**Beginner path:**
- Big-O intuition (not the maths)
- Arrays vs linked lists
- Task: "Reverse a string without using a built-in reverse function"

**Intermediate path:**
- Hash maps and their use cases
- Binary search
- Recursion
- Task: "Two Sum problem — first brute force, then optimise with a hash map"

**Advanced path:**
- Trees (BST, traversals)
- Graph search (BFS/DFS)
- Dynamic programming intro
- Task: "Implement level-order traversal of a binary tree iteratively"

---

## 11. RUST

**Core arc:** Ownership → Borrowing → Structs/Enums → Error handling → Traits → Concurrency

**Beginner path:**
- Why Rust? Memory safety without GC
- Variables, mutability, basic types
- Ownership in simple terms
- Task: "Write a function that takes a string and returns its length without transferring ownership"

**Intermediate path:**
- Borrowing and lifetimes
- `Result` and `Option`, `?` operator
- Structs, impls, traits
- Task: "Implement a simple stack with push/pop using a Vec and proper error handling"

**Advanced path:**
- Lifetimes in depth
- Concurrency with threads and channels
- Async Rust (tokio)
- Task: "Convert this sync HTTP client code to async using tokio"

---

## 12. CLOUD (AWS / GCP / AZURE)

**Core arc:** Core services → Compute → Storage → Networking → Serverless → Cost

**Beginner path:**
- What cloud is and why it matters
- The three major providers and their rough equivalents
- S3/GCS/Blob storage concepts
- Task: "Describe how you'd host a static website on cloud storage"

**Intermediate path:**
- EC2/GCE/VMs vs Lambda/Cloud Functions
- IAM and permissions
- VPCs and basic networking
- Task: "Design the IAM roles for a three-tier web app with least-privilege access"

**Advanced path:**
- Infrastructure as Code (Terraform/CDK)
- Cost optimisation strategies
- Multi-region architecture
- Task: "Rewrite this CloudFormation stack in Terraform and add auto-scaling"

---

## 13. LINUX / COMMAND LINE

**Core arc:** Navigation → Files → Permissions → Processes → Scripting → Admin

**Beginner path:**
- `ls`, `cd`, `pwd`, `mkdir`, `rm`
- Reading files: `cat`, `less`, `head`, `tail`
- Task: "Navigate to the home directory, create a folder structure, and write a file using the CLI"

**Intermediate path:**
- Pipes and redirection (`|`, `>`, `>>`, `2>&1`)
- `grep`, `awk`, `sed` basics
- File permissions and `chmod`
- Task: "Write a one-liner to find all `.log` files modified in the last 24h and count lines"

**Advanced path:**
- Shell scripting (bash)
- Process management (`ps`, `kill`, `top`, `systemd`)
- Cron jobs, environment variables
- Task: "Write a bash script that backs up a directory, compresses it, and logs the result"

---

## 14. LLMs & PROMPT ENGINEERING

**Core arc:** How LLMs work → Prompting techniques → RAG → Fine-tuning → Agents

**Beginner path:**
- What an LLM is at a high level (not deep ML)
- Tokens, context windows
- Basic prompting: role, task, format
- Task: "Write 3 versions of the same prompt — poor, okay, and excellent — for the same task"

**Intermediate path:**
- Few-shot, chain-of-thought, system prompts
- Temperature and sampling
- RAG architecture
- Task: "Design a RAG pipeline for a customer support bot — what's in the knowledge base?"

**Advanced path:**
- Fine-tuning vs RAG trade-offs
- Agentic patterns (tool use, ReAct, multi-agent)
- Evals and measuring prompt quality
- Task: "Write a system prompt for an AI coding assistant — then break it with adversarial input and patch it"

---

## 15. WEB SCRAPING

**Core arc:** HTML structure → requests → parsing → JavaScript sites → ethics/legality

**Beginner path:**
- How HTML is structured (DOM, tags, classes, IDs)
- `requests` + `BeautifulSoup` basics
- Task: "Scrape the titles and links from a public news page"

**Intermediate path:**
- Handling pagination
- Headers, cookies, rate limiting
- Parsing tables
- Task: "Scrape a multi-page result set and export to CSV"

**Advanced path:**
- Playwright/Selenium for JS-rendered pages
- Anti-bot detection and respectful scraping
- Scrapy for scale
- Task: "Rewrite this requests scraper to handle JS-rendering with Playwright"

---

## GENERIC TEMPLATE (use for any topic not listed above)

**Core arc:** What is it → Why it matters → Core concepts → Hands-on → Next steps

**Beginner path:**
- Define the topic in plain language
- Give a real-world analogy
- Cover the 2–3 most fundamental concepts
- Task: "Apply concept #1 in a small, concrete exercise"

**Intermediate path:**
- Go deeper on the most interesting/powerful aspect
- Show a real-world use case
- Highlight common mistakes
- Task: "Solve a mid-complexity problem using the concepts covered"

**Advanced path:**
- Edge cases, limitations, and nuances
- Compare with alternatives
- Point to cutting-edge developments
- Task: "Design or architect something using the topic — justify decisions"

**Questions to ask for unfamiliar topics:**
- "What made you interested in [topic] specifically?"
- "Have you seen it used somewhere? Where?"
- "What do you think it does — even a rough guess?"
