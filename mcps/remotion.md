---
title: remotion MCP (retired)
description: "Retired from the stack. Wrapped Remotion for programmatic video generation; replaced by a deterministic HTML-to-video pipeline that composites real assets instead of generating scenes."
tags: [mcp, remotion, video-generation, retired, deterministic-render]
---

# remotion

> **status: retired.** this MCP is no longer part of the stack. the repo it
> pointed at is archived. kept here because "what replaced it and why" is more
> useful than a deleted file.

---

## what it was

an MCP server that drove [Remotion](https://remotion.dev) so Claude could
generate video programmatically: React components rendered to frames, frames
rendered to MP4.

## why it is gone

two reasons, in order of how much they mattered.

**1. the render step was heavy for what it produced.** a React render pipeline
is a lot of machinery to stand up for a 15-second brand reel.

**2. it could invent things.** a generative video step will happily produce a
version of your product that does not exist. for anything with a real asset in
it (a real screenshot, a real logo, real numbers on a real chart), that is
not a small problem.

## what replaced it

an HTML-to-video pipeline: scene HTML, rendered in headless Chrome, with WebGL
shader transitions between scenes, stitched with ffmpeg.

| | remotion MCP | what runs now |
|---|---|---|
| input | React components | plain HTML scenes |
| cost | render time | $0 |
| output | varies per run | deterministic, same input gives same video |
| invention | possible | none, it composites the assets you give it |

deterministic is the whole point. the video shows the real asset, or it does
not render.

## if you want programmatic video anyway

Remotion is genuinely good, and none of the above says otherwise. it was the
wrong fit for **my** use, which is motion graphics over real assets rather
than generated scenes. if you are producing something React-shaped and
data-driven, go look at it properly.
