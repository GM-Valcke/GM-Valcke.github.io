---
layout: default
title: Creation log
---

# {{ page.title }}

Welcome,
This page contains updates on the projects I'm working on and would love to share. 
Below you can find a list of projects that are finished (enough) to be ready for adoption. 


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

## Creations ready for adoption

- [Spellwrighters](/spellwrighters)
- [FATE CORE Character sheet templates and examples (.tex and .pdf)](/FATE-CORE-charsheets)


## 3D printing service

[English](/3Dprinting/)
[Nederlands](/3DprintingNL/)

## Contact me

[Contact](/contact/)

