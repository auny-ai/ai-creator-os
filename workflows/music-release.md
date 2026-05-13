# music release workflow 🎵
### Suno → Soundboost AI → DistroKid → everywhere

this is the full pipeline for releasing an AI-generated track
to every streaming platform. from prompt to live on Spotify,
the whole thing runs in under an hour.

---

## tools

| tool | role |
|------|------|
| Claude | writes Suno prompts, manages metadata and release prep |
| Suno | generates the track |
| Soundboost AI | masters for streaming |
| DistroKid | distributes to all platforms |
| Claude Cowork | builds hyperfollow pages autonomously |
| Obsidian vault | stores all release data, streaming links, ISRC codes |

---

## the pipeline

```
1. Claude writes Suno prompt
2. Suno generates — review and select best take
3. Soundboost AI masters the track
4. DistroKid upload — metadata, artwork, release date
5. Hyperfollow page built
6. Streaming links saved to vault
7. ASCAP registration (batch, not per release)
```

---

## step 1 — prompt writing

describe the emotional register, energy, or theme to Claude.
Claude writes a structured Suno prompt using the bracket system.
see [stack/suno.md](../stack/suno.md) for prompt structure and real examples.

one session typically produces 5-10 prompt variations.
generate all of them, then pick the best 1-3 takes per prompt.

---

## step 2 — generation and selection

generate each prompt in Suno. listen through all takes.
criteria for selection:
- does it hit the emotional target from the brief?
- are the quality controls respected (no white noise, clean transitions)?
- would you listen to this at 2am?

export the selected take as WAV.

---

## step 3 — mastering (Soundboost AI)

upload the WAV to [Soundboost AI](https://soundboost.ai).
select your loudness target for streaming (-14 LUFS for Spotify).
download the master.

the master is your release file. label it clearly:
`[title]_master.wav`

---

## step 4 — DistroKid upload

→ [get DistroKid](https://distrokid.com/vip/seven/11119560) — 7% off

upload at [distrokid.com](https://distrokid.com/vip/seven/11119560) with:

- **title** — finalized track name
- **artist** — your artist name exactly as it appears on other releases
- **artwork** — 3000x3000px minimum, JPG or PNG, no text in corners
- **genre** — pick the closest match
- **release date** — set at least 7 days out for playlist consideration
- **ISRC** — let DistroKid generate automatically unless you have one

timeline: live on Spotify and Apple Music within 24-72 hours.

---

## step 5 — hyperfollow page

a hyperfollow page is a pre-save and streaming link page for
the release. DistroKid generates one automatically.

in this system, Claude Cowork reads the release details from
the vault and builds hyperfollow pages autonomously — filling
in all fields, adding streaming links as they go live.

manually: go to DistroKid → HyperFollow → create for this release.

---

## step 6 — save to vault

after the release goes live, save to your vault:
- title, release date, ISRC
- hyperfollow page URL
- streaming links (Spotify, Apple Music, YouTube Music, etc.)
- DistroKid release ID

this keeps your full catalog current and accessible for any
future session that needs it — content posts, ASCAP registration,
streaming link updates.

---

## step 7 — ASCAP registration

register with your performing rights organisation to collect
performance royalties. do this in batches, not per release —
once a month or once per album.

in this system, Claude Cowork handles ASCAP registration
autonomously using the catalog data from the vault. a full
150-song catalog was registered in a single session.

manually: log into ASCAP, register each title with its ISRC
and release date.

---

## content from this workflow

every release is content:
- "new track out" post with hyperfollow link
- behind-the-prompt post — share the Suno prompt that made it
- build-in-public post — the pipeline itself is the content
- Suno promptshare post — drop the prompt, invite people to try it
