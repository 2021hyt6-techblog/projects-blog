---
layout: default
title: Posts
permalink: /posts/
---

{% for post in site.posts %}
  <h1><b>{{ post.title }}</b></h1>
  <h3><u>{{ post.author }}</u></h3>
  <time datetime="{{ page.date | date: "%d %B %Y" }}">{{ post.date | date_to_long_string }}</time>
  <p>{{ post.content }}</p>
  <hr><br>
{% endfor %}

