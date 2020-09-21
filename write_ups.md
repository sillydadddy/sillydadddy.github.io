---
title: Write-ups
permalink: /write-ups/
show_excerpts: true
entries_layout: grid
---


<ul>
  {% for post in site.categories.write-ups %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>