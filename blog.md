---
layout: default
title: Blog
permalink: /blog/
---

<div class="ri-section-header" style="margin-bottom: 36px;">
  <span class="ri-section-tag">Writing</span>
  <h2>Blog</h2>
  <p style="color: #85b8d4; font-size: 15px; margin-top: 8px; margin-bottom: 0;">Thoughts, updates, and things worth writing down.</p>
</div>

<div class="blog-posts">
  {% for post in site.posts %}
    <div class="blog-card">
      <div class="blog-card-meta">{{ post.date | date: "%B %-d, %Y" }}</div>
      <h2 class="blog-card-title">
        <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
      {% if post.excerpt %}
      <p class="blog-card-excerpt">{{ post.excerpt | strip_html | truncate: 200 }}</p>
      {% endif %}
      <a class="blog-card-link" href="{{ post.url | prepend: site.baseurl }}">Read more &rarr;</a>
    </div>
  {% endfor %}
</div>
