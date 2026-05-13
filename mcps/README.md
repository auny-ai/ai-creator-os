# custom MCPs 🔌

these are MCP servers built specifically for this system.
each one is a self-contained tool that plugs directly into
Claude Desktop and runs mid-session without leaving the
conversation.

---

## what's here

| MCP | what it does | status | repo |
|-----|-------------|--------|------|
| [auny-vault](./auny-vault.md) | read and write your Obsidian vault | ✅ live | [auny-ai/ai-creator-os](https://github.com/auny-ai/ai-creator-os) |
| [grok](./grok.md) | X-native search + read X links + web research | ✅ live | [auny-ai/ai-creator-os](https://github.com/auny-ai/ai-creator-os) |
| [codex](./codex.md) | code review and code chat via Codex | ✅ live | [auny-ai/ai-creator-os](https://github.com/auny-ai/ai-creator-os) |
| [remotion](./remotion.md) | programmatic video generation via Remotion | ✅ live | [aunysillyme/remotion-mcp](https://github.com/aunysillyme/remotion-mcp) |

---

## when to build a custom MCP vs connect a hosted one

**build a custom MCP when:**
- the tool you need doesn't have an official MCP connector
- you need capability available across every session, not just once
- you want to own the tool surface area completely

**connect a hosted MCP when:**
- the vendor has an official connector (Linear, Typefully, Beehiiv, etc.)
- the capability is standard enough that a generic connector covers it

the hosted connectors (Linear, Typefully, Beehiiv, Google Drive, Gmail,
Calendly, and more) are set up in Claude Desktop under
Settings → Integrations. no code required.

---

## monetization note

each custom MCP is also a sellable product. the code +
a setup guide + a short walkthrough video = a Gumroad listing.
every MCP built here has that path available.
