---
title: Blog
layout: page
permalink: /blog/
icon: fas fa-pen-nib
order: 4
---

<div id="post-list">
  {% for post in site.posts %}
    <article class="post-item">
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p class="post-meta">{{ post.date | date: "%b %d, %Y" }}</p>
      <p>{{ post.excerpt }}</p>
    </article>
  {% endfor %}
</div>
