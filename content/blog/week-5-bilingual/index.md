---
title: 'Week five: the site speaks Russian now'
summary: Adding a second language to a Hugo site, and a short look back at the month.
date: 2026-09-01
authors:
  - me
tags:
  - Weekly notes
  - Hugo
---

Final week of the project, and the biggest single change: the site is now bilingual. There's a language switcher in the header, and every page exists in English and Russian.

Hugo's multilingual support is built in, which I didn't expect from a "simple" static site generator. You declare a second language in the config, and then each content file gets a translated twin: `index.md` for English, `index.ru.md` for Russian, side by side in the same folder. Hugo pairs them up, builds two versions of the site and links them together, so the switcher on any page takes you to the same page in the other language, not to the other homepage.

The mechanics took an evening. The translations took the rest of the week. Translating your own writing is a strange exercise: you know exactly what the author meant, and you still catch yourself arguing with him. Some jokes refuse to move between languages. A few sentences I just rewrote from scratch, because a literal translation read like furniture assembly instructions.

Menu labels, section titles and interface strings needed their own pass. The template ships with translations for standard interface text, so buttons and dates localized themselves. My own strings, like the menu items, I listed per language in the config.

Since this is the last weekly note, a quick tally of the month. The site went from an empty template to: a filled CV with education, skills and experience, links to seven research profiles, two project pages, ten posts and two languages. Along the way I properly learned Git basics, Markdown, a bit of YAML, and more about broken relative links than I ever planned.

The real lesson is quieter, though. A website is never finished, but it can be alive: small regular updates beat heroic rewrites. One post a week filled a blog. The same trick probably works for studying, and that's the habit I'm taking away from this project.
