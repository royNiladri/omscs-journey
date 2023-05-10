---
title: "CS-6300 SDP"
subject-name: "Software Development Process"
layout: term
term: "spring-2023"
permalink: "sdp"
summary: ""
---

{% assign term = site.data.terms | where_exp: "term", "page.url contains term.url" | first %}

# Recommended Prerequisites
Nothing much is expected to start this class. It is decently paced and all relevant knowledge can be covered during the course. 
But if you have never used object oriented paradigm, or not used a language like Java, it will help to get a jump start on that.
Additional knowledge of using Android Studio too will be a good (though this too is covered briefly as part of the class). As of this semester, we used Java, and not Kotlin, and expect it to be the same for next few semesters.

# Development Environment
- Java 11
- IntelliJ IDEA(You can get license using your student account from GitHub Student pack)
    - AFAIK, the community edition too will be fine for this class.
- Android Studio (version will be mention in class setup guide)

All software are compatible with M1 MacBook Pro, as well as Windows.

# Grade Distribution

Item Description | Grade Contribution
:--|--:
Assignments | 44%
Group Project (team-based) | 18%
Collaboration (for group project) | 10%
Individual Project | 25%
Participation (Ed Discussion, Lectures and Quizzes) | 3%

Note that the class tracks progress of lectures based on Ed Lessons. So even if you are downloading content to watch it in a flight, you'll still need to run through the lectures on Ed to get participation points. Also, it needs to follow the prescribed schedule. Some anomaly is likely allowed, but going through the whole lesson at once at the beginning or end will likely deduct points as well.

# Projects/Assignments
This class is not designed to be front loaded. All s=assignments are released exactly on a Saturday (Monday, if it depends on a previous deliverable), and expected on the next Sunday. While most of the assignments/projects are small enough to complete in a weekend, I would strongly recommend to start early and identify blockers early in case you need help. Office hours happen every week and can be a great help.

## Assignments
The assignments are generally smaller projects that can be turned over in a week's time. The topics covered in Assignments are:
- Git Usage
- Java Fundamentals & JUnit
- Getting started with Android
- Software Design
- White Box Testing

A6 (White box testing) contributes 15% to the grade and is not auto graded. It is possibly the only assignment that will define your grade. The average can fall below 80, and given the class does not have a significant curve, it can drag your grade to B. Give it the time it requires and think through it. Talking to a rubber duck, or non-tech family might help.

## Group Project
In this project, you'll produce multiple design documents as a team and develop and test an android app. There is no auto grading for the textual deliverables. The team is selected based on a survey by the professor/TA. There is a post assessment survey to estimate member's contribution that helps deter dead weight in the team. The project itself contributes 18% and all members will get the same points here, but the collaboration, that contributes 10%, will likely be different based on contributions.

## Individual Project
This is the heaviest contributor to grade. You'll need to design tests and develop an app with the tests. Most of the deliverables are auto graded. Coming up with the test case and writing those test cases (70-90 cases) is possibly the hardest and most time consuming part of the assignment. Once you have the test framework, coding the actual implementation is relatively straightforward. 

# Exams
This is the fun part of the class - there are no exams!

# Learning outcome and application
This class beautifully introduces you to the Software Development Process and some of its most popular paradigms. The class is well paced, and Professor Orso and TAs are very much involved and helpful. They will of course not spoon feed you, but if you are coming from a class like ML, the support and respect for students will be a appreciated!

This class time and again illustrates the importance of spending time on thoughtful design and pragmatic test coverage. It urges students to push for clarifying non functional requirements and take those into consideration as well when working on real life projects.
