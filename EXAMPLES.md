# Usage Examples

`.decisions` is flexible. Teams may organize it however they prefer.

Below are common patterns.

---

## Small Project


.decisions/  
project.md  
log.md


Example:

```
2026-03-10
[RK] Dropped onboarding flow from v1.  
Adds weeks of work, not needed to validate the idea.
```

---

## Session Logging


.decisions/  
sessions/  
2026-03-12.md  


Example:
```
2026-03-12  
[SK] Switched to local storage over a database.  
No accounts in v1, database was overkill.
```

---

## Team Structure


.decisions/  
project.md  
sessions/  
frontend/  
backend/  


Example:
```
2026-03-13 
[JN] Reworked hero layout.
Improves CTA visibility.
```

---

## Architecture Decisions


.decisions/  
architecture/  
api.md  


Example:  
```
2026-03-14 
[RK] Using REST instead of GraphQL.  
Reason: simpler client integration.
```
