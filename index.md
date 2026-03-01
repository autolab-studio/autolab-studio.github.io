---
layout: default
title: "자동화 프로그램 개발"
description: "업무 자동화 프로그램 개발 전문. Python 파이썬 기반 웹 크롤링, Selenium 웹 매크로 제작, 엑셀 연동 자동화까지 맞춤 제작합니다."
is_home: true
---

 <div class="card">
  <h2>이런 상황에 계신 분들께 추천 드립니다.</h2>
  <ul>
    <li>엑셀/반복 업무 때문에 시간이 너무 많이 든다</li>
    <li>웹사이트 데이터를 자동으로 수집/정리하고 싶다</li>
    <li>본인만의 매크로 프로그램을 제작하고 싶다</li>
  </ul>
  <div class="badges">
    <span class="badge">Python</span>
    <span class="badge">Selenium</span>
    <span class="badge">Excel 자동화</span>
    <span class="badge">크롤링</span>
    <span class="badge">알림봇</span>
  </div>
</div>

<div class="card">
  <h2>프로그램 리스트</h2>

  <div class="post-grid">
    {% for post in site.posts limit:3 %}
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

  <p class="muted" style="margin-top:10px;">
    <a href="{{ '/blog/' | relative_url }}">블로그 전체 보기 →</a>
  </p>
</div>
