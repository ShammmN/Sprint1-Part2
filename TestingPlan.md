QA Testing Plan
Game Being Tested: [Name]

Dev Team: [Team name/repo]

QA Team: [Your names]

Date: [Week 6 dates]

Game Overview (From README)
Game Type: [Dungeon Crawler / Text Adventure / Card Game / Trivia / Other]

Core Mechanics:

[Mechanic 1]
[Mechanic 2]
[Mechanic 3]
Win Condition: [How do you win?]

Lose Condition: [How do you lose?]

Player Inputs: [What commands/inputs does the game accept?]

Testing Strategy by Day
Tuesday: Happy Path & Core Mechanics
Goal: Does the game work as the dev team said it would?

Test Scenarios:

[ ] Start the game cleanly (no crashes at launch)
[ ] Follow the happy path (win the game normally)
[ ] Follow the lose path (lose the game)
[ ] Core mechanic 1 works as described
[ ] Core mechanic 2 works as described
[ ] Core mechanic 3 works as described
[ ] All UI/output is readable and clear
Known issues found today:

[Issue 1]
[Issue 2]
Wednesday: Input Validation & Edge Cases
Goal: What breaks the game? What unexpected inputs does it not handle?

Test Scenarios:

[ ] Enter garbage input (letters when it expects numbers, etc.)
[ ] Enter empty input (just press enter)
[ ] Enter negative numbers (if applicable)
[ ] Enter huge numbers (999999)
[ ] Rapid repeated inputs (spam input)
[ ] Boundary cases (min/max values, off-by-one scenarios)
[ ] Try to break win/lose logic (can you get stuck?)
[ ] State persistence (does the game track things correctly?)
Known issues found today:

[Issue 1]
[Issue 2]
Thursday: Complex Scenarios & State Management
Goal: Does the game handle weird sequences or complex game states?

Test Scenarios:

[ ] Test combinations: [specific sequence that might break things]
[ ] Long gameplay (play for 10+ rounds without winning)
[ ] Rapid state changes (quick back-and-forth actions)
[ ] Test any inventory/item systems
[ ] Test any scoring/progression systems
[ ] Try weird orderings (does it matter what you do first?)
[ ] Look for off-by-one errors (1 too many, 1 too few)
Known issues found today:

[Issue 1]
[Issue 2]
Friday: Final Pass & Handoff
Goal: Did we miss anything? Consolidate findings.

Test Scenarios:

[ ] Spot-check critical paths (game-breaking issues)
[ ] Replay one more round of complex scenarios
[ ] Verify all bugs are documented and reproducible
[ ] Review severity/priority assignments
[ ] Final summary and recommendations
Known issues found today:

[Issue 1]
[Issue 2]
Bug Categories (Track What You Find)
By Severity
Critical: Game crashes or is unplayable
High: Core feature broken or incorrect
Medium: Feature partially works but has issues
Low: Cosmetic, minor, or edge case only
By Type
Input Validation: Game doesn't handle bad input
Logic Error: Game mechanics don't work as described
State Management: Game loses track of data (score, health, etc.)
UI/UX: Output is confusing or unclear
Performance: Game is slow or hangs
Other: [Category]
