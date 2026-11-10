---
type: Precedent
title: Compilers
description: Compilers made assembly unread; where that analogy with agents breaks.
tags:
- precedents
- determinism
status: draft
generated:
  by: claude/claude-fable-5-2
  at: '2026-11-10T19:50:00Z'
---

# Compilers

## What was automated

Translation from a high-level language to assembly.

## What replaced human inspection

Trust in the tool and in its tests. Nobody reads the generated assembly any more.

## Lesson for code

A level stops being read as soon as the tool that produces it is reliable enough. This is the precedent behind the idea that source code could become "the new assembly".

## Where the analogy breaks

This is the weakest point of the whole argument and should be stated plainly.

| | Compiler | Agent |
| --- | --- | --- |
| Same input, same output | Yes | No |
| Input | A formal language with defined semantics | Natural language, ambiguous |
| How trust is earned | Correctness is established once for the tool, then reused | Each output has to be verified on its own |

Trust in a compiler transfers from one compilation to the next. Trust in an agent does not transfer in the same way. So "code becomes unread like assembly" only holds if per-output verification is strong enough to stand in for tool-level correctness.

## Related

- [Precedents overview](overview.md)
- [Verification bottleneck](../concepts/verification-bottleneck.md)
- [Scenario 2: the specification becomes the language](../scenarios/02-spec-as-language.md)
