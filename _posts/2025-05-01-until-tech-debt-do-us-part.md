---
title: "Until tech debt do us part"
categories:
  - Coding
tags:
  - Programming
  - Android
  - iOS
  - Archtecture
---
You have just got a brand new credit card. What do you spend it on? And then what happens to the debt that you accrued? 

While monetary debt is very easy to put thoughts to what it means for you, technical debt not so simple and a polarizing topic, when you are in a codebase for a long time, you get to know its ins and outs, and its shortcomings. These shortcomings can then compound to the point where a person writing code could of taken 2 days to get a feature out, but then takes 5 days, be down to many reasons but are generally down to these. 

- Cutting corners to meet a deadline development or architecturally
- In-ability to see the items being added are contributing to debt
- In-ability to pay off this debt (in my opinion the most insidious kind)

## Why is it called Debt?

When we think of debt, we think of the lunch that we have brought on that new credit card we got. This debt is generally ok and is paid off before the month is up before interest gets charged. Now lets take this metaphor further, what happens when we have many people charging and paying for "time" to hit a deadline. Do we think we can pay this off before the interest is owed?


>💡 Ward Cunningham was one of the first people to coin the term "Technical debt" 
> http://c2.com/doc/oopsla92.html


Interest luckily "*only*" needs to be payed when you have to go through the code that is a problem.  **I want to challenge this thought**, people believe that Technical debt only needs to be paid when the area within the app is being edited, while this is mostly true, there are cases where this breaks down. 

- What happens when you have a new hire comes in and asks about this side of the codebase?
- What happens when a feature you are working on could of used some code from that area?
- What choices have developers made, that have actively taught them to ignore that code?

## The Problem

What happens when we actively ignore issues? When this happens technical knowledge of the part of the codebase is lost, as everyone actively ignores it. And when a person moves away from the codebase it is lost forever, becoming a black box. 

When this happens we do not learn from our mistakes, and then at the worst case, when we do not learn from our faults. We make that mistake again, we create the problem that we ignore again. 

How many times must we re-write our apps in the name of "moving faster" that we then create the problems that we dreaded and moved away from in the beginning?