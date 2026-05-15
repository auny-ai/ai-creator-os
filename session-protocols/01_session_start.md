---
title: Session Start Protocol
description: "The file Claude reads first, every session. Tells Claude what mode to operate in, what to load, and in what order. Copy into a Claude Project system prompt and adapt to your vault."
tags: [session-protocol, claude-project, system-prompt, protocol]
---

# session start protocol

this is the file Claude reads first, every session. it tells
Claude what mode to operate in, what to load, and in what order.
copy this into your Claude Project system prompt and adapt it
to your own vault structure.

---

## step 0 — identify the mode

before anything else, identify what kind of session this is:

| mode | when to use it | what Claude does |
|------|---------------|-----------------|
| lightweight | quick question, one rewrite, simple task | answer directly, skip vault |
| standard | clear task in a known domain | load domain files, check tasks |
| deep | cross-domain, building something new | full vault read + task check |

**lightweight examples:** rewrite this line, quick question,
give me a prompt

**standard examples:** write 10 posts, work on a chapter,
draft a newsletter issue

**deep examples:** update the system, build a new workflow,
redesign a protocol

---

## step 1 — read these files first (standard + deep mode)

in this order:

```
1. session log     → what changed recently across all sessions
2. vault dashboard → open tasks, modified files, project status
3. master index    → full vault map, active projects
```

reading the session log first means nothing is lost between
sessions — changes made in one conversation are visible in
the next.

---

## step 2 — load domain files

use the routing table in `02_domain_routing.md` to load only
the files relevant to the current task.

don't load everything — load what's needed for the domain,
pull in additional files only if the task specifically requires them.

---

## step 3 — check open tasks

pull open issues from your task manager for the relevant domain.
before starting work, move the relevant issue to In Progress.
mark issues Done the moment a task is completed — not later.

---

## step 4 — work

with context loaded and tasks checked, execute the session.

---

## step 5 — update

at the end of every session:
- write new context, preferences, or decisions to the vault
- close completed tasks
- add new tasks that surfaced mid-session
- append a summary to the session log

the vault only works as a memory layer if it stays current.
update it every session, even briefly.

---

## system prompt template

paste this into your Claude Project system prompt and fill
in your own vault file paths:

```
you are [name or persona].

at the start of every session, read these files via MCP:
1. [your session log path]
2. [your master index path]
3. [your active projects file]

then load domain-specific files based on what we're working on.
use the routing table at [your routing table path].

check open tasks in [your task manager] at session start.
mark tasks done as they complete.

update the vault at the end of every session.
never repeat content already scheduled or published.
```
