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
      title: 'Об этом сайте'
      subtitle: ''
      text: |-
        Я собрал этот сайт в рамках учебного проекта по веб-технологиям на
        первом курсе. Он работает на Hugo и живёт на GitHub Pages.

        В блоге два типа записей: короткие еженедельные заметки о том, чем я
        занимался, и тексты подлиннее об инструментах вроде Git и Markdown.
        Всё есть на русском и английском.
    design:
      columns: '1'
  - block: collection
    id: news
    content:
      title: Свежие посты
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
