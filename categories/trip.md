---
layout: default
title: trip
permalink: /category/trip/
---

{% assign posts = site.posts | where: "category", "trip" %}

<ul>
  {% for post in posts %}
    <li>
      <a href="{{ post.url | relative_url }}">
        {{ post.title }}
      </a>
      <span>{{ post.date | date: "%Y-%m-%d" }}</span>
    </li>
  {% endfor %}
</ul>