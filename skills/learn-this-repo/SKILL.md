---
name: learn-this-repo
description: Give a beginner-friendly tour of an unfamiliar project or GitHub repo - what it does, how it's organised, how to run it and where to start. Use when the user opens a new codebase or clones a repo, asks "what is this project", "how do I run this", "explain this repo", or types "/learn-this-repo".
---

# Learn this repo

1. **Scan, don't read everything.** Look at the README, package.json / pyproject.toml / requirements.txt, the top-level folders, entry points (main, index, app, server) and any docs/ folder.
2. **Write the tour** in this shape:

```
## What it is
<2 sentences, plain words>

## How it's organised
- folder/: what lives here
(5–8 lines max)

## How to run it
1. install: <exact command from the repo>
2. start: <exact command>
3. open: <url or what you should see>

## How it works (the main flow)
<3–5 steps: input comes in → ... → result>

## Good first things to try
- <a small, safe change or experiment>
```

3. Only give commands you actually found in the repo. If something is missing (env vars, API keys), say exactly what. Never guess secrets.
4. Offer: "Want me to run it for you?"
