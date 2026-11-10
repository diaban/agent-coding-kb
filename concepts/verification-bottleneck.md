# The verification bottleneck

## Claim

When writing code costs almost nothing, the scarce resource becomes the human attention able to establish that the code is correct. The bottleneck of software development moves from production to verification.

## Reasoning

For decades, writing cost more than reading, and the person who wrote the code understood it while creating it. With an agent, that understanding exists nowhere: it has to be rebuilt by reading. Every pull request adds to a verification debt.

Three responses are already visible:

1. **Read less, but read evidence.** The human no longer reads the diff; they check that tests, types and controls passed.
2. **Delegate review.** A second model reviews the first one's code, and the human arbitrates its remarks.
3. **Move upstream.** Human attention shifts to what defines the work: specifications, acceptance criteria, architecture.

Human effort therefore concentrates at both ends of the chain: defining what to build, then judging the evidence that it is correct.

## Consequence

The value of a team moves with the bottleneck. A large, trustworthy test suite becomes a more strategic asset than the code it verifies, because it is what makes it possible to let agents work.

## Objections

- The claim rests on adoption and review figures that are mostly unverified. See [findings](../findings/review-bottleneck.md).
- Reading evidence only works if the evidence means something. See [Goodhart's law](goodharts-law.md).

## Related

- [Precedents](../precedents/README.md): the same shift in other industries
- [Inertia and lock-in](inertia-lock-in.md)
- [Scenario 2: the specification becomes the language](../scenarios/02-spec-as-language.md)
