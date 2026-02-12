**Use Ctrl + F to find your game**

# QA Testing Plan
## Game Being Tested: Fshng Game

Dev Team: Marcus C., Ayah, Evan, Bianca, Maddy

QA Team: Sham, Elizabeth, Melo, Alex

Date: 02/12/2026

**Game Overview (From README)**
**Short explanation of what the game is about:**

Fishing
- Catch enough fish to survive the round
- You cast enough line to try to catch enough fish to feed to the shark that is circling you. Each round you have a limited number of casts to catch enough fish to feed to the shark. You don't cast enough fish you die.

**Game Type: Other (Fishing game)**
**Core Mechanics:**
- Drag mouse around to catch/collect fish
  
**Win Condition:** Catch a fish
  
**Lose Condition:** Didn't catch a fish by the end of the round

**Player Inputs:** Click your mouse (only input)

# Testing Strategy by Day
**Tuesday:** Happy Path & Core Mechanics

**Goal:** Does the game work as the dev team said it would?

*hint it doesn't*

## Test Scenarios:

- [x] Start the game cleanly (no crashes at launch)
- [x] Follow the happy path (win the game normally)
- [x] Follow the lose path (lose the game)
- [x] Core mechanic 1 works as described
- [x] All UI/output is readable and clear

**Known issues found today:**
1. Entire UI missing, there was supposed to be a starting game page
2. Cannot upgrade even though it was supposed to be an option

**Wednesday:** Input Validation & Edge Cases
Goal: What breaks the game? What unexpected inputs does it not handle?

**Test Scenarios:**
- [x] Try to break win/lose logic (can you get stuck?)
- [x] State persistence (does the game track things correctly?)

**Known issues found today:**
1. Don't need to catch a fish in order to win the game and go to the next round
    
**Wednesday:** Complex Scenarios & State Management

**Goal:** Does the game handle weird sequences or complex game states?

**Test Scenarios:**

- [x] Test combinations: [specific sequence that might break things]
- [x] Long gameplay (play for 10+ rounds without winning)
- [x] Rapid state changes (quick back-and-forth actions)
- [x] Look for off-by-one errors (1 too many, 1 too few)

**Known issues found today:**
1. Played 5 rounds without catching a fish and nothing happened

**Wednesday:** Final Pass & Handoff

**Goal:** Did we miss anything? Consolidate findings.

Test Scenarios:

- [x] Spot-check critical paths (game-breaking issues)
- [x] Replay one more round of complex scenarios
- [x] Verify all bugs are documented and reproducible
- [x] Review severity/priority assignments
- [x] Final summary and recommendations
Known issues found today:
No other issues were found, just those three.
   
# Bug Categories (Track What You Find)
## By Severity
- Critical: Game crashes or is unplayable
- High: Core feature broken or incorrect
- Medium: Feature partially works but has issues
- Low: Cosmetic, minor, or edge case only

## By Type
- Input Validation: Game doesn't handle bad input
- Logic Error: Game mechanics don't work as described
- State Management: Game loses track of data (score, health, etc.)
- UI/UX: Output is confusing or unclear
- Performance: Game is slow or hangs
---

# Bug Summary Table

| Day  | Bugs Found | Critical | High | Medium | Low | Total |
|------|------------|----------|------|--------|-----|-------|
| Tue  |     1       |          |      1    |        |          |      1    |
| Wed  |      2      |          |     2     |        |          |      2    |
| Thu  |             |          |           |        |          |           |
| Fri  |             |          |           |        |          |           |
| **Total** |     3  |      0   |    3      |  0     | 0        |    3      |


# Additional QA Notes

## Testing Environment
**Environment Used:**  
- You play it through PyCharm using PyGame and it should be a window popup


## Blockers / Code Issues
**Did the game run successfully?**  
- The game ran but it more so a shell of the acutal game it was supposed to be

## Assumptions
**Anything unclear about how the game should work?**  
- You have to click to start the game, doesn't tell you

# Recommendations for Dev Team

## High-Priority Fixes
1. Upgrading isn't an option
2. Can still win the game without even catching anything
3. No starting game menu

-----------------------------------------------------------


## Game Being Tested: Echo of Terminal 7 - Surrounded Edition

Dev Team: Nayan Patel, Khani Lyan, Gauhar Veeravalli, Quint Bunting

QA Team: Sham, Elizabeth, Melo, Alex

Date: 02/12/2026

**Game Overview (From README)**
-  Echo of Terminal 7 is a top‑down sci‑fi puzzle adventure built with Pygame.
You control a stranded scientist exploring a dying research station, moving between rooms in a central hub and solving environmental puzzles to restore power, uncover “The Herd” experiment, and stabilize the Slip‑Drive. The game focuses on light exploration, simple movement, and room‑based mini‑games rather than combat.


**Short explanation of what the game is about:**
- Puzzle Game - Sci-Fi Puzzle
- Multiple Minigames
- Must solve mini games to then fight the boss.

**Game Type**
- Top - Down Puzzle Adventuge (PyGame)

**Core Mechanics:**
- For Movements: W/A/S/D and ARROW Keys - Move up / left / down / right
- For Interaction: "E" - Interact / Use 
  
**Win Condition:** Solve all the puzzles, fight the boss at the end.
  
**Lose Condition:** Lose against the boss at the end.

**Player Inputs:** 
- WASD / Arrow keys for movements
- Mouse Left Click for minigames (Botany, Engineering Room, Power Grid Room)
- Text / Typing Input for minigame (Server Room)
- Mouse Left Click for shooting the boss
- Mouse Movement to aim shots when fighting the boss.

# Testing Strategy by Day
**Tuesday:** Happy Path & Core Mechanics

**Goal:** Does the game work as the dev team said it would?
- No. 

## Test Scenarios:

- [x] Start the game cleanly (no crashes at launch)
- [] Follow the happy path (win the game normally)
- [x] Follow the lose path (lose the game)
- [] Core mechanic 1 works as described
- [] All UI/output is readable and clear

**Known issues found today:**
1. In the Power Grid Room the Green button doesn't work
2. Text Boxes in the other mini game rooms are blacked out.

**Wednesday:** Input Validation & Edge Cases
Goal: What breaks the game? What unexpected inputs does it not handle?
- So far the fact that the first puzzle (the power grid) doesn't work, this won't allow you to continue the game. The game handles inputs correctly.

**Test Scenarios:**
- [x] Try to break win/lose logic (can you get stuck?): **YES**
- [x] State persistence (does the game track things correctly?) **YES**

**Known issues found today:**
1. You can solve 3 out of the 4 puzzles and still fight the boss in the end
    
**Wednesday:** Complex Scenarios & State Management

**Goal:** Does the game handle weird sequences or complex game states?

**Test Scenarios:**

- [x] Test combinations: [specific sequence that might break things]
- [x] Long gameplay (play for 10+ rounds without winning)
- [x] Rapid state changes (quick back-and-forth actions)
- [x] Look for off-by-one errors (1 too many, 1 too few)

**Known issues found today:**
1. None

**Wednesday:** Final Pass & Handoff

**Goal:** Did we miss anything? Consolidate findings.

Test Scenarios:

- [x] Spot-check critical paths (game-breaking issues)
- [x] Replay one more round of complex scenarios
- [x] Verify all bugs are documented and reproducible
- [x] Review severity/priority assignments
- [x] Final summary and recommendations
Known issues found today:
No other issues were found, just those three.
   
# Bug Categories (Track What You Find)
## By Severity
- Critical: Game crashes or is unplayable
- High: Core feature broken or incorrect
- Medium: Feature partially works but has issues
- Low: Cosmetic, minor, or edge case only

## By Type
- Input Validation: Game doesn't handle bad input
- Logic Error: Game mechanics don't work as described
- State Management: Game loses track of data (score, health, etc.)
- UI/UX: Output is confusing or unclear
- Performance: Game is slow or hangs
---

# Bug Summary Table

| Day  | Bugs Found | Critical | High | Medium | Low | Total |
|------|------------|----------|------|--------|-----|-------|
| Tue  |            |          |      |        |     |       |
| Wed  |            |          |      |        |     |       |
| Thu  |     3      |     2    |   1  |        |     |   3   |
| Fri  |            |          |      |        |     |       |
| **Total** |   3   |     2    |   1  |        |     |       |

# Additional QA Notes

## Testing Environment
**Environment Used:**  
- You play it through PyCharm using PyGame and it should be a window popup
- macOS Tahoe 26.2 
- pycharm 2025.3.2.1


## Blockers / Code Issues
**Did the game run successfully?**  
- The game ran but it more so a shell of the acutal game it was supposed to be

## Assumptions
**Anything unclear about how the game should work?**  
- You have to click to start the game, doesn't tell you

# Recommendations for Dev Team

## High-Priority Fixes
1. Fixing the Green Button in the Power Grid Room
2. Fixing the Text Box issues
3. Fixing the logic so that you must complete ALL 4 puzzles before being able to fight the boss.

---
# Game Being Tested: BlackJack

Dev Team: Samuel Taiwo, Jessica Kamienski, Karan Modi, Maxwell Noffsinger

QA Team: Sham, Elizabeth, Melo, Alex

Date: 02/11/2026

**Game Overview (From README)**
-  In this virtual blackjack game, players will compete with a dealer to win money by playing BlackJack. The player begins with 1500 dollars to bet and can gain or lose money according to their bet each round. If the player reaches 0 or decides to stop playing, the game ends and a summary is printed to the screen. There are modifiers and different game modes for the player to interct with.


**Short explanation of what the game is about:**
- Virtual BlackJack Game
- Card Game / Player vs Computer (P vs CPU)
- Possible upgrades / tweaks to normal BlackJack

**Game Type**
- Card Game 

**Core Mechanics:**
- For Interaction: Use left click for everything.
  
**Win Condition:** 
- Be the one closest to 21 points without going over
- Dealer goes over 21 points
  
**Lose Condition:** 
- Dealer is closer to 21 points. 
- You get more than 21 points

**Player Inputs:** 
- Mouse Left Click to decided whether you want to "hit" or "stand"

# Testing Strategy by Day
**Tuesday:** Happy Path & Core Mechanics

**Goal:** Does the game work as the dev team said it would?
- Base Game Yes. Upgrades / Different Modes No.

## Test Scenarios:

- [x] Start the game cleanly (no crashes at launch)
- [x] Follow the happy path (win the game normally)
- [x] Follow the lose path (lose the game)
- [x] Core mechanic 1 works as described
- [x] All UI/output is readable and clear

**Known issues found today:**
1. When clicking on the Russian Mode and then starting the game, the game freezes and crashed
2. Upgrades add an extra card which breaks the game logic. This also breaks the rules of blackjack, you can't have more than 21 points and still win.

**Wednesday:** Input Validation & Edge Cases
Goal: What breaks the game? What unexpected inputs does it not handle?
1. Russian Mode
2. Upgrade Extra Cards
3. Handles all inputs correctly

**Test Scenarios:**
- [x] Try to break win/lose logic (can you get stuck?): **NO**
- [x] State persistence (does the game track things correctly?) **YES**

**Known issues found today:**
1. Some Upgrades don't work at all
    
**Wednesday:** Complex Scenarios & State Management

**Goal:** Does the game handle weird sequences or complex game states?

**Test Scenarios:**

- [x] Test combinations: [specific sequence that might break things]
- [x] Long gameplay (play for 10+ rounds without winning)
- [x] Rapid state changes (quick back-and-forth actions)
- [x] Look for off-by-one errors (1 too many, 1 too few)

**Known issues found today:**
1. All issues were found today

**Wednesday:** Final Pass & Handoff

**Goal:** Did we miss anything? Consolidate findings.

Test Scenarios:

- [] Spot-check critical paths (game-breaking issues)
- [x] Replay one more round of complex scenarios
- [x] Verify all bugs are documented and reproducible
- [x] Review severity/priority assignments
- [x] Final summary and recommendations
Known issues found today:
No other issues were found, just those three.
   
# Bug Categories (Track What You Find)
## By Severity
- Critical: Game crashes or is unplayable
- High: Core feature broken or incorrect
- Medium: Feature partially works but has issues
- Low: Cosmetic, minor, or edge case only

## By Type
- Input Validation: Game doesn't handle bad input
- Logic Error: Game mechanics don't work as described
- State Management: Game loses track of data (score, health, etc.)
- UI/UX: Output is confusing or unclear
- Performance: Game is slow or hangs
---

# Bug Summary Table

| Day  | Bugs Found | Critical | High | Medium | Low | Total |
|------|------------|----------|------|--------|-----|-------|
| Tue  |            |          |      |        |     |       |
| Wed  |     3      |    2     |      |    1   |     |   3   |
| Thu  |            |          |      |        |     |       |
| Fri  |            |          |      |        |     |       |
| **Total** |   3   |    2     |      |    1   |     |       |

# Additional QA Notes

## Testing Environment
**Environment Used:**  
- You play it through PyCharm using PyGame and it should be a window popup
- macOS Tahoe 26.2 
- pycharm 2025.3.2.1


## Blockers / Code Issues
**Did the game run successfully?**  
- The game ran but it more so a shell of the acutal game it was supposed to be

## Assumptions
**Anything unclear about how the game should work?**  
- You have to click to start the game, doesn't tell you

# Recommendations for Dev Team

## High-Priority Fixes
1. Fix the Russian Mode
2. Fix the upgrading card count, make sure you can't get above 21 points (or just get rid of the whole upgrade option)
3. Fix the fact that some upgrades just don't work at all.

---

## Game Being Tested: CHRISTOFER: THE RISE OF MARK-HAM

Dev Team: Gabe, Rahul, Huzaifah, and Troy

QA Team: Sham, Elizabeth, Melo, Alex

Date: 02/12/2026

**Game Overview (From README)**
-  Using your randomly generated character, Navigate through the Ruins of Be-Ta to stop Chris-tofer, the Script-King, from merging with the Dungeon Core. Battle enemies, collect items, and upgrade your stats as you descend through 30 floors of procedurally-generated rooms.


**Short explanation of what the game is about:**
- It is a walk through of a interactive story which is what makes it a text based game. The game walks you through a story where you go up against different enemies and get to choose by entering numbers that correspond with movement choices given.  It also has another interactive part where the code generates a line of different colored blocks and you have to press enter when it gets to green to win.  

**Game Type**
- Text game(some might say)
- Interactive story

**Core Mechanics:**
- Mechanic 1: Playing the light game, in which you press enter whenever the light turns green.
- Mechanic 2: Going through the interactive story.

  
**Win Condition:** Solve all the puzzles, fight the boss at the end.
  
**Lose Condition:** Lose against the boss at the end.

**Player Inputs:** 
- Press return or enter keys when the light is green, when told, or after entering a number. 
- Press a number according to the options given to continue through the story

# Testing Strategy by Day
**Tuesday:** Happy Path & Core Mechanics

**Goal:** Does the game work as the dev team said it would?

*hint it doesn't*

## Test Scenarios:

- [x] Start the game cleanly (no crashes at launch)
- [x] Follow the happy path (win the game normally)
- [x] Follow the lose path (lose the game)
- [x] Core mechanic 1 works as described
- [x] All UI/output is readable and clear

**Known issues found today:**
1. Going into settings causes the text speed to be extremely slow

**Wednesday:** Input Validation & Edge Cases
Goal: What breaks the game? What unexpected inputs does it not handle?

**Test Scenarios:**
- [x] Try to break win/lose logic (can you get stuck?)
- [x] State persistence (does the game track things correctly?)

**Known issues found today:**
1. The special features do not work, trying to use an item crashes the game.
2. Can not use certain abilities
    
**Thursday:** Complex Scenarios & State Management

**Goal:** Does the game handle weird sequences or complex game states?

**Test Scenarios:**

- [x] Test combinations: [specific sequence that might break things]
- [x] Long gameplay (play for 10+ rounds without winning)
- [x] Rapid state changes (quick back-and-forth actions)
- [x] Look for off-by-one errors (1 too many, 1 too few)

**Known issues found today:**
1. The games text speed is extremely slow even if you enter a high number to make it fast.

**Thursday:** Final Pass & Handoff

**Goal:** Did we miss anything? Consolidate findings.

Test Scenarios:

- [x] Spot-check critical paths (game-breaking issues)
- [x] Replay one more round of complex scenarios
- [x] Verify all bugs are documented and reproducible
- [x] Review severity/priority assignments
- [x] Final summary and recommendations

Known issues found today:
1. The game works overall but is very unclear and its special features crash or do not work correctly.
   
# Bug Categories (Track What You Find)
## By Severity
- Critical: Game crashes or is unplayable
- High: Core feature broken or incorrect
- Medium: Feature partially works but has issues
- Low: Cosmetic, minor, or edge case only

## By Type
- Input Validation: Game doesn't handle bad input
- Logic Error: Game mechanics don't work as described
- State Management: Game loses track of data (score, health, etc.)
- UI/UX: Output is confusing or unclear
- Performance: Game is slow or hangs
---

# Bug Summary Table

| Day  | Bugs Found | Critical | High | Medium | Low | Total |
|------|------------|----------|------|--------|-----|-------|
| Tue  |     1       |          |          |    1    |          |      1    |
| Wed  |      2      |      1   |          |     1   |          |     2     |
| Thu  |       1      |          |     1      |    1    |          |    1       |
| Fri  |             |          |           |        |          |           |
| **Total** |     4  |      1   |      1    |  2     | 0        |    4      |


# Additional QA Notes

## Testing Environment
**Environment Used:**  
- You play it through virtual studio code and run the files and the game play is in the terminal


## Blockers / Code Issues
**Did the game run successfully?**  
- The game ran and had some cool features such as the "graphics" like the text color, however there are some bugs and features that can crash the game.

## Assumptions
**Anything unclear about how the game should work?**  
- Yes, the Readme overall is very unclear, at first we thought the game was a website. Then we started actually playing the game it wasn't clear which one is the main game because there are two games: one interactive story and the light game. When you play the games it is unclear that you have to pre

# Recommendations for Dev Team

## High-Priority Fixes
1. Create a start menu or a better ReadMe, so there are clearer instructions on what the game is supposed to be.
2. Fix the text speed settings.
3. Fix the item feature so that it can be used without the game crashing.

---
## QA Sign-Off

**Testing Completed By:** 02/11/2026
**Date Submitted:** 02/13/2026

**Testing Completed By:** 02/11/2026
**Date Submitted:** 02/13/2026
