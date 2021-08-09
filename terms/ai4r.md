---
title: "CS-7638 AI4R"
subject-name: "Artificial Intelligence for Robotics"
layout: term
term: "summer-2021"
permalink: "ai4r"
summary: ""
---

{% assign term = site.data.terms | where_exp: "term", "page.url contains term.url" | first %}

<div></div>

### Summer 2021 Schedule

<details>
    <summary>Click to expand/collapse</summary>

| Week #     | Deadline    | Name                         |
|:-----------| :---------: | :--------------------------- |
| 1          | 23-May-2021 | 📚 Localization              |
| 1          | 23-May-2021 | 📝 Problem Set 1             |
| 2          | 30-May-2021 | 📚 Kalman Filters            |
| 2          | 30-May-2021 | 📝 Problem Set 2             |
| 2          | 30-May-2021 | 📚 Particle Filters          |
| 2          | 30-May-2021 | 📚 Kinetic Bicycle Model 101 |
| 2          | 30-May-2021 | 📝 Problem Set 3             |
| 3          | 06-Jun-2021 | 💻 Kalman Filter Project     |
| 4          | 13-Jun-2021 | 📚 Search                    |
| 4          | 13-Jun-2021 | 📝 Problem Set 4             |
| 4          | 13-Jun-2021 | 📚 PID Control               |
| 4          | 13-Jun-2021 | 📝 Problem Set 5             |
| 5          | 20-Jun-2021 | 💻 Particle Filter Project   |
| 6          | 27-Jun-2021 | 📚 SLAM                      |
| 6          | 27-Jun-2021 | 📝 Problem Set 6             |
| 7          | 02-Jul-2021 | 💻 PID Mini-Project          |
| 8          | 11-Jul-2021 | 💻 Search Project            |
| 10         | 25-Jul-2021 | 💻 SLAM Project              |
| 11         | 31-Jul-2021 | ✒ Final                      |

 
</details>

**Note:** Deadlines here are mostly 1 day prior to official deadlines

# Recommended Prerequisites
The course will use **Python 3** as the programming language. I will confirm if using libraries like `numpy` are allowed for the projects and problem sets. Basic understanding of **probability** will be expected.

# Development Environment
_[Section is under progress]_
- VS Code [Extensions listed below]
    - Jupyter
    - Python (Pylance)
- Anaconda (Python3)

I create Jupyter Notebooks for the class and problem sets for ease of working. If published to GitHub private repo (do not publish projects/problem set solutions to public repository as at violates Academic Policies), it is rendered as a formatted notebook. Read more about that at [GitHub Blog](https://github.blog/2015-05-07-github-jupyter-notebooks-3/) or [Jupyter Blog](https://blog.jupyter.org/rendering-notebooks-on-github-f7ac8736d686)

# Projects
## [01 Meteorites](#meteorites)
The objective of this project was to localize falling meteorites and shoot them down. Meteorites could be detected first at any part of the screen, and there are restrictions on how far the turret can be rotated in 1 timestamp. Also, the turret could either be rotated, or fired, and not both. This project was an exciting hands on for `Kalman Filters`.

{% include youtube.html id="xB63bpXEzdA" %}

### Tips
Piazza posts, office hours and reference links have been greatly helpful. Focus on solving localization first as that has most of the weightage. Once localized, even a very simple targeting algorithm (as discussed in Piazza/office hours) will work. Note that the meteorites passed in subsequent calls are not sorted in any order, and blasted meteorites are passed on in subsequent calls as well. So you need to keep track of meteorites by ID and consider only those that are alive when targetting.

## [02 Mars Glider](#mars-glider)
A glider is dropped from a shuttle in orbit of Mars. Given a low resolution map, radar sensor and barometric sensor, we have to localize the glider and then navigate it back to the centre of the map. The on-board sensors are noisy and we have limited time to complete the navigation. This project was based on `Particle Filters`

{% include youtube.html id="eDNV03VIxgY" %}

### Tips
The hard part of the problem was parameter tuning. I sadly have not been able to score perfectly, but have enough to earn a little extra credit! I would recommend reading through the problem statement, browsing through all relevant Piazza posts and ruthlessly tuning parameters. Using the visualization helps in determining what is going wrong. There are a lot of trade-offs to consider, and bear in mind that Gradescope machine will be slower and hence might produce lesser score than on local. Finally, generate random test cases using provided utility to verify tuned parameters.

## [03 Rocket PID](rocket-pid)
In this (mini) project we were to control different types of rocket propulsion system using PID controller. The graph below is the last part which is based on a bi-propellent rocket model (fuel + liquid oxidizer). We were to adjust both the throttles to control the propulsion for a smooth takeoff and landing. We were to match the given velocity profile, while ensuring we do not run out of fuel or make a re-entry with a high velocity. The coding part was relatively simple, but tuning the gains of the controller was time consuming. This project provided good understanding of the individual effects of proportional, integral and derivative parts of the controller.
<figure style="margin: auto; display:block; width: 70%">
<img src="assets/images/rocket-pid.png" alt="Rocket PID control graph">
<figcaption>Rocket PID control graph</figcaption>
</figure>

### Tips
Again, the hard part is tuning. While you can write some harness to find out parameters using twiddle, or other algorithm, tuning it by hand imparts wisdom and deeper understanding of PID. And of course it is fun to watch the graphs gradually fall in place, and throttle oscillations dying out!

## [04 Warehouse](#warehouse)
This project is based on Search module. A robot in a warehouse is tasked with picking up boxes and delivering them to the destination. The first part can be solved using A*. In the second part, the robot can start at any point, and needs to deliver a box. The grids have different weights, mimicking rough terrain. DP is well suited for this. The last part introduces stochasticity, and the robot often fails to execute given commands. Part C is significantly more challenging, and accounts for 15% of the project grade.

{% include youtube.html id="RFxm9fSE77Q" %} <!--TODO: Add video -->

### Tips
Read the documentations as many times as needed. There are a lot of details in there. Go through how the code is wired up. Follow Piazza, and start engaging is discussions early. As of Summer 2021, the Problem Set solution was a bit flawed, and you need to modify that code to score full points. Cost calculations are not trivial, so join the office hours, or go through the recoding. Without those I don not think I could get full score. Note that parts A and B offer extra credit, and perfecting them might give you a little boost if you are missing a few test cases in part C.

## [05 Gemfinder](#gemfinder)
In this project we built a functional Graph SLAM. A robot is tasked with extracting gems, and it has to localize itself and then start extracting gems by moving to their locations. It is split into 2 parts. In the first part we chalk out the SLAM part, while following move commands from test cases. In the second part we were to extract the gems and figure out ways to reach to them. This was a project where you could get decent score quite easily, but ironing out those last wrinkles will take a lot of time and effort. Here as well the robot will be stochastic, and factoring in noise is a non-trivial exercise here.

#### Tips
The usual: start early, follow Piazza, keep an eye on office hours. Some things to ponder for part 2:
- What to do when you get stuck trying to extract at a wrong place?
- What to do if there are no gems in horizon?
## [Optional HW Challenge: Face Tracker](#face-tracker)
This is a rather open assignment for extra credit. You can use any hardware available and make a demonstration of sensing the environment and then affecting it in a way. You should use one of the techniques used in the classes. Since I did not have any experience with hardware, I decided to take the easy road and take up the guided HW project.

The documentation listed all possible hardware required, wiring diagram, and python packages and installation guides. I used a Raspberry Pi 4, but due to lockdown I could not get hold of pi hats, and specified motors. So I picked generic servos and ran with those! I had to write my own motor code, but that was a learning too. If you want to get started at that, check out the video by [Explaining Computers](https://www.youtube.com/watch?v=xHDT4CwjUQE). The meat of the challenge was to write a Kalman filter to track the face and make the camera follow it as closely as possible.

Here is my attempt at it:
{% include youtube.html id="vY7pAA5Pr9Q" %}

### Equipment list (Attaching links for India):
*   [Raspberry Pi 4 4GB model](https://www.thingbits.in/products/raspberry-pi-4-model-b-4-gb-ram)
*   [Sandisk 32GB Class 10 SD Card](https://www.thingbits.in/products/sandisk-32gb-class-10-microsd-memory-card-with-noobs)
*   [Mini HDMI to HDMI cable](https://www.thingbits.in/products/micro-hdmi-to-standard-hdmi-cable-for-raspberry-pi-4)
*   [Raspberry PI 5MP Camera Board Module](https://www.amazon.in/gp/product/B00E1GGE40/ref=ppx_yo_dt_b_asin_title_o04_s00?ie=UTF8&psc=1)
*   [ePro Labs KIT-0010 Breadboard + 60 Pieces Jumper Wires Set](https://www.amazon.in/gp/product/B01BLJGS7M/ref=ppx_yo_dt_b_asin_title_o04_s01?ie=UTF8&psc=1)
*   [Easy Electronics Set of 2 SG90 Servo Motors/Blue color](https://www.amazon.in/gp/product/B077TQD1N4/ref=ppx_yo_dt_b_asin_title_o05_s00?ie=UTF8&psc=1)
*   [Servo bracket PT pan/tilt camera platform](https://www.amazon.in/gp/product/B08GG75JD2/ref=ppx_yo_dt_b_asin_title_o03_s00?ie=UTF8&psc=1)

Total cost of all the above materials was around **INR 7,300**.

Other Stuff (optional):
*   [PiBOX India Raspberry Pi 4 Case](https://www.amazon.in/gp/product/B082ZQSHFZ/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1)
*   [TP-Link USB Hub](https://www.amazon.in/gp/product/B00V4BGD00/ref=ppx_yo_dt_b_asin_title_o02_s00?ie=UTF8&psc=1)
*   Logitech Wireless Keyboard and Mouse
*   Dell Monitor

# Final
In Summer 2021, it constitutes of 11% of the grade. If you score perfect grades in the project, and do the extra credit assignment, you can skip the final and still land an A! The format might change in the future, but as of now it is a closed everything exam. No notes, no internet, no calculator (other than 4 function calculator by HonorLock). A full room scan is required, but mirrors are not needed during the exam. Ensure to read the Exam policy document of your semester for exact details.

# Learning outcome and applications
This course is a very good introduction to robot motion. It starts off by localization, followed by path planning, and finally motion model. SLAM integrates all the parts together and the projects helped deeper reasoning into how things work in real world. The consistent example of an autonomous vehicle kept the learning on track! The hardware project, though it contributed very little credits, was a fun way to break from the shackles of the screen, and interact with the real world.
