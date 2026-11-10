---
type: Scenario
title: 'Scenario 3: all-harness'
description: Most code becomes disposable under an agent harness; software splits into two layers.
tags:
- scenarios
- harness
status: draft
generated:
  by: claude/claude-fable-5-2
  at: '2026-11-10T19:50:00Z'
---

# Scenario 3: all-harness

## Claim

If agents become the main interface, the application stops being a visible product. Most code becomes disposable: written, run once, deleted. Software does not disappear; it splits into two layers.

## What it looks like

The user states an intent and a harness of agents carries it out. It composes tools, writes throwaway code, and generates an interface if needed. No fixed menus or screens.

Three consequences:

- **Code becomes a means, not a product.**
- **The language that matters is the tool interface**: schemas, protocols such as MCP, permissions.
- **Verification moves from compile time to run time**: sandboxes, access policies, audit logs, reversible actions. What is controlled is what the agent is allowed to do, not a piece of code.

## What resists

- **Cost and determinism.** Redoing the reasoning on every request is expensive and does not always give the same result. A task repeated millions of times ends up frozen into code, the way a JIT compiler compiles the hottest paths.
- **Shared state.** A bank, a marketplace or a booking system are rules and data shared by millions of people. The interface can fade; that base cannot.
- **The harness is itself software.** Models, inference engines, databases and tools form a substrate that becomes even more critical.

## Two layers

| Layer | Content | What "language" means there |
| --- | --- | --- |
| Ephemeral actions | Throwaway scripts, generated interfaces | Protocols and permissions |
| Verified base | What is repeated, shared or critical | Languages centred on guarantees |

## A further threshold: agent-decided crystallization

When the frequency of a task multiplied by the cost of reasoning exceeds the cost of freezing it, the agent itself writes durable software from its own execution traces. Speculative.

## Signals to watch

- Share of tasks solved by code that is never committed.
- Durable code produced by agents from their own traces.

## Objections

- If this scenario wins broadly, a dedicated agent language ([scenario 5](05-language-under-the-language.md)) loses much of its interest.
- Run-time control assumes actions are reversible, which many real-world actions are not.

## Related

- [Scenario 2](02-spec-as-language.md): disposable software
- [Existing projects](../languages/existing-projects.md): ALaS
