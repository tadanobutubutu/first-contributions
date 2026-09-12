---
name: add-or-update-readme-translation
description: Workflow command scaffold for add-or-update-readme-translation in first-contributions.
allowed_tools: ["Bash", "Read", "Write", "Grep", "Glob"]
---

# /add-or-update-readme-translation

Use this workflow when working on **add-or-update-readme-translation** in `first-contributions`.

## Goal

Adds or updates a translated version of the README file for a specific language.

## Common Files

- `docs/translations/README.*.md`
- `Contributors.md`

## Suggested Sequence

1. Understand the current state and failure mode before editing.
2. Make the smallest coherent change that satisfies the workflow goal.
3. Run the most relevant verification for touched files.
4. Summarize what changed and what still needs review.

## Typical Commit Signals

- Edit or create docs/translations/README.[lang].md for the target language.
- Optionally update Contributors.md to credit the translator.
- Commit the changes with a message referencing the translation.
- Open a pull request.

## Notes

- Treat this as a scaffold, not a hard-coded script.
- Update the command if the workflow evolves materially.