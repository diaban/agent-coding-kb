---
type: Scenario
title: 'Scenario 1: lock-in'
description: Dominant languages are hardened, not replaced, and niche languages decline.
tags:
- scenarios
- lock-in
status: draft
generated:
  by: claude/claude-fable-5-2
  at: '2026-11-10T19:50:00Z'
---

# Scenario 1: lock-in

## Claim

The dominant languages gain even more ground because models are best at them. They are hardened, not replaced, and the number of languages in real use shrinks to a handful.

## What it looks like

- Teams migrate to strict typing (TypeScript, Rust) because agents benefit from errors caught at compile time.
- Strict profiles appear: no escape hatches (`any`, `unsafe`), mandatory annotations.
- Niche languages decline, since agents write them worse.

## Why it is likely

The [lock-in loop](../concepts/inertia-lock-in.md) is self-reinforcing, and this scenario requires nobody to make a costly bet. It is what happens by default.

## Signals to watch

- Share of TypeScript, Python and Rust in generated code.
- Decline of niche languages in new projects.
- Adoption of strict profiles and lint rules written for agents.

## Objections

- A monoculture is fragile: shared flaws propagate everywhere.
- It leaves the real limits of current languages in place, in particular hidden effects and unverifiable contracts. See [real vs overrated limits](../languages/real-vs-overrated-limits.md).

## Related

- [Cold start](../languages/cold-start.md): the strict-profile route
- [Scenario 2](02-spec-as-language.md), compatible with this one
