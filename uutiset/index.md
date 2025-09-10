---
layout: default
title: Uutiset
---

# Uutiset

<ul class="wrap">
  {% for post in site.posts %}
    <li style="margin:0 0 12px 0;">
      <a href="{{ post.url }}">{{ post.title }}</a>
      <small> · {{ post.date | date: "%d.%m.%Y" }}</small>
    </li>
  {% endfor %}
</ul>
