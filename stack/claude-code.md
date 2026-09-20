---
title: Claude Code
description: "The build surface. Where every MCP server, website and automation in this system was written, with no prior coding background. Added to the stack after v1."
tags: [claude-code, building, mcp-servers, cloudflare-workers, no-code-background]
---

# Claude Code 💻
### the build surface

**not in v1 of this repo.** v1 described a system you *use*. Claude Code is
how the system got *built*.

---

## what it is

Claude in a terminal, with the ability to read and write files, run commands,
and hold a whole repo in context.

## what i build with it

- every custom MCP server in this system
- aunysillyme.com and auny.media, from scratch
- the scheduled jobs that run without me
- the audio mastering pipeline
- the HTML-to-video renderer

## the honest part

i had no prior coding background when i started. that is not a
"anyone can do it" line. it is a specific claim about what changed: i can
describe what a thing should do precisely, and precision is most of the job.

what i still had to learn, because no model does it for you:

- **what "done" means.** a model will tell you it finished. the artifact tells
  you whether it did. check the artifact.
- **that a green test can be meaningless.** before trusting a passing test,
  break the code on purpose and confirm the test goes red. if it stays green,
  the test was never testing anything.
- **that a second model has to review the first.** see [mcps/codex.md](../mcps/codex.md).

---

## the loop

1. describe the thing in plain language, including what it must never do
2. let it build
3. make it prove the thing works, with output you can read
4. hand it to a different model to attack
5. fix what reproduces, keep a test per fix

---

## where the vault fits

Claude Code reads the same vault as everything else. that means a build
session already knows the naming conventions, the routing rules, and what i
decided last month and why.

the vault is not documentation *about* the system. it is an input *to* it.
