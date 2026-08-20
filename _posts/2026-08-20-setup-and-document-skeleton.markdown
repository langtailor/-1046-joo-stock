---
layout: post
title: "1주차 — 개발 환경 구축 및 문서 골격 작성"
date: 2026-08-20 16:15:00 +0900
categories: 진행사항
---

사업 착수일. 로컬 개발 환경을 구축하고 제안서 사이트의 표지·목차·1장 골격을 작성했습니다.

## 완료

**개발 환경**

- 빌드 의존성 8종 설치 (`libreadline-dev`, `zlib1g-dev`, `autoconf`, `bison`, `libyaml-dev`, `libncurses-dev`, `libffi-dev`, `libgdbm-dev`)
  - Ubuntu 26.04에서 `libncurses5-dev`는 제거되어 `libncurses-dev`로 대체
- rbenv + ruby-build 설치, `~/.bashrc` 초기화 구문 자동 등록
- Ruby **3.3.12** 소스 빌드 및 `rbenv global` 적용
  - 당초 3.3.5 예정이었으나 3.3.x 최신 패치 버전으로 상향. GitHub Pages 빌더와 동일 계열 유지
- Jekyll **4.4.1**, Bundler **4.0.19** 설치

**문서 사이트**

- `jekyll new . --force`로 사이트 생성 (`README.md`·`.git` 보존), `bundle install` 완료 (38 gems)
- 표지 페이지 작성 — 사업명, 개발 기간, 개발팀 4명
- 목차 페이지 작성 — 5장 구성
- 1장 사업 개요 페이지 작성 — minima 기본 About 페이지 교체
- `_config.yml` 정리 — `title`을 사업명으로, `description` 작성, `email`·`url`·`github_username` 실제 값 반영, 미사용 `twitter_username` 제거
- minima 기본 샘플 글 삭제

**운영**

- `CLAUDE.md` 작성 — 도메인 규칙, 배포 전략, 문서 작성 규칙, 진행사항 기록 규칙
- `CLAUDE.md`가 정적 파일로 사이트에 공개되던 문제 확인 후 `_config.yml`의 `exclude`로 차단
- 로컬 미리보기 서버 구동 (`0.0.0.0:4000`)

**검증 결과**

| 경로 | 응답 |
| --- | --- |
| `/` (표지) | HTTP 200 |
| `/toc/` (목차) | HTTP 200 |
| `/about/` (1장 사업 개요) | HTTP 200 |
| `/CLAUDE.md` | HTTP 404 (의도된 차단) |

## 진행 중

- **1장 본문 미확정** — 사업 목적 / 주요 사업 내용 / 기대 효과 3개 항목이 *작성 예정* 상태입니다. 확정 내용을 받는 대로 채웁니다.
- **2~5장 페이지 미생성** — 목차에는 정의되어 있으나 실제 페이지는 아직 없습니다.
- **배포 미착수** — 현재 로컬 미리보기만 동작합니다. 데모 도메인(`fin.ragtaylor.com`) 배포는 미설정 상태입니다.

## 다음 작업

- 데모 사이트에 `noindex` 메타 적용 (`_includes/custom-head.html`)
- 프로덕션 도메인(`fin.ragtailor.com`) DNS 레코드 사전 생성 — 전환 시점의 전파 대기를 없애기 위함
- 2~5장 페이지 골격 생성 및 목차 링크 연결
- `/todo/` 미결 항목 페이지 생성
- 생성 파일 git 커밋 (현재 전부 untracked)
- 실제 발주처 확인 후 표기 여부 결정

## 확인 필요

- 1장 본문 3개 항목의 확정 내용
- 실제 발주처 — 목차 양식은 한국소프트웨어진흥원 제안요청서 양식안을 참고한 것이며, 해당 기관은 양식의 출처일 뿐 발주처가 아닙니다. 표지·본문에 임의 표기하지 않은 상태입니다.
