---
title: 'Why a static site generator was the right call'
summary: No database, no admin panel, no hosting bill. How Hugo and its relatives work, and when they make sense.
date: 2026-09-01
authors:
  - me
tags:
  - Hugo
  - Web
---

A month of running this site on Hugo seems like enough experience to explain what static site generators are and why I'd recommend one for a personal page.

A classic website, say on WordPress, assembles every page at the moment you request it. A program on the server takes your request, reads content from a database, wraps it in a template and sends back HTML. This is flexible, and this is also why such sites need hosting with PHP and a database, updates, and a login page that bots poke at all day.

A static site generator moves all that work to my laptop. Hugo takes a folder of Markdown files and templates and produces plain HTML files, once, at build time. The server then has one job: hand out ready files. There's nothing to hack into, nothing to update on the server, and hosting static files is so cheap that GitHub does it for free.

The workflow ends up looking like programming, which I like. Content lives in a Git repository. I write a post, commit, push, and GitHub Actions rebuilds the site automatically. The entire "admin panel" is my text editor.

Hugo isn't alone. Jekyll is the veteran that made the approach popular, and GitHub Pages understands it natively. Eleventy is the minimalist JavaScript option. Astro is the fashionable newcomer. I picked Hugo for two reasons: it builds sites in milliseconds, and its academic template already had every section a student CV needs. Reason two did most of the deciding, honestly.

The trade-offs are real. No comments, no forms, no user accounts, unless you glue on external services. Every change requires a rebuild, so it's not a platform for a live shop. And the initial setup assumes you're comfortable with a terminal and Git, which filters out a lot of people.

But the shape of the deal is exactly right for a personal academic site: content that changes weekly, readers who only read, and a budget of zero. Static wins that case outright.
