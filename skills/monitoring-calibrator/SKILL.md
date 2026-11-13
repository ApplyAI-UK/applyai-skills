---
name: monitoring-calibrator
description: Review a monitoring report against an analyst's feedback and propose precise edits to the shared monitoring process, with a changelog entry. Use when calibrating a monitoring assistant, when a report included the wrong items or missed something, or when asked to improve, tune or fix the monitoring process.
---

# Monitoring calibrator

Built by Apply AI. Improve the process once, and every client benefits.

You help a team improve its shared monitoring process after a report misses the mark. You fix the process, not the individual report, so the improvement reaches every client.

This skill proposes edits for a person to approve. It does not change any file on its own.

## Inputs

Ask for anything missing:

1. The report that was produced
2. What the analyst would have done differently, such as items that should not have been included, items that were missed, or wording that was off
3. The current shared process (for example `process.md`)
4. The client profile, if the feedback might be specific to one client

## Steps

1. **Diagnose.** For each piece of feedback, decide which stage caused it (gather, filter, verify, summarise or report) and why. If the cause is outside the process, such as a source that could not be searched, say so plainly instead of changing the process.
2. **Decide where the fix belongs.**
   - Applies to every client → the shared process
   - Applies to one client only → that client's profile
   - A missing or blocked source → the team's notes, not the process
3. **Choose the smallest fix.** Prefer, in this order:
   - adding or sharpening a worked example for that stage
   - tightening one existing rule
   - adding a new rule, only if nothing existing covers it
4. **Write the edits** as exact before-and-after text for each change, ready to paste in.
5. **Write a changelog entry** in this form:
   `[date] · [stage] · [what changed] · [why]`
6. **Suggest a test.** Name one recent report to re-run so the team can confirm the change works and nothing else has broken.

## Rules

- Change as little as possible. One clear example beats three new rules.
- Never weaken the verify stage to include more items.
- Keep the process the same for every client.
- Use British English.
