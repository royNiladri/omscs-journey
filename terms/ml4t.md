---
title: "CS-7646 ML4T"
subject-name: "Machine Learning for Trading"
layout: term
term: "fall-2021"
permalink: "ml4t"
summary: ""
---

{% assign term = site.data.terms | where_exp: "term", "page.url contains term.url" | first %}

# Recommended Prerequisites
This is one of those classes that assume very little of your background and gives you enough time and support to bootstrap. Some basic knowledge of Python and statistics will help, but you'll get enough time to ramn up during the first half of the course. Schedules, reading links and projects from perious term can be found on the [course website](http://lucylabs.gatech.edu/ml4t).

# Development Environment
- VS Code [Extensions listed below]
    - Jupyter
    - Python (Pylance)
- Anaconda (Python3)

I create Jupyter Notebooks for the class and problem sets for ease of working. If published to GitHub private repo (do not publish projects/problem set solutions to public repository as at violates Academic Policies), it is rendered as a formatted notebook. Read more about that at [GitHub Blog](https://github.blog/2015-05-07-github-jupyter-notebooks-3/) or [Jupyter Blog](https://blog.jupyter.org/rendering-notebooks-on-github-f7ac8736d686)

**Important**: Many people run into issues of running on Windows mahine. I had used Kubuntu 20.04, and students in discussion forum have confirmed that they were able to complete the semester in M1 Mac. The class provides a VM that you can use, or use anaconda and isntall the dependencies they list out. Also note that for exam, honorlock is used and it will not run on Linux. You'll need a Windows or Mac machine for the exam.
# Projects
There were a total of 8 projects in this class. In general the complexity increases with each projects, and in some cases, you'll need to write ~10 page reports. Most prjects have local testing scripts and have unlimited sumbission to Gradescope tetsing. Also note that some projects are cumulative. Do not skip one as you might need to use the code from that in multiple later projects. 

Some general things to keep in mind:
- Start early
- Test edge cases if not covered in the provided grading script
- If rubric is mentioned, go though all the points and validate it is covered
- Ensure all `print` statements are either behind a verbose flag that is set to false by default, or commented before submitting.
- Ensure graphs are saved in files and not shown blocking the execution (do no use something analogous to `plt.show()`).

## Project 8 (Capstone)
This project brings together everything we learned in the class. If you have failed to score perfectly for previous projects, ensure to fix them before attempting this. It uses code from most of the previous ones. It covers trading, tracking portfolio day by day, and training AI/ML model to predict trades. It has 20% contribution to the total grade. Start early, follow forum discussion, especially the ones started by instructors/TAs. This has parameter tuning, and will eat up significant time - plan accordingly.

## Extra Credit
There was an opportunity to earn 2% on extra credit, but I did not find the time to work on it.

# Exams
There are two exams - midterm, and final. Each of these contribute to 12.5% of total grade. It is a closed everything exam. No notes, no internet, no calculator. A full room scan is required, but mirrors are not needed during the exam. Ensure to read the Exam policy document of your semester for exact details. If you cover the topics and brush through the readings, it is fairly easy to score full marks. The final is not cumulative. Be sure to watch "The Big Short" - understand the terms, remember the characters!

# Learning outcome and applications
TBD