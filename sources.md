# Sources

## References

| Key | Source |
| --- | --- |
| S1 | [Cloud Next '26: Momentum and innovation at Google scale](https://blog.google/innovation-and-ai/infrastructure-and-cloud/google-cloud/cloud-next-2026-sundar-pichai/), Google, April 2026 |
| S2 | [State of Code Developer Survey](https://www.sonarsource.com/blog/state-of-code-developer-survey-report-the-current-reality-of-ai-coding/), Sonar, January 2026 |
| S3 | [The State of Agentic Engineering, September 2026](https://developertoolkit.ai/en/ladder/state-of-agentic-engineering-2026/?track=cto), a compilation of figures from Anthropic, DX, Stripe, Faros and METR |
| S4 | [Announcing the 2025 DORA Report](https://cloud.google.com/blog/products/ai-machine-learning/announcing-the-2025-dora-report), Google Cloud, September 2025 |
| S5 | [ll-lang](https://github.com/Neftedollar/ll-lang), GitHub repository |
| S6 | [ALaS](https://github.com/dshills/alas), GitHub repository |
| S7 | Lisanne Bainbridge, "Ironies of Automation", *Automatica*, 1983 |

## Verification status

No figure in this base has been checked against its source while building it. All were carried over from the second synthesis document (November 2026). "Secondary" means the figure was taken from the compilation S3 and not from the original publication.

| Figure | Used in | Source | Status |
| --- | --- | --- | --- |
| Google: 75% of new code AI-generated | [ai-authored-code](findings/ai-authored-code.md) | S1 | Not checked |
| Anthropic: over 80% of merged lines | [ai-authored-code](findings/ai-authored-code.md) | S3, secondary | Not checked; find the original |
| DX: 51.9% average share, 27.4% baseline | [ai-authored-code](findings/ai-authored-code.md) | S3, secondary | **Suspect**: the baseline date (Q1 2026) is probably wrong |
| Sonar: 42% of committed code, 65% expected in 2027 | [ai-authored-code](findings/ai-authored-code.md) | S2 | Not checked |
| Stripe: over 1,300 PRs per week with no human-written line | [ai-authored-code](findings/ai-authored-code.md) | S3, secondary | Not checked; find the original |
| Sonar: 96% do not fully trust, 48% always verify, 38% find review harder | [review-bottleneck](findings/review-bottleneck.md) | S2 | Not checked |
| DX: median PR size 44 to 72 lines | [review-bottleneck](findings/review-bottleneck.md) | S3, secondary | Not checked |
| Faros: review time +441%, unreviewed merges +31%, incidents per PR +243% | [review-bottleneck](findings/review-bottleneck.md) | S3, secondary | **Needs context**: no period or baseline given |
| METR: tasks 19% longer (2025), later follow-up | [review-bottleneck](findings/review-bottleneck.md) | S3, secondary | Not checked; find the METR publications |
| Stripe: over 3 million tests, two CI runs maximum | [automated-checks](findings/automated-checks.md) | S3, secondary | Not checked |
| Anthropic: no circuit breakers yet | [automated-checks](findings/automated-checks.md) | S3, secondary | Not checked |
| Anthropic trial: 50% vs 67% on a comprehension quiz | [ironies-of-automation](concepts/ironies-of-automation.md) | S3, secondary | Not checked; find the original |
| Google: complex migration six times faster than a year earlier | [02-spec-as-language](scenarios/02-spec-as-language.md) | None given | **Unsourced** |
| Compression gain of 1.25x to 2x | [real-vs-overrated-limits](languages/real-vs-overrated-limits.md) | None | **Unsourced**, inherited from v1 |
| v1: 15–30% of context wasted, 20–50% gain | [archive/v1](archive/v1.md) | None | **Unsourced**, superseded |

## Main weakness

Most quantitative evidence rests on a single secondary compilation (S3). The priority is to replace each "secondary" entry with its original publication.
