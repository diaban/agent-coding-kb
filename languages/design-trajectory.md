# Design trajectory for an agent language

## Claim

A language designed for agents will stand out by its guarantees more than by its token density. Current languages were designed for humans who keep context in their heads, which is exactly what an agent lacks.

## Five steps

1. **Strict typing and machine-readable errors.** Already here with TypeScript and Rust.
2. **Explicit effects and contracts.** The pieces exist separately: Koka for effects; Dafny, Lean or Verus for proven contracts.
3. **Code stored as structure**, with a human view generated on demand. Unison already stores code as a hashed syntax tree. See [AST](../concepts/ast.md).
4. **Verified summaries at every level.** Each module exposes a signature, its effects and its invariants, guaranteed by the compiler. The agent loads the graph of these summaries for the whole project and only unfolds an implementation on demand.
5. **Learned representations.** In the longer term, the densest format may not be designed by humans but learned by the models.

## Why step 4 matters

It is what would give an agent a global view of a real project. Compression alone is bounded (see [real vs overrated limits](real-vs-overrated-limits.md)); a compiler-verified summary lets the agent skip the implementation safely, which is a different order of gain.

## Objections

- Steps 1 to 3 exist in separate languages; no production language combines them.
- Step 5 is speculation and runs into the verification obstacle described in [scenario 6](../scenarios/06-no-language.md).
- The sequence is a design argument, not an observed trend.

## Related

- [Cold start](cold-start.md)
- [Constrained decoding](../concepts/constrained-decoding.md)
- [Existing projects](existing-projects.md)
