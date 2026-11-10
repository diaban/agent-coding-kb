---
type: Precedent
title: Market finance
description: Algorithmic trading led to risk limits and automatic circuit breakers.
tags:
- precedents
- circuit-breakers
status: draft
generated:
  by: claude/claude-fable-5-2
  at: '2026-11-10T19:50:00Z'
---

# Market finance

## What was automated

Trading, through algorithms.

## What replaced human inspection

Risk limits and circuit breakers, strengthened after the flash crash of 2010.

## Lesson for code

Put automatic circuit breakers in place for when incidents get out of hand, because they act before a human has time to react. For software, that means approval rules that tighten on their own when rollbacks or incidents per pull request rise.

## State of play

Anthropic reports not having such breakers yet (see [automated checks](../findings/automated-checks.md)).

## Where the analogy breaks

Markets have a single, fast, shared signal: price. Software incidents are heterogeneous and often detected late, so the trigger is harder to define.

## Related

- [Precedents overview](overview.md)
- [Scenario 4: the backlash](../scenarios/04-backlash.md)
