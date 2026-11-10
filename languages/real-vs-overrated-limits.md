# Real vs overrated limits of current languages

## Claim

Current languages do limit agents, but not where the first synthesis said. The real limits concern what an agent cannot know without reading a lot of code. The limits tied to tokenization are mostly overrated.

## The limits

| Limit | Verdict | Why |
| --- | --- | --- |
| Errors detected at run time (Python, JavaScript) | Real | Costly loop: write, run, read a message written for a human, start again |
| Hidden effects (network, database, global state) | Real | The agent has to read a lot of code to know what a function touches |
| Unverifiable contracts | Real | Invariants and assumptions live in comments that drift |
| Text as the only source of truth | Real | Renaming or moving code becomes a fragile text edit |
| Macros and implicit behaviour | Real | What the agent reads differs from what is compiled |
| Several ways to write the same thing | Real, secondary | More ambiguity and variation in what the agent produces |
| Global verbosity (boilerplate, declarations) | Real but bounded | A gain of roughly 1.25x to 2x: useful for cost and latency, not enough to give a global view of a large project |
| Splitting syntax into tokens (operators, indentation) | Overrated | Modern tokenizers merge whitespace and operators such as `===` or `=>` into single tokens |
| Long identifiers | Overrated | An explicit name helps the model; opaque names degrade its performance |

## What v1 claimed

The [first synthesis](../archive/v1.md) built its case on a "token tax":

- identifiers fragmented into 4 to 8 sub-tokens,
- 15% to 30% of the context window spent on cosmetic markers,
- operators split into individual characters,
- a 20% to 50% gain in effective context from a machine-first language.

None of these figures had a source.

## Objections and things to verify

- **The 1.25x to 2x factor is v1's unsourced "20% to 50%" converted into a multiplier.** It is still unsourced. To measure or drop.
- The tokenizer claim should be checked against the tokenizers of current models.
- "Opaque names degrade performance" is plausible and commonly reported, but no study is cited here.
- **Short naming conventions are inconsistent with this table.** The second synthesis listed them as an "optimization" for the current stages while also saying short identifiers hurt. This base takes the second position.

## Related

- [Design trajectory](design-trajectory.md)
- [AST](../concepts/ast.md)
