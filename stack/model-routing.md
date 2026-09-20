---
title: model routing
description: "Sending each task to the model that is actually best or cheapest for it, instead of one model doing everything. The single biggest structural change since v1."
tags: [model-routing, claude, codex, gemini, grok, orchestration, cost]
---

# model routing 🚦
### no tool does everything

v1 of this repo said Claude is chief of staff, with ChatGPT for a second
opinion. that was true and it was not enough. this is the routing table now.

---

## the table

| task | model | why |
|---|---|---|
| reasoning, writing, anything in my voice | Claude | it knows the system |
| adversarial code audit | Codex (GPT) | different family, so it does not agree with Claude's own work |
| deep research, large context | Gemini | context window |
| anything live on X | Grok | X-native, nothing else is |
| bulk classification, high volume | Hermes, Qwen | cheap or free per item |

---

## the rule that pays for itself

**whoever wrote the thing does not review the thing.**

a model reviewing its own work agrees with itself, and the agreement reads
like confidence. it is not. changing the reviewing model is the entire
mechanism.

## the second rule

**route by what the job actually needs, not by which tool you like.**

a bulk tagging job over 400 items does not need the most capable model. it
needs a cheap one and a spot check. a decision that is expensive to get wrong
needs the opposite.

## the third rule

**a cheap model is not a cheap answer for everything.** the cheapest lane i
use is good at producing structure and bad at citing a source. so it never
gets a job where a number, a line reference, or a citation is the output. if
it returns a figure, i re-derive the figure.

---

## what this looks like in practice

most sessions are still just Claude. the routing matters at the edges: the
audit before something ships, the research pass that needs live data, the
batch job where doing it in the expensive lane would be silly.

the win is not really cost. it is that a second opinion is structural instead
of something i remember to ask for.
