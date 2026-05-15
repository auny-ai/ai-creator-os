---
title: Typefully
description: "Social media scheduling tool built for X (Twitter), with support for LinkedIn, Threads, Bluesky, and Mastodon. MCP-connected so Claude can draft posts directly into the queue without copy-paste."
tags: [typefully, social-media-scheduling, x, twitter, mcp]
---

# Typefully 📅

Typefully is a social media scheduling tool built specifically
for X (Twitter), with support for LinkedIn, Threads, Bluesky,
and Mastodon. it has an MCP connector, which means Claude can
draft posts directly into your queue without any copy-paste.

→ [get Typefully](https://typefully.com/?via=aunysillyme)

---

## how you can use it

- schedule posts and threads across multiple platforms
- manage multiple social accounts from one place
- view analytics on what's performing — impressions, engagement,
  saves, profile clicks
- use the queue system to space posts automatically
- connect to Claude via MCP so posts go straight from session
  to queue

---

## setup

1. create an account at [typefully.com](https://typefully.com/?via=aunysillyme)
2. connect your social accounts
3. enable the Typefully MCP in Claude Desktop under
   Settings → Integrations
4. find your social set ID — you'll need it when Claude drafts
   posts via MCP (it's in your Typefully account settings)

---

## how i use it

at the end of every content session, Claude drafts posts directly
into my Typefully queue via MCP. i don't copy-paste anything.
Claude calls the Typefully MCP with the post text, the social set
ID, and the platform — and the draft appears in my queue ready
to review.

for threads specifically, Claude builds the full tweet array in
one call — hook tweet through closing tweet, in order, sometimes
with a quote post on the first tweet if we're reacting to
something.

i also pull Typefully analytics at the start of every session —
last 30 published posts, scheduled queue, and recent performance
data. Claude reads this before writing anything so it knows what's
already out and what's already planned. nothing gets repeated,
and format rotation is enforced.

two accounts managed through Typefully:
- @AunySillyMe (main)
- your secondary brand account (if applicable)
