---
title: "CS-6601 AI"
subject-name: "Artificial Intelligence"
layout: term
term: "spring-2022"
permalink: "ai"
summary: ""
---

{% assign term = site.data.terms | where_exp: "term", "page.url contains term.url" | first %}

# Recommended Prerequisites
A good understanding of Python is a must for this class. There are a lot of theoretical concepts to grasp and you will not find time to pick up a new language on the side. Good understanding of linear algebra and probability are good to have. If you are not from a CS background and starting OMSCS, this is not the class to begin with!

The class intro says that it might be curved, but generally the class median is above 90, and hence the cut-off is unlikely to fall below 90. It is a hard class, but students find a way to cope up. So do not count on the cut-off to fall to get your desired grade. Work assuming there is no curve to begin with, and you'll do fine. 
# Development Environment
- VS Code [Extensions listed below]
    - Jupyter
    - Python (Pylance)
- Anaconda (Python3)

The class will provide a requirements file at the start, and you will have to create an environment using the same. The instructions use Anaconda/Miniconda, but I believe using Python virtual environment should be fine as well. Most assignments are Jupyter Notebooks, and have helper functions to export that as `.py` files for submission to Gradescope.

# Projects
The projects go hand in hand with the class lectures and reading. The Readme files often have additional resources linked which are often critical to solving the problem. Be prepared to do a lot of reading and watching external videos for this class. Also avoid watching explicit solutions as that might lead to class policy violation. TAs are active and often conduct Office hours and code reviews - use them when stuck. Ed discussions also have great discussions and tips. As always, start early. It not only helps you get more time to code and think, and use the most of of throttled Gradescope submissions, but also get core tips before the discussion threads explode with unmanageable comments.
The first two projects are the hardest, and very difficult to get a full score. The other projects are relatively easier, but still require a lot of time and effort. Good vectorization is a must for some projects, as nested for loops will time out in Gradescope.

**Note:** While all the projects are available in the GA Tech GitHub account, they are tweaked considerably before release. I would not advise to start working on them prior to they are released. Also, the order of the projects may vary from term to term.

## 01 Search
This covers different search algorithms. It starts with the BFS, UCS, and continues into A*, and a lot of different flavours and optimizations on A*. Understanding explore and frontier sets (closed/open) as well as when the shortest path is found in crucial. If you are doing a fulltime job, might need to plan a 2 day leave! (I took it and still managed a mid 90).

## 02 Adversarial search/Game playing
The game is some flavour of isolation (discussed in the lecture and the book). You will incrementally build an AI agent that plays the game first against a player selecting random moves, and later against Peter's AI. You'll have to implement minimax with alpha-beta pruning and some further optimizations.

## 03 Bayes Net
This too is a relatively hard assignment. The theory is tricky, and you will have to solve parts of it on paper before it makes sense to code. The code too is not straightforward - you'll need to hand calculate probability tables and enter them. It might look easy when you look back at it, but do not underestimate it at the beginning.

## 04 Decision Tree and Random Forest
This is a relatively easier assignment. I might be prejudiced as I had written decision trees in other class ([ML4T](/ml4t)). It is well guided and the only parts which were a little tricky were the Gini impurity and entropy calculations.

## 05 Expectation Maximization
This is easy and frustrating at the same time! You'll have to go through the readings to understand the concepts, and you can theoretically run for loops wherever you see a sigma notation, but it will timeout in Gradescope. You'll need to vectorize the implementations and that will take time based on your prior knowledge with matrix and Python vectorization skills.

## 06 HMM
I skipped this project as there was best of 5. It was based on `Pattern Recognition through time`. For the most part, it appeared to be much easier than the other assignments.

# Exams
The exams are take-home, open note, open book. You cannot access internet. It is not proctored and you can work on it at your convenience.

## Midterm 
It was a ~25 page question paper covering all the topics covered so far. Partial credits are offered wherever it made sense. If you came up with an answer and feel it is right, raise a regrade request clearly stating your reasons, and you might get some points based on the soundness of your logic.

## Finals
The finals felt tougher than the midterm. If you want to score better, go through the assigned readings and internalize the concepts (I guide others to a treasure I cannot possess). The paper was around 50 pages long, and had a lot of interesting back stories to the problem. But it was not as well managed as you would like. There were multiple iterations of clarifications, some questiond changed multiple times.

# Extra Credit and Grading
There are multiple EC opportunities spread across projects and additional tasks like Meta lectures and surveys. It is higly recommended to hoard as much as extra credit as possible as the exams will likely bring your grades down.

# Learning outcome and application
TBD
