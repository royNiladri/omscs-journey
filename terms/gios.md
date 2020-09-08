---
title: "CS-6200 GIOS"
subject-name: "Graduate Intro to Operating Systems"
summary: "Fail fast is another important thing that I reinforced in this class. New job, same city relocation, Covid-19 outbreak - with all these, it took me a while to start project 3 and the last few nights were a nightmare. ... I had to turn in Project 3 half baked, but after the finals, it bothers me less. Lost a finger, but saved the rest of the body!"
layout: term
term: "spring-2020"
permalink: "/gios"
---

{% assign term = site.data.terms | where_exp: "term", "page.url contains term.url" | first %}

# Recommended Prerequisites
1. Good understanding of Computer architecture. Bare basics should suffice
2. Some exposure to C programming, preferably the ability to read through manuals. Brush up Networking and String (lots of pitfalls here) in C to gain an edge.

# 3 Months in Update <small>April 5, 2020</small>
Well, it's a lot of work! I really did not expect the projects to be so much work! The lectures are well structured. A lot of the things covered are present in the unofficial reading list books (I have been following OSTEP for the most part). The papers that accompany are a bit archaic, but definitely shed some light on how things worked, and why we have some of the things work the way they do now.

Okay, I guess I fast-forwarded a little. The course structure is as follows:

**Projects (3+ 1 extra credit)**|**40%**
**Midterm**|**25%**
**Finals**|**30%**
**Participation**|**5%**

If you read other posts asking you to start the projects early, you better follow that. It really is a lot of work, and the midterm and final are worth more than one single project. Time management is crucial and you need to fail fast if you want to survive the semester.

With all these being said, if you have prior exposure to undergraduate OS course and some advanced C programming skills up your sleeved, you should be able to sail across the course pretty comfortable.

***[P.S. : With  the onset of COVID-19 outbreak, the deadlines of project has been adjusted to allow a little more time. This is a trying time for everyone and hope we comes out of it with minimum losses. For me motivation has definitely taken a hit! People dying in thousands every day, loss of job, unable to spend time with family - so much negativity around. Hope we can overcome this in the coming couple of months.]***

# Secret to success <small>May 5, 2020</small>
First read the <em>Prerequisites</em> section if you have not! That being said, the exams are weighed towards concepts and understanding and not too specific details that you will need to mug up. So go though the contents **multiple times**. Make sure you understand every nuance. Work out the sample questions. Do out of order revisions. Watch out for errata. Following through Piazza posts served as a lifesaver both for projects and exams. Plus, you get participation points if that helps bump your grade (do note that quality of contribution is also taken into account). Slack channel is also very active and helpful. Last but not the least, start projects early (this cannot be stressed enough).

# Learning outcome and applications
First and foremost this course is an excellent material for patience and perseverance! That is a very essential skill to have for any successful engineer in the industry, more so if we are looking to bag some R&D roles. I used this opportunity to push myself through nights, reading through dozens of stackoverflow questions, going through manuals multiple times, watching out for Piazza posts and so on. A lot of hard work went in, and it was pretty rewarding in the end. (Did panic the last month though).

*Fail fast* is another important thing that I reinforced in this class. New job, same city relocation, Covid-19 outbreak - with all these, it took me a while to start project 3 and the last few nights were a nightmare. But towards the end, I realised, this might go for a toss, and finals are worth more. I stopped giving the project my 100% and started working on the lectures and readings that had been pending. I had to turn in Project 3 half baked, but after the finals, it bothers me less. Lost a finger, but saved the rest of the body!

Basic Operating system concepts, distributed systems, scheduling, multithreading - basically everything mentioned in the syllabus was covered in appropriate details. Among these, what I already put to work is multithreading and file handling. My workplace uses Java, but knowing how things worked under the hood, allowed to me think differently about the problem, and come up with an interesting and efficient solution.

Another key takeaway was the fact most things are never perfect and we need to find a balance between usability and design/development cost, along with current hardware/software/network limitations.

Last but not the least, **[RTFM](https://www.google.com/search?q=rtfm)**!!