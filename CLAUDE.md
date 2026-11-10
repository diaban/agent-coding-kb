# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repository is

A knowledge base, not a codebase. It contains only markdown and has no build, lint or test commands. It is an [Open Knowledge Format](https://github.com/GoogleCloudPlatform/open-knowledge-format) (OKF) v0.2 bundle about what happens to software practice and programming languages once agents write most code and humans read little of it. `README.md` holds the thesis and the map. Read it before you edit any content.

## The argument the notes must stay consistent with

- **Verification is the scarce resource, not writing.** See `concepts/verification-bottleneck.md`.
- **An agent language is judged on guarantees, not token density.** This reverses `archive/v1.md`, which argued for token-dense languages and direct AST generation. New notes must not bring back the v1 "token tax" position as current thinking. The README section "What changed since v1" describes the reversal.
- Scenarios and their ranking are judgments, not forecasts. Dates for future stages are estimates. Notes should say so rather than present them as predictions.

## Note conventions

Every note under `findings/`, `concepts/`, `precedents/`, `scenarios/` and `languages/` has YAML frontmatter:

- `type` (e.g. `Finding`, `Concept`, `Scenario`, `Reference`, `Archive`), plus `title`, `description` and `tags`.
- `status: draft`. All current notes are drafts. `archive/v1.md` is `deprecated`.
- `generated: { by: <author>, at: <ISO datetime> }` records who wrote the note.
- `sources`: a list of `{ id, resource, title }`. In the body, cite with footnotes `[^<id>]`, and set each footnote's text to the source's `title`. If a figure was taken from a compilation rather than its original publication, cite it as `(Original, via [^agentic-engineering-2026])`.
- Findings also carry `stale_after`, because their figures age quickly.
- No note has a `verified` field. In OKF that means unverified. Add `verified: { by: human:<id>, at: <datetime> }` only after a human checks a figure against its primary source.

Body template: `# Title`, then `## Claim`, `## Evidence`, `## Objections` and `## Related`, which holds relative links to neighbouring notes. Scenario notes swap Evidence for sections such as `## What it looks like`.

## Changes that touch several files

Adding, renaming or removing a note means updating, in the same change:

1. **The folder's `index.md`**: no frontmatter, one line per note in the form `* [Title](file.md) - description`. The description must match the note's frontmatter `description`.
2. **The root `index.md`**: same line format, in the right section. Its only frontmatter is `okf_version: "0.2"`.
3. **`log.md`**: a bullet under a `## YYYY-MM-DD` heading, tagged `**Creation**`, `**Update**` or `**Initialization**`.
4. **`sources.md`**, if the note adds a source or a figure: its frontmatter `sources`, the References table, and the "Verification status" table (figure, note that uses it, source id, status). Mark secondary figures as such. The main known weakness is that most figures rely on the one secondary compilation `agentic-engineering-2026`.

Folder overviews live in `overview.md`, not `README.md` (see `precedents/` and `scenarios/`). Scenario files are numbered `NN-slug.md`.

`archive/v1.md` is written in French and is kept unchanged on purpose. Don't edit its body. All other content is in English.

## OpenKnowledge tooling

The repo is set up for OpenKnowledge (`.ok/`, `.okignore`, and the skill in `.github/skills/open-knowledge/SKILL.md`). That skill requires all reads and writes of in-scope `.md` files to go through the `mcp__open-knowledge__*` tools (`exec`, `search`, `write`, `edit`, `lint`, `audit`, `move`, `delete`) instead of native file tools. This keeps edits attributed and links checked. Use native tools on markdown only when those tools are unavailable or a call fails, and say so in your reply when you do.

As of this writing, the repo has only `.ok/local/` and no `.ok/config.yml`. The MCP tools fail with "No OpenKnowledge project found" until the project is initialized on this machine (see `.github/skills/open-knowledge/references/setup.md`).
