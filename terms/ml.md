---
title: "CS-7641 ML"
subject-name: "Machine Learning"
layout: term
term: "fall-2022"
permalink: "ml"
summary: ""
---

{% assign term = site.data.terms | where_exp: "term", "page.url contains term.url" | first %}

# Prologue
I had attempted this during fall of 2021 with [ML4T](/ml4t). It did not go well. It was too much work and too chaotic and to save my grades I ended up withdrawing just before midterms & focussed my energy on ML4T. I expected the next time I took it after ML4T and AI, it would make more sense. Do note that [CS 6601 AI](/ai) is listed as a prerequisite for this course.  

This is not a class for the weak of heart. It will eat up a lot of time, energy and motivation. If you do not need this to get your degree, or browsing through courses, it would strongly recommend to stay away from it. At the end, if you have survived, you do learn a lot, but the experience is utterly frustrating. There are a lot of people who enjoy the class, sadly I am not one of them. Some thrive in the chaos, but I do not!

# Recommended Prerequisites
As so many others, a good understanding of Python is a must for this class. There are a lot of theoretical concepts to grasp and you will not find time to pick up a new language on the side. Good understanding of linear algebra and probability are good to have. If you are not from a CS background and starting OMSCS, this is not the class to begin with! (If this feels repetitive from my post on AI, its because it is!)


# Development Environment
- VS Code [Extensions listed below]
    - Jupyter
    - Python (Pylance)
- Anaconda (Python3)

This class offers a lot of flexibility ranging from choosing datasets to choosing frameworks. There are some suggestions like mlrose-hiive and MDP-toolbox, but you are free to choose differently.

# Projects
The projects are open ended and focuses more on analysis. You can use any library or write code from scratch (not recommended due to time constraints), but the most import part are the graphs, and the accompanying explanations. Be sure to include as many whys as possible:
- Why did you choose that dataset?
- What all hyper-parameter tuning did you do and why?
- Why did you get the results you got?
- What other changes can you do and why

Some recommendations for choosing dataset:
* Do not start with huge dataset as you will have to do many runs and if each run is taking you over an hour, it will impact how much tuning you can do before the deadline.
* It might be a good idea to include one dataset with some imbalance in the classes.
* Have at least one dataset with 10+ columns so that you can get reasonable behavior for dimensionality reduction.

Some generic report writing tips:
* You'll be pressed for real estate based on the page limit.
* Reduce margins, but do not go overboard with it
* Using font below 10 is not recommended. Expect your grader to be able to read it without zooming.
* Reduce image sizes so that at least the trends can be seen without zoom. For more details on units or other markers, it should be fine if one needs to zoom to read that.
* Use columns to make the most of the space. Instead of 2 column layout, I found adding 2-3 images in a table or and image and analysis side by side is a much better visual experience without straining the eye of the reader.
* In general, your grader is a human so use your good judgement to not make his/her life hell while grading your assigment.

Once again, **office hours are crucial**. If they are at an inconvenient time, watch the recordings. The projects have a 50% weightage on you final grade.

## Supervised Learning
You start with two "interesting" classification datasets and run different supervised methods and compare and contrast their performance. Be sure to choose datasets that show come contrast across different algorithms and among themselves for few of them. Hyper parameter tuning plots and learning curves are a must, along with ample analysis of why they are the way they are.

## Randomized Optimization
Here you choose some problem domains (using recommended libraries are helpful here as they come with prebuilt problems), and run different randomized optimization to solve them. Again you'll need to tune the parameters and note the impact. Be sure to summarize which algorithm is the right fit for which problem and why. 

## Unsupervised Learning & Dimensionality Reduction
Mix and match of different dimensionality reduction (or feature transformation) with clustering algorithms. You'll run each individually and then combine them. As always, analysis is the key. How do the different dataset fare with different DR techniques. How does the clustering work without DR and with different DR.

## Reinforcement Learning (MDP)
Select 2 MDP (you can use one from the recommended library and one from [Open AI Gym](https://github.com/Farama-Foundation/Gymnasium)), and run it through a model based learning and a model-free learning. Compare and contrast the relative performance and analyze the why. Rewards are the domain knowledge, so be sure to tweak the rewards as you deem necessary.

# Exams
There are two (non cumulative) exams, which are closed everything. You dod not get even a scratch paper. Both of them have 25% weightage each and the final has the possibility of overriding the midterm if better. The questions are subjective with a mix of True/False (you get points for explanation only), and long answer type. Mathematical derivations are not needed.

## Midterm
This is a very long paper, and supposedly designed as such that it cannot be completed. So ensure to focus your time and energy to questions that you are well aware of. I started with the T/F questions and I would recommend to not do that. They contribute little, and at the beginning you tend to write more than required.

## Final
While it was supposed to be easier, and some students agreed, I beg to differ. I felt it was harder, but there was enough time to complete the paper this time. I ended up getting lower for final and hence no grade substitution for me!

# Learning outcome and application
TBD

# Epilogue
Grading is the fun part. Every thing is subjective. The projects are graded by different TAs, and you get varying grades throughout the semester. The requirements are fluid and most of the hard requirements are discussed in Office hours. The subjective exams are also a hit and miss. I felt I fared better in the final, but ended up scoring lower. While this might be a good mock of real life where your efforts and the results are not linearly related, but as a part time student with other responsibilities, I expected a saner and structured approach to the class. If you are over the mean of class overall and also for most of the assignments and exams, you can expect to get an A (no promises though).

<figure style="margin: auto; display:block; width: 70%">
<img src="assets/images/ml-grades.png" alt="ML Grade distribution">
<figcaption>Grade Distribution for ML over the years <a href="https://lite.gatech.edu/lite_script/dashboards/grade_distribution.html">(source)</a> </figcaption>
</figure>

While the professor is very active in discussion forum and even slack, but half the time you'll get unhelpful snarky remarks. The head TA and the experienced classmates will make the class bearable.
