---
title: Session Log Template
description: "Single rolling log file every Claude session writes to. Makes context portable — changes made in one conversation are visible in the next because Claude reads this file first. One file, newest entries at top."
tags: [template, session-log, context, claude]
---

# session log template

the session log is the single file every Claude session writes
to. it's what makes context portable — changes made in one
conversation are visible in the next because Claude reads this
file first.

keep one rolling session log. append to it after every session.
don't create a new file per session — one file, newest entries
at the top.

---

## template

```markdown
# session log
last updated: [date]

---

## [date] — [session type / what was worked on]

**what happened:**
- [key action or output from this session]
- [new file created or updated]
- [decision made]

**vault changes:**
- [file name] → [what changed]

**tasks:**
- closed: [task ID + name]
- opened: [task ID + name]
- in progress: [task ID + name]

**carry forward:**
- [anything Claude should know at the start of the next session]

---
```

---

## example

```markdown
# session log
last updated: May 13, 2026

---

## May 13, 2026 — github repo build (ai-creator-os)

**what happened:**
- built README.md and TOOLS.md for auny-ai/ai-creator-os
- built all 9 /stack files
- planned /content-types folder (written, art, music, video)
- added News-Reactive Educational Thread format to content manual
- Suno affiliate link added to all_links.md

**vault changes:**
- 📐 Protocols/all_links.md → new affiliate link added
- ✍️ Content & Brand/content_manual.md → new format added
- 📐 Protocols/01_session_start.md → external material rule added
- 🐙 GitHub/github_strategy.md → stack file format documented

**tasks:**
- opened: AUN-XXX — build ai-creator-os repo files

**carry forward:**
- /session-protocols, /templates, /mcp-setup, /vault-structure,
  /content-system still to build
```
