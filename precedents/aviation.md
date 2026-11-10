---
type: Precedent
title: Aviation
description: Aviation certifies software by tracing each requirement to its tests.
tags:
- precedents
- certification
status: draft
generated:
  by: claude/claude-fable-5-2
  at: '2026-11-10T19:50:00Z'
---

# Aviation

## What was automated

Automatic piloting and fly-by-wire controls.

## What replaced human inspection

Certification of embedded software (DO-178C): traceability from every requirement to its tests, and levels of criticality that set the required rigour.

## Lesson for code

Match the rigour of verification to criticality, and link each specification to its evidence.

## Where the analogy breaks

Certification is slow and expensive by design, and applies to a narrow class of software. It is a model for critical code, not for the bulk of what agents write.

## Related

- [Precedents overview](overview.md)
- [Ironies of automation](../concepts/ironies-of-automation.md): the same field produced the warning about lost skills
- [Scenario 4: the backlash](../scenarios/04-backlash.md)
