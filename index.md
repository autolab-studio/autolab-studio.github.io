---
layout: default
title: "자동화 프로그램 제작"
description: "업무 자동화 프로그램 개발 전문. Python 파이썬 기반 웹 크롤링, Selenium 웹 매크로 제작, 엑셀 연동 자동화까지 맞춤 제작합니다."
is_home: true
---

<div class="card">
  <h1 style="margin-top:0;">업무 자동화 프로그램 제작</h1>

  <p style="font-size:18px; line-height:1.6;">
    반복적인 업무를 자동화하여 시간을 절약하세요.<br>
    Python 기반 <b>웹 자동화 · 데이터 수집 · 매크로 프로그램</b>을 맞춤 제작합니다.
  </p>

  <div class="badges" style="margin-top:12px;">
    <span class="badge">Python 자동화</span>
    <span class="badge">웹 크롤링</span>
    <span class="badge">Selenium 매크로</span>
    <span class="badge">Excel 자동화</span>
    <span class="badge">알림봇</span>
  </div>
</div>

<div class="card">
  <h2>이런 상황에 계신 분들께 추천 드립니다</h2>

  <ul>
    <li>엑셀/반복 업무 때문에 시간이 너무 많이 든다</li>
    <li>웹사이트 데이터를 자동으로 수집/정리하고 싶다</li>
    <li>본인만의 매크로 프로그램을 제작하고 싶다</li>
    <li>업무 자동화를 통해 시간을 절약하고 싶다</li>
  </ul>
</div>

<div class="card">
  <h2>기본 견적 안내</h2>

  <ul>
    <li><b>간단한 단산 처리 프로그램</b> : 5만원~</li>
    <li><b>엑셀 연동 프로그램</b> : 10만원~</li>
    <li><b>크롤링 및 웹 연동 자동화 프로그램</b> : 15만원~</li>
  </ul>

  <p class="muted">
    ※ 작업 범위, 난이도, 예외 처리, 계정 수, 데이터 양에 따라 견적은 달라질 수 있습니다.
  </p>
</div>

<div class="card">
  <h2>개발자 소개</h2>

  <ul>
    <li><b>학력</b>: 건국대학교 서울캠퍼스 컴퓨터공학과 (학사 · 석사 졸업)</li>
    <li><b>경력</b>: 앱 개발 경력 <b>4년 이상</b></li>
    <li><b>자동화 프로그램 개발 경험 다수</b></li>
    <li><b>크몽</b>: 작업 <b>50회+</b>, 만족도 <b>100%</b></li>
  </ul>

  <p class="muted">
    단순한 기능 구현이 아니라, 실제 업무 흐름을 이해하고 시간을 절약할 수 있는 실용적인 자동화 솔루션을 만드는 것을 목표로 합니다.
  </p>
</div>

<div class="card">
  <h2>프로그램 제작 사례</h2>

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
    <a href="{{ '/blog/' | relative_url }}">프로그램 제작 사례 더보기 →</a>
  </p>
</div>