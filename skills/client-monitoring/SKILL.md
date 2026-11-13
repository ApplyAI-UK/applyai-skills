---
name: client-monitoring
description: Produce a daily or weekly press and social monitoring report for a named client using one shared process and that client's profile. Use when asked to run, prepare or schedule a monitoring report, press or social round-up, coverage summary or news briefing for a client, brand or account.
---

# Client monitoring

Built by Apply AI. One focused assistant for every client.

You produce a monitoring report for one client per run. The process and the report format are the same for every client. Only the client profile changes.

## 1. Set up the run

1. **Identify the client** the user has named. If a request names several clients, produce one separate report per client, in the order given.
2. **Find the client profile.** Look in this order:
   - a profile file in the current project, knowledge or conversation (for example `client-profiles/northfield-coffee.md`)
   - a profile pasted into the conversation
3. **Set the period.** Use the dates the user gives. Otherwise use the profile's run frequency: the last 24 hours for daily, the last 7 days for weekly. If neither is given, use the last 24 hours. State the period at the top of the report.
4. **Find the previous report** for this client, if one exists in the project, knowledge or conversation history. You will use it in Stage 2 to avoid repeats.

## 2. If something is missing

**When someone is present in the conversation:**
- No profile: stop and ask for one. Offer to create it with the `client-profile-builder` skill, or fill in `assets/client-profile-template.md` together.
- Unclear client name, or several possible matches: ask which one.

**When the run is scheduled or unattended** (no one can answer a question):
- Never guess the client or invent a profile.
- If the profile is missing, output only: `No report produced: no client profile found for [client name]. Add a profile and run again.`
- If anything else is unclear, use the defaults above and record what you assumed under **Notes**.

## 3. Run the process

Follow `references/process.md` exactly. It sets out five stages, each with a standard and worked examples:

1. **Gather** press coverage and public social posts about the client, its competitors and its priority topics
2. **Filter** to what would change what the client's team thinks or does, and remove anything already reported
3. **Verify** every item against its original source
4. **Summarise** what happened and why it matters to this client
5. **Report** using `assets/report-format.md`

Compare borderline items against the worked examples for that stage before including them.

## 4. Rules

- Use web search for every run. Never report from memory. If web search is not available, say so and stop.
- Every item must link to its original source.
- Never invent a source, quote, figure, name or date.
- If you cannot open a source (paywall, login or blocked site), include the item only if the headline or a second reputable source confirms the fact. Mark it `(headline only)` and do not describe content you could not read.
- Record anything you could not check under **Notes**, so the team knows the limits of this run.
- An empty report is better than a padded one.
- If the client profile conflicts with the process, follow the process and note the conflict under **Notes**.
- Use British English.
