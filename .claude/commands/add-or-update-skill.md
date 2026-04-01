---
name: add-or-update-skill
description: Workflow command scaffold for add-or-update-skill in everything-claude-code.
allowed_tools: ["Bash", "Read", "Write", "Grep", "Glob"]
---

# /add-or-update-skill

Use this workflow when working on **add-or-update-skill** in `everything-claude-code`.

## Goal

Adds a new skill or updates an existing skill for an agentic workflow, including documentation and sometimes related manifests.

## Common Files

- `skills/*/SKILL.md`
- `.agents/skills/*/SKILL.md`
- `AGENTS.md`
- `README.md`
- `README.zh-CN.md`
- `docs/zh-CN/AGENTS.md`

## Suggested Sequence

1. Understand the current state and failure mode before editing.
2. Make the smallest coherent change that satisfies the workflow goal.
3. Run the most relevant verification for touched files.
4. Summarize what changed and what still needs review.

## Typical Commit Signals

- Create or update a SKILL.md file under skills/{skill-name}/ or .agents/skills/{skill-name}/
- Optionally update AGENTS.md, README.md, and localized docs
- Update manifests/install-modules.json and/or install-components.json if the skill is part of installable modules
- Optionally add or update related agent markdown files
- Optionally update tests or scripts if the skill introduces new hooks or behaviors

## Notes

- Treat this as a scaffold, not a hard-coded script.
- Update the command if the workflow evolves materially.