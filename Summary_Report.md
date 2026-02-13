Use Ctrl + F to find your game
# QA Summary Report

**Game Tested:** Fshng Game  
**Dev Team:** Marcus C, Ayah, Bianca, Maddy  
**QA Team:** Elizabeth, Sham, Melo, Alex
**Testing Period:** Week 6 (Tue–Fri)  
**Report Date:** 02/13/2026 

---

## Executive Summary

We conducted comprehensive QA testing on Fshng Game over 4 days. Our team tested the fishing mechanic, ran multiple test plays (around 38), and filed 3 GitHub issues documenting bugs across all severity levels.

**Key Finding:**  
Core game works, doesn't have upgrade system or anything of that such, and very plain UI.

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
- **Feature 1:** 100% tested  
- **Feature 2:** 80% tested  
- **Feature 3:** Not tested (reason)  

### Test Types
- Functional testing (does it work?)  
- Negative testing (what breaks it?)  
- Boundary testing (edge values)  
- Exploratory testing (creative scenarios)  

---

## Bug Summary

### By Severity
- **Critical:** [#] bugs (game-breaking)  
- **High:** [#] bugs (core features broken)  
- **Medium:** [#] bugs (partial functionality issues)  
- **Low:** [#] bugs (cosmetic or minor edge cases)  

**Total Bugs Filed:** [#]

### By Category
- **Input Validation:** [#] bugs  
- **Logic Errors:** [#] bugs  
- **State Management:** [#] bugs  
- **UI/UX Issues:** [#] bugs  
- **Other:** [#] bugs  

---

# Critical Issues (Must Fix Before Handoff)

These bugs prevent the game from being playable or break core mechanics.

| # | Title | Severity | Steps to Reproduce | GitHub Issue |
|---|--------|----------|-------------------|--------------|
| 1 | [Title] | Critical | [Brief steps] | [Link] |
| 2 | [Title] | Critical | [Brief steps] | [Link] |

---

# High-Priority Issues (Fix ASAP)

These bugs affect core features but don't prevent gameplay.

| # | Title | Severity | GitHub Issue |
|---|--------|----------|--------------|
| 1 | [Title] | High | [Link] |
| 2 | [Title] | High | [Link] |
| 3 | [Title] | High | [Link] |

---

# Medium & Low Priority Issues

Documented in GitHub Issues. These can be deferred or fixed in sequence.

---

## Testing Insights

### What Worked Well
- [Feature X performed as expected]  
- [Code quality made testing easier]  
- [Clear documentation helped understanding]  

### Areas for Improvement
- [Input validation is weak]  
- [State management has logic errors]  
- [Error messages are unclear]  

### Patterns Noticed
- [Did bugs cluster in certain areas? Did specific input types break the game?]

---

# Recommendations for Dev Team

## Critical Fixes (Priority 1)
- Fix [Issue X] — affects [feature]  
- Fix [Issue Y] — prevents [win/lose condition]  

## Important Fixes (Priority 2)
- Improve input validation in [feature]  
- Fix state tracking in [feature]  

## Polish / Optional Fixes (Priority 3)
- [Cosmetic improvements]  
- [Nice-to-have enhancements]  

---

## Test Environment

**Platform:** [Python terminal / Replit / Codespaces]  
**Game Version:** [Commit hash or date]  
**Testing Tools:** Manual testing + GitHub Issues  

---

## All GitHub Issues

Complete list of filed bugs:  
See dev team repo for all open GitHub Issues tagged `qa-week6`

- **Total:** [#] issues  
- **Closed:** [#] (if dev team fixed any during testing)  
- **Open:** [#] (for dev team to fix in Week 7)  

---

## Conclusion

[Summary of testing effort and findings. One paragraph.]

The game has **[#] documented issues** ranging from critical to cosmetic. With focused effort on critical bugs, the core gameplay loop is playable. Input validation and state management are the areas needing most attention.

---

# QA Team Sign-Off

**Test Lead:** [Name]  
**Submitted:** [Date/Time]  

**Team Members:**
- [Name]  
- [Name]  
- [Name]  
- [Name]  

---

# Appendix: Detailed Test Scenarios

### Scenario 1: [Happy Path]
**Result:** [Passed / Failed / Partial]  
**Notes:** [What did we learn?]

### Scenario 2: [Input Validation]
**Result:** [Passed / Failed / Partial]  
**Notes:**  

### Scenario 3: [Edge Cases]
**Result:** [Passed / Failed / Partial]  
**Notes:**  

---

# Questions for Dev Team (If Applicable)

If there were ambiguities in how the game should work, note them here so dev team can clarify in Week 7:

- [Question about mechanic X]  
- [Unclear behavior in feature Y]  

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
