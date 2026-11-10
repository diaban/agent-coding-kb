# Agent coding knowledge base

Notes on what happens to software practice and programming languages once agents write most of the code and humans read little of it.

## Thesis

Code is less and less read by humans, yet agents keep writing it in languages designed to be read by humans. That gap is held in place by inertia: community, ecosystems, and above all the training data that makes models best at the most popular languages.

This knowledge base asks what that tension produces over time, and which thresholds ("singularities") it could cross: stricter versions of today's languages, specifications replacing code as the thing humans read, an all-harness world of disposable code, a language built for agents, or no language at all.

Two positions structure the notes:

1. **The scarce resource is verification, not writing.** When producing code costs almost nothing, what limits a team is the human attention needed to establish that the code is correct. See [verification bottleneck](concepts/verification-bottleneck.md).
2. **A language for agents will be judged on guarantees, not token density.** The first version of this work argued the opposite; see [what changed since v1](#what-changed-since-v1).

## Map

| Folder | What it holds |
| --- | --- |
| [findings/](findings/) | What the numbers say today: share of AI-written code, the review bottleneck, the shift to automated checks |
| [concepts/](concepts/) | The ideas the argument rests on |
| [precedents/](precedents/README.md) | Industries that automated production before software did |
| [scenarios/](scenarios/README.md) | Six possible futures, with the signals that would confirm each |
| [languages/](languages/) | What actually limits agents in current languages, existing projects, the cold-start problem |
| [open-questions.md](open-questions.md) | What this base does not answer |
| [sources.md](sources.md) | Every figure, its source, and whether it has been checked |
| [archive/v1.md](archive/v1.md) | The first synthesis (in French), kept unchanged |

## How to read a note

Each note follows the same template:

- **Claim**: the point in one or two sentences.
- **Evidence**: what supports it, with links to [sources.md](sources.md).
- **Objections**: what weakens it or remains unproven.
- **Related**: neighbouring notes.

## Status of the content

- Figures come from the second synthesis document (November 2026). Most were taken from one secondary compilation and have **not** been checked against primary sources. [sources.md](sources.md) tracks the status of each.
- Scenarios and their ranking are judgments, not forecasts.
- Dates attached to future stages are estimates.

## What changed since v1

The [first synthesis](archive/v1.md) argued that human-readable languages impose a "token tax" on models and that languages would evolve toward maximum density, ending in direct generation of syntax trees.

The current position keeps the question and reverses the answer:

| | v1 | Now |
| --- | --- | --- |
| Scarce resource | The context window | Human attention spent on verification |
| What makes a good agent language | Density per token | Verifiable guarantees |
| Driver of change | Technical (tokenization) | Economic (cost of review) |
| Precondition | None | Nobody reads the code any more |

What v1 got wrong, and one idea from it worth keeping, are covered in [real vs overrated limits](languages/real-vs-overrated-limits.md) and [constrained decoding](concepts/constrained-decoding.md).
