---
layout: default
title: "블로그"
description: "자동화 제작 사례와 팁"
---

<div class="card">
  <h2>최근 글</h2>
  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <span class="post-meta"> — {{ post.date | date: "%Y-%m-%d" }}</span>
      </li>
    {% endfor %}
  </ul>
</div>
