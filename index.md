---
layout: default
title: Home
description: Daniele Zanaga — physicist and data researcher.
---

<div class="home-intro">
  <h1>Daniele Zanaga</h1>
  <p class="lead">Physicist and data researcher.</p>
  <p>
    Welcome to my personal site. I work at VITO on satellite imagery, global land-cover
    mapping, vegetation and biodiversity change, AI, computer vision, and large-scale
    geospatial data.
  </p>
</div>

<section class="latest-post">
  <h2>Latest blog post</h2>
  {% assign latest_post = site.posts | first %}
  {% if latest_post %}
    <p><time datetime="{{ latest_post.date | date: '%Y-%m-%d' }}">{{ latest_post.date | date: "%b %-d, %Y" }}</time></p>
    <h3><a href="{{ latest_post.url | relative_url }}">{{ latest_post.title }}</a></h3>
    <p>{{ latest_post.excerpt | strip_html | truncate: 190 }}</p>
  {% else %}
    <p>No posts yet.</p>
  {% endif %}
</section>

<section class="contact-block">
  <h2>Contact</h2>
  <ul class="contact-list">
    <li><a href="https://www.linkedin.com/in/dzanaga/">LinkedIn</a></li>
    <li><a href="https://x.com/dzanaga_">X</a></li>
    <li><a href="https://github.com/dzanaga">GitHub</a></li>
  </ul>
</section>
