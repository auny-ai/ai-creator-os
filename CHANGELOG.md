# changelog

all meaningful updates to ai-creator-os are logged here.
built in public. the system evolves as the work does.

---

## v2.0.0 · September 2026

four months of drift, caught up in one pass. v1 described a system i used
inside one Claude window. this describes the system that actually runs now.

**corrected (v1 was wrong about these):**
- `codex` was listed as a custom MCP. it is a **CLI lane**, not an MCP server.
  [mcps/codex.md](./mcps/codex.md) now says so, and says what it is actually for.
- `remotion` was listed as live. it is **retired**, and the repo it pointed at
  is archived. [mcps/remotion.md](./mcps/remotion.md) explains what replaced it
  and why deterministic rendering mattered more than the framework.
- the MCP table linked all four servers to this docs repo instead of their own.

**added:**
- [stack/claude-code.md](./stack/claude-code.md): the build surface. every MCP
  server, site and automation in this system was written here, with no prior
  coding background.
- [stack/cloudflare.md](./stack/cloudflare.md): the servers moved from local
  processes to hosted Workers, which is what made the vault reachable from the
  phone and from jobs that run with nobody watching.
- [stack/model-routing.md](./stack/model-routing.md): which model gets which
  job, and the rule that pays for itself: whoever wrote the thing does not
  review the thing.
- [mcps/README.md](./mcps/README.md): rewritten. roughly fifteen servers now,
  split into hosted and local.

**updated:**
- [TOOLS.md](./TOOLS.md): the full stack, with a "what changed" note under each
  section that moved. images went to ChatGPT Image, design to Claude Design,
  Canva went from regular to rare. Stripe, Vercel, Adobe and the always-on box
  are new.
- [README.md](./README.md): repo tree, and a step 7 for when one window is not
  enough.

**the honest summary:** the thesis of v1 holds. a vault as the memory layer is
still the whole idea. what changed is that the system stopped being something i
sit down at and started being something that also runs while i am asleep.

---

## v1.0.0 · May 2026

initial release.

**what's in v1:**
- full stack documentation (9 tools)
- content-type workflows (written, art, music, video)
- custom MCP documentation (auny-vault, grok, codex, remotion)
- session protocols (start, domain routing, content session)
- templates (idea card, session log, workflow doc, monetization tracker)
- vault structure guide (folder map, naming conventions)
- workflow docs (music release, music video, content batching)
- MCP setup guide

**built by:** [@AunySillyMe](https://x.com/AunySillyMe)
**newsletter:** [Explained Without Fluff](https://explained-without-fluff.beehiiv.com)

---

*updates ship when something real changes. 🕷️*
