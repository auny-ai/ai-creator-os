---
title: Content Batching Workflow
description: "Produces a full day of content (posts across all pillars and formats) drafted to Typefully in one Claude session. Centers on a research-and-context loop that runs before any writing starts."
tags: [content-workflow, content-batching, typefully, claude-workflow]
---

# content batching workflow ✍️
### a full day of content in one Claude session

this workflow produces a full batch of posts across all pillars
and formats, drafted directly to Typefully, in one session.
the key is the research and context loop that runs before
a single word gets written.

---

## tools

| tool | role |
|------|------|
| Claude | reads vault, researches, writes all posts |
| Obsidian vault | stores voice, formats, history, protocols |
| Grok MCP | X-native trend research across pillars |
| Typefully | receives drafts via MCP, no copy-paste |

---

## the pipeline

```
1. vault read — content manual, working manual, session log
2. pull Typefully — last 30 published, current queue
3. pull analytics — last 7 days
4. research — Grok MCP across all active pillars
5. state content direction explicitly
6. check format rotation and recent topics
7. write batch with comment-pulling questions
8. draft to Typefully via MCP
```

---

## step 1 — vault read

Claude reads at session start:
- content manual — voice rules, formats, pillars
- working manual — what's active, what to avoid
- session log — what changed recently

this is the context that produces content that sounds like
you instead of like a generic AI output. don't skip it.

---

## step 2 — pull Typefully

before writing anything, Claude pulls:
- last 30 published posts (no repeats)
- current scheduled queue (no conflicts)

this step alone prevents the most common batching mistake —
writing something you already posted last week.

---

## step 3 — analytics

pull performance data for the last 7 days:
- top posts by impressions
- top posts by engagement (replies, saves)
- which formats are currently landing

weight recent data more heavily. last week is more signal
than last quarter.

---

## step 4 — research

Claude runs Grok MCP searches across each active pillar.
filter rule: trending ≠ relevant. only results that map
to your pillars and your voice make it into the batch.

your pillars define the search — not the other way around.
see [content-system/content_pillars.md](../content-system/content_pillars.md) to build yours.

---

## step 5 — content direction

before writing, Claude states explicitly:
- what signals came out of research
- which pillars to weight this session
- which formats to prioritize based on analytics
- anything to avoid (overused formats, covered topics)

this step turns data into direction. don't rush past it.

---

## step 6 — format check

confirm before writing:
- no same format twice in a row in the batch
- every post longer than a one-liner has a comment-pulling
  question that can't be answered yes or no
- format rotation covers a full spread across the day

see [content-system/formats_reference.md](../content-system/formats_reference.md) for the full
format library and what each one optimizes for.

---

## step 7 — write

write the full batch. each post includes:
- full post text
- format label
- suggested time slot based on your posting schedule
- service CTA where applicable

your posting schedule, time slots, and format cadence
are personal to your account and audience. build yours
based on your own analytics — when your audience is most
active, what formats perform at what times of day.

---

## step 8 — draft to Typefully

Claude calls the Typefully MCP for each post. drafts go
straight to your queue — no copy-paste.

for threads: Claude builds the full tweet array in one call.
for quote posts: Claude includes the source URL in the call.

review drafts in Typefully before scheduling.

---

## what makes this different from just asking Claude to write posts

the research step. most AI-generated content fails because
it has no signal from the real world — it's just a model
guessing what might perform.

this workflow pulls live X data, live analytics, and vault
context before writing a word. the output is grounded in
what's actually trending in your pillars and what's actually
been working for your specific account.

that's the gap.
