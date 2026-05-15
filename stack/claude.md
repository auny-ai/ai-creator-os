---
title: Claude
description: "AI assistant by Anthropic. Acts as chief of staff in ai-creator-os — reads the vault before every session, executes tasks mid-session, writes outputs back, and connects to every other tool in the stack via MCP."
tags: [claude, anthropic, ai-assistant, mcp, chief-of-staff]
---

# Claude 🤖

Claude is an AI assistant made by Anthropic. In this system it acts
as a chief of staff — reading your vault before every session,
executing tasks mid-session, and writing outputs back to your vault
when done. It connects to every other tool in this stack via MCP.

---

## how you can use it

- writing and editing content across any format or platform
- research, summarization, and trend analysis
- building and documenting workflows
- managing projects via MCP-connected tools (Linear, Typefully, etc.)
- thinking through decisions, strategies, and creative directions
- writing code, building tools, and creating systems

Claude works best when it has context. the more it knows about your
goals, voice, and system upfront — the less you have to explain
every session.

---

## setup

1. create an account at [claude.ai](https://claude.ai)
2. start a Project — this gives Claude persistent instructions
   across all sessions in that project
3. write a system prompt that tells Claude who you are, what you're
   building, and how you want it to operate
   (see [session-protocols/01_session_start.md](../session-protocols/01_session_start.md) for a template)
4. connect your Obsidian vault via MCP
   (see [mcp-setup/setup_guide.md](../mcp-setup/setup_guide.md))

---

## how i use it

every session starts with Claude reading four vault files:
the master index, the session start protocol, the workflow system,
and the content pillars. from that read, it knows what i'm building,
what my voice sounds like, what tools i have available, and what's
currently open in Linear.

a content session looks like this:
1. Claude reads the content manual and working manual from the vault
2. i drop a trending post, article, or topic
3. Claude analyzes it against my pillars and voice
4. we build a thread, batch, or standalone post together
5. Claude drafts directly to Typefully via MCP — no copy-paste

a music session looks like this:
1. Claude reads the music manual from the vault
2. i describe a sound direction or emotional register
3. Claude writes Suno prompts calibrated to my prompt style
4. i generate, review, pick tracks
5. Claude handles distribution prep — hyperfollow pages,
   streaming links, ASCAP registration notes

the system prompt that makes all of this work is in
[session-protocols/01_session_start.md](../session-protocols/01_session_start.md)
