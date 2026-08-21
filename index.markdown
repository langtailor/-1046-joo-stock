---
layout: default
title: 표지
---

<div class="cover">

  <p class="cover-doctype">개발 제안서</p>

  <h1 class="cover-title">
    금융 공시(DART/SEC) 복합 문서 구조화 및 <br /> Hybrid RAG pipeline 구축 <br />(Latency -40%, Recall@5 92% 달성)
  
  </h1>

  <p class="cover-subtitle">National Financial Data Media Automation<br />and Next-Generation Public Service Platform</p>

  <hr class="cover-rule" />

  <dl class="cover-meta">
    <dt>개발 기간</dt>
    <dd>2026년 8월 20일 (목) ~ 2026년 10월 27일 (화)<br /><span class="cover-note">총 69일 / 약 10주</span></dd>

    <dt>개발팀 : 래그테일러 </dt>
    <dd>테일러 · 왓슨 · 앨리스 · 토마스<br /><span class="cover-note">4명</span></dd>

    <dt>문서 작성일</dt>
    <dd>2026년 8월 20일</dd>

    <dt>깃허브 주소</dt>
    <dd><a href="https://github.com/ragtailor/fin.ragtaylor.com">https://github.com/ragtailor/fin.ragtaylor.com</a></dd>

    <dt>데모 사이트</dt>
    <dd><a href="https://fin.ragtaylor.com">https://fin.ragtaylor.com</a></dd>
  </dl>

  <p class="cover-next"><a href="{{ '/toc/' | relative_url }}">목차 &rarr;</a></p>

</div>

<style>
.cover {
  max-width: 46rem;
  margin: 3rem auto 4rem;
  text-align: center;
}
.cover-doctype {
  font-size: 0.95rem;
  letter-spacing: 0.35em;
  text-transform: uppercase;
  opacity: 0.65;
  margin-bottom: 2.5rem;
}
.cover-title {
  font-size: clamp(1.6rem, 4.5vw, 2.6rem);
  line-height: 1.45;
  font-weight: 700;
  margin: 0 0 1.25rem;
  word-break: keep-all;
}
.cover-subtitle {
  font-size: 0.95rem;
  line-height: 1.7;
  opacity: 0.6;
  margin-bottom: 3rem;
}
.cover-rule {
  width: 4rem;
  margin: 0 auto 3rem;
  border: 0;
  border-top: 2px solid currentColor;
  opacity: 0.3;
}
.cover-meta {
  display: grid;
  grid-template-columns: auto 1fr;
  gap: 1.1rem 2rem;
  max-width: 32rem;
  margin: 0 auto;
  text-align: left;
}
.cover-meta dt {
  font-weight: 600;
  white-space: nowrap;
  opacity: 0.7;
}
.cover-meta dd {
  margin: 0;
  line-height: 1.6;
}
.cover-note {
  font-size: 0.85rem;
  opacity: 0.55;
}
.cover-next {
  margin-top: 3.5rem;
  font-size: 1.05rem;
}

@media (max-width: 30rem) {
  .cover-meta {
    grid-template-columns: 1fr;
    gap: 0.35rem 0;
  }
  .cover-meta dd { margin-bottom: 1rem; }
}
</style>
