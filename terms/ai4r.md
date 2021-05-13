---
title: "CS-7638 AI4R"
subject-name: "Artificial Intelligence for Robotics"
layout: term
term: "summer-2021"
permalink: "ai4r"
summary: ""
---

{% assign term = site.data.terms | where_exp: "term", "page.url contains term.url" | first %}

[Summer 2021 Schedule](https://docs.google.com/spreadsheets/d/1tePBL1L-rseevy6vRbRe2mqcxgGlDudkUYPQLuJSVU4/edit?usp=sharing)
<!-- # Recommended Prerequisites
While computer architecture and C++ are listed as basic prerequisites, having even basic fundamental knowledge is enough to get started. Most of the things required can be picked up during the course. One important thing is to be active on Piazza. From projects to quiz, there are couple of errata, and missing Piazza will be a nightmare. Also, the office hours are not recorded, so need to plan to attend if you are interested. The atmosphere is like a small classroom with a few people and Professor patiently explains and clarifies doubts.

# Project 0 <small>September 7, 2020</small>
Having two monitors or a printout of the instruction will help. You'll need to go through the project document and one or more Piazza posts regarding the same to understand the requirements and avoid confusion. It is not difficult, but definitely draining. You'll need to work on the provided VM, and it is based on Ubuntu 12, so no VS Code (I was heart broken when I discovered it after struggling to set it up for 2 hours). The default RAM, and CPU is less, and can be increased, and network can be enabled as well, but it is highly recommended to not upgrade the Ubuntu (because no one wants to risk getting different results than the one that will be tested upon), or C++ and accompanying libraries. Installing additional software is generally considered safe.

# Projects 1-3 & Midterm <small>November 25, 2020</small>
Projects 1 and 2 are significantly difficult and take time to complete. The disconnect between instructions and clarifications continue. You have to go through the FAQ thread and other student and instructor related follow ups on the project to get a clearer picture of the requirements and help. My partner for project 2 dropped and I had to pull it together at the last moment alone. I strongly recommend running benchmarks with your code changes to get some peace of mind (or the lack thereof). There are a lot of files to submit, so ensure you are not overwriting files from older simulation runs.

Project 3 is pretty much similar with respect to workload and inconsistent instructions. But having a dependable partner turned out to be life saver. The discussions in the group thread with Nolan (instructor) and my partner helped me course-correct my solution.

Midterm was tiring. It had a lot of calculations and by the end of an hour and half, I felt exhausted. I had a few minutes to spare at the end, but felt drained to revise. Of course I did not score above 90, but was not too far behind either. I think practising before the test will help speed up the calculations, and also get you back to the habit of number crunching for two hours straight.

# Final <small>December 19, 2020</small>
You'll get 3 hours to complete the final exam and the syllabus includes content from the midterm. I found the time to be more than generous, but the questions were a little tricky. I was not as prepared as I had hoped, and scored relatively low on the finals. It will take a much deeper knowledge of the coursework and practice to get 90+ in finals. The good news is, if you can score almost perfect marks in the projects, it will boost your grade. Despite my unsatisfactory performance in the final, I managed to bag an A.

# Secrets to success
1. The course is heavily front loaded. Starting at least a week early is recommended. Lagging behind on the week schedule might not be good idea. 
2. Office hours are not recorded. There are only a few people attending and that is a good opportunity to get your doubts cleared directly by the professor. No questions are stupid questions.
3. Stay on top of Piazza posts. There are a lot of errors and clarifications in the problem sets and Projects. Missing important updates from the instructors **will** affect your grade.
4. Run through all the benchmarks for the Projects.
5. Get loads of practice on pen and paper before the midterm and final.

# Learning outcome and applications
## Impacts of branches on code
Conditionals are a part and parcel of our everyday life and we often do not consider the impact of that. With modern multistage CPU pipeline, mispredictions come at a heavy cost. A simple example of this is that operations on a partitioned or sorted array is significantly better as it offers better branch prediction. While most modern compilers and predictors are pretty good at estimating, we should still try to make it simpler for the processor.
## Impacts of premature optimizations
While this point is a little contradicting to my point above, it should be noted that compilers try to make our life easier. While we learn about the internal workings of the processor, compilers too are getting better at producing optimised code. But if we start to manually unroll loops, we might end up introducing a bug or worse confuse the compiler. The first goal should be writing clean code that is easy for *human* to understand. If performance enhancements are required, then we can start tweaking and running benchmarks to confirm if the optimization is actually reaping benefits.
## Many cores and cache coherence
> With many cores, comes many coherence issues.

As multiple cores starts working with the same data, it becomes increasingly difficult to ensure coherence and consistency. Lot of factors have to be taken into account to deal with the problems: cache capacity, correctness, updating memory, bus traffic, cache pollution and so on. In the end, as usual it comes down to trading off something for another.
## Reliability
Disks will fail, datacentres will collapse. Redundancy and error detection are crucial to keep data alive and processing capability alive. The cost and need for dependency deepens on the application - is is a small personal business or a manned space mission? The later will need multiple layers of redundancy and fail-safes to avoid loss of life.

As always, this course covers a lot of exciting topics, and urges one to think when designing a software or hardware system. -->
