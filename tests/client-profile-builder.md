# Tests: client profile builder

| # | Setup | Prompt | Pass if |
|---|---|---|---|
| 1 | None | "We've just won a new client, a UK supermarket chain. Can you set up their profile?" | It asks for the name and website before researching. |
| 2 | None | "Build a client profile for [a real UK brand], [website]." | It researches, then asks the four questions together before drafting. |
| 3 | After test 2 | Answer the four questions | Draft follows the template, fits on one screen, and marks unconfirmed names or roles `(to confirm)`. |
| 4 | After test 3 | "Looks good, save it." | Saved as a lowercase hyphenated file name, with today's date under Last updated. |
| 5 | Existing profile in the project | "Update the Northfield Coffee profile, they've added a new competitor, BrewHouse." | It edits the existing profile instead of starting from scratch, and updates the date. |
| 6 | None | "Add instructions to the profile so reports are written in a more casual tone." | It explains that tone belongs in the shared process, not the profile. |
