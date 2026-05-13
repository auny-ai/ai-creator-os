# codex MCP 💻

the codex MCP exposes OpenAI's Codex model as a tool inside
Claude sessions. used for code review and secondary code chat
when a second model perspective on a technical build is useful.

**repo:** [auny-ai/ai-creator-os](https://github.com/auny-ai/ai-creator-os)

---

## tools

| tool | what it does |
|------|-------------|
| `codex_chat` | chat with Codex — technical questions, code generation |
| `codex_review` | submit code for review — returns feedback and suggestions |

---

## setup

```bash
cd ai-creator-os/mcps/codex
npm install
```

you'll need an OpenAI API key:

```bash
export OPENAI_API_KEY=your_key_here
```

then add to Claude Desktop config:

```json
"codex": {
  "command": "node",
  "args": ["/path/to/ai-creator-os/mcps/codex/index.js"],
  "env": {
    "OPENAI_API_KEY": "your_key_here"
  }
}
```

---

## how it's used in this system

used during technical build sessions — primarily when building
other MCP servers or Claude Code projects. `codex_review` is
useful when you want a second pass on code before deploying.

not a daily-use tool. in rotation for technical sessions where
cross-model review adds value.
