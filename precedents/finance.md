# Market finance

## What was automated

Trading, through algorithms.

## What replaced human inspection

Risk limits and circuit breakers, strengthened after the flash crash of 2010.

## Lesson for code

Put automatic circuit breakers in place for when incidents get out of hand, because they act before a human has time to react. For software, that means approval rules that tighten on their own when rollbacks or incidents per pull request rise.

## State of play

Anthropic reports not having such breakers yet (see [automated checks](../findings/automated-checks.md)).

## Where the analogy breaks

Markets have a single, fast, shared signal: price. Software incidents are heterogeneous and often detected late, so the trigger is harder to define.

## Related

- [Precedents overview](README.md)
- [Scenario 4: the backlash](../scenarios/04-backlash.md)
