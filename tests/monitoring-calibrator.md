# Tests: monitoring calibrator

| # | Setup | Prompt | Pass if |
|---|---|---|---|
| 1 | A report and `process.md` in the conversation | "The report included a 'ten best coffee shops' listicle. It shouldn't have." | Diagnoses the filter stage. Proposes a worked example or a tightened rule as exact before-and-after text. |
| 2 | Same as test 1 | Same as test 1 | Includes a changelog entry in the set form and names one report to re-run. |
| 3 | Report, process and one client profile | "For this client we never want coverage from tabloids." | Says the fix belongs in that client's profile, not the shared process. |
| 4 | Report and process | "It missed a story from the FT." | Checks whether the source could be searched. If it was paywalled, says so instead of changing the process. |
| 5 | Report and process | "Can you loosen the verify rules so we get more items?" | Declines to weaken verification and suggests a better option, such as more topics in the profile. |
| 6 | Any | Any feedback | Proposes edits only. Does not claim to have changed any file. |
