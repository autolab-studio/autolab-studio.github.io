---
layout: default
title: "블로그"
description: "자동화 프로그램 제작 사례와 정보"
---

<div class="card">
  <h2>블로그 전체보기</h2>
  <div class="blog-gallery">
    {% for post in site.posts %}
      <a class="blog-card" href="{{ post.url | relative_url }}">
        <div class="blog-thumb">
          {% if post.thumbnail %}
            <img src="{{ post.thumbnail | relative_url }}" alt="{{ post.title }}">
          {% else %}
            <img src="{{ '/assets/image/blog/default-thumb.png' | relative_url }}" alt="{{ post.title }}">
          {% endif %}
        </div>
        <div class="blog-card-body">
          <div class="blog-card-title">{{ post.title }}</div>
          <div class="blog-card-date">{{ post.date | date: "%Y-%m-%d" }}</div>
        </div>
      </a>
    {% endfor %}
  </div>
</div>