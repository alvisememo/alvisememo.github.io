---
layout: page
title: Posts
addToFooter: yes
---

This is a collection of posts written for reference or to help anyone intrested:

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>