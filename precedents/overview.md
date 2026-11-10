---
type: Overview
title: Precedents from other industries
description: Five industries that automated production and what replaced human inspection.
tags:
- precedents
status: draft
generated:
  by: claude/claude-fable-5-2
  at: '2026-11-10T19:50:00Z'
---

# Precedents from other industries

## Claim

Each time an industry automated its production, human inspection of the product gave way to control of the process. Software is on the same path, with a few decades of hindsight available.

## Overview

| Field | What was automated | What replaced human inspection | Lesson for code |
| --- | --- | --- | --- |
| [Manufacturing](manufacturing.md) | Series production | Statistical process control, built-in quality, stopping the line at the first defect | Steer the pipeline instead of inspecting each diff |
| [Compilers](compilers.md) | Translation to assembly | Trust in the tool and its tests | A level stops being read once the tool producing it is reliable enough |
| [Chip design](chip-design.md) | Logic synthesis, place and route | Simulation, formal equivalence checking, automatic design rules | Verification becomes the core of the job |
| [Aviation](aviation.md) | Autopilot, fly-by-wire | Certification with traceability from requirement to test | Match rigour to criticality |
| [Market finance](finance.md) | Algorithmic trading | Risk limits and circuit breakers | Automatic breakers that act before a human can |

## Four regularities

1. **The process is controlled, no longer the product.** Exhaustive inspection is dropped in favour of indicators on the pipeline.
2. **The level of abstraction rises.** The lower level becomes an implementation detail nobody reads.
3. **Verification becomes the dominant cost.** It absorbs the effort freed by automating production.
4. **Regulation follows incidents.** Certification, standards and circuit breakers arrive after the first visible failures, rarely before.

## Objections

- These are analogies. Each one breaks somewhere, and each note says where. The most important break is in [compilers](compilers.md): a compiler is deterministic, an agent is not.
- The cases were selected because they fit. Industries where automation stalled or was rolled back are not covered.

## Related

- [Verification bottleneck](../concepts/verification-bottleneck.md)
- [Scenario 4: the backlash](../scenarios/04-backlash.md)
