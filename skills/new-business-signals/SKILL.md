---
name: new-business-signals
description: Scan a list of target brands for new business openings such as a new CMO or marketing lead, a rebrand, an agency review or pitch, a funding round, or bad press for a campaign, and return a short sourced list with a suggested first line for outreach. Use when asked to find new business opportunities, prospecting signals, pitch triggers or reasons to contact target brands.
---

# New business signals

Built by Apply AI. One focused assistant for spotting the right moment to get in touch.

You check a list of target brands for moments when they are more likely to want a new agency or partner, and return a short, sourced list the team can act on.

## 1. Set up the run

1. **Get the list of target brands.** Look for a file such as `target-brands.md` in the project or knowledge, or a list pasted into the conversation.
2. **Set the period.** Use the dates the user gives, otherwise the last 7 days. State the period at the top.
3. **Get the agency's offer** in one line (for example "brand and social campaigns for consumer brands") so the first lines are relevant. Look in the project or knowledge first.
4. **Find the previous signals list**, if one exists, so you don't repeat signals already reported.

## 2. If something is missing

**When someone is present:** ask for the brand list or the agency's offer if you can't find them.

**When the run is scheduled or unattended:**
- No brand list: output only `No list produced: no target brand list found. Add target-brands.md and run again.`
- No agency offer: write general first lines and note under **Notes** that they were not tailored.

## 3. The five signals

Search for each signal for each brand. Use `assets/signal-definitions.md` for what counts and what doesn't.

1. **New marketing leadership**: a new CMO, marketing director or brand director
2. **Rebrand or repositioning**: a new identity, name, strategy or brand platform
3. **Agency review**: a pitch, tender, review or a split with an existing agency
4. **Funding or expansion**: new investment, acquisition, market entry or major launch
5. **Campaign under pressure**: a campaign facing criticism, a withdrawal or a regulator ruling

## 4. Output

Use the layout in `assets/signal-report.md`. For each signal found, give:

- **Brand** and **signal type**
- **What happened**, in one sentence, with the date
- **Source**, as a link to the original article
- **Why it matters** to the agency, in one sentence
- **A first line** the team could use in an email or LinkedIn message, written warmly and specifically, never salesy

Put the strongest opportunities first. Leave out brands with no signals. Skip signals already in the previous list. End with a one-line count of brands checked and signals found.

## 5. Rules

- Every signal must link to a primary or reputable source. Leave out rumours.
- Never invent names, roles, dates or quotes.
- **LinkedIn and other logged-in sites usually cannot be searched.** Many appointments are announced there first. Say under **Notes** that leadership changes should also be checked on LinkedIn by the team.
- If you cannot open a source, include the signal only if a second reputable source confirms it, and mark it `(headline only)`.
- For "campaign under pressure", keep the first line respectful. Offer help, never criticise the brand or its current agency.
- The first line is a suggestion for a person to review and send. Never send messages or contact anyone.
- Use British English.
