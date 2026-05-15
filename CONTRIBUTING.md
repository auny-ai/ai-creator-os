# contributing

this repo documents my (Auny's) personal AI operating system, but it's MIT-licensed and meant to be forked, copied, and adapted. so contributions are welcome — within the kind of thing this project is.

---

## what makes sense to contribute

- **typo and grammar fixes** — anywhere in the docs
- **broken link fixes** — if you find one, open a PR
- **clarifications** — if a step is confusing, a setup instruction is incomplete, or a workflow has a gap, suggest a fix
- **MCP setup fixes for other platforms** — the setup guide is mac-first. if you got it working on windows or linux and want to add platform-specific notes, open a PR
- **new workflow examples in your own fork** — share a link in an issue, i'll feature it

## what doesn't make sense

- **rewriting the voice** — the lowercase casual prose is intentional. this isn't a corporate doc
- **adding tools to my stack docs** — `/stack/*.md` is what *i* use. fork it for your stack
- **expanding scope** — this is a personal operating system documented publicly, not a community wiki

---

## voice and style conventions

if you do contribute prose, match the existing voice:

- **lowercase headers** — `## what this is`, not `## What This Is`
- **direct, conversational tone** — no buzzwords, no corporate phrasing
- **specific over abstract** — "Claude reads your vault before every task" beats "leverages context-aware AI"
- **show, don't tell** — real examples beat theoretical capabilities
- **no exclamation marks**
- **em-dashes are fine. semicolons aren't**

---

## file structure rules

content files (`/stack/`, `/content-types/`, `/workflows/`, `/mcps/`, `/session-protocols/`, `/templates/`, `/vault-structure/`, `/mcp-setup/`, `/content-system/`) start with YAML frontmatter:

```yaml
---
title: Short Title
description: "One-sentence description of what the file does. Wrap in double quotes if it contains a colon."
tags: [tag1, tag2, tag3]
---
```

the `description` is what LLMs use to decide whether to surface the file for a query — so write it like a useful summary, not marketing copy.

snake_case for filenames inside subfolders. kebab-case for top-level workflow files (`music-release.md`, `content-batching.md`).

---

## how to propose a change

1. **small fix?** open a PR directly against `main`
2. **larger change or unsure?** open an issue first, describe what you want to change and why
3. **adapting this for your own use?** you don't need permission. fork it, build your own, share what you make if you want

---

## questions

[@AunySillyMe on X](https://x.com/AunySillyMe) — DMs open.
