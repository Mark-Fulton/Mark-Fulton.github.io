---
title: "Three things to look for reviewing code"
categories:
  - Coding
tags:
  - Programming
  - Android
  - iOS
  - Archtecture
---
In the Three principals for pull requests  page, I mentioned three things to look at, here are three more things to be aware of when coding. 

### Complexity

- Is the code more complex than it should be?
- Is the **intent** of the code **clear** to you, or a hypothetical new employee first looking at the App?
- Check this at every line of the code — are individual lines too complex?
- Are functions too complex?
- Are classes too complex?

“Too complex” usually means **“can’t be understood quickly by code readers.”** It can also mean **“developers are likely to introduce bugs when they try to call or modify this code.”**

A particular type of complexity is **over-engineering**, where developers have made the code more generic than it needs to be, or added functionality that isn’t presently needed by the system.

> Reviewers should be especially vigilant about over-engineering. Encourage developers to solve the problem they know needs to be solved now, not the problem that the developer speculates might need to be solved in the future.
> 

### Tests

- Will the tests actually fail when the code is broken?
- If the code changes beneath them, will they start producing false positives?
- Does each test make simple and useful assertions?
- Are the tests separated appropriately between different test methods?

Make sure that you have unit tests that are appropriate for the change. In general, tests should be added in the same commit as the code itself.

Make sure that the tests in the code is correct, sensible, and useful. Tests do not test themselves, and we rarely write tests for our tests—a human must ensure that tests are valid.

### Comments

- Did the developer write clear comments in understandable English?
- Are all of the comments actually necessary?

Usually comments are useful when they **explain why** some code exists, and should not be explaining *what* some code is doing. If the code isn’t clear enough to explain itself, then the code should be made simpler. There are some exceptions (regular expressions and complex algorithms often benefit greatly from comments that explain what they’re doing, for example) but mostly comments are for information that the code itself can’t possibly contain, like the reasoning behind a decision.