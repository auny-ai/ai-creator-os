# naming conventions

consistent naming is what makes the vault navigable by Claude
without manual guidance. when files are named predictably,
Claude can find what it needs without you directing every search.

---

## the rules

**folders:**
- emoji prefix on every folder
- short descriptive name after the emoji
- sentence case — not ALL CAPS, not all lowercase

```
✅ ✍️ Content & Brand
✅ 🤖 AI Workflows
✅ 📐 Protocols
❌ content
❌ AI WORKFLOWS
❌ my-notes-folder
```

**files:**
- snake_case — all lowercase, underscores between words
- no spaces in file names
- descriptive — says what the file contains, not just a label

```
✅ content_manual.md
✅ session_log.md
✅ ai_operating_system.md
❌ Manual.md
❌ notes.md
❌ stuff.md
```

**hub files:**
- every folder that has multiple files gets a README.md
- the README maps what's in the folder and what each file is for
- Claude reads the README to navigate a folder without opening
  every file

---

## special files

| file | purpose | naming rule |
|------|---------|------------|
| master vault map | maps the whole vault | `_index.md` — underscore prefix so it sorts to top |
| session log | what changed, every session | `📝 Session Log.md` — emoji prefix, sentence case |
| HQ file | active projects, routing | `🕷️ [Name] HQ.md` or similar |
| protocol files | how sessions run | numbered prefix: `01_`, `02_`, etc. |
| workflow docs | one per workflow | descriptive snake_case: `suno_to_distrokid.md` |
| idea cards | one per idea | descriptive snake_case: `mcp_setup_guide_product.md` |

---

## why the emoji prefixes matter

Claude navigates the vault by reading file and folder names.
emoji prefixes make folders visually distinct so Claude can
identify them in a directory listing without reading every name.

when Claude calls `list_files` on the vault root and sees:
```
✍️ Content & Brand
🤖 AI Workflows
📐 Protocols
🎵 Music
```

it immediately knows which folder to go to for which domain —
without needing a separate map.

this is the detail that makes the system feel smart.
