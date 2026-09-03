---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2026-09-03
type: landing

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      background:
        gradient_mesh:
          enable: true
      name:
        size: md
      avatar:
        size: medium
        shape: circle
  - block: markdown
    content:
      title: 'About this site'
      subtitle: ''
      text: |-
        I built this site as part of a first-semester web technologies project.
        It runs on Hugo and lives on GitHub Pages.

        The blog has two kinds of posts: short weekly notes on what I studied,
        and longer write-ups on tools like Git and Markdown.
    design:
      columns: '1'
  - block: collection
    id: news
    content:
      title: Recent posts
      subtitle: ''
      text: ''
      page_type: blog
      count: 10
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      offset: 0
      order: desc
    design:
      view: card
      spacing:
        padding: [0, 0, 0, 0]
---
