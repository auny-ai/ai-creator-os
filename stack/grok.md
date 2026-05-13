# Grok 🔍

Grok is xAI's AI model with native access to X (Twitter) data
in real time. in this system it serves two roles: research layer
(what's trending on X right now, across specific topics) and
image generation (dark cinematic character posts and abstract
surreal art via Grok Imagine).

---

## how you can use it

- search X natively — find what's trending on any topic right now
- web search with current information beyond a training cutoff
- generate images with Grok Imagine — character art, abstract art,
  cinematic scenes
- use Agent Mode in Grok Imagine for multi-step visual workflows
- get a second model perspective on complex questions or large docs

---

## setup

**for web and X search:**
access at [x.ai/grok](https://x.ai/grok) or via the X app

**for MCP integration with Claude:**
the custom Grok MCP in this system was built as a local Node.js
server. setup guide in [mcp-setup/setup_guide.md](../mcp-setup/setup_guide.md)

**for Grok Imagine:**
available inside the Grok interface — no separate setup needed

---

## how i use it

**research layer:**
i built a custom Grok MCP that runs inside Claude sessions.
three tools: `x_search`, `grok_web_search`, `grok_chat`.
when a trending post or topic comes up mid-session, Claude
searches X natively without leaving the conversation — no
tab switching, no copy-pasting results back in.

every content session includes a research pass across my content
pillars using this MCP. Claude searches what's trending in AI,
X strategy, personal branding, and human psychology — then
filters results against my pillars and voice before writing anything.

**image generation:**
Grok Imagine handles two content types for me:
- dark cinematic character posts — consistent character, dark mode,
  form-fitting, caramel skin, gold nose stud
- abstract surreal art — cosmic, glitch, skeleton, transformation
  themes. no character, pure concept.

**Agent Mode (music video pipeline):**
i use Grok Imagine's Agent Mode to produce full music videos
in a single conversation. the workflow: lyric storyboard →
scene-by-scene animation prompts → 6-second clips → stitch in
CapCut. my BLACK and PINK music videos were both built this way.
full workflow doc in [workflows/music-video.md](../workflows/music-video.md)
