---
layout: default
title: Blog
permalink: /blog/
---

# Blog

Notes on science, data, maps, and related work.

{% for post in site.posts %}
<article class="post-summary">
  <p><time datetime="{{ post.date | date: '%Y-%m-%d' }}">{{ post.date | date: "%b %-d, %Y" }}</time></p>
  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
  <p>{{ post.excerpt | strip_html | truncate: 220 }}</p>
</article>
{% else %}
<p>No posts yet.</p>
{% endfor %}
