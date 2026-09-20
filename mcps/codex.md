---
title: codex (not an MCP)
description: "Correction to v1: Codex is a CLI lane, not an MCP server. A second model from a different family whose only job is adversarially auditing code Claude wrote, before it ships."
tags: [codex, code-review, adversarial-audit, cli, correction]
---

# codex

> **status: this is not an MCP.** v1 of this repo listed `codex` as a custom
> MCP server. it never settled into one. Codex is a **CLI lane**: a separate
> model you call from the terminal, not a tool Claude loads. this file is kept
> and corrected rather than deleted, because the correction is the useful part.

---

## what it is

OpenAI's Codex, run from the command line as a second model with its own view
of a codebase.

## what it is for

**one job: attacking code Claude wrote.**

Claude writes, Codex attacks, Claude verifies and fixes, i review. the value
is entirely in the model being from a different family. a model auditing its
own output agrees with itself, and the agreement feels like confidence.

## the rule

**whoever wrote the code does not review the code.** if Codex wrote it, the
audit goes to Claude instead. the direction does not matter; the difference
does.

## when it runs

always, before shipping, for:
- anything touching auth, tokens or secrets
- any public-facing endpoint
- any new or changed MCP server
- anything parsing input from somewhere i do not control
- deletion or bulk-mutation logic

skip it for one-line config changes and throwaway scripts.

## how to brief it

write the brief before you run it, and put the **reasoning** in, not just the
code. you want the reasoning attacked too.

- what the thing is and where it runs
- who can reach it
- what you already verified, so it does not re-report known ground
- the design decisions you made **and why**, so it can tell you the why is wrong

the last one is the one people skip. on the most recent audit i ran, Codex
did not find a bug i missed. it found that a security decision i made was
based on a false assumption, and explained the case where my reasoning broke.
i changed the design.

## one round

run it once. fix what reproduces. add a test per fix. record what you did
with each finding, including the ones you decided not to act on and why.

do not run a second pass hoping for a cleaner report. the tests are what
verify the fixes now.

## verify before you believe it

an audit is a claim, not a fact. reproduce every finding yourself before you
change anything. some will not reproduce.
