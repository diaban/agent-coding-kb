---
type: Concept
title: The cold-start problem
description: A new agent language has no training data; three routes to reduce that cost.
tags:
- languages
- training-data
status: draft
generated:
  by: claude/claude-fable-5-2
  at: '2026-11-10T19:50:00Z'
---

# The cold-start problem

## Claim

Compiling to existing languages solves the ecosystem problem, not the training-data problem. The agent still has to write in a language it has almost never seen.

## Three routes

1. **A strict profile of an existing language.** Keep the syntax of TypeScript or Rust, remove the escape hatches (`any`, `unsafe`), and make effects and contracts mandatory. Only the annotations are new. This is the strategy that let TypeScript succeed against JavaScript.
2. **The loop with the compiler.** Machine-readable errors let the agent learn during the task. Useful, but not enough against millions of examples.
3. **Verified synthetic data.** Models write programs, the compiler and proofs reject the wrong ones, and training uses the rest. This is what moved models forward in formal mathematics with Lean.

## Consequences

- **The more guarantees a language offers, the cheaper its cold start**, because the compiler can filter generated data.
- **Companies that train models will largely decide the language of agents.** A language the models master becomes the norm in practice.
- In the short term the most realistic route is a strict profile. A new language will only take hold if its guarantees let it produce its own training data.

## Objections

- The Lean comparison is suggestive, not a demonstration: proofs have a checker that settles correctness, while most programs do not.
- Route 1 leads to [scenario 1](../scenarios/01-lock-in.md), not to a new language.

## Related

- [Inertia and lock-in](../concepts/inertia-lock-in.md)
- [Scenario 5](../scenarios/05-language-under-the-language.md)
