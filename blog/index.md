---
layout: default
title: "블로그"
description: "자동화 프로그램 제작 사례와 정보"
---

<div class="card">
  <h2>프로그램 제작 사례</h2>

  <div class="post-grid">
    {% for post in site.posts %}
      <a class="post-card" href="{{ post.url | relative_url }}">
        <div class="post-thumb">
          {% if post.thumbnail %}
            <img src="{{ post.thumbnail | relative_url }}" alt="{{ post.title }}">
          {% else %}
            <div class="post-thumb-fallback">No Image</div>
          {% endif %}
        </div>

        <div class="post-info">
          <div class="post-title">{{ post.title }}</div>
          <div class="post-date">{{ post.date | date: "%Y-%m-%d" }}</div>
        </div>
      </a>
    {% endfor %}
  </div>
</div>