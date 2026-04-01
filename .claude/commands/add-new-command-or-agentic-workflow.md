---
name: add-new-command-or-agentic-workflow
description: Workflow command scaffold for add-new-command-or-agentic-workflow in everything-claude-code.
allowed_tools: ["Bash", "Read", "Write", "Grep", "Glob"]
---

# /add-new-command-or-agentic-workflow

Use this workflow when working on **add-new-command-or-agentic-workflow** in `everything-claude-code`.

## Goal

Adds a new command or agentic workflow to the system, often including new .md command files, agent definitions, and skill orchestrators.

## Common Files

- `commands/*.md`
- `agents/*.md`
- `skills/*/SKILL.md`
- `scripts/*.sh`
- `examples/*`

## Suggested Sequence

1. Understand the current state and failure mode before editing.
2. Make the smallest coherent change that satisfies the workflow goal.
3. Run the most relevant verification for touched files.
4. Summarize what changed and what still needs review.

## Typical Commit Signals

- Create one or more new command markdown files in commands/ (e.g., gan-build.md, santa-loop.md, prp-*.md)
- Add or update agent definitions in agents/ (e.g., gan-generator.md, opensource-forker.md)
- Add or update skill orchestrator in skills/ (e.g., skills/gan-style-harness/SKILL.md, skills/opensource-pipeline/SKILL.md)
- Optionally add shell orchestrators or scripts (e.g., scripts/gan-harness.sh)
- Optionally add documentation or examples

## Notes

- Treat this as a scaffold, not a hard-coded script.
- Update the command if the workflow evolves materially.