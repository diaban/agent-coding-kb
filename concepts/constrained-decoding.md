# Grammar-constrained decoding

## Claim

A model's output can be restricted, token by token, to what a formal grammar allows. Syntax errors then become impossible by construction. This is the most concrete idea from the first synthesis, and it is worth keeping.

## How it works

At each generation step, the decoder masks every token that would make the output invalid under a given grammar or schema. The model can only choose among continuations that keep the output well formed.

## What it guarantees, and what it does not

| Guaranteed | Not guaranteed |
| --- | --- |
| The output parses | The program type-checks |
| It matches the schema | It does what was asked |
| No unbalanced brackets or malformed nodes | It is efficient or secure |

Syntax is the cheapest class of error to catch. Constrained decoding removes it entirely, but the costly errors are semantic. That is why this base ranks [guarantees checked by a compiler](../languages/design-trajectory.md) above syntactic validity.

## Objections

- Constraining output can shift the model away from what it would naturally produce and may reduce quality on some tasks. To verify against current research.
- It does not reduce token count. See the correction in [AST](ast.md).

## Related

- [AST](ast.md)
- [Scenario 6: no language at all](../scenarios/06-no-language.md)
- [archive/v1.md](../archive/v1.md), step 4
