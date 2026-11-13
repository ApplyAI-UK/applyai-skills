# Tests: client monitoring

| # | Setup | Prompt | Pass if |
|---|---|---|---|
| 1 | Example profile in the project | "Run today's monitoring report for Northfield Coffee." | The skill loads without being named. Report uses the set format, states the period, and every item has a source link. |
| 2 | Example profile in the project | Same as test 1 | Northfield Coffee is fictional, so the report says no developments for the brand, or covers only competitors and topics. It invents nothing about the brand. |
| 3 | No profile anywhere | "Run a monitoring report for Harbour Roasters." | It asks for a profile and offers to build one. It does not produce a report. |
| 4 | No profile, run as a scheduled task | "Run today's monitoring report for Harbour Roasters." | Output is the single "No report produced" line. |
| 5 | Real client profile, plus yesterday's report in the conversation | "Run today's report for [client]." | Nothing from yesterday's report repeats, unless marked `Update` with what is new. |
| 6 | Real client profile | "Run a weekly report for [client] covering 1 to 7 November." | The period stated matches the dates given. No items fall outside it. |
| 7 | Real client profile with a paywalled trade title in approved sources | "Run today's report for [client]." | Any item from a source it couldn't read is marked `(headline only)` and listed under Notes. |
| 8 | Two real profiles | "Run today's reports for [client A] and [client B]." | Two separate reports, each using only its own profile. |
| 9 | Web search switched off | "Run today's report for [client]." | It says web search is unavailable and stops. It does not report from memory. |
