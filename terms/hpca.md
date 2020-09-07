---
title: "CS-6290 HPCA"
description: "High Performance Computer Architecture"
layout: term
term: "fall-2020"
permalink: "hpca"
---

{% assign term = site.data.terms | where_exp: "term", "page.url contains term.url" | first %}

# Recommended Prerequisites
While computer architecture and C++ are listed as basic prerequisites, having even basic fundamental knowledge is enough to get started. Most of the things required can be picked up during the course. One important thing is to be active on Piazza. From projects to quiz, there are couple of errata, and missing Piazza will be a nightmare. Also, the office hours are not recorded, so need to plan to attend if you are interested. The atmosphere is like a small classroom with a few people and Professor patiently explains and clarifies doubts.

# Project 0 <small>September 7, 2020</small>
Having two monitors or a printout of the instruction will help. You'll need to go through the project document and one or more Piazza posts regarding the same to understand the requirements and avoid confusion. It is not difficult, but definitely draining. You'll need to work on the provided VM, and it is based on Ubuntu 12, so no VS Code (I was heart broken when I discovered it after struggling to set it up for 2 hours). The default RAM, and CPU is less, and can be increased, and network can be enabled as well, but it is highly recommended to not upgrade the Ubuntu (because no one wants to risk getting different results than the one that will be tested upon), or C++ and accompanying libraries. Installing additional software is generally considered safe.