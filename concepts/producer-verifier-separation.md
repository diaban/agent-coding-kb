---
type: Concept
title: Separation between producer and verifier
description: Whoever produces the work should not certify it.
tags:
- verification
- risk
status: draft
generated:
  by: claude/claude-fable-5-2
  at: '2026-11-10T19:50:00Z'
---

# Separation between producer and verifier

## Claim

Whoever produces the work should not certify it. An agent that writes both the code and its tests breaks that principle.

## Background

Financial audit and civil engineering inspection rest on this separation.

## Emerging practices

- Tests written independently of the implementation.
- A review model distinct from the authoring model.
- Specifications written before generation.

## Objections

- Two models from the same family, trained on similar data, may not be independent in the sense an auditor is. How much independence a second model provides is unmeasured here.

## Related

- [Goodhart's law](goodharts-law.md)
- [Automated checks take over](../findings/automated-checks.md)
