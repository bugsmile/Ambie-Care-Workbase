---
title: Ambie-Care (Rooted) 지식베이스 인덱스
type: index
last_updated: 2026-04-23
---

# Ambie-Care Workbase — Wiki Index

> **제품:** Rooted — UWB 레이더 기반 비접촉 AI 앰비언트 홈 안전 솔루션  
> **타겟:** B2B 요양시설 · B2G 지자체 · B2C 보호자 가족  
> **핵심 KSF:** 오탐 제로 · Zero-Friction UX · 공간 맥락 Moat · EMR Lock-in

---

## 빠른 참조

| 항목 | 값 |
|-----|---|
| 오탐 현황 (As-Is) | 12회/일/가구 |
| 오탐 목표 (To-Be) | ≤0.3회/월 |
| 핵심 페르소나 | 박지수 (보호자 딸, 38세) |
| B2B 목표 가격 | ₩100k/월/시설 |
| B2C 목표 가격 | ₩30k/월 + 설치비 ₩49k |
| Wave 1 목표 | B2B 5~10개 시설 클로즈드 베타 |
| SOM 최대 세그먼트 | S1 요양시설 ₩26B |
| 규제 포지셔닝 | 라이프케어 스마트홈 기기 (의료기기 아님) |

---

## Sources (원본 분석 요약)

| 파일 | 제목 | 핵심 내용 |
|-----|------|---------|
| [01-porters-forces.md](sources/01-porters-forces.md) | Porter's Five Forces | 대체재 위협 Very High, 구매자 교섭력 High |
| [02-competitive-analysis.md](sources/02-competitive-analysis.md) | 경쟁사 분석 | 케어벨·오파스넷·아카라라이프·유메인·비알랩 5사 비교 |
| [03-value-chain.md](sources/03-value-chain.md) | 케어벨 가치사슬 | Lock-in 구조·Two-Track 전략 벤치마킹 |
| [04-ksfs.md](sources/04-ksfs.md) | KSF Top 5 | 오탐·Moat·Two-Track·EMR·데이터생태계 |
| [05-problem-definition.md](sources/05-problem-definition.md) | 문제 정의 | B2B/B2G/B2C 3관점 + 공통 문제 교차분석 |
| [06-tam-sam-som.md](sources/06-tam-sam-som.md) | 시장 규모 | 글로벌 $329.4B(2034), 국내 168조(2030) |
| [07-persona-spectrum.md](sources/07-persona-spectrum.md) | 페르소나 스펙트럼 | 핵심·인접·극단·비사용자 4유형 |
| [08-customer-journey-map.md](sources/08-customer-journey-map.md) | 고객 여정 지도 | P1~P5 페인포인트, P4=최대 위기(알람피로) |
| [09-aos-dos.md](sources/09-aos-dos.md) | AOS/DOS 분석 | 12 페르소나 전원 Q1, 4단계 개발 로드맵 |
| [10-jtbd-interview.md](sources/10-jtbd-interview.md) | JTBD 인터뷰 | 현재·이탈·비사용자 3그룹, MVP = 알람피로 제거 |
| [11-vps.md](sources/11-vps.md) | Value Proposition Sheet | MVP 필수기능, Not-To-Do, GTM Wave 전략 |
| [12-prd.md](sources/12-prd.md) | PRD v0.3 | FR·NFR·리스크·DB 스키마 전체 |
| [13-srs-v03.md](sources/13-srs-v03.md) | SRS v3.0 (바이브 코딩 MVP) | Next.js+Prisma+Supabase 스택, 무료 티어 제약, 4개 핵심 결정 |

---

## Entities (핵심 주체)

### 페르소나

| 파일 | 이름 | 유형 | 핵심 특징 |
|-----|------|------|---------|
| [persona-park-jisu.md](entities/persona-park-jisu.md) | 박지수 | 핵심 페르소나 | 38세 보호자 딸, 원거리 독거 어머니 케어 |
| [persona-jeong-minseok.md](entities/persona-jeong-minseok.md) | 정민석 | 인접 페르소나 | 43세 지자체 복지과장, B2G 구매결정자 |
| [persona-jang-younghee.md](entities/persona-jang-younghee.md) | 장영희 | 극단 페르소나 | 새벽 데이터 공백 → 소송 피해 가족 |
| [persona-go-taesik.md](entities/persona-go-taesik.md) | 고태식 | 비사용자 페르소나 | 72세 어르신, "환자 취급" 거부 → 전환 조건 |

### 경쟁사

| 파일 | 회사 | 포지션 | 차별 포인트 |
|-----|------|--------|-----------|
| [company-carebell.md](entities/company-carebell.md) | 케어벨 | B2B 프리미엄 선두 | UWB + Lock-in, Rooted의 주요 벤치마킹 대상 |
| [company-opasnet.md](entities/company-opasnet.md) | 오파스넷 | B2G 공공 선두 | IR-UWB 고성능, 관제 특화 |
| [company-aqaralife.md](entities/company-aqaralife.md) | 아카라라이프 | AIoT 스마트홈 | 생태계형, PRD Won't 결정 대상 |
| [company-umain.md](entities/company-umain.md) | 유메인 | UWB 칩셋 원천 | 독자 SoC 설계, R-03 공급망 참조 |
| [company-brlab.md](entities/company-brlab.md) | 비알랩 | 수면 분석 특화 | 스마트 매트리스, 화장실 동선 부재 |

---

## Concepts (핵심 개념)

| 파일 | 개념 | 한줄 요약 |
|-----|------|---------|
| [false-alarm.md](concepts/false-alarm.md) | 오탐률 | KSF #1 — 12회/일 → 0.3회/월, 신뢰 붕괴의 핵심 |
| [zero-friction.md](concepts/zero-friction.md) | Zero-Friction UX | 착용·충전·조작 없이 작동, B2C 수용성 극대화 |
| [uwb-radar.md](concepts/uwb-radar.md) | UWB 레이더 | 비영상 비접촉 센싱, 공간 분석의 기술 기반 |
| [ambient-care.md](concepts/ambient-care.md) | 앰비언트 케어 | 공간 자체가 돌보는 방식, 웨어러블과의 근본 차이 |
| [space-context-moat.md](concepts/space-context-moat.md) | 공간 맥락 Moat | 화장실 체류시간 등 웨어러블 불가 데이터 → 해자 |
| [emr-integration.md](concepts/emr-integration.md) | EMR 연동 | Webhook 자동 연동 → 이중 기록 제거 + B2B Lock-in |
| [daily-report.md](concepts/daily-report.md) | 데일리 리포트 | 아침 7:30 보호자 보고, B2C 잔존율 방어 루틴 |
| [two-track-lineup.md](concepts/two-track-lineup.md) | Two-Track 라인업 | B2G 보급형 + B2B 프리미엄 동시 공략 전략 |

---

## 미처리 소스

없음 — 모든 원시 소스 처리 완료 ✅

---

## 운영 로그

→ [log.md](log.md) 참조

---

## 핵심 관계도

```
[UWB 레이더]
    └─→ [앰비언트 케어]
            ├─→ [Zero-Friction] ─→ [고태식 전환]
            ├─→ [공간 맥락 Moat] ─→ [웨어러블 방어]
            └─→ [오탐률] ─→ [박지수 신뢰 형성]
                              └─→ [데일리 리포트] ─→ [잔존율]

[EMR 연동] ─→ [B2B Lock-in] ─→ [케어벨 벤치마킹]

[Two-Track 라인업]
    ├─→ Track A: [정민석] → B2G 조달
    └─→ Track B: [요양시설] → B2B 프리미엄
```
