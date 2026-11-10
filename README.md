# 🧋 Nimbi's Claude Code Skills Pack

Thanks for commenting **LEARN AI**! ✨
This pack has 9 skills, 1 helper agent and 2 templates. They make Claude Code plan before it builds, fix bugs properly, explain things simply, and turn your vague prompts into clear "bubble-tea orders".

Made by **@gk.aigenz** · free to use · please don't resell it ([license](LICENSE)).

## ⬇️ Download

**👉 [Download the ZIP](https://github.com/Hackennn/gk.aigenz-free-skill-pack/archive/refs/heads/main.zip)** (one click, no GitHub account needed)

Or with git: `git clone https://github.com/Hackennn/gk.aigenz-free-skill-pack.git`

---

## What's inside

| Skill | Type this | What it does |
|---|---|---|
| 🧋 **bubble-tea-prompt** | `/bubble-tea-prompt write a birthday message` | Turns a vague request into a clear prompt (WHO · WHAT · LENGTH · STYLE) |
| 🗺️ **plan-first** | `/plan-first add a contact form` | Short plan + risks, then waits for your OK before touching files |
| 🔧 **fix-it** | `/fix-it` (paste your error) | Reproduce → find the real cause → smallest fix → prove it works |
| 🐣 **explain-simply** | `/explain-simply what is an API?` | Plain-words explanation with an everyday analogy |
| 🐟 **handoff-summary** | `/handoff-summary` | Saves a `HANDOFF.md` so a fresh chat can continue without forgetting |
| 🌐 **quick-website** | `/quick-website portfolio for a baker` | One-file, mobile-friendly landing page, no setup needed |
| ✅ **review-before-ship** | `/review-before-ship` | Checks your changes for bugs, leaked keys and leftovers before you push |
| 📱 **content-repurpose** | `/content-repurpose` + your script | Hooks, caption, pinned comment, carousel outline from one script |
| 🧭 **learn-this-repo** | `/learn-this-repo` | Beginner tour of any project: what it is, how to run it, where to start |

**Agent:** `second-opinion` is a read-only reviewer. Say "get a second opinion on this" after a big change.

**Templates:**
- `templates/CLAUDE.md`: project memory, so Claude remembers your rules every session
- `templates/settings.json`: a safe preset that auto-allows harmless commands (git status, tests) and blocks reading `.env` secrets and `rm -rf`

You don't always need the `/command`. Claude also picks the right skill on its own when your request matches (e.g. "this is broken, help" → fix-it).

---

## Install (2 minutes)

You need **Claude Code** installed first: https://docs.claude.com/en/docs/claude-code/overview

Unzip the download. You'll get a folder called `gk.aigenz-free-skill-pack-main`. Open a terminal **inside that folder**, then run:

**Mac / Linux**
```bash
mkdir -p ~/.claude/skills ~/.claude/agents
cp -R skills/* ~/.claude/skills/
cp agents/* ~/.claude/agents/
```

**Windows (PowerShell)**
```powershell
New-Item -ItemType Directory -Force "$HOME\.claude\skills", "$HOME\.claude\agents" | Out-Null
Copy-Item -Recurse -Force skills\* "$HOME\.claude\skills\"
Copy-Item -Force agents\* "$HOME\.claude\agents\"
```

Restart Claude Code, type `/`, and you'll see the new skills in the list. 🎉

> Installing into `~/.claude` makes the skills work in **every** project.
> To use them in only one project, copy them into that project's `.claude/skills/` and `.claude/agents/` folders instead.

### Optional: the templates
- **CLAUDE.md**: copy `templates/CLAUDE.md` into your project folder and fill in the `[brackets]`.
- **settings.json**: copy it to `your-project/.claude/settings.json`. If that file already exists, merge the `permissions` lists by hand instead of overwriting it.

---

## Try these first

1. `/bubble-tea-prompt write an email to my boss` and watch a vague prompt become a clear one.
2. `/learn-this-repo` inside any project you downloaded from GitHub.
3. `/quick-website a link-in-bio page for my bubble tea stall, soft pastel style`

## Make them yours
Every skill is a plain text file: `skills/<name>/SKILL.md`. Open it, change the steps or the tone, save, and restart Claude Code. That's it.

---

New fun AI lesson every week with Nimbi 🧋 → **@gk.aigenz**
