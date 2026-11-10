---
name: review-before-ship
description: Review the current changes before committing or publishing - bugs, leaked secrets, leftovers and missing checks - and report only real problems. Use when the user says "review", "check my changes", "is this ready", "before I push", or "/review-before-ship".
---

# Review before ship

1. See what changed: `git status` and `git diff` (staged and unstaged). If it isn't a git repo, ask which files changed.
2. Check every change against this list:
   - **Breaks**: wrong logic, typos in names, empty/null cases not handled, off-by-one, wrong file paths
   - **Secrets**: API keys, passwords, tokens, `.env` contents or personal data added to code or commits
   - **Leftovers**: debug logs, commented-out code, TODOs that block release, test-only shortcuts
   - **Safety**: deleting data without confirmation, running user input as code or SQL, wide-open permissions
   - **Proof**: was it actually run or tested? If not, say so
3. Report a short list, most serious first:
   `file:line - problem - suggested fix`
   If nothing is wrong, say "Looks ready" and list what you checked.
4. Don't change any files unless the user asks you to fix the findings.
