---
layout: page
title: 4. 개발 일정 및 추진 체계
permalink: /schedule/
---

## 1) 단계별 개발 일정 {#s4-1}

전체 기간 **2026년 8월 20일 (목) ~ 10월 27일 (화)**, 총 69일 / 10주.

개발은 **애자일 스크럼** 방식으로 진행하며, **2주 단위 스프린트 5회**로 나눕니다. 진행 상황은 아래 칸반 보드로 관리합니다.

### 칸반 보드 {#kanban}

**스프린트 1** 기준입니다 (2026-08-21 현재). 전체 스프린트 구성은 아래 [스프린트 일정](#sprint-plan)을 보십시오.

<div class="kanban-wrap">
<div class="kanban">

  <div class="kb-head">백로그</div>
  <div class="kb-head">할 일</div>
  <div class="kb-head">진행 중</div>
  <div class="kb-head">리뷰</div>
  <div class="kb-head">완료</div>

  <div class="kb-lane">테일러 <span>PM</span></div>
  <div class="kb-cell">
    <div class="kb-card is-blocked">실제 발주처 확인<em>사용자 확인 대기</em></div>
  </div>
  <div class="kb-cell">
    <div class="kb-card">1~5장 본문 확정 취합<em>2장 기능마다 필수/선택 부여</em></div>
  </div>
  <div class="kb-cell">
    <div class="kb-card">GitHub 도메인 소유 확인<em>TXT 레코드 발급 대기</em></div>
    <div class="kb-card">DNS 레코드 사전 생성<em>소유 확인 후 CNAME</em></div>
  </div>
  <div class="kb-cell"></div>
  <div class="kb-cell">
    <div class="kb-card is-done">제안서 사이트 골격 · 목차</div>
    <div class="kb-card is-done">배포 방식 결정<em>로컬 미리보기 전용</em></div>
    <div class="kb-card is-done">미결 항목 페이지 일원화</div>
  </div>

  <div class="kb-lane">왓슨 <span>Flutter 클라이언트</span></div>
  <div class="kb-cell">
    <div class="kb-card is-blocked">클라이언트 요구 사항 확정<em>2장 5) 대민 서비스 기능 대기</em></div>
  </div>
  <div class="kb-cell"><div class="kb-card is-pending">작성 예정</div></div>
  <div class="kb-cell"></div>
  <div class="kb-cell"></div>
  <div class="kb-cell"></div>

  <div class="kb-lane">앨리스 <span>데이터 파이프라인</span></div>
  <div class="kb-cell">
    <div class="kb-card is-blocked">수집 · 연계 요구 사항 확정<em>2장 3) 4) 대기</em></div>
  </div>
  <div class="kb-cell"><div class="kb-card is-pending">작성 예정</div></div>
  <div class="kb-cell"></div>
  <div class="kb-cell"></div>
  <div class="kb-cell"></div>

  <div class="kb-lane">토마스 <span>에이전트</span></div>
  <div class="kb-cell">
    <div class="kb-card is-blocked">에이전트 요구 사항 확정<em>2장 6) 아키텍처 대기</em></div>
  </div>
  <div class="kb-cell"><div class="kb-card is-pending">작성 예정</div></div>
  <div class="kb-cell"></div>
  <div class="kb-cell"></div>
  <div class="kb-cell"></div>

  <div class="kb-lane">공통 <span>환경 · 운영</span></div>
  <div class="kb-cell"></div>
  <div class="kb-cell"></div>
  <div class="kb-cell">
    <div class="kb-card">AWS 환경 구성<em>IAM 계정 전환 · RDS 접속 URL</em></div>
  </div>
  <div class="kb-cell"></div>
  <div class="kb-cell">
    <div class="kb-card is-done">개발 환경 구축<em>Ruby 3.3.12 · Jekyll 4.4.1</em></div>
  </div>

</div>
</div>

<p class="kb-legend">
  <span class="kb-key is-done"></span> 완료
  <span class="kb-key"></span> 진행 가능
  <span class="kb-key is-blocked"></span> 선행 확인 대기
  <span class="kb-key is-pending"></span> 미배정
</p>

> 왓슨 · 앨리스 · 토마스 세 레인이 백로그에서 막혀 있습니다. 우선순위 기준(필수/선택 2단계)은 확정되었으나 **2장 요구 사항 본문이 아직 없어** 등급을 매길 대상 자체가 없는 상태입니다. **10주 일정에서 이 대기가 길어질수록 후반 스프린트가 압축됩니다.** 일정상 가장 먼저 풀어야 할 항목입니다.

### 스프린트 일정 {#sprint-plan}

스프린트 경계는 착수일 기준 14일 단위이며, 기존 주차 구분(7일 단위)과 정확히 맞물립니다. 마지막 스프린트만 13일입니다.

<!-- TODO: 스프린트 목표 열을 확정 내용으로 채울 것. 기간·일수·주차는 계산된 값이므로 수정하지 말 것. -->

| 스프린트 | 기간 | 일수 | 주차 | 스프린트 목표 |
| --- | --- | --- | --- | --- |
| [스프린트 1]({{ '/sprint/1/' | relative_url }}) | 2026-08-20 (목) ~ 09-02 (수) | 14 | 1~2주차 | 개발 환경 구축, 제안서 문서 골격 |
| 스프린트 2 | 2026-09-03 (목) ~ 09-16 (수) | 14 | 3~4주차 | *작성 예정* |
| 스프린트 3 | 2026-09-17 (목) ~ 09-30 (수) | 14 | 5~6주차 | *작성 예정* |
| 스프린트 4 | 2026-10-01 (목) ~ 10-14 (수) | 14 | 7~8주차 | *작성 예정* |
| 스프린트 5 | 2026-10-15 (목) ~ 10-27 (화) | 13 | 9~10주차 | *작성 예정* |

스프린트 2 이후의 목표는 [2장 개발 요구 사항]({{ '/requirements/' | relative_url }})이 확정된 뒤 배정합니다. 확정 전에 임의로 채우지 마십시오. 우선순위 기준은 **필수/선택 2단계**로 확정되었으므로(2장 5)), 배정할 때 **필수 항목을 앞 스프린트에 먼저 배치**합니다.

### 스크럼 운영 규칙 {#scrum-rules}

<!-- TODO: 회의 시각·도구는 확정 후 기입. 주기는 스프린트 구조상 확정값. -->

| 활동 | 주기 | 참여 | 산출물 |
| --- | --- | --- | --- |
| 스프린트 계획 | 스프린트 첫날 | 전원 | 스프린트 백로그 |
| 데일리 스크럼 | 매일 (시각 *미정*) | 전원 | 칸반 보드 갱신 |
| 스프린트 리뷰 | 스프린트 마지막 날 | 전원 | 데모 · 산출물 |
| 회고 | 스프린트 리뷰 직후 | 전원 | 개선 항목 |

- 백로그 우선순위 결정과 카드 배정은 **테일러(PM)**가 담당합니다.
- 카드는 `백로그 → 할 일 → 진행 중 → 리뷰 → 완료` 순으로만 이동합니다.
- **완료 처리는 검증한 뒤에만** 합니다. 실행 결과·응답 코드 등 확인 가능한 근거를 남기십시오.

> 실제 진행 상황은 [개발 로그]({{ '/log/' | relative_url }})에 기록합니다. 계획과 실적이 어긋나면 이 표가 아니라 개발 로그에 사유를 남기고, 표는 확정된 계획만 유지합니다.

## 2) 조직 구성 및 역할 분담 {#s4-2}

개발 인원 4명. 역할은 확정되었습니다.

<!-- TODO: 2장 요구 사항 7개 항목과의 대응(담당 영역 세부)은 요구 사항 확정 후 배정할 것. 이름·역할은 확정값이므로 수정하지 말 것. -->

| 이름 | 역할 | 담당 영역 | 비고 |
| --- | --- | --- | --- |
| 테일러 | PM | 일정 · 범위 관리, 스프린트 운영, 백로그 우선순위 결정, 산출물 검토 | 대외 커뮤니케이션 겸임 |
| 왓슨 | 앱 개발 | Flutter 기반 대민 서비스 클라이언트 | |
| 앨리스 | 파이프라인 개발 | 금융데이터 수집 · 연계 및 처리 파이프라인 | |
| 토마스 | 에이전트 개발 | 에이전트 설계 및 구현 | |

각 담당 영역과 [2장 개발 요구 사항]({{ '/requirements/' | relative_url }}) 7개 항목의 대응 관계는 요구 사항이 확정된 뒤 배정합니다.

> 10주 / 4명은 여유가 큰 편성이 아닙니다. 2장의 기능 우선순위(필수/선택)와 함께 검토해 담당 영역이 겹치거나 비지 않는지 확인하십시오.

## 3) 위험 관리 방안 {#s4-3}

<!-- TODO: 확정 내용으로 교체 -->

| 구분 | 위험 요인 | 영향 | 대응 방안 |
| --- | --- | --- | --- |
| 일정 | *작성 예정* | | |
| 기술 | *작성 예정* | | |
| 데이터 | *작성 예정* | | |
| 인력 | *작성 예정* | | |

---

[← 3. 주요 개발 수행 지침]({{ '/guidelines/' | relative_url }}) · [목차]({{ '/toc/' | relative_url }}) · [5. 부록 →]({{ '/appendix/' | relative_url }})

<style>
/* 칸반 보드 — 4장 1) 단계별 개발 일정 */
.kanban-wrap {
  overflow-x: auto;
  margin: 1.25rem 0 0.75rem;
  padding-bottom: 0.5rem;
}
/* 본문 폭(minima 기본 740px)보다 보드가 넓다. 화면이 넉넉하면 본문 폭을
   넘겨 표시하고, 좁으면 보드만 가로 스크롤한다. */
@media (min-width: 60rem) {
  .kanban-wrap {
    width: 52rem;
    margin-left: calc((100% - 52rem) / 2);
  }
}
.kanban {
  display: grid;
  grid-template-columns: repeat(5, minmax(9.4rem, 1fr));
  gap: 0.4rem;
  min-width: 50rem;
}
.kb-head {
  font-size: 0.78rem;
  font-weight: 700;
  letter-spacing: 0.02em;
  text-align: center;
  padding: 0.4rem 0.3rem;
  border-radius: 3px;
  background: rgba(128, 128, 128, 0.14);
  word-break: keep-all;
}
.kb-lane {
  grid-column: 1 / -1;
  margin-top: 0.7rem;
  padding: 0.35rem 0.1rem 0.3rem;
  font-size: 0.86rem;
  font-weight: 700;
  border-bottom: 1px solid rgba(128, 128, 128, 0.32);
  word-break: keep-all;
}
.kb-lane span {
  font-weight: 400;
  font-size: 0.74rem;
  opacity: 0.6;
  margin-left: 0.4rem;
}
.kb-cell {
  min-height: 2.6rem;
  padding: 0.35rem;
  border-radius: 3px;
  background: rgba(128, 128, 128, 0.05);
  display: flex;
  flex-direction: column;
  gap: 0.35rem;
}
.kb-card {
  background: #fff;
  border: 1px solid rgba(128, 128, 128, 0.3);
  border-left: 3px solid #2a7ae2;
  border-radius: 3px;
  padding: 0.4rem 0.5rem;
  font-size: 0.79rem;
  line-height: 1.45;
  word-break: keep-all;
}
.kb-card em {
  display: block;
  font-style: normal;
  font-size: 0.71rem;
  line-height: 1.4;
  opacity: 0.62;
  margin-top: 0.2rem;
}
.kb-card.is-done {
  border-left-color: #3d9970;
  opacity: 0.72;
}
.kb-card.is-blocked {
  border-left-color: #d64545;
}
.kb-card.is-pending {
  border-left-color: rgba(128, 128, 128, 0.45);
  border-style: dashed;
  font-style: italic;
  opacity: 0.65;
}
.kb-legend {
  font-size: 0.76rem;
  opacity: 0.8;
  margin-top: 0.4rem;
}
.kb-legend .kb-key {
  display: inline-block;
  width: 0.7rem;
  height: 0.7rem;
  border-radius: 2px;
  background: #2a7ae2;
  margin: 0 0.15rem 0 0.9rem;
  vertical-align: baseline;
}
.kb-legend .kb-key:first-child {
  margin-left: 0;
}
.kb-legend .kb-key.is-done {
  background: #3d9970;
}
.kb-legend .kb-key.is-blocked {
  background: #d64545;
}
.kb-legend .kb-key.is-pending {
  background: rgba(128, 128, 128, 0.45);
}
</style>
