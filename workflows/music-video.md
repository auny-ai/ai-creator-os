# music video workflow 🎬
### Grok Imagine Agent Mode → full music video in one conversation

this workflow produces a complete music video from song lyrics
in a single Grok Imagine Agent Mode conversation. no video
editing experience needed. 30-45 minutes start to finish.

the BLACK and PINK music videos were both built this way.

---

## tools

| tool | role |
|------|------|
| Claude | writes the scene-by-scene storyboard |
| Grok Imagine (Agent Mode) | generates animated video clips per scene |
| CapCut | stitches clips, syncs to audio, final export |

---

## the pipeline

```
1. Claude writes scene-by-scene storyboard from lyrics
2. Grok Imagine Agent Mode generates clips scene by scene
3. B-roll generated for instrumental gaps
4. clips downloaded
5. CapCut — arrange, sync to audio, export
```

---

## step 1 — storyboard

paste your lyrics into Claude. ask for a scene-by-scene
storyboard — one visual scene per lyric section with:
- the lyric line(s) it covers
- what's happening visually
- mood, lighting, color palette
- character position and motion direction

example prompt to Claude:
```
write a scene-by-scene storyboard for this music video.
one scene per lyric section. include: lyric covered,
visual description, mood, lighting, color palette.
keep the visual style consistent — dark cinematic,
[character spec if applicable].

lyrics:
[paste lyrics]
```

---

## step 2 — generation in Grok Imagine Agent Mode

open Grok Imagine and enable Agent Mode.

paste the full storyboard. Grok will work through it scene
by scene, generating animated clips for each one.

tips:
- be specific in the storyboard — vague directions produce
  inconsistent character and style
- if a clip doesn't match, say "regenerate scene 3 with
  more [specific detail]" — Agent Mode holds the context
- request 6-second clips — long enough for a full lyric
  line, short enough to stay visually interesting

---

## step 3 — B-roll for instrumental gaps

for sections with no lyrics (intro, bridge, outro), request
B-roll clips that match the visual theme of the video.

example:
```
generate 3 B-roll clips for the instrumental bridge —
same visual style as the rest of the video, abstract
motion, [color palette], no character needed
```

---

## step 4 — download

download all clips from the Grok session in order.
label them by scene number before importing to CapCut:
`scene_01.mp4`, `scene_02.mp4` etc.

---

## step 5 — CapCut edit

1. create new project, import all clips in order
2. import your audio track
3. arrange clips on the timeline — match lyric sections
   to their corresponding scene clips
4. trim clip start/end points to sync with the beat
5. add any transitions (keep them minimal — cuts work better
   than fades for this style)
6. export at highest resolution available

---

## content from this workflow

- post the finished video with a short caption and a question
- post the storyboard prompt as a behind-the-scenes thread
- "I made this music video in 45 minutes" — process post
  showing before/after of the storyboard and the final video
- the workflow itself is a sellable guide
