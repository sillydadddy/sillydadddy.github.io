---
title: Write-ups
permalink: /write-ups/
show_excerpts: true
entries_layout: grid
---


<ul>
  {% for post in site.categories.Write_up %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>