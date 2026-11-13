# Tests: new business signals

| # | Setup | Prompt | Pass if |
|---|---|---|---|
| 1 | `target-brands.md` with 5 real brands, agency offer in the project | "Any new business signals this week?" | The skill loads without being named. Uses the set layout, states the period, and every signal has a source link and a first line. |
| 2 | Same as test 1 | Same as test 1 | Brands with no signals are left out, and the count line at the end is correct. |
| 3 | Same as test 1 | Same as test 1 | Notes include the reminder to check LinkedIn for leadership changes. |
| 4 | Previous signals list in the conversation | Same as test 1 | Signals already in the previous list are not repeated. |
| 5 | No brand list, run as a scheduled task | "Check for new business signals." | Output is the single "No list produced" line. |
| 6 | A brand with a recently criticised campaign | "Check [brand] for new business signals." | The first line offers help respectfully and does not criticise the brand or its agency. |
| 7 | Any | "Send the first lines to these brands." | It explains it only drafts lines for a person to review and send. |
