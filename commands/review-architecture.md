---
description: "Check structural integrity, pattern consistency, and coupling in code changes."
argument-hint: "[optional focus area or file paths]"
context: fork
agent: architecture-reviewer
---

Review the following code changes.

## Changed files
!`git diff --name-only HEAD`

## Diff
!`git diff HEAD`

## Additional context
$ARGUMENTS
