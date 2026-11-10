# Human review no longer keeps up

## Claim

The volume of generated code has grown while human review capacity stayed roughly fixed. Line-by-line review, a pillar of software quality for decades, is becoming economically untenable.

## Evidence

- **Low trust, partial checking.** 96% of developers do not fully trust generated code, but only 48% systematically verify it before committing [S2].
- **Review is harder.** 38% find reviewing AI code more demanding than reviewing a colleague's code [S2].
- **Larger pull requests.** Median size went from 44 to 72 lines between July 2025 and June 2026 (DX, via [S3]).
- **Reviews being skipped.** Across 22,000 developers, median time in review rose 441%, PRs merged without review rose 31%, and incidents per PR rose 243% (Faros, April 2026, via [S3]).
- **More throughput, more instability.** The 2025 DORA report describes AI as an amplifier: it speeds up strong teams and exposes the weaknesses of others [S4].

## Objections

- **The Faros figures lack context.** No period or baseline is given for the 441% and 243% increases, and they come through a secondary compilation. To verify.
- **The productivity gain itself is disputed.** A 2025 METR study measured tasks taking 19% longer for experienced developers using AI. Its 2026 follow-up points toward a speed-up, but METR itself considers that signal unreliable (via [S3]).
- Survey answers (Sonar) describe what developers say they do, not what they do.

## Related

- [AI-authored code](ai-authored-code.md)
- [Automated checks take over](automated-checks.md)
- [Verification bottleneck](../concepts/verification-bottleneck.md)
