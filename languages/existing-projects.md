# Existing projects

## Claim

Projects building languages for agents mostly put forward reliability, not compactness. They remain experimental.

## ll-lang

- Presents itself as typed and token-efficient, with errors formatted to be read by an LLM.
- Compiles to F#, TypeScript, Python and Java.
- Works around the lack of training data and ecosystem by targeting existing languages.
- Repository: [S5]

## ALaS

- Built on a canonical JSON format validated by a schema.
- Its promise is the absence of ambiguity, not compactness.
- Repository: [S6]

**To clarify.** The second synthesis described ALaS once as a language and once as a tool "designed to orchestrate agents rather than to write applications". The repository should be read to settle which it is.

## Related ideas already in production languages

- **Unison** stores code as a hashed syntax tree.
- **Koka** makes effects explicit in types.
- **Dafny, Lean, Verus** support contracts that are proven.
- **TypeScript and Rust** already provide strict typing and structured errors.

## Objections

- Descriptions here come from the projects' own presentation and have not been tested.
- Both projects face the obstacle common to any new agent language: no training data. See [cold start](cold-start.md).

## Related

- [Scenario 5: the language under the language](../scenarios/05-language-under-the-language.md)
- [Design trajectory](design-trajectory.md)
