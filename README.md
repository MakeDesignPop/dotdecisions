# .decisions

Code has git.  
Decisions have .decisions/

A lightweight convention for preserving the reasoning behind how a project evolves.

Codebases track implementation and history well, but the reasoning behind decisions often disappears.

```
src/        → implementation
tests/      → verification
.git/       → history
.decisions/ → reasoning
```
`.decisions` introduces a simple folder inside a repository where short notes capture *why* choices were made.

These notes are intentionally small.  
1–5 lines is usually enough.  
They capture reasoning while it is fresh, creating a permanent memory for the project.  
Humans and AI tools can both read and write them.  

---

## The Problem

Reasoning behind decisions usually lives in:

- chat conversations
- issue threads
- commit messages
- someone's memory

Weeks later the context is gone.

AI-assisted development makes this worse. Much of the reasoning happens in temporary chats that are never preserved with the code.

---

## The Idea

`.decisions` is a folder inside your repository where short notes capture *why* choices were made.

```
.decisions/
  project.md
  log.md
```

Entries are intentionally small. 1–5 lines is usually enough.
Humans and AI tools can both read and write them.

---

## Core Rules

1. A project may include a `.decisions/` folder
2. Files inside are Markdown
3. Entries should be short — 1–5 lines recommended
4. Humans or AI may write entries
5. No required structure

---

## Philosophy

Short reasoning notes, not documentation.
If you're writing more than a few lines, you're documenting — not deciding.

---

## Why Not Just Use AI Memory?

AI systems are powerful for reasoning, but long-term memory inside models is temporary and costly.

Repositories already provide durable storage.

By keeping reasoning inside the project:

- the context travels with the code
- future developers understand decisions
- future AI tools can read the reasoning

A repository may live for decades.

`.decisions` ensures the reasoning lives with it.

---

## Examples

**project.md** — written once at the start

```
Purpose: task management tool
Stack: Next.js, Postgres
Constraints: must work without an account, fast load time
Goal: simple over feature-rich
```

**log.md** — append as you go

```
2026-03-07
Dropped onboarding flow from v1.
Adds weeks of work, not needed to validate the idea.

2026-03-09
Switched to local storage over a database.
No accounts in v1, database was overkill.

2026-02-10
Removed animations.
Doubles UI work, not a launch priority.
```

---

## Status

Draft open convention. Work in progress.

Feedback and contributions welcome.

---

*A new practice for a new way of building.*
