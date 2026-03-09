# .decisions Specification

`.decisions` is a lightweight convention for storing project reasoning inside a repository.

## Core Rules

1. Projects may include a `.decisions/` folder.
2. Files inside are Markdown.
3. Entries should be short (1–5 lines recommended).
4. Humans or AI tools may write entries.
5. No required structure.

## Recommended Files

.decisions/
project.md
log.md


### project.md

Written once.

Example:

Purpose: task management tool
Stack: Next.js, Postgres
Constraints: must work without an account, fast load time
Goal: simple over feature-rich

### log.md

Append-only reasoning stream.

Example:

2026-03-07
Dropped onboarding flow from v1.
Adds weeks of work, not needed to validate the idea.

2026-03-08
Switched to local storage over a database.
No accounts in v1, database was overkill.

2026-03-09
Removed animations.
Slows down the UI, ship fast first.
