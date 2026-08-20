---
layout: page
title: 개발 로그
permalink: /log/
---

개발 기간 **2026년 8월 20일 ~ 10월 27일** 중의 진행사항 기록입니다.

<ul class="log-list">
{% for post in site.posts %}
  <li class="log-item">
    <time class="log-date" datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y-%m-%d" }}</time>
    <a class="log-title" href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>

{% if site.posts.size == 0 %}
*아직 작성된 기록이 없습니다.*
{% endif %}

<style>
.log-list {
  list-style: none;
  margin: 2rem 0 0;
  padding: 0;
}
.log-item {
  display: flex;
  gap: 1.25rem;
  align-items: baseline;
  padding: 0.7rem 0;
  border-bottom: 1px solid rgba(128, 128, 128, 0.25);
}
.log-date {
  flex: none;
  font-variant-numeric: tabular-nums;
  opacity: 0.6;
  font-size: 0.9rem;
}
.log-title {
  line-height: 1.5;
  word-break: keep-all;
}

@media (max-width: 30rem) {
  .log-item {
    flex-direction: column;
    gap: 0.2rem;
  }
}
</style>
