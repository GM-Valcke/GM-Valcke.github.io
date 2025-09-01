---
layout: default
title: My Creations
---

# {{ page.title }}

Welcome — this site hosts blog posts and downloadable files (PDFs, zips, game builds).

## Latest posts

<ul>
  {% for post in site.posts %}
    <li><a href="{{ post.url }}">{{ post.title }}</a> — {{ post.date | date: "%B %e, %Y" }}</li>
  {% endfor %}
</ul>

## Files

Put PDFs and other downloads in the `files/` folder. Example:

- [Character sheet (PDF)](/files/character-sheet.pdf)
