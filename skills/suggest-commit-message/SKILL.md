---
name: suggest-commit-message
description: Suggest a concise Conventional Commit message from a git diff, staged changes, or a change summary. Use for commit-message help or choosing a commit type such as feat, fix, docs, refactor, test, or chore.
---

# Suggest Commit Message

Suggest one accurate, concise commit message using:

```text
<type>[optional scope][optional !]: <imperative description>
```

## Rules

- Use the diff or user summary; do not invent details.
- Choose the primary type: `feat` (new capability), `fix` (bug), `docs`, `refactor`, `test`, `build`, `ci`, or `chore` (maintenance/configuration).
- Add a scope only when it improves clarity.
- Use a lowercase imperative description with no trailing period.
- Add `!` only for a confirmed breaking change.

Return the recommendation in a code block. Add a brief explanation only when the choice is ambiguous; otherwise provide one message.

Example for adding project tooling:

```text
chore: add mise configuration
```
