---
type: Concept
title: Ironies of automation
description: Supervising automation erodes the skill needed to take over when it fails.
tags:
- risk
- skills
status: draft
generated:
  by: claude/claude-fable-5-2
  at: '2026-11-10T19:50:00Z'
sources:
- id: agentic-engineering-2026
  resource: https://developertoolkit.ai/en/ladder/state-of-agentic-engineering-2026/?track=cto
  title: The State of Agentic Engineering, September 2026 (secondary compilation)
- id: bainbridge-1983
  resource: Lisanne Bainbridge, Ironies of Automation, Automatica 19(6), 1983
  title: Ironies of Automation (Bainbridge, 1983)
---

# Ironies of automation

## Claim

The main risk is not that agents write bad code. It is that humans lose the ability to notice.

## The paradox

In 1983, Lisanne Bainbridge described a paradox observed in aviation and industry [^bainbridge-1983]. The more a system is automated, the more the human merely supervises. They then lose the skill needed to take over, at the exact moment the automation fails on a hard case.

## Evidence in software

In a trial run by Anthropic in January 2026, the group coding with AI scored 50% on a comprehension quiz, against 67% for the group coding by hand (via [^agentic-engineering-2026]).

## Objections

- One trial, reported through a secondary source. To verify against the original publication, including sample size and task type.
- A comprehension quiz right after a task does not measure long-term skill.

## Related

- [Automation bias](automation-bias.md)
- [Aviation precedent](../precedents/aviation.md)
- [Open questions](../open-questions.md): how to keep the skill

[^agentic-engineering-2026]: The State of Agentic Engineering, September 2026 (secondary compilation)
[^bainbridge-1983]: Ironies of Automation (Bainbridge, 1983)
