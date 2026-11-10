---
type: Concept
title: Abstract syntax tree (AST)
description: The abstract syntax tree and why code stored as structure matters.
tags:
- ast
- representation
status: draft
generated:
  by: claude/claude-fable-5-2
  at: '2026-11-10T19:50:00Z'
---

# Abstract syntax tree (AST)

## Definition

An abstract syntax tree is the hierarchical representation of a program's logical structure, stripped of cosmetic detail such as whitespace, comments and grouping parentheses.

In the traditional chain:

```
source text  --parsing-->  AST  --compilation-->  bytecode or machine code
```

Today a model produces readable text so that a parser can extract an AST from it. The text layer exists for human readers.

## Why it matters here

Two ideas in this base depend on the AST:

- **Code stored as structure.** If the tree, not the text, is the source of truth, then renaming or moving code is a structural operation instead of a fragile text edit. Unison already stores code as a hashed syntax tree. Text becomes a view generated on demand.
- **Structured generation.** A model can be constrained to emit only valid trees. See [constrained decoding](constrained-decoding.md).

## A correction to v1

The [first synthesis](../archive/v1.md) presented "AST-native" generation as both the end of text and the densest possible format. These two promises conflict: an AST serialized as JSON costs more tokens than the source text it represents, not fewer. The benefit of working on structure is validity and precise edits, not compactness.

## Objections

- Models are trained overwhelmingly on text. Whether they can work as well on structured representations is an open empirical question. See [scenario 6](../scenarios/06-no-language.md).

## Related

- [Real vs overrated limits](../languages/real-vs-overrated-limits.md)
- [Design trajectory](../languages/design-trajectory.md)
