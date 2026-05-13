# remotion MCP 🎬

the remotion MCP brings programmatic video generation into
Claude sessions. Remotion is a framework for creating videos
using React — this MCP exposes it as a tool Claude can call
directly to generate video content without leaving the conversation.

**repo:** [aunysillyme/remotion-mcp](https://github.com/aunysillyme/remotion-mcp)

---

## tools

| tool | what it does |
|------|-------------|
| `list_templates` | lists available Remotion video templates |
| `new_slideshow` | generates a new slideshow video from content |
| `render_video` | renders a video from a Remotion template |

---

## setup

```bash
git clone https://github.com/aunysillyme/remotion-mcp.git
cd remotion-mcp
npm install
```

add to Claude Desktop config:

```json
"remotion": {
  "command": "node",
  "args": ["/path/to/remotion-mcp/index.js"]
}
```

full setup instructions in the
[remotion-mcp repo](https://github.com/aunysillyme/remotion-mcp).

---

## how it's used in this system

used for programmatic video content — primarily slideshow-style
videos where the structure is data-driven rather than manually
composed. Claude can generate the content, call the MCP to render
it, and produce a video file ready to post.

pairs well with the written content workflow — a thread or
educational piece can become a video slideshow in the same session.
