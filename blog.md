---
layout: page
title: Blog
permalink: /blog/
---

<div class="blog-page">
  <h1>Blog</h1>
  <p class="intro">Insights on operations management, process optimization, and industrial analytics</p>

  <div class="posts-list">
    {% for post in site.posts %}
      <article class="post-preview">
        <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
        <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
        <p class="post-excerpt">{{ post.excerpt }}</p>
        <a href="{{ post.url | relative_url }}" class="read-more">Read more →</a>
      </article>
    {% endfor %}
  </div>

  {% if site.posts.size == 0 %}
    <p class="no-posts">No blog posts yet. Check back soon for insights on operations optimization and process control.</p>
  {% endif %}
</div>
