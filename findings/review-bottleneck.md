---
type: Finding
title: Human review no longer keeps up
description: Human review capacity no longer keeps up with generated code.
tags:
- review
- metrics
status: draft
generated:
  by: claude/claude-fable-5-2
  at: '2026-11-10T19:50:00Z'
stale_after: '2027-05-10T00:00:00Z'
sources:
- id: sonar-state-of-code-2026
  resource: https://www.sonarsource.com/blog/state-of-code-developer-survey-report-the-current-reality-of-ai-coding/
  title: State of Code Developer Survey (Sonar, January 2026)
- id: agentic-engineering-2026
  resource: https://developertoolkit.ai/en/ladder/state-of-agentic-engineering-2026/?track=cto
  title: The State of Agentic Engineering, September 2026 (secondary compilation)
- id: dora-2025
  resource: https://cloud.google.com/blog/products/ai-machine-learning/announcing-the-2025-dora-report
  title: Announcing the 2025 DORA Report (Google Cloud, September 2025)
---

# Human review no longer keeps up

## Claim

The volume of generated code has grown while human review capacity stayed roughly fixed. Line-by-line review, a pillar of software quality for decades, is becoming economically untenable.

## Evidence

- **Low trust, partial checking.** 96% of developers do not fully trust generated code, but only 48% systematically verify it before committing [^sonar-state-of-code-2026].
- **Review is harder.** 38% find reviewing AI code more demanding than reviewing a colleague's code [^sonar-state-of-code-2026].
- **Larger pull requests.** Median size went from 44 to 72 lines between July 2025 and June 2026 (DX, via [^agentic-engineering-2026]).
- **Reviews being skipped.** Across 22,000 developers, median time in review rose 441%, PRs merged without review rose 31%, and incidents per PR rose 243% (Faros, April 2026, via [^agentic-engineering-2026]).
- **More throughput, more instability.** The 2025 DORA report describes AI as an amplifier: it speeds up strong teams and exposes the weaknesses of others [^dora-2025].

## Objections

- **The Faros figures lack context.** No period or baseline is given for the 441% and 243% increases, and they come through a secondary compilation. To verify.
- **The productivity gain itself is disputed.** A 2025 METR study measured tasks taking 19% longer for experienced developers using AI. Its 2026 follow-up points toward a speed-up, but METR itself considers that signal unreliable (via [^agentic-engineering-2026]).
- Survey answers (Sonar) describe what developers say they do, not what they do.

## Related

- [AI-authored code](ai-authored-code.md)
- [Automated checks take over](automated-checks.md)
- [Verification bottleneck](../concepts/verification-bottleneck.md)

[^sonar-state-of-code-2026]: State of Code Developer Survey (Sonar, January 2026)
[^agentic-engineering-2026]: The State of Agentic Engineering, September 2026 (secondary compilation)
[^dora-2025]: Announcing the 2025 DORA Report (Google Cloud, September 2025)
