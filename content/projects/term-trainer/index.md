---
title: Console flashcard trainer in Python
summary: A small command-line program for memorizing terms and definitions, written to survive my first exams.
date: 2026-06-15
tags:
  - Python
---

A command-line flashcard trainer I wrote in my final school year to prepare for exams, and still use for university terminology.

Cards are stored as a JSON file of question and answer pairs, sorted into decks. The trainer shows a random card, waits for the answer, and moves cards you got wrong into a repeat pile that comes back more often, a simplified version of spaced repetition. Progress is saved between sessions.

It's plain Python with no external dependencies: standard library only, about three hundred lines. Writing it taught me file handling, JSON, and the difference between code that works and code you can read a month later. The first version had a function called `do_stuff2`. The current one doesn't.
