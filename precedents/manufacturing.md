---
type: Precedent
title: Manufacturing
description: Manufacturing replaced inspection of parts with control of the process.
tags:
- precedents
- process-control
status: draft
generated:
  by: claude/claude-fable-5-2
  at: '2026-11-10T19:50:00Z'
---

# Manufacturing

## What was automated

Series production.

## What replaced human inspection

- Statistical process control (Shewhart): monitor the process with indicators instead of inspecting every part.
- Built-in quality (Deming): quality is designed into the process, not added by inspection at the end.
- Stopping the line at the first defect (Toyota).

## Lesson for code

Steer the pipeline instead of inspecting each diff, and stop the pipeline when an indicator degrades.

## Where the analogy breaks

Manufactured parts are meant to be identical, so sampling works. Every pull request is different, so a statistical sample of diffs says less about the ones not sampled.

## Related

- [Precedents overview](overview.md)
- [Automated checks take over](../findings/automated-checks.md)
