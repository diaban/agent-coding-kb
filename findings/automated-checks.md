---
type: Finding
title: Automated checks are taking over from review
description: Automated checks are replacing line-by-line human review.
tags:
- verification
- testing
status: draft
generated:
  by: claude/claude-fable-5-2
  at: '2026-11-10T19:50:00Z'
stale_after: '2027-05-10T00:00:00Z'
sources:
- id: agentic-engineering-2026
  resource: https://developertoolkit.ai/en/ladder/state-of-agentic-engineering-2026/?track=cto
  title: The State of Agentic Engineering, September 2026 (secondary compilation)
---

# Automated checks are taking over from review

## Claim

Teams that let agents write most of their code are replacing "a human read the diff" with "a set of automated checks passed". The human reads evidence instead of code.

## Evidence

- **Stripe relies on more than 3 million tests.** An agent gets at most two continuous-integration runs before a human steps in (via [^agentic-engineering-2026]).
- **"Done" is defined as a list of commands that must pass**: tests, type checking, lint.
- **Review agents read the code**, and the human reads their conclusions instead of the full diff.
- **Circuit breakers are still missing.** Anthropic acknowledges it does not yet have mechanisms that would tighten approval when rollbacks or incidents rise, and says it wants to build them before merging more code without human review (via [^agentic-engineering-2026]).

## Objections

- If tests become the only acceptance criterion, an agent can satisfy them without solving the problem. See [Goodhart's law](../concepts/goodharts-law.md).
- An agent that writes both the code and its tests certifies its own work. See [producer-verifier separation](../concepts/producer-verifier-separation.md).
- Stripe's pull requests are still reviewed by humans. Stripe is evidence that agents write the code, not that nobody reads it.

## Related

- [Review bottleneck](review-bottleneck.md)
- [Finance precedent](../precedents/finance.md): circuit breakers
- [Scenario 2: the specification becomes the language](../scenarios/02-spec-as-language.md)

[^agentic-engineering-2026]: The State of Agentic Engineering, September 2026 (secondary compilation)
