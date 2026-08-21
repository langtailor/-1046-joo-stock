---
layout: page
title: 스프린트 1 — 일자별 진행
permalink: /sprint/1/
---

**2026-08-20 (목) ~ 09-02 (수)** · 14일 · 1~2주차

스프린트 목표는 **개발 환경 구축, 제안서 문서 골격**입니다. 스프린트 전체 구성과 칸반 보드는 [4장 1) 단계별 개발 일정]({{ '/schedule/' | relative_url }}#s4-1)을 보십시오.

<!-- TODO: 08-22 이후 행을 진행에 따라 채울 것. 날짜·요일은 계산된 값이므로 수정하지 말 것.
     작성 시점 기준의 사실만 기록하고, 검증하지 않은 완료 처리를 하지 말 것. -->

<div class="daily-wrap" markdown="1">

| 날짜 | 요일 | 수행 내용 | 산출물 · 결과 | 상태 |
| --- | --- | --- | --- | --- |
| 08-20 | 목 | **팀명 · 프로젝트 타이틀 설정**<br>· 개발팀명 `래그테일러` 확정, 팀원 4명 표지 기재<br>· 프로젝트 타이틀 설정 — 표지 제목 · 영문 부제<br>· `_config.yml`의 `title` · `description` · `email` · `url` · `github_username` 설정<br><br>**Jekyll 구조 작업**<br>· rbenv로 Ruby 3.3.12 빌드, Jekyll 4.4.1 · Bundler 4.0.19 설치<br>· `jekyll new`로 사이트 생성, `bundle install` (38 gems)<br>· 표지 · 목차 · 1~5장 페이지 골격 작성, 이전/다음 링크 연결<br>· 개발 로그 permalink 고정 (`/log/:year/:month/:day/:title/`)<br>· `_includes/head.html` 오버라이드 — `noindex` 메타 출력<br>· `_config.yml`의 `exclude`로 `CLAUDE.md` 공개 차단<br>· `/todo/` 미결 항목 페이지 작성 | 제안서 사이트 골격 (9개 페이지)<br>`CLAUDE.md`<br>커밋 4건<br>로컬 미리보기 HTTP 200 | 완료 |
| 08-21 | 금 | **인프라**<br>· AWS 루트 계정으로 로그인 후 IAM 계정 생성, IAM 계정으로 재로그인<br>· RDS 접속 URL(엔드포인트) 생성<br><br>**문서 · 사이트**<br>· 역할 분담 확정 — 테일러 PM / 왓슨 Flutter / 앨리스 파이프라인 / 토마스 에이전트<br>· 4장 1)을 애자일 스크럼으로 재작성 — 스프린트 5회 · 칸반 보드 · 스크럼 운영 규칙<br>· 목차 하위 18개 항목에 앵커 링크 연결<br>· 사업명 정본을 표지 제목으로 확정하고 `_config.yml` · 1장 · `CLAUDE.md` 일치<br>· RFP 하네스 작성 (`.claude/rules/rfp-harness.md`) — 요구사항 11개 분류 체계 · 추적성 규칙 · PMR<br>· **클라이언트 스택 Flutter 확정**, R&R은 4장 2) 배정 유지 — 참고 자료의 Next.js/Vercel · FE-BE 재배정 안은 미채택<br>· **벡터 저장소 Aurora pgvector 확정** — 참고 자료의 OpenSearch/Pinecone 미채택, 별도 벡터 DB 미도입<br>· `fin.ragtailor.com` DNS 사전 생성 조사 — Cloudflare 확인, 소유 확인 TXT 선행 필요 판단<br>· 이 페이지 작성 | 4장 1) · 2) 본문<br>칸반 보드<br>개발 로그 1건 | 진행 중 |
| 08-22 | 토 | *작성 예정* | | 대기 |
| 08-23 | 일 | *작성 예정* | | 대기 |
| 08-24 | 월 | *작성 예정* | | 대기 |
| 08-25 | 화 | *작성 예정* | | 대기 |
| 08-26 | 수 | *작성 예정* | | 대기 |
| 08-27 | 목 | *작성 예정* | | 대기 |
| 08-28 | 금 | *작성 예정* | | 대기 |
| 08-29 | 토 | *작성 예정* | | 대기 |
| 08-30 | 일 | *작성 예정* | | 대기 |
| 08-31 | 월 | *작성 예정* | | 대기 |
| 09-01 | 화 | *작성 예정* | | 대기 |
| 09-02 | 수 | *작성 예정* | | 대기 |

</div>

> 작성 시점 기준의 **사실만** 기록합니다. 검증하지 않은 완료 처리를 하지 마십시오 — 서버가 떴다면 실제 HTTP 응답을 확인한 뒤 기록합니다. 주차 단위 요약은 [개발 로그]({{ '/log/' | relative_url }})에 별도로 남깁니다.

---

[← 4. 개발 일정 및 추진 체계]({{ '/schedule/' | relative_url }}#s4-1) · [목차]({{ '/toc/' | relative_url }}) · [개발 로그]({{ '/log/' | relative_url }})

<style>
/* 일자별 진행 표 — 스프린트 상세 페이지 */
.daily-wrap {
  overflow-x: auto;
  margin: 1.5rem 0;
}
@media (min-width: 60rem) {
  .daily-wrap {
    width: 52rem;
    margin-left: calc((100% - 52rem) / 2);
  }
}
.daily-wrap table {
  min-width: 46rem;
  font-size: 0.82rem;
  line-height: 1.6;
}
.daily-wrap th,
.daily-wrap td {
  vertical-align: top;
  word-break: keep-all;
  padding: 0.5rem 0.6rem;
}
.daily-wrap td:nth-child(1),
.daily-wrap td:nth-child(2),
.daily-wrap td:nth-child(5) {
  white-space: nowrap;
  font-variant-numeric: tabular-nums;
}
.daily-wrap td:nth-child(3) {
  min-width: 22rem;
}
.daily-wrap td:nth-child(4) {
  font-size: 0.78rem;
  opacity: 0.75;
}
</style>
