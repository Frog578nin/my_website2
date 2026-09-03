---
title: 'What do scientists actually program in?'
summary: Python, R, Julia, and the Fortran code that refuses to die. A first-year map of scientific programming.
date: 2026-08-27
authors:
  - me
tags:
  - Python
  - Scientific computing
---

When I picked applied informatics, I assumed scientific programming meant "Python, probably". Half right. Here's the map as I understand it now, after some digging for this post.

Python is the default. Not because the language itself is fast (it isn't), but because of the libraries around it: NumPy for arrays, SciPy for numerical methods, pandas for data tables, Matplotlib for plots. The trick is that these libraries are written in C and Fortran underneath, so Python is mostly a friendly steering wheel on top of fast machinery. This is what we're taught at university, and it's what I write.

R lives next door, in statistics. Biologists, sociologists and economists run their models in it, and its plotting library ggplot2 makes charts that Python users quietly envy. I tried R once and its counting from one instead of zero still feels illegal.

Julia is the young ambitious one. The pitch: write code that looks as simple as Python but runs at near-C speed, without the two-language sandwich. People who use it love it loudly. It's a decade and a half old and still much smaller than Python, which shows how much ecosystems matter compared to language design.

Fortran is the surprise. The language is from 1957, older than my grandparents' TV, and it still runs a serious share of the world's weather forecasts and physics simulations. Partly because it's genuinely good at number crunching, partly because nobody wants to rewrite a million lines of tested code to get identical answers slightly differently. Old code that works is infrastructure, like bridges.

MATLAB deserves a mention: strong in engineering departments, built-in everything, but proprietary and paid, so universities love it and graduates often leave it.

My takeaway as a student: learn Python properly, because it's the common language. Then let the field choose the second one for you. Statistics pulls toward R, heavy simulation toward Julia or C++. And if you ever meet Fortran, be polite. It's older than your professor and will outlive us both.
