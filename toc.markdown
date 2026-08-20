---
layout: page
title: 목차
permalink: /toc/
---

<div class="toc">

<section class="toc-part">
  <h2><a href="{{ '/about/' | relative_url }}">1. 사업 개요</a></h2>
  <ol class="toc-items">
    <li>사업 목적</li>
    <li>주요 사업 내용</li>
    <li>기대 효과</li>
  </ol>
</section>

<section class="toc-part">
  <h2><a href="{{ '/requirements/' | relative_url }}">2. 개발 요구 사항</a></h2>
  <ol class="toc-items">
    <li>목적</li>
    <li>개발 범위</li>
    <li>금융데이터 수집 및 연계</li>
    <li>미디어 자동화 처리</li>
    <li>대민 서비스 플랫폼 기능</li>
    <li>시스템 아키텍처</li>
    <li>보안 및 개인정보 보호</li>
  </ol>
</section>

<section class="toc-part">
  <h2><a href="{{ '/guidelines/' | relative_url }}">3. 주요 개발 수행 지침</a></h2>
  <ol class="toc-items">
    <li>일반 사항</li>
    <li>개발 표준 및 산출물</li>
    <li>품질 관리 및 테스트</li>
  </ol>
</section>

<section class="toc-part">
  <h2><a href="{{ '/schedule/' | relative_url }}">4. 개발 일정 및 추진 체계</a></h2>
  <ol class="toc-items">
    <li>단계별 개발 일정</li>
    <li>조직 구성 및 역할 분담</li>
    <li>위험 관리 방안</li>
  </ol>
</section>

<section class="toc-part">
  <h2><a href="{{ '/appendix/' | relative_url }}">5. 부록</a></h2>
  <ol class="toc-items">
    <li>용어 정의</li>
    <li>관련 서식</li>
  </ol>
</section>

</div>

<p class="toc-back"><a href="{{ '/' | relative_url }}">&larr; 표지</a></p>

<style>
.toc {
  max-width: 42rem;
  margin: 2rem 0 3rem;
}
.toc-part {
  margin-bottom: 2.25rem;
}
.toc-part h2 {
  font-size: 1.15rem;
  font-weight: 700;
  margin: 0 0 0.75rem;
  padding-bottom: 0.5rem;
  border-bottom: 1px solid currentColor;
  border-bottom-color: rgba(128, 128, 128, 0.35);
}
.toc-items {
  list-style: none;
  margin: 0;
  padding: 0;
  counter-reset: toc-sub;
}
.toc-items li {
  counter-increment: toc-sub;
  padding: 0.3rem 0 0.3rem 2.4rem;
  position: relative;
  line-height: 1.6;
  word-break: keep-all;
}
.toc-items li::before {
  content: counter(toc-sub) ")";
  position: absolute;
  left: 0.6rem;
  opacity: 0.6;
  font-variant-numeric: tabular-nums;
}
.toc-back {
  margin-top: 2.5rem;
}
</style>
