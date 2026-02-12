# QA Testing Plan
## Game Being Tested: Fshng Game

Dev Team: Marcus C., Ayah, Evan, Bianca, Maddy

QA Team: Sham, Elizabeth, Melo, Alex

Date: 02/12/2026

**Game Overview (From README)**
**Short explanation of what the game is about:**
- Fishing
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

---

## QA Sign-Off

**Testing Completed By:** 02/11/2026
**Date Submitted:** 02/13/2026
