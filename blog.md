---
layout: default
title: Blog
permalink: /blog/
---

<div class="blog-header">
  <h1>Blog</h1>
  <p class="blog-description">Thoughts, updates, and things worth writing down.</p>
</div>

<ul class="post-list">
  {% for post in site.posts %}
    <li class="post-item">
      <span class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</span>
      <h2 class="post-item-title">
        <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
      {% if post.excerpt %}
      <p class="post-excerpt">{{ post.excerpt | strip_html | truncate: 160 }}</p>
      {% endif %}
      <a class="post-read-more" href="{{ post.url | prepend: site.baseurl }}">Read more &rarr;</a>
    </li>
  {% endfor %}
</ul>
