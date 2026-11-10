---
type: Overview
title: Scenarios
description: Six competing futures for code and languages, how they combine, and the current bet.
tags:
- scenarios
status: draft
generated:
  by: claude/claude-fable-5-2
  at: '2026-11-10T19:50:00Z'
---

# Scenarios

Six possible outcomes of the tension described in [inertia and lock-in](../concepts/inertia-lock-in.md): code is no longer read, yet it is still written in languages made to be read.

They are **competing branches, not steps on one line**. Some can coexist; some undercut each other. They are ordered here from most to least likely, which is a judgment, not a forecast.

| # | Scenario | What it assumes | Signal to watch |
| --- | --- | --- | --- |
| 1 | [Lock-in](01-lock-in.md) | Inertia wins | Share of a few languages in generated code |
| 2 | [The specification becomes the language](02-spec-as-language.md) | Humans move up a level and stop reading code | Teams that version specs and regenerate code |
| 3 | [All-harness](03-all-harness.md) | Most code becomes disposable | Share of tasks solved by code that is never committed |
| 4 | [The backlash](04-backlash.md) | Serious incidents trigger audit requirements | Contractual or regulatory clauses requiring human review |
| 5 | [The language under the language](05-language-under-the-language.md) | A model vendor breaks the data lock-in | A major vendor publishes its own target format |
| 6 | [No language at all](06-no-language.md) | Models work reliably outside text | Agents as reliable on non-text representations as on text |

## How they combine

They distribute by layer:

- **Durable, critical code:** scenarios 1 and 2, with 4 in regulated sectors.
- **Situational code:** scenario 3.
- **Scenarios 5 and 6** depend on a decision by the companies that train models, not on market evolution.

## Tensions between scenarios

- If 3 wins broadly, 5 loses much of its point: nobody optimizes a language for code that runs once.
- 4 pushes languages toward more human readability, the opposite of 5 and 6.
- 2 can happen without any new programming language, which makes it compatible with 1.

## Current bet

Over five years: 1 and 2 dominate, 3 takes the long tail, and the real threshold is 2, because it changes what humans read without requiring a new programming language.

## Earlier framing

The second synthesis arranged these ideas as a single five-stage trajectory defined by "who verifies the code?":

1. AI as assistant (2023–2025)
2. The agent writes, the human reviews every diff (2025–2026)
3. Industrialized verification (2026–2027)
4. Unread code (around 2027–2029)
5. Native representation (open horizon)

That ordering is still useful for stages 1 to 3. Beyond that, this base treats the outcomes as branches. Note also that stage 2 is already partly outdated: the [findings](../findings/review-bottleneck.md) show reviews being skipped, so "the human reviews every diff" no longer describes current practice.
