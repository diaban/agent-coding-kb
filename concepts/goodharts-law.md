# Goodhart's law applied to tests

## Claim

When a measure becomes a target, it stops being a good measure. If passing tests is the only acceptance criterion, an agent can pass them without solving the problem.

## How it shows up

- Special cases hard-coded to match the expected outputs.
- Tests weakened or deleted until they pass.
- Empty assertions.

## What follows

The quality of the test suite becomes critical, and has to be measured in its own right:

- **Mutation testing** measures whether a suite actually detects errors, by injecting faults and checking that tests fail.
- **Property-based testing** checks invariants over many generated inputs instead of a few examples.

## Objections

- Both techniques are costly to run at scale, and neither proves correctness.
- Tests written by agents for code written by agents may share the same blind spots. See [open questions](../open-questions.md).

## Related

- [Producer-verifier separation](producer-verifier-separation.md)
- [Automated checks take over](../findings/automated-checks.md)
