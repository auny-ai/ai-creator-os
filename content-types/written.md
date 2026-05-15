---
title: Written Content (Content Type)
description: "End-to-end workflow for text content — X posts, threads, newsletters, articles. Claude drafts, Typefully schedules, Beehiiv handles the newsletter. The vault connects them by storing voice, formats, and history."
tags: [written-content, content-type, x, newsletter, typefully, beehiiv]
---

# written content ✍️

written content covers everything text-based — X posts, threads,
newsletters, and articles. in this system Claude handles the
drafting, Typefully handles scheduling, and Beehiiv handles
the newsletter. the vault is what connects them — it stores
your voice, your formats, and your history so nothing has to
be re-explained.

---

## tools in this workflow

| tool | role |
|------|------|
| Claude | drafts all written content, reads vault context first |
| Obsidian | stores voice, formats, content history, session protocols |
| Typefully | schedules and publishes posts across platforms |
| Beehiiv | newsletter sending, subscriber management, shop |
| Grok (MCP) | real-time X trend research mid-session |

→ [Claude](../stack/claude.md) · [Obsidian](../stack/obsidian.md) ·
[Typefully](../stack/typefully.md) · [Beehiiv](../stack/beehiiv.md) ·
[Grok](../stack/grok.md)

---

## X posts and threads

**the workflow:**

1. Claude reads your content manual and recent post history
   from the vault
2. research pass — Grok MCP searches what's trending across
   your content pillars right now
3. Claude filters results against your voice and formats,
   states a content direction
4. posts and threads are drafted — format rotation enforced
   (no same format back to back), comment-pulling question
   included in every post that isn't a one-liner
5. Claude drafts directly to Typefully via MCP — no copy-paste

**what to build in your vault first:**
- a content manual (your voice rules, formats, pillars)
- a working manual (what's currently active, what to avoid)
- a session log (what was posted recently)

template: [templates/session_log.md](../templates/session_log.md)

---

## newsletter

**the workflow:**

1. Claude reads the newsletter manual from the vault
2. topic and angle identified — often pulled from a thread
   that performed well that week
3. Claude drafts the full issue in the newsletter voice
   (different register from X — longer, more structured)
4. review and edit in Beehiiv
5. schedule or send

**the content loop:**
X threads → newsletter deep dives → X posts promoting the issue
→ newsletter topics suggest new threads. the two systems feed
each other.

---

## articles and long-form

**the workflow:**

1. identify the topic — usually a workflow or system worth
   documenting in depth
2. Claude drafts in the technical voice (evidence-forward,
   specific, no buzzwords) — see [stack/claude.md](../stack/claude.md)
3. publish to GitHub, newsletter, or both
4. X thread version drafted as a companion piece

the article that became this repo started as an X thread.
most long-form content in this system starts that way.
