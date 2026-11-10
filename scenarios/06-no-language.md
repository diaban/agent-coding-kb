---
type: Scenario
title: 'Scenario 6: no language at all'
description: 'The programming language disappears: non-text output, or the model runs the task itself.'
tags:
- scenarios
- representation
status: draft
generated:
  by: claude/claude-fable-5-2
  at: '2026-11-10T19:50:00Z'
---

# Scenario 6: no language at all

## Claim

The programming language disappears as an artifact. Two distinct variants exist, and they fail for different reasons.

## Variant A: the model emits something other than text

The model produces low-level output directly (binary, WebAssembly), a structured representation such as a syntax tree, or a representation learned by the models themselves. Text becomes at most a view generated for humans.

**Obstacle: verification.** A format nobody can read and no existing tool can check removes the means of establishing correctness, which is the scarce resource in the first place. See [verification bottleneck](../concepts/verification-bottleneck.md).

## Variant B: the model executes the task itself

No program is written. The model performs the task on each request.

**Obstacle: cost and determinism.** Reasoning on every request is expensive and does not always give the same result. Repeated tasks get frozen into code anyway. See [scenario 3](03-all-harness.md).

## Signals to watch

- Agents performing as reliably on structured or non-text representations as on text.
- Models trained on representations with no human-written corpus.

## Objections

- Models are trained overwhelmingly on text. This is the hardest form of the cold-start problem.
- The first synthesis expected this outcome to bring density. It does not: see the correction in [AST](../concepts/ast.md).

## Related

- [Constrained decoding](../concepts/constrained-decoding.md)
- [archive/v1.md](../archive/v1.md), step 4
