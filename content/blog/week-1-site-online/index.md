---
title: 'Week one: the site is online'
summary: How I got a Hugo template running on GitHub Pages, and what went wrong along the way.
date: 2026-08-09
authors:
  - me
tags:
  - Weekly notes
  - Hugo
---

This week I had one goal: get an empty version of this site on the internet. It sounded simple. It took three evenings.

The site runs on Hugo, a static site generator, with the Academic CV template. The idea is that I write plain text files, Hugo turns them into HTML, and GitHub Pages hosts the result for free. No servers, no databases, nothing to pay for. Perfect for a student.

The first evening went into installing everything. Hugo itself installs in one command, but the template also wanted Node and pnpm, and my laptop had an old Node version that broke the build with a wall of red text. Updating Node fixed it. I still don't fully understand what Tailwind does in this setup, but the build needs it.

The second evening was about the template itself. I cloned the starter repository, ran the local server and got the demo site of a fictional professor with fake publications. Deleting someone else's fake life from your own website is a strange kind of work.

The third evening: deployment. The repository already had a GitHub Actions workflow, so in theory every push to main rebuilds the site. In practice I spent an hour staring at a blank page because of the base URL. My site lives at a subpath, `/my_website2/`, and until you write that into the config, all styles and links point to the wrong place. The page loaded, but as bare unstyled text, like the internet in 1995.

Once the URL was fixed, everything clicked. Push, wait two minutes, refresh, see the change. That loop feels good.

Next week: filling in the actual content about me, so the site stops being an empty shell with my name on it.
