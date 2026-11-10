---
name: plan-first
description: Make a short, concrete plan before building anything non-trivial, then wait for approval. Use when the user asks for a new feature, a multi-file change or a new project, or says "plan first", "how would you build", or "/plan-first".
---

# Plan first, build second

Rushing into code is how AI makes a mess. One minute of planning saves thirty minutes of fixing.

## Steps

1. **Understand.** Restate the goal in one sentence. Read the files that matter (search, don't guess). Note what already exists that can be reused.
2. **Plan.** At most 7 numbered steps. Each step names the file(s) it touches and what changes.
3. **Risks.** Up to 3 things that could go wrong or are unclear (data loss, breaking changes, missing info).
4. **Done means.** One line: how we will know it works (a command to run, a page to open, a test to pass).
5. **Stop and ask.** End with "Go ahead with this plan?" and do not edit files until the user says yes.

## Rules

- Smallest plan that solves the problem. No "nice to have" extras unless asked.
- Prefer changing existing code over adding new files.
- If the request is tiny (one obvious edit), skip the plan and just do it.
