---
type: Concept
title: Inertia and lock-in
description: 'Why agents keep writing human languages: a self-reinforcing lock-in.'
tags:
- lock-in
- training-data
status: draft
generated:
  by: claude/claude-fable-5-2
  at: '2026-11-10T19:50:00Z'
---

# Inertia and lock-in

## Claim

Agents keep writing in the most widely used human languages even though humans read the result less and less. This is not a temporary lag. It is a self-reinforcing lock-in.

## The paradox

Languages such as Python, TypeScript or Java were designed for human readers who keep context in their heads. If the reader disappears, the design constraint disappears too. Yet nothing changes, for three reasons:

- **Community and ecosystem.** Libraries, tooling, hiring and documentation all exist for current languages.
- **Organizational inertia.** Existing codebases, and the people accountable for them, are in those languages.
- **Training data.** Models are best at the languages with the most public code.

## Why it reinforces itself

1. Models perform best in the most common languages.
2. So agents are asked to write in those languages.
3. So even more code is produced in those languages.
4. So the next generation of models is even better at them.

Each turn of the loop raises the cost of entry for any new language. A language nobody has written in has no data, and an agent writes badly in a language it has almost never seen.

## What could break it

- A strict profile of an existing language, which reuses the data. See [cold start](../languages/cold-start.md).
- Verified synthetic data, which lets a language with strong guarantees generate its own training corpus.
- A decision by a company that trains models. Whoever trains the models largely decides which language agents master.

## Objections

- The loop is a reasoned argument, not a measured effect. A signal to track: the share of a handful of languages in generated code, and the decline of niche languages.
- Lock-in on languages may matter less if most code becomes disposable. See [scenario 3](../scenarios/03-all-harness.md).

## Related

- [Scenario 1: lock-in](../scenarios/01-lock-in.md)
- [Scenario 5: the language under the language](../scenarios/05-language-under-the-language.md)
