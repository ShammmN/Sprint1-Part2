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
