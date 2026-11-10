---
name: bubble-tea-prompt
description: Turn a vague request into a clear, specific prompt using the bubble-tea order method (WHO / WHAT / LENGTH / STYLE + context). Use when the user says "improve my prompt", "make this prompt better", "/bubble-tea-prompt", or gives a one-line request that is missing who it's for, what exactly they want, how long, or what style.
---

# Bubble-tea prompt

A vague order gets a random drink. A clear order gets the perfect one.
Your job: turn the user's request into a "regular's order" before doing any work.

## Steps

1. Read the request (from `$ARGUMENTS` if given, otherwise the user's last message).
2. Fill the 4 slots. Take each from the request or the context when it is there; never invent facts about the user.
   - **WHO**: who it's for / who will read it (audience, age, expertise)
   - **WHAT**: the exact thing to produce (email, list, code, table, script…)
   - **LENGTH**: how long (sentences, words, bullets, seconds, lines of code)
   - **STYLE**: tone and voice (warm, formal, funny, simple English, Malay / Chinese / English…)
3. Add the optional extras only if they matter: **CONTEXT** (background facts the AI needs), **MUST / MUST NOT** (constraints), **EXAMPLE** (a sample of the style they like).
4. If 2 or more of the 4 slots are truly unknown, ask ONE short question that covers them all, with suggested answers. Otherwise pick sensible defaults and say which ones you picked.
5. Show the result in this shape:

```
☕ ORDER CARD
WHO:    ...
WHAT:   ...
LENGTH: ...
STYLE:  ...
(CONTEXT / MUST / EXAMPLE if used)

✨ Upgraded prompt:
"..."
```

6. Ask "Run it now?" If the user says yes (or already asked you to just do it), carry out the upgraded prompt.

## Example

Input: `write a birthday message`

```
☕ ORDER CARD
WHO:    my mum, turning 60
WHAT:   a birthday message for a card
LENGTH: 3 sentences
STYLE:  warm, a bit funny

✨ Upgraded prompt:
"Write a birthday message for my mum, who is turning 60. Keep it to 3 sentences, warm and a bit funny, suitable for a handwritten card."
```

(The WHO came from the user's answer to the one clarifying question.)
