---
title: Cloudflare Workers
description: "Where the custom MCP servers live. Moving them from local processes to hosted Workers is what made the vault reachable from every device and from scheduled jobs. Added to the stack after v1."
tags: [cloudflare, workers, hosting, mcp-servers, serverless]
---

# Cloudflare Workers ☁️
### where the servers live

**not in v1 of this repo.** v1's MCP servers ran as local processes on one
laptop. that works right up until you want the system anywhere else.

---

## what changed when they moved

| local process | hosted Worker |
|---|---|
| one machine | every device, plus the phone |
| only while the app is open | always |
| a scheduled job cannot reach it | a scheduled job can |
| no cost | still effectively no cost at this volume |

the phone one is bigger than it sounds. the vault stopped being something i
sat down at and became something i could reach from anywhere.

---

## what runs there

the vault door, X, X Ads, Google Workspace, Google Tasks, a client hub, a
calculator, and a cross-poster. full list in
[mcps/README.md](../mcps/README.md).

---

## the two rules i learned the hard way

**one deployment per server.** a local copy and a hosted copy of the same
server will drift. i rotated a key in one and left the other running on the
stale one, and spent a day blaming the vendor.

**fail closed.** if the thing that checks credentials cannot run, the server
must refuse, not serve. a server that opens up when its auth is
misconfigured is worse than one that is plainly broken, because it looks
fine.

---

## secrets

never in the code, never in the URL, never printed in a terminal. Workers has
its own secret store and that is where they go.

a key in a URL is a key in every log that URL touches.
