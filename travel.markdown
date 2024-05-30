---
layout: page
title: travel
permalink: /travel/
---

{% for post in site.posts %}
  <h3> <a href="{{ post.url | relative_url }}">{{ post.title }}</a> </h3>
  {{ post.excerpt }}
{% endfor %}
