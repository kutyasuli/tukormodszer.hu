---
layout: page
title: Sikertörténetek
underMenu: Sikertörténetek
---

<div>
{% for post in site.posts %}
  {% if post.category == "siker" %}
    <h3><a href="{{ post.url }}">{{ post.title }}</a> <small>({{ post.date | date: "%Y.%m.%d" }})</small></h3>
    <p>{{ post.excerpt | remove: "<p>" | remove: "</p>" }}<br><a href="{{ post.url }}">Tovább...</a></p>
  {% endif %}
{% endfor %}
</div>
