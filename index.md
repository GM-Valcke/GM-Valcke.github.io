---
layout: default
title: My Creations
---

# {{ page.title }}

Welcome — this site hosts blog posts and downloadable files (PDFs, zips, game builds).

## Latest posts

<ul>
  {% for post in site.posts %}
    <li style="margin-bottom: 1.5em;">
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <small>{{ post.date | date: "%B %e, %Y" }}</small><br>

      {% if post.image %}
        <img src="{{ post.image }}" alt="{{ post.title }}" style="max-width:150px; float:left; margin-right:1em;">
      {% endif %}

      <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>

      <div style="clear:both;"></div>
    </li>
  {% endfor %}
</ul>

## Files

Put PDFs and other downloads in the `files/` folder. Example:

- [Character sheet (PDF)](/files/character-sheet.pdf)
