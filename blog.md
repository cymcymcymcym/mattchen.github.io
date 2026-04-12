---
layout: page
title: Blog
permalink: /blog/
---

{% for post in site.posts %}
  <div style="margin-bottom: 20px;">
    <b><a href="{{ post.url }}">{{ post.title }}</a></b>
    <span style="color: #666;">— {{ post.date | date: "%b %d, %Y" }}</span>
  </div>
{% endfor %}

{% if site.posts.size == 0 %}
  <p>Nothing here yet.</p>
{% endif %}
