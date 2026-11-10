# Scenario 4: the backlash

## Claim

Serious incidents lead to audit requirements. Human readability becomes mandatory again in regulated sectors, and languages there evolve toward more clarity, not less.

This is the counter-scenario. It was missing from both syntheses.

## What it looks like

- Standards, certification or insurance for generated code.
- Contractual clauses requiring human review above a criticality level.
- Approval that tightens automatically when incidents rise (circuit breakers).
- A split between regulated code, kept auditable, and everything else.

## Why it is plausible

In every [precedent](../precedents/README.md), regulation followed incidents. The [findings](../findings/review-bottleneck.md) already report rising incidents per pull request, if those figures hold.

## Signals to watch

- First contractual or regulatory requirements on verification of generated code.
- A widely publicized incident attributed to unreviewed generated code.
- Incident thresholds per pull request that trigger mandatory review.

## Objections

- Regulation may require evidence (tests, traceability) and not human reading. In that case it reinforces [scenario 2](02-spec-as-language.md) instead of opposing it.
- It would likely stay confined to regulated sectors.

## Related

- [Aviation](../precedents/aviation.md), [finance](../precedents/finance.md)
- [Open questions](../open-questions.md): who is accountable
