---
name: handoff-summary
description: Write a compact handoff summary of the current session so work can continue in a fresh chat without losing context. Use when the chat is getting long, before /clear, when switching tasks, or when the user says "handoff", "summarize for a new chat", or "/handoff-summary".
---

# Handoff summary

AI is a goldfish: in long chats, old details get pushed out. Before starting fresh, save what matters.

Write the summary in exactly this shape. Save it as `HANDOFF.md` in the project root, replacing any old one, and show it to the user.

```markdown
# Handoff · <date>

## Goal
<one or two sentences: what we are trying to achieve>

## Done so far
- <finished item> (<file or command>)

## Current state
- Works: ...
- Broken / unverified: ...

## Decisions & preferences
- <choices made and why; user preferences to keep>

## Next steps
1. <the very next action>
2. ...

## Key files
- `path/to/file`: what it is
```

## Rules

- Facts only. Mark anything not checked as "unverified".
- Keep it under ~40 lines. Link to files instead of pasting code.
- Finish with: "Start a new chat and paste: `Read HANDOFF.md and continue from Next steps.`"
