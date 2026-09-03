---
title: Personal academic website
summary: This site. Hugo, the Academic CV template, GitHub Pages and a build that runs itself.
date: 2026-08-31
tags:
  - Hugo
  - Web
links:
  - icon: brands/github
    url: https://github.com/Frog578nin/my_website2
    label: Source code
---

The site you're reading is itself a study project for a web technologies course. The task: build a personal academic site with a CV, blog and research profile links, and publish it properly.

It's built with Hugo, a static site generator, on the Academic CV template. All content is Markdown and YAML files in a public GitHub repository. On every push, GitHub Actions rebuilds the site and deploys it to GitHub Pages, so publishing a post is one `git push` and no manual uploads.

What I learned building it: Git beyond the basics, Markdown, YAML configs and their unforgiving indentation, how GitHub Actions pipelines work, and how multilingual routing works in Hugo, since the whole site exists in English and Russian.
