# QA Fix Verification Report

**Game Tested:**
- CHRISTOFER: THE RISE OF MARK-HAM
  
**Dev Team:**
- Gabe, Rahul, Huzaifah, and Troy

**QA Team:**
- Elizabeth, Melo, Alex, Sham

**Date:**
- 02/18/2026

---

## Summary

- **Total Bugs from Week 6:**  4
- **Bugs Verified as Fixed:** 2  
- **Bugs Still Present:** 2  
- **Regressions Found:** 1  

---

## Bug Verification Details

For each bug reported in Week 6, document whether the fix worked.

---

### Bug #1

**Original Issue:**  
- Cannot use items within a fight.

**Severity:**  
- Critical

**Status:** 
- partially fixed

**Verification Notes:**  
- The game keeps making you do basically the same things, like you are entering in a loop. However I think it is part of the game, it just needs a message to tell the user that they do not have that item or if they did use that item or not. It is not clear.

---

### Bug #2

**Original Issue:**  
- Hit enter, press random buttons and will enter a loop.

**Severity:**  
- Critical  

**Status:** 
- Fixed 

**Verification Notes:**  
- Added a message that lets the user know their input is invalid and does not go into a loop/crash.

---

### Bug #3

**Original Issue:**  
- Changing the text speed in setting by setting it to a higher number make the text slow.

**Severity:**  
- Medium

**Status:** 
- Not fixed  

**Verification Notes:**  
- The text speed still becomes slower when you set it to a higher number like 200. This setting could use more detail on how it works like a scale of what are allowed inputs and what they do. 

---

### Bug #4

**Original Issue:**  
- Cannot use certain abilities that are an available option

**Severity:**  
- High 

**Status:** 
- Fixed 

**Verification Notes:**  
- The game gives the user a pop up message letting them know they do not have access/own that item yet. 

---

---

## Regressions (New Bugs from Fixes)

Did fixing bugs introduce new bugs?

---

### Regression #1

**What Happened:**  
- Tried to test the items feature but the game does not let you use the item and puts you in almost like a loop of the same events and not really progressing.

**When It Occurs (Steps to Reproduce):**  
1. Open the game  
2. Enter 1 to play and play through
3. Try to use an item
4. Observe as the game does not do anything with the item and it asks the same questions over again

**Severity:** 
- Medium 

**Related to Fix:**  
- Trying to test the item game feature that previously had issues. 

---

---

## Overall Assessment

**Game Status After Fixes:**  
- The game looks good and the graphics are very cool. The game now has more user input handling like handling invalid user input. Although there are still a couple issues that need to be fixed, the game overall is very well done and creative. The color clicker part now ties in to the interactive story game too and it is very cool. 

**Recommendation for Dev Team:**  
- One recommendation for the Dev team is to add more information on the features because it can be hard to understand what they do and/or how to use them. 

**Testing Approach Used:**  
- We did each issue one by one. First we read the issue to see what exactly we were looking for, then we read how to recreate it and did observing to see if we can find the error. We took notes on what happened when we recreated the previous errors, seeing if the errors were fixed and if any new issues arose. 

---

## Sign-Off

**QA Team:**

- Sham  
- Alex  
- Melo  
- Elizabeth 

**Verification Completed:** 02/18/2026 


Game Tested: BlackJack
Dev Team: Samuel, Jessica, Karan, Maxwell
QA Team: Sham, Alex, Elizabeth, Melo
Date: 2/18/2026
Summary
Total Bugs from Week 6: 3
Bugs Verified as Fixed: 3
Bugs Still Present: 0
Regressions Found: 0
Bug Verification Details
Bug #1
Original Issue: Game crashes in Russian BlackJack mode after clicking Hit
Severity: Critical
Status: Fixed
Verification Notes: We launched the game, enabled Russian Mode from the menu, clicked Deal, then clicked Hit. In Week 6, the game froze and crashed at this point. After the fix, clicking Hit in Russian Mode no longer causes a freeze or crash. The game now correctly ignores the Hit action in Russian Mode since it is not a valid move in that mode. The round continues as expected.
Bug #2
Original Issue: Extra card upgrade ignores the 21-point bust rule on the deal
Severity: Critical
Status: Fixed
Verification Notes: We played until earning an upgrade point, upgraded Extra Cards, then clicked Deal multiple times across several rounds. In Week 6, the player could start with 3 cards totaling over 21 and still win by clicking Stand. After the fix, the upgrade no longer deals a third card directly. Instead, it re-rolls the starting hand up to the number of attempts unlocked and picks the best result under 21. We never started a round with a bust, and the bust logic on Hit and Stand worked normally throughout testing.
Bug #3
Original Issue: Upgrade buttons are unclickable at times even when upgrade points are available

Severity: Medium
Status: Fixed
Verification Notes: We won multiple blackjack rounds to earn upgrade points, then clicked the upgrade buttons (Extra Cards, Dealer Nerves, Bonus Payout) across approximately 10 separate attempts. In Week 6, the buttons would sometimes do nothing and the counter would not update. After the fix, the buttons responded correctly every time. The counter updated as expected (for example, 0/2 to 1/2) and points were deducted properly. We did not encounter the intermittent issue during this round of testing.
Regressions (New Bugs from Fixes)
Did fixing the bugs above introduce any new bugs?
No regressions were found. All three fixes were tested thoroughly, and no new issues came up during verification.
Overall Assessment
Game State After Fixes: The game is in a solid state. All three bugs from Week 6 have been resolved. Russian Mode no longer crashes, the card upgrade system works as intended without allowing a bust on deal, and the upgrade buttons are responsive. The game is fully playable from start to finish.
What the Dev Team Should Prioritize if Given More Time: General polish and additional edge case testing around the Russian Roulette mode, since it has more complex state handling than the rest of the game. It would be beneficial to ensure multiplier streaks and payout logic remain stable during extended play sessions.
Testing Approach Used: We re-ran the exact reproduction steps from each Week 6 bug report to confirm the fixes. We also played through several full sessions to verify that normal gameplay felt correct. Bug 3 received additional attention since it was originally intermittent, so we repeated that test more times than the others to ensure confidence in the fix.


Sign-Off
QA Team:
 Sham
 Alex
 Melo
 Elizabeth
Verification Completed: 02/18/2026
