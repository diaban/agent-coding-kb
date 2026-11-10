# Scenario 2: the specification becomes the language

## Claim

Code stays in conventional languages, but nobody looks at it. The durable artifact, read and versioned by humans, becomes the specification and its tests. The "new language" appears above the code, not in its place, and it stays human-readable.

## What it looks like

- Specs and tests are versioned, reviewed and discussed more than code.
- Acceptance criteria are reviewed before generation.
- Regenerating costs less than understanding and maintaining, so code is regenerated when the spec changes ("disposable software").
- The durable asset is the spec plus the verification suite, the way a mould and quality control are worth more than one produced part.

## Why it matters most

It changes what humans read without requiring any new programming language. It is therefore compatible with [lock-in](01-lock-in.md) and does not need anyone to break the training-data barrier.

## Signals to watch

- Teams that version specs and regenerate code on each change.
- Full rewrites and migrations handed to agents. Google is reported to have announced a complex migration running six times faster than a year earlier; this figure has no source in the synthesis (see [sources](../sources.md)).
- "Done" defined as commands that must pass (already visible, see [automated checks](../findings/automated-checks.md)).

## Objections

- Natural-language specifications are ambiguous. Making them precise enough to regenerate from may recreate a programming language under another name.
- Regeneration is not deterministic: two generations from the same spec can differ in behaviour not covered by tests. See [compilers](../precedents/compilers.md).
- It depends entirely on test quality. See [Goodhart's law](../concepts/goodharts-law.md).

## Related

- [Verification bottleneck](../concepts/verification-bottleneck.md)
- [Open questions](../open-questions.md): who is accountable when nobody read the code
