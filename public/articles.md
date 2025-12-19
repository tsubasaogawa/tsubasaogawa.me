---
permalink: /articles
title: articles
---
## articles

<ul>
  {% for post in site.posts %}
    <li>{{ post.year }}-{{ post.month }}-{{ post.day }} <a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
