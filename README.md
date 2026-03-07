# .decisions

Code has git.  
Decisions have .decisions.

A lightweight convention for preserving the reasoning behind how a project evolves.

```
src/        → implementation
tests/      → verification
.git/       → history
.decisions/ → reasoning
```

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

## Examples

**project.md** — written once at the start

```
Purpose: expense tracking app
Stack: React Native, SQLite
Constraints: must work offline, mobile first
Goal: simple over scalable
```

**log.md** — append as you go

```
2026-02-07
Removed caching layer.
Traffic too low to justify the complexity.

2026-02-09
Switched to a third-party auth library.
Not worth maintaining custom auth at this stage.

2026-02-10
Dropped dark mode from v1.
Doubles UI work, not a launch priority.
```

---

## Status

Draft open convention. Work in progress.

Feedback and contributions welcome.

---

*A new practice for a new way of building.*
