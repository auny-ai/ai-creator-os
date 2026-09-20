# tools 🛠️
### my full stack: what i use, what it does, what you get

> some links below are affiliate links. they get you a discount or bonus and help support what i build. always disclosed. 🧡

**updated september 2026.** the stack in v1 was nine tools and one Claude surface. it is bigger now, and the shape changed: the vault is still the memory layer, but the work moved from one chat window to a fleet of servers i built and a set of models i route between.

---

## the core system

| tool | what i use it for | link |
|------|------------------|------|
| **Claude** | chief of staff. content, workflows, writing, all of it | [claude.ai](https://claude.ai) |
| **Claude Code** | the build surface. websites, MCP servers, automations, everything technical. i had no prior coding background | [claude.com/claude-code](https://claude.com/claude-code) |
| **Claude Design** | all design work: PDFs, digital products, brand kits, layouts | [claude.ai](https://claude.ai) |
| **Obsidian** | vault. the memory layer every AI tool reads from | [obsidian.md](https://obsidian.md) |
| **MCP** | connects everything to Claude so it reads and writes mid-session | [modelcontextprotocol.io](https://modelcontextprotocol.io) |
| **Cloudflare Workers** | hosts the MCP servers i built, so they work from every device | [workers.cloudflare.com](https://workers.cloudflare.com) |

**what changed:** v1 was Claude Desktop reading a local vault. now the vault lives behind a Worker, so the same memory reaches the desktop app, the phone, and scheduled jobs that run while i sleep.

---

## the models i route between

no tool does everything. each one has a job.

| model | what it gets | why |
|------|------------------|------|
| **Claude** | reasoning, writing, vault work, anything with my voice in it | it knows the system |
| **Codex (GPT)** | adversarial code review, second implementations | different model family, so it catches what Claude misses in its own work |
| **Gemini** | deep research, large-context analysis | context window |
| **Grok** | anything live on X, real-time search | X-native, nothing else is |
| **Hermes / Qwen** | bulk classification and high-volume extraction | cheap or free per item |

**what changed:** v1 listed one AI doing everything with ChatGPT as a second opinion. now it is an explicit routing table. the rule that made the difference: whoever wrote the code does not review the code.

---

## content & social

| tool | what i use it for | link |
|------|------------------|------|
| **Typefully** ✦ | schedule and manage all social posts | [get 20% off →](https://typefully.com/?via=aunysillyme) |
| **Beehiiv** ✦ | newsletter. Explained Without Fluff | [20% off first 3 months →](https://www.beehiiv.com/?via=Auny-H) |
| **Creator Buddy** ✦ | X growth analytics | [creatorbuddy.io →](https://www.creatorbuddy.io/?via=auny) |

---

## images, design & video

| tool | what i use it for |
|------|------------------|
| **ChatGPT Image** | most image generation and infographics |
| **Claude Design** | PDFs, digital products, brand kits, layouts |
| **Adobe Firefly** | reference-driven image, video and animation work |
| **Adobe Creative Suite** | editing and production, connected over MCP |
| **Grok Imagine** | character art, cinematic visuals, music video clips |
| **CapCut** | video editing and stitching |
| **Three.js** | 3D and interactive visuals, connected over MCP |
| **Canva** | quick one-off social graphics, rarely |

**what changed:** v1 pointed all image work at Grok Imagine. images now start in ChatGPT Image, design work goes to Claude Design, and Firefly covers reference-driven generation. Canva went from a regular tool to a rare one.

---

## music & creative

| tool | what i use it for | link |
|------|------------------|------|
| **Suno** ✦ | AI music creation, full albums | [get extra credits →](https://suno.com/invite/@aunysillyme) |
| **DistroKid** ✦ | music distribution to all platforms | [7% off →](https://distrokid.com/vip/seven/11119560) |
| **ASCAP** | rights registration | [ascap.com](https://www.ascap.com) |

mastering runs through a Python DSP pipeline i built rather than a service, targeting -14 LUFS and -1 dBTP.

---

## project & product

| tool | what i use it for | link |
|------|------------------|------|
| **Linear** | project tracking: issues, sprints, all open work | [linear.app](https://linear.app) |
| **Stripe** | payments for products and services | [stripe.com](https://stripe.com) |
| **Buy Me a Coffee** | consulting calls and digital products | [buymeacoffee.com](https://buymeacoffee.com) |
| **Gumroad** | digital products | [gumroad.com](https://gumroad.com) |
| **Calendly** | book calls | [calendly.com](https://calendly.com) |
| **Vercel** | hosting for aunysillyme.com | [vercel.com](https://vercel.com) |

---

## the parts that run without me

this is the biggest thing that did not exist in v1.

| piece | what it does |
|------|------------------|
| **an always-on cloud box** | runs scheduled jobs: research digests, index rebuilds, mirrors, health checks |
| **a fleet of bots** | handle the things with no API: portal logins, ad reads, inbox digests, image and video jobs |
| **scheduled Claude sessions** | wake up on a cron, do a job, write the result to the vault, and stop |

the point of v1 was that Claude remembers between sessions. the point of v2 is that some sessions start without me.

---

## the pieces i built

fifteen or so MCP servers, written in Claude Code, most hosted on Cloudflare Workers. full list and what each one does: [mcps/README.md](./mcps/README.md).

the short version: the vault door, X (reads, writes and ads), Google Workspace, Google Tasks, a client hub, an exact-arithmetic calculator, a code runner, and a memory layer.

---

## ✦ affiliate disclosure

links marked ✦ are affiliate links. here's exactly what each one does:

| tool | you get | i get |
|------|---------|-------|
| Typefully | nothing | 20% recurring commission |
| Beehiiv | 20% off first 3 months | recurring commission |
| Suno | extra credits | credits/commission |
| DistroKid | 7% off | $10 per paid signup |
| Creator Buddy | nothing | 10% commission |

these cost you nothing extra. when you use them, you support what i build here. 🧡

i am an Adobe Firefly ambassador. that is a partnership, not an affiliate link, and it is non-exclusive: i use and cover competing tools freely, and i say so when a post is sponsored.
