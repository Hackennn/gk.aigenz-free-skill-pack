---
name: fix-it
description: Calm, step-by-step bug fixing - reproduce, find the real cause, make the smallest fix, prove it works. Use when the user reports an error, a crash or a failing test, says "it doesn't work", pastes a stack trace, or types "/fix-it".
---

# Fix it (properly)

## Steps

1. **Reproduce.** Run the failing command / test / page and capture the exact error. If you cannot run it, ask the user for the exact error text and the steps.
2. **Locate.** Follow the error to the file and line. Read the surrounding code before changing anything.
3. **Explain the cause** in 1–2 plain sentences ("X is undefined because Y runs before Z").
   If you have more than one theory, list them and check the most likely first. Don't guess-and-patch.
4. **Smallest fix.** Change as little as possible, fixing the cause rather than the symptom. No side refactors.
5. **Prove it.** Re-run the same command / test and show the before → after result.
6. **Report:**
   - What was broken
   - Why
   - What I changed (file:line)
   - How I checked it

## Never

- Delete or skip a failing test to make it "pass".
- Hide an error with an empty try/catch.
- Say it's fixed without re-running it.
