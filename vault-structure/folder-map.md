---
title: Vault Folder Map
description: "The folder structure ai-creator-os runs on. Organized so Claude can navigate precisely — emoji prefixes make folders distinct, naming is consistent. Start with the minimum viable vault and expand as your system grows."
tags: [vault-structure, obsidian, folder-organization, naming]
---

# vault folder map

this is the folder structure that ai-creator-os runs on. it's
organized so Claude can navigate precisely — emoji prefixes
make folders distinct and searchable, and the naming is
consistent enough that Claude can infer where things live
without being told every time.

copy this structure and adapt it to your own work areas.
you don't need every folder on day one. start with the
core files and expand as your system grows.

---

## minimum viable vault (start here)

```
your-vault/
│
├── _index.md                    ← master map of the whole vault
├── 📝 Session Log.md            ← what changed, every session
├── 🕷️ [Your HQ file].md        ← active projects + routing
│
├── ✍️ Content & Brand/
│   ├── content_manual.md        ← voice rules, formats, pillars
│   └── content_pillars.md       ← what you post about and why
│
├── 📐 Protocols/
│   ├── 01_session_start.md      ← what Claude reads first
│   ├── 02_domain_routing.md     ← which files load for which tasks
│   └── all_links.md        ← every link you use, in one place
│
└── 🤖 AI Workflows/
    └── ai_operating_system.md   ← every tool + how they connect
```

---

## full structure (expand as needed)

```
your-vault/
│
├── _index.md
├── 📝 Session Log.md
├── 🕷️ [HQ file].md
│
├── ✍️ Content & Brand/
│   ├── content_manual.md
│   ├── working_manual.md        ← what's active right now
│   ├── content_pillars.md
│   └── visual_brand.md          ← image gen specs, character details
│
├── 📐 Protocols/
│   ├── 00_vault_access.md
│   ├── 01_session_start.md
│   ├── 02_domain_routing.md
│   ├── 03_content_session.md
│   └── all_links.md
│
├── 🤖 AI Workflows/
│   ├── ai_operating_system.md
│   ├── workflow_system.md
│   ├── stack_inventory.md
│   ├── monetization_tracker.md
│   └── workflows/               ← one file per documented workflow
│
├── 💼 Business/
│   ├── services_ecosystem.md
│   └── client_intake_template.md
│
├── 📬 Newsletter/
│   └── newsletter_manual.md
│
├── 🎵 Music/
│   ├── music_manual.md
│   ├── discography.md
│   ├── suno_analysis.md
│   └── Lyrics/
│
├── 📦 Products/
│   └── [one folder per product]
│
├── 💰 Ideas/
│   └── [one idea card per idea]
│
├── 🧠 Identity/
│   ├── who_am_i.md
│   └── cognitive_profile.md
│
└── 🐙 GitHub/
    └── github_strategy.md
```

---

## naming conventions

see `naming-conventions.md` for the full rules.

**the short version:**
- emoji prefix on every folder — makes them visually distinct
  and easier for Claude to navigate
- snake_case for all file names — no spaces, no caps
- descriptive names — `content_manual.md` not `manual.md`
- one topic per file — don't combine unrelated things
- hub files use README.md — so Claude knows what's in the folder

---

## the files Claude reads every session

these are the four files that make the session protocol work.
build these first, before anything else:

1. **`_index.md`** — what's in the vault, what's active
2. **`📝 Session Log.md`** — what changed recently
3. **`✍️ Content & Brand/content_manual.md`** — your voice and formats
4. **`📐 Protocols/01_session_start.md`** — how sessions run
