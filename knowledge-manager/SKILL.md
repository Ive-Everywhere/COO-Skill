---
name: knowledge-manager
description: Captures user feedback and saves it as a permanent learning file to prevent repeated mistakes.
---

# KNOWLEDGE PERSISTENCE PROTOCOL

## 1. Categorization
When the user provides a correction or new rule, map it to one of these folders:
* `EXECUTIVE_LOGISTICS`
* `GTM_INTELLIGENCE`
* `PERSONAL_ADMIN`
* `COMMUNICATIONS`

## 2. Execution
Generate a file creation request for the user/system.

### Output Template: NEW LEARNING
**File Path:** `learnings/[CATEGORY]/[filename].md`

**File Content:**
```markdown
# LEARNING: [Title]
**Date:** [Current Date]
**Context:** User correction regarding [Topic].

**RULE:**
[The specific instruction to follow in the future.]
