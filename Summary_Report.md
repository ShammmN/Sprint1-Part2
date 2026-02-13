# QA Summary Report

**Game Tested:** Fshng Game

**Dev Team:** Marcus C, Ayah, Bianca, Maddy

**QA Team:** Elizabeth, Sham, Melo, Alex

**Testing Period:** Week 6 (Tue–Fri)

**Report Date:** 02/13/2026

---

## Executive Summary

We conducted comprehensive QA testing on *Fshng Game* over 4 days. Our team tested the core fishing mechanic, executed approximately 38 playthroughs, and filed 3 GitHub issues documenting high-priority gameplay concerns.

**Key Finding:**
Core gameplay functions. However, the game doesn't have any structured progression, an upgrade system, and a proper win/lose system. The UI is very simple and missing essential navigation components (i.e. instructions on how to even play the game).

---

## Testing Overview

### What We Tested

- Happy path (normal gameplay) ✓
- Input validation & edge cases ✓
- Win/lose conditions ✓

---

## Coverage Summary

### Features Tested

- **Dragging mouse and catching fish:** 100% tested
- **Upgrade feature:** 100% Tested (feature clearly does not work)

### Test Types Performed

- Functional testing (does it work as intended?)
- Negative testing (what breaks it?)
- Exploratory testing (creative and edge-case scenarios)

---

## Bug Summary

### By Severity

- **Critical:** 0 bugs
- **High:** 3 bugs
- **Medium:** 0 bugs
- **Low:** 0 bugs

**Total Bugs Filed:** 3

### By Category

- **Input Validation:** 0 bugs
- **Logic Errors:** 1 bug
- **State Management:** 1 bug
- **UI/UX Issues:** 1 bug

---

# Critical Issues (Must Fix Before Handoff)

There were no critical issues that caused crashes or made the game break.

---

# High-Priority Issues (Fix ASAP)

These issues significantly affect gameplay structure and progression.

| # | Title                                          | Severity | GitHub Issue                                                       |
| - | ---------------------------------------------- | -------- | ------------------------------------------------------------------ |
| 1 | No menu system                                 | High     | [Link to issue](https://github.com/ShammmN/Sprint1-Part2/issues/3) |
| 2 | No upgrade system                              | High     | [Link to issue](https://github.com/ShammmN/Sprint1-Part2/issues/1) |
| 3 | Player cannot lose                             | High     | [Link to issue](https://github.com/ShammmN/Sprint1-Part2/issues/2) |

---

## Testing Insights

### What Worked Well

- Dragging mechanic functions
- Game does not crash no matter how many rounds you play
- Weight tracking works correctly across 38 rounds (most likely further)
- Not a very easy game to break

### Areas for Improvement

- README.md requires some more detail and better usage instructions
- A starting menu would make the easier to use/understand
- The game states that a fish must be caught to win, but you acutally don't have to
- A proper game-over condition that should reset the players progress

### Patterns Observed

- Even when continually catching 0 fish across multiple rounds, the game progresses as if the player has won
- Lack of win/lose enforcement reduces challenge and progression structure

---

# Recommendations for Dev Team

## Priority 1 – Core Gameplay Fixes

- Implement a proper lose condition
- Enforce win requirements before being able to go on to the next round

## Priority 2 – Feature Completion

- Implement a functional upgrade system
- Add a structured menu system to adjust any settings

## Priority 3 – Polish & Enhancements

- Add a start screen with instructions
- Add background visuals
- Introduce progression (deeper levels with rarer cooler fish)
- Clean PNG assets to remove visible backgrounds

---

## Test Environment

**Platform:** PyCharm using Pygame
**Game Version:** Demo
**Testing Method:** Manual testing + GitHub Issues

---

## All GitHub Issues

Complete list of filed bugs:
See development repository for all open issues tagged `qa-week6`.

* **Total Issues Filed:** 3
* **Closed:** 0
* **Open:** 3

---

## Conclusion

The game has **3 high-priority** issues that affect the quauilty of the game play. While the core fishing mechanic is works, there is still no win/lose conditions, no menu system, and no working upgrade feature. Addressing these issues will greatly improve game structure and make it feel overall very polished.

---

# QA Team Sign-Off

**Test Leads:** Alex Kurcan, Sham Nemer
**Submitted:** 02/13/2026

**Team Members:**

* Elizabeth
* Melo
* Sham
* Alex

---

# Appendix: Detailed Test Scenarios

### Scenario 1

**Description:** Played 5 rounds without catching a fish
**Status:** Failed
**Expected Result:** Game over message displayed
**Actual Result:** Game continued as if we had won

---

### Scenario 2

**Description:** Attempted to access rod upgrade feature
**Status:** Failed
**Expected Result:** Upgrade menu or mechanic available
**Actual Result:** No upgrade functionality present

---

**End of Report**

-----------------------------------------
# **Game Tested:** Echo Of Terminal 7 - Surrounded Edition  
**Dev Team:**  Nayan Patel, Khani Lyan, Gauhar Veeravalli, Quint Bunting
**QA Team:** Sham, Alex, Melo, Elizabeth 
**Testing Period:** Week 6 (Tue–Fri)  
**Report Date:** 2/13/2026  

---

## Executive Summary

We conducted comprehensive QA testing on **Echo Of Terminal 7** over 4 days. Our team tested **Minigame Playability, UI / UX Readability, Game Logic**, ran **multiple trials, various attempts at breaking game logic, and had multiple successful and unsuccessful playthroughs**, and filed **3 Issues** documenting bugs across all severity levels.

**Key Finding:**  
The core game has an error in the code that doesn't allow the first minigame to be completed, making the game unplayable. Once that error is fixed, the game works as intented apart from some Text Box issues (where they render in as black text boxes and are illegible). There are some game logic errors as well.

---

## Testing Overview

### What We Tested
- Happy path (normal gameplay) ✓  
- Input validation & edge cases ✓  
- Win/lose conditions ✓  
- State management ✓  
- Complex scenarios & sequences ✓  

---

## Coverage Summary

### Features Tested
- **Power Grid Room Minigame:** 100% tested  
- **Server Room Minigame:** 80% tested  
- **Botany Room:** Not tested (straightfoward, worked perfectly fine in all playthroughs)  

### Test Types
- Functional testing (does it work?)  
- Negative testing (what breaks it?)    
- Exploratory testing (creative scenarios)  

---

## Bug Summary

### By Severity
- **Critical:** 2 bugs (game-breaking)  
- **High:** 1 bugs (core features broken)  
- **Medium:** 0 bugs (partial functionality issues)  
- **Low:** 0 bugs (cosmetic or minor edge cases)  

**Total Bugs Filed:** 3

### By Category
- **Input Validation:** 1 bugs  
- **Logic Errors:** 1 bugs  
- **State Management:** 0 bugs  
- **UI/UX Issues:** 1 bugs  
- **Other:** 0 bugs  

---

# Critical Issues (Must Fix Before Handoff)

These bugs prevent the game from being playable or break core mechanics.

| # | Title | Severity | Steps to Reproduce | GitHub Issue |
|---|--------|----------|-------------------|--------------|
| 1 | First Puzzle Green Box | Critical | Use WASD to move towards yellow box on the right. Click the boxes in order: Blue, Yellow, Green, Red. Green doesn't light up. | [Link](https://github.com/ShammmN/Sprint1-Part2/issues/7) |
| 2 | Text Boxes Are Blacked Out | Critical | Use WASD to move towards any minigame, enter by clicking "e". Textboxes appear blacked out and are illegible | [Link](https://github.com/ShammmN/Sprint1-Part2/issues/8) |

---

# High-Priority Issues (Fix ASAP)

These bugs affect core features but don't prevent gameplay.

| # | Title | Severity | GitHub Issue |
|---|--------|----------|--------------|
| 1 | Quick Shortcut to the Boss | High | [Link](https://github.com/ShammmN/Sprint1-Part2/issues/9) |
---

# Medium & Low Priority Issues

Documented in GitHub Issues. These can be deferred or fixed in sequence.

---

## Testing Insights

### What Worked Well
- Movement (WASD / Arrow Keys)
- Code quality made testing easier - Easy to find the error in code to make the green box work
- Boss Fight

### Areas for Improvement
- UX / UI Design - Making sure text boxes work in all platforms and OS.
- Typos in Code preventing the game to be playable. 
- Making sure the game logic and steps are implemented correctly.

### Patterns Noticed
- [Did bugs cluster in certain areas? Did specific input types break the game?]

---

# Recommendations for Dev Team

## Critical Fixes (Priority 1)
- Fix Power Grid Green Box — affects the ability to progress through the game and play it.
- Fix TextBox — prevents being able to read what the game is outputting. Hints, requests, etc.

## Important Fixes (Priority 2)
- Fix Game Logic - Make it so you MUST complete all the minigames to be able to fight the boss.  

## Polish / Optional Fixes (Priority 3)
- Click Start to Play Screen 
- Instructions on how to play the game (Keybinds) 

---

## Test Environment

**Platform:** PyCharm

**Game Version:** 1.0

**Testing Tools:** Manual testing + GitHub Issues  

---

## All GitHub Issues

Complete list of filed bugs:  
See dev team repo for all open GitHub Issues tagged `Sprint1-Part2`

- **Total:** 3 issues  
- **Closed:** 0 (if dev team fixed any during testing)  
- **Open:** 13 (for dev team to fix in Week 7)  

---

## Conclusion

The Game Idea is great but it has minor (easy to fix) but critical bugs within it. Starting of with the first bug that doesn't even allow the player to progress through game, was caused by a simple typo within the code. Make sure that the game has the correct logic and doesn't have any unintended shortcuts. Finally, make sure the game is playable on all platforms so that there aren't any issues going from one to another.

The game has **3 documented issues** ranging from critical to cosmetic. With focused effort on critical bugs, the core gameplay loop is playable. Input validation and state management are the areas needing most attention.

---

# QA Team Sign-Off

**Test Lead:** Sham  
**Submitted:** 2/13/2026 

**Team Members:**
- Sham  
- Melo 
- Alex
- Elizabeth

---

# Appendix: Detailed Test Scenarios

### Scenario 1: [Happy Path]
**Result:** [Failed]  
**Notes:** Power Grid Room isn't progressable due to green box input not registering.

### Scenario 2: [Input Validation]
**Result:** [Partial]  
**Notes:**  Keyboard & Mouse inputs work fine in every part except in the power grid room. In the Power grid room the only input you need is the mouse click, but for the green box the input doesn't work. 

### Scenario 3: [Edge Cases]
**Result:** [Passed]  
**Notes:**  Nothing noted here.

---

# Questions for Dev Team (If Applicable)

If there were ambiguities in how the game should work, note them here so dev team can clarify in Week 7:

- Does the game have the same text box issues, when ran on macOS, if ran on Windows?
- Are you meant to be able to play only 3 / 4 minigames and still fight the boss? Is it designed to be like a shortcut / quickplay version?

---

**End of Report**


# BlackJack Summary Report

**Game Tested:** BlackJack
**Dev Team:** Sam, Jessica, Karan, Maxwell
**QA Team:** Alex, Sham, Elizabeth, Melo
**Testing Period:** Week 6 (Tue–Fri)
**Report Date:** 2/13/26

---

## Executive Summary

We conducted comprehensive QA testing on BlackJack over 4 days. Our team tested [3 core features], ran [1 test scenario], and filed 2 test features documenting bugs across all severity levels.

**Key Finding:**  
The core game works, but there are other features of the game that would make the game crash or just not work at all.


---

## Testing Overview

### What We Tested
- Happy path (normal gameplay) ✓  
- Input validation & edge cases ✓  
- Win/lose conditions ✓  
- State management ✓  
- Complex scenarios & sequences ✓  

---

## Coverage Summary

### Features Tested
**Normal Blackjack Mode:** 100% tested  
- **Russian Blackjack Mode:** 80% tested (crashes prevented full testing)  
- **Upgrade System:** 75% tested (intermittent failures limited coverage)

### Test Types
-Functional testing (does it work?) ✓  
- Negative testing (what breaks it?) ✓  
- Boundary testing (edge values) ✓  
- Exploratory testing (creative scenarios) ✓
---

## Bug Summary

### By Severity
- **Critical:** [1] bugs (game-breaking)  
- **High:** [1] bugs (core features broken)  
- **Medium:** [0] bugs (partial functionality issues)  
- **Low:** [1] bugs (cosmetic or minor edge cases)  

**Total Bugs Filed:** [#]

### By Category
- **Input Validation:** [1] bugs  
- **Logic Errors:** [1] bugs  
- **State Management:** [0] bugs  
- **UI/UX Issues:** [0] bugs  
- **Other:** [1] bugs  

---

# Critical Issues (Must Fix Before Handoff)

These bugs prevent the game from being playable or break core mechanics.



| 1 | [Game Crashes in Russian BlackJack Mode] | Critical | [Enter the game, enter russian mode] | [https://github.com/ShammmN/Sprint1-Part2/issues/4] |


---

# High-Priority Issues (Fix ASAP)

These bugs affect core features but don't prevent gameplay.

| 2 | [Adding an extra card ignores the bust of 21 points] | Critical | [Play the blackjack normal game, if you happen to get the bust of 21, the game ignores it] | [https://github.com/ShammmN/Sprint1-Part2/issues/5] |


---

# Medium & Low Priority Issues

| 3 | [Not Able to Upgrade at Times] | Medium | [Play the normal mode, win the game, use the upgrade point you got by winning] | [https://github.com/ShammmN/Sprint1-Part2/issues/6] |

---

## Testing Insights

### What Worked Well
- [The game worked pretty well besides the fact that russian blackjack does not work]
- [Code quality made testing easier]  
- [Clear documentation helped understanding]  

### Areas for Improvement
- The game seems fine how it is. Just fix the bugs and it is perfect


# Recommendations for Dev Team

## Critical Fixes (Priority 1)
- Fix Russian Blackjack crash — game is completely unplayable in this mode  
- Fix bust detection at 21+ — prevents proper win/lose condition enforcement  

## Important Fixes (Priority 2)
- Improve input validation in [Russian Roulette]  

## Polish / Optional Fixes (Priority 3)
Fix the upgrades
---

## Test Environment

**Platform:** [Pycharm]  
**Testing Tools:** Manual testing + GitHub Issues  

---


- **Total:** [3] issues  
- **Closed:** [0] (if dev team fixed any during testing)  
- **Open:** [3] (for dev team to fix in Week 7)  

---

## Conclusion

[Our team conducted comprehensive testing of BlackJack over a 4-day period, executing functional, negative, boundary, and exploratory tests across all core features. The game has 3 documented issues ranging from critical to medium severity. The normal gameplay mode functions correctly and provides a solid foundation. However, critical bugs in Russian Blackjack mode (game crashes on entry) and the bust detection system (ignores scores exceeding 21) must be addressed before handoff. Additionally, the upgrade system experiences intermittent failures that impact player progression. With focused effort on resolving the 2 critical bugs, the core gameplay loop will be fully playable and ready for release. Input validation and game state logic are the primary areas requiring developer attention.]

The game has 3 documented issues** ranging from critical to cosmetic. With focused effort on critical bugs, the core gameplay loop is playable. Input validation and state management are the areas needing most attention.

---

# QA Team Sign-Off

**Test Lead:** [Sham]  
**Submitted:** [2/13/26]

**Team Members:**
- Alex
- Sham 
- Elizabeth  
- Melo

---

# Appendix: Detailed Test Scenarios

### Scenario 1: [Happy Path]
**Result:** [Passed]  
**Notes:** [The normal mode works]

### Scenario 2: [Input Validation]
**Result:** [Failed]  
**Notes:**  [The upgrades and russian roulette do not work when you click on them]

### Scenario 3: [Edge Cases]
**Result:** [Passed]
**Notes:**  [All boundary conditions handled correctly.]

---

**End of Report**
