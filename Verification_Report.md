# QA Fix Verification Report

**Game Tested:**
- TickleThePickle
  
**Dev Team:**
- Elizabeth, Melo, Alex, Sham

**QA Team:**
- Khani, Nayan, Gauhar, Quint

**Date:**
- 02/17/2026

---

## Summary

- **Total Bugs from Week 6:** 7  
- **Bugs Verified as Fixed:** 7  
- **Bugs Still Present:** 0  
- **Regressions Found:** 2  

---

## Bug Verification Details

For each bug reported in Week 6, document whether the fix worked.

---

### Bug #1

**Original Issue:**  
- The upgrade Key "p" can not increase damage/allow you to shoot multiple projectiles. 

**Severity:**  
- High 

**Status:** 
- Fixed 

**Verification Notes:**  
- This bug was fixed and now you can upgrade once per wave for 150 points by pressing 'P'.

---

### Bug #2

**Original Issue:**  
- There is no screen displaying that you can not upgrade with the incorrect amount of points

**Severity:**  
- High  

**Status:** 
- Fixed 

**Verification Notes:**  
- Added a pop up message that lets the user know they can not upgrade due to insuffienct points or if they already got their upgrade that round.

---

### Bug #3

**Original Issue:**  
- The game does not end when the pickles get to the bottom of the screen

**Severity:**  
- High 

**Status:** 
- Fixed 

**Verification Notes:**  
- Added a line/border to end the game when the Pickle Soldiers reach it.

---

### Bug #4

**Original Issue:**  
- The Pickle Soldiers do not hurt you when they collide with the player.

**Severity:**  
- High 

**Status:** 
- Fixed 

**Verification Notes:**  
- Added a line/border to end the game when the Pickle Soldiers reach it which stops the soldiers from touching the player.

---

### Bug #5

**Original Issue:**  
- Pressing the 'Q' key to quit does not work

**Severity:**  
- Medium

**Status:** 
- Fixed 

**Verification Notes:**  
- Added code so that when the user presses the 'Q' key it asks for verification to quit and resets them back to the start screen.

---

### Bug #6

**Original Issue:**  
- The Pickle Soldiers and Vampire images are not fully transparent even as a clipart image

**Severity:**  
- Low

**Status:** 
- Fixed 

**Verification Notes:**  
- The images are now fixed and do not have a white background by swapping the images out for better ones.  

---

### Bug #7

**Original Issue:**  
- Ending screen after boss fight is not visible with the natural browser zoom of the game 

**Severity:**  
- Medium

**Status:** 
- Fixed 

**Verification Notes:**  
- Added a won verification and a lost verification screen after the end of the boss fight. 

---

---

## Regressions (New Bugs from Fixes)

Did fixing bugs introduce new bugs?

---

### Regression #1

**What Happened:**  
- Tried to combine pieces of code and ended up breaking the boarder for the Pickle Soilders movement.

**When It Occurs (Steps to Reproduce):**  
1. Open the game  
2. Play but dont shoot
3. Observe as the Pickle Soldiers move off the screen

**Severity:** 
- Critical 

**Related to Fix:**  
- Trying to fix the clipart images bug.

---

### Regression #2

**What Happened:**  
- After you press 'Q' to quit and restart, it speeds up then if you press 'Q' to quit again and restart it again, it speeds up so much it crashes. 

**When It Occurs (Steps to Reproduce):**  
1. Open the game  
2. Play but then press 'Q' to quit 
3. Restart the game and play
4. Observe as the all the game movements speed up
5. Press 'Q' to quit
6. Restart the game and play again
7. Observe as the game speeds up much faster and crashes

**Severity:** 
- Critical 

**Related to Fix:**  
- Trying to fix the press 'Q' key to quit option. 

---

## Overall Assessment

**Game Status After Fixes:**  
- The game is now very improved and has a lot of cool new features. It takes into account a lot of issues that a user could face that were not thought of before. The graphics are now much nicer and higher quality. We also added more quality features that help the user navigate the game so it is easier to understand. 

**Recommendation for Dev Team:**  
- One recommendation for the Dev team is to keep the PNG images and not use images with a clear background because that does not work well. Also do pretests for small things like if a user decided not to play the game at all, to make sure you take all possible issues into account. 

**Testing Approach Used:**  
- We did each issue one by one. First we read the issue, then tested it to see how exactly it works. After we made sure we understood the issue then we fixed it and ran another test to make sure the game runs as intended with the updated coded. When we test is when we can see if there is a new problem formed or not and then we went throught again fixing the code and testing it.

---

## Sign-Off

**QA Team:**

- Sham  
- Alex  
- Melo  
- Elizabeth 

**Verification Completed:** [Date/Time]
