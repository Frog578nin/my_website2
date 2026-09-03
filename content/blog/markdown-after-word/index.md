---
title: 'Markdown after years of Word'
summary: A markup language you can learn in ten minutes, and why every post on this site is written in it.
date: 2026-08-13
authors:
  - me
tags:
  - Markdown
  - Tools
---

Every post on this site is a plain text file. This one is called `index.md`, and the `md` stands for Markdown, a lightweight markup language. "Lightweight" is the honest part of the name: the whole syntax fits on one page and you can learn most of it in ten minutes.

The idea is that you mark up text with characters that already look like what they mean. Asterisks around a word make it **bold**. A `#` at the start of a line makes a heading. A dash makes a list item. A pair of square brackets and parentheses make a link. The raw file stays readable even before it's converted to HTML, which is the point: Markdown was designed so the source looks like an email a human would write.

For comparison, the same emphasis in HTML is `<strong>bold</strong>`, and in LaTeX it's `\textbf{bold}`. Both are more powerful. Both are also more typing for the everyday case of "I just want some notes with headings".

What surprised me is how many places speak Markdown once you start noticing. GitHub renders README files with it. Jupyter notebooks use it for text cells. Telegram and Discord understand pieces of it. Hugo, which builds this site, takes my `.md` files and turns them into pages. So one small skill keeps paying off in tools I already use.

After years of school essays in Word, the difference in feel is big. Word mixes what you write with how it looks, and the how constantly interrupts: fonts jump, lists misbehave, one pasted fragment ruins the formatting of a whole page. In Markdown the file is just text. Styling is someone else's job, in my case the site template's. I write, it looks fine, we don't argue.

Markdown has limits. Tables are clumsy. Anything with precise layout, like a lab report with numbered formulas, wants LaTeX instead, and that's a topic for a separate post. But for notes, posts and documentation it hits a sweet spot: almost no effort, almost no way to mess it up.
