---
type: Scenario
title: 'Scenario 5: the language under the language'
description: An agent language takes hold as an intermediate representation humans never see.
tags:
- scenarios
- agent-language
status: draft
generated:
  by: claude/claude-fable-5-2
  at: '2026-11-10T19:50:00Z'
---

# Scenario 5: the language under the language

## Claim

A language for agents does take hold, but as an intermediate representation. The agent writes in it, it compiles to existing languages, and humans never see it.

## What it looks like

- Explicit effects and contracts, checked by a compiler.
- Machine-readable errors.
- Compilation to existing targets, so the ecosystem problem is avoided.

## What it requires

Someone has to break the [training-data lock-in](../concepts/inertia-lock-in.md). The plausible route is verified synthetic data: models write programs, the compiler and proofs reject the wrong ones, and training uses the rest. That requires a company that trains models to decide to do it.

## Signals to watch

- A major model vendor publishes its own target format or language.
- Agent languages or intermediate representations used in production, not only in experiments.

## Objections

- Compiling to existing languages solves the ecosystem problem, not the training-data problem. See [cold start](../languages/cold-start.md).
- A strict profile of an existing language gets most of the benefit at a fraction of the cost, which favours [scenario 1](01-lock-in.md).
- If most code becomes disposable ([scenario 3](03-all-harness.md)), the investment is hard to justify.

## Related

- [Existing projects](../languages/existing-projects.md): ll-lang, ALaS
- [Design trajectory](../languages/design-trajectory.md)
