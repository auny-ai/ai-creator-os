---
title: MCP (Model Context Protocol)
description: "Open protocol that lets Claude connect directly to external tools and data sources mid-session. The infrastructure layer that turns Claude from a chat interface into an operating system."
tags: [mcp, model-context-protocol, anthropic, protocol, ai-tools]
---

# MCP (Model Context Protocol) 🔌

MCP is an open protocol that lets Claude connect directly to
external tools and data sources mid-session. instead of copying
and pasting between apps, Claude reads from and writes to your
tools in real time. in this system, MCP is what turns Claude from
a chat interface into an operating system.

---

## how you can use it

- connect your Obsidian vault so Claude reads and writes files
  without leaving the conversation
- connect Linear so Claude can create, update, and close issues
  mid-session
- connect Typefully so Claude drafts posts directly to your
  scheduling queue
- connect Beehiiv, Google Drive, Gmail, Calendly, and more
- build custom MCP servers for tools that don't have one yet

a full list of available MCP connectors is at
[claude.ai/integrations](https://claude.ai/integrations)

---

## setup

1. open Claude Desktop
2. go to Settings → Integrations
3. connect the tools you want Claude to access
4. for Obsidian specifically — there's no official MCP yet.
   use the setup guide in [mcp-setup/setup_guide.md](../mcp-setup/setup_guide.md) to
   connect your vault via a custom MCP server

---

## how i use it

i run two custom MCP servers for my vault:

**`auny-vault` (local)** — a Node.js server that connects directly
to my Obsidian vault on my filesystem. seven tools: list,
read, write, append, patch, search, delete. Claude uses this in
every desktop session — reads vault files before tasks, writes
session logs and new docs after.

**`auny-vault-hosted` (remote)** — the same seven tools deployed
as a hosted server. used on iPhone or any device without local
filesystem access. the vault syncs automatically so the hosted
version stays current.

beyond the vault, i have MCP connections for:
- **Linear** — Claude creates and closes issues mid-session
  without me touching the app
- **Typefully** — Claude drafts posts directly to my queue
- **Beehiiv** — Claude reads newsletter analytics and drafts
  mid-session
- **Grok** — custom MCP for X-native search and trend research
  without leaving Claude

the setup guide for the vault MCP is in [mcp-setup/setup_guide.md](../mcp-setup/setup_guide.md)
