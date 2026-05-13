# content session protocol

a content session produces a full day (or multiple days) of
posts — drafted, formatted, and queued in Typefully via MCP.
this protocol runs in order every time. skipping steps produces
generic output. following them produces content that sounds
like you.

---

## the sequence

```
1. READ       vault files for this domain
2. PULL       recent published posts (last 30)
3. PULL       scheduled queue (what's already planned)
4. PULL       analytics (last 7 days)
5. RESEARCH   trending topics across your pillars
6. SIGNAL     state content direction explicitly
7. CHECK      format rotation and recent content
8. WRITE      posts in full with comment-pulling questions
9. DRAFT      to Typefully via MCP
```

---

## step 1 — read

load from vault:
- content manual (voice rules, formats, pillars)
- working manual (what's currently active or off-limits)
- session log (what changed recently)

this is the context that makes content sound like you
instead of like a generic AI output.

---

## step 2 + 3 — pull published + scheduled

pull from Typefully:
- last 30 published posts (know what's already out)
- current scheduled queue (know what's already planned)

this prevents repeating yourself and prevents scheduling
conflicts.

---

## step 4 — pull analytics

pull performance data for the last 7 days:
- which posts got the most impressions
- which got the most engagement (replies, saves)
- which formats are currently working

weight recent posts more heavily than older ones.
what worked last week is more signal than what worked
three months ago.

---

## step 5 — research

run a trend search across your content pillars using your
research tool (Grok MCP for X-native data, Gemini for
web-depth research).

search each active pillar:
- AI and tools
- X and content strategy
- personal branding
- monetization
- human psychology
- music and creativity

keep only results that map to your pillars and your voice.
trending ≠ relevant.

---

## step 6 — state content direction

before writing a single post, Claude should state:
- what signals came out of the research
- what pillar weighting makes sense for this session
- what formats to prioritize based on recent analytics
- anything to avoid (formats overused recently, topics
  already covered)

this step turns data into direction. it's the difference
between a session that produces good content and one that
produces a lot of content.

---

## step 7 — check rotation

confirm:
- no same format twice in a row in the batch
- no topic already covered in the last 7 days
- every post longer than a one-liner has a comment-pulling
  question that can't be answered with yes or no

---

## step 8 — write

draft all posts for the session. include:
- full post text
- format label (so you can see rotation at a glance)
- suggested time slot
- service CTA if applicable (rotated — never same service
  twice in a row)

---

## step 9 — draft to Typefully

Claude calls the Typefully MCP for each post:
- social set ID (your account)
- platform (X, LinkedIn, Threads, etc.)
- post text
- quote post URL if applicable (for reactive content)
- community ID if posting to a community

drafts go to Typefully as saved drafts — not published.
review before scheduling.
