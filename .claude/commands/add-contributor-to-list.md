---
name: add-contributor-to-list
description: Workflow command scaffold for add-contributor-to-list in first-contributions.
allowed_tools: ["Bash", "Read", "Write", "Grep", "Glob"]
---

# /add-contributor-to-list

Use this workflow when working on **add-contributor-to-list** in `first-contributions`.

## Goal

Adds a new contributor's name to the Contributors.md file, typically as a first open source contribution.

## Common Files

- `Contributors.md`

## Suggested Sequence

1. Understand the current state and failure mode before editing.
2. Make the smallest coherent change that satisfies the workflow goal.
3. Run the most relevant verification for touched files.
4. Summarize what changed and what still needs review.

## Typical Commit Signals

- Edit Contributors.md to add a new line with the contributor's name (and sometimes a link or additional info).
- Commit the change with a message referencing the addition.
- Open a pull request (often auto-merged or reviewed).

## Notes

- Treat this as a scaffold, not a hard-coded script.
- Update the command if the workflow evolves materially.