# FieryTale Schedule Template

## Purpose

이 문서는 FieryTale의 일정, 마일스톤, 담당자, 리스크, 결정 사항을 한 곳에서 추적하기 위한 템플릿이다.

사람이 직접 편집하기 쉽도록 표와 체크리스트를 중심으로 작성하고, Codex가 다음 작업을 이어받기 쉽도록 아래 섹션 이름은 가능하면 유지한다.

## Editing Rules

- 날짜는 `YYYY-MM-DD` 형식으로 쓴다.
- 일정 단위는 기본적으로 `주차`, `일자`, `마일스톤` 중 하나로 정리한다.
- 완료 여부는 체크박스 또는 `상태` 열로 표시한다.
- 일정 변경이 생기면 기존 내용을 지우기보다 `Change Log`에 이유를 남긴다.
- 막연한 목표보다 확인 가능한 완료 기준을 쓴다.
- 담당자가 미정이면 `TBD`로 적고, 열린 질문에 남긴다.

## Schedule Summary

| Item | Content |
| --- | --- |
| Schedule Name | FieryTale 기획 및 프로토타입 개발 일정 |
| Period | 2026-06-08 ~ 2026-07-22 |
| Owner | TBD |
| Team Size | TBD |
| Main Goal | 6월 25일까지 핵심 기획을 확정하고, 7월 22일까지 플레이 가능한 프로토타입을 개발한다. |
| Current Status | Draft |
| Last Updated | 2026-06-08 |

## Planning Assumptions

현재 일정은 아래 가정을 기준으로 한다.

- 개발 엔진: Unreal Engine
- 초기 목표: 2 vs 2 서버 권한 기반 TPS/AOS 프로토타입
- 전투 시스템: Gameplay Ability System, GAS
- 주요 리스크: 멀티플레이, 서버 권한 전투, GAS, AOS 승패 흐름
- 기획 기간: 2026-06-08 ~ 2026-06-25
- 개발 기간: 2026-06-26 ~ 2026-07-22
- 기획 단계에서는 핵심 플레이 정체성, 매치 규칙, 전장, 캐릭터, GAS 구조, 개발 백로그를 확정한다.
- 개발 단계에서는 한 판이 서버 권한으로 끝까지 진행되는 얇은 프로토타입을 우선 구현한다.
- 최종 아트, 대규모 콘텐츠, 상용 서비스 수준의 완성도는 현재 일정에서 제외한다.

## Phase Overview

| Phase | Period | Main Objective | Exit Criteria |
| --- | --- | --- | --- |
| Phase 1. Planning | 2026-06-08 ~ 2026-06-25 | 프로토타입 구현에 필요한 핵심 기획 확정 | 열린 핵심 쟁점이 결정되고 개발 백로그가 준비됨 |
| Phase 2. Development | 2026-06-26 ~ 2026-07-22 | 서버 권한 기반 2 vs 2 프로토타입 구현 | 테스트 빌드에서 한 판을 시작부터 종료까지 진행 가능 |

## Milestones

| Milestone | Target Date | Owner | Completion Criteria | Status |
| --- | --- | --- | --- | --- |
| M1. Core Design Decision | 2026-06-14 | TBD | 시점, 핵심 플레이 정체성, MVP 포함 범위 확정 | Not Started |
| M2. Match Design Complete | 2026-06-20 | TBD | 매치 규칙, 전장 구조, 역할군, 초기 캐릭터 초안 확정 | Not Started |
| M3. Development Ready | 2026-06-25 | TBD | GAS 전투 규칙, 구현 백로그, 담당자, 테스트 기준 확정 | Not Started |
| M4. Multiplayer Foundation | 2026-07-01 | TBD | 서버 접속, 팀 배정, 스폰, 이동 동기화 확인 | Not Started |
| M5. Combat Prototype | 2026-07-08 | TBD | 서버 권한 공격, 피해, 사망, 리스폰 확인 | Not Started |
| M6. Match Objective | 2026-07-15 | TBD | 구조물 피해, 넥서스 파괴, 승패 판정 확인 | Not Started |
| M7. Final Playtest Build | 2026-07-22 | TBD | 한 판을 시작부터 종료까지 반복 테스트 가능 | Not Started |

상태 값은 `Not Started`, `In Progress`, `Blocked`, `Done`, `Cut` 중 하나를 우선 사용한다.

## Weekly Plan

### Planning Week 1: 2026-06-08 ~ 2026-06-14

목표: 프로토타입의 핵심 플레이 정체성과 MVP 범위를 결정한다.

| Task | Owner | Deliverable | Completion Criteria | Status |
| --- | --- | --- | --- | --- |
| 핵심 플레이 정체성 결정 | TBD | 시점 및 전투 방향 결정 문서 | TPS 유지 또는 시점 전환에 대한 결론이 있음 | Not Started |
| MVP 범위 설정 | TBD | 포함/제외 기능 목록 | 미니언, 성장, 역할군의 MVP 포함 여부가 명확함 | Not Started |
| 목표 플레이 경험 정리 | TBD | 핵심 플레이 루프 | 플레이어가 한 판에서 반복할 행동을 설명할 수 있음 | Not Started |

주요 완료 기준:

- [ ] MVP 시점과 조작 방식을 결정한다.
- [ ] 프로토타입에 포함할 기능과 제외할 기능을 구분한다.
- [ ] 한 판의 목표 플레이 타임 가설을 정한다.

### Planning Week 2: 2026-06-15 ~ 2026-06-21

목표: 매치 규칙, 전장 구조, 캐릭터 설계의 구현 기준을 확정한다.

| Task | Owner | Deliverable | Completion Criteria | Status |
| --- | --- | --- | --- | --- |
| 매치 규칙 설계 | TBD | CoreMatchRules 문서 | 시작, 진행, 사망, 리스폰, 종료 규칙이 있음 | Not Started |
| 전장 구조 설계 | TBD | 2라인 전장 블록아웃 기준 | 스폰, 라인, 구조물, 주요 교전 공간이 정의됨 | Not Started |
| 캐릭터 역할 설계 | TBD | 역할군 및 초기 캐릭터 2종 초안 | 각 캐릭터의 역할과 핵심 능력이 구분됨 | Not Started |

주요 완료 기준:

- [ ] 2 vs 2 매치의 전체 흐름을 문서화한다.
- [ ] 전장 블록아웃에 필요한 배치 기준을 확정한다.
- [ ] 초기 캐릭터 2종의 역할과 전투 방식을 정한다.

### Planning Final: 2026-06-22 ~ 2026-06-25

목표: 개발 착수에 필요한 기술 기획과 백로그를 확정한다.

| Task | Owner | Deliverable | Completion Criteria | Status |
| --- | --- | --- | --- | --- |
| GAS 전투 기획 | TBD | Attribute, Ability, Effect, Tag 초안 | 기본 공격부터 사망까지 필요한 요소가 정의됨 | Not Started |
| 개발 백로그 작성 | TBD | 우선순위 및 담당자 목록 | 모든 P0 작업에 담당자와 완료 기준이 있음 | Not Started |
| 테스트 계획 작성 | TBD | 기능 및 네트워크 테스트 체크리스트 | 주차별 테스트 조건과 기록 방식이 있음 | Not Started |
| 기획 동결 리뷰 | TBD | 개발 착수 승인 목록 | 핵심 열린 질문이 해결되거나 개발 가정으로 명시됨 | Not Started |

주요 완료 기준:

- [ ] 6월 25일 기준 개발 착수 범위를 동결한다.
- [ ] 모든 P0 작업에 담당자와 완료 기준을 지정한다.
- [ ] 미확정 사항은 개발을 막지 않는 가정으로 명시한다.

### Development Week 1: 2026-06-26 ~ 2026-07-01

목표: 프로젝트 골격과 멀티플레이 접속 흐름을 구축한다.

| Track | Owner | Deliverable | Completion Criteria | Status |
| --- | --- | --- | --- | --- |
| Network / Game Rules | TBD | 서버 접속, 팀 배정, 스폰 | 2명 이상이 접속해 서로의 이동을 확인함 | Not Started |
| GAS / Combat | TBD | ASC 및 AttributeSet 골격 | 서버에서 Health 값이 초기화되고 동기화됨 | Not Started |
| Character / Input | TBD | 이동, 카메라, 조준 | 기본 조작이 멀티플레이 환경에서 동작함 | Not Started |
| Map / Level | TBD | 2라인 회색 박스 맵 | 양 팀 스폰과 주요 구조물 위치를 확인할 수 있음 | Not Started |

주요 완료 기준:

- [ ] 서버와 클라이언트 접속 흐름이 동작한다.
- [ ] 팀별 스폰과 캐릭터 이동이 동기화된다.
- [ ] 기본 전투 시스템을 연결할 프로젝트 골격이 준비된다.

### Development Week 2: 2026-07-02 ~ 2026-07-08

목표: 서버 권한 기반 전투 루프를 구현한다.

| Track | Owner | Deliverable | Completion Criteria | Status |
| --- | --- | --- | --- | --- |
| GAS / Combat | TBD | 기본 공격, 피해, 사망 | 플레이어가 상대를 공격해 사망시킬 수 있음 | Not Started |
| Network / Game Rules | TBD | 사망 및 리스폰 흐름 | 서버가 사망을 판정하고 캐릭터를 리스폰함 | Not Started |
| Character / Input | TBD | 전투 입력 및 조준 보정 | 공격 입력과 시각적 방향이 일치함 | Not Started |
| Art / TA | TBD | 임시 무기, 애니메이션, 피격 피드백 | 공격과 피격 여부를 플레이어가 구분할 수 있음 | Not Started |

주요 완료 기준:

- [ ] 기본 공격이 서버 권한으로 처리된다.
- [ ] 피해, 사망, 리스폰이 모든 클라이언트에 동기화된다.
- [ ] 최소한의 공격 및 피격 피드백이 제공된다.

### Development Week 3: 2026-07-09 ~ 2026-07-15

목표: AOS 구조물과 매치 승패 흐름을 완성한다.

| Track | Owner | Deliverable | Completion Criteria | Status |
| --- | --- | --- | --- | --- |
| Network / Game Rules | TBD | 매치 시작, 종료, 승패 판정 | 넥서스 파괴 시 서버가 승자를 결정함 | Not Started |
| GAS / Combat | TBD | 구조물 피해 처리 | 허용된 대상과 적 구조물에 피해를 줄 수 있음 | Not Started |
| Map / Level | TBD | 구조물 및 교전 공간 배치 | 2라인에서 목표 구조물까지 진행 가능함 | Not Started |
| UI / Feedback | TBD | 체력, 팀, 승패 표시 | 플레이어가 현재 상태와 결과를 확인할 수 있음 | Not Started |

주요 완료 기준:

- [ ] 구조물이 서버 권한으로 피해를 받고 파괴된다.
- [ ] 넥서스 파괴로 매치가 정상 종료된다.
- [ ] 2 vs 2 한 판의 핵심 흐름이 연결된다.

### Development Final: 2026-07-16 ~ 2026-07-22

목표: 반복 플레이 테스트가 가능한 최종 프로토타입을 정리한다.

| Track | Owner | Deliverable | Completion Criteria | Status |
| --- | --- | --- | --- | --- |
| Integration | TBD | 전체 기능 통합 빌드 | 한 판을 시작부터 종료까지 반복 진행 가능함 | Not Started |
| QA / Network Test | TBD | 테스트 결과 및 버그 목록 | 주요 P0 버그가 해결되거나 우회 방법이 문서화됨 | Not Started |
| Balance / Level | TBD | 최소 수치 및 전장 조정 | 플레이 테스트를 막는 심각한 밸런스 문제가 없음 | Not Started |
| Documentation | TBD | 구현 상태와 후속 백로그 | 완료, 미완료, 제외 항목이 구분되어 있음 | Not Started |

주요 완료 기준:

- [ ] 2명 이상이 접속해 한 판을 끝까지 진행한다.
- [ ] 핵심 네트워크 및 승패 흐름을 반복 테스트한다.
- [ ] 7월 22일 기준 빌드와 남은 이슈를 문서화한다.

## Daily Plan

필요한 경우 아래 표를 복사해 날짜별로 추가한다.

### YYYY-MM-DD

오늘의 목표: TBD

| Priority | Task | Owner | Expected Output | Status |
| --- | --- | --- | --- | --- |
| P0 | TBD | TBD | TBD | Not Started |
| P1 | TBD | TBD | TBD | Not Started |
| P2 | TBD | TBD | TBD | Not Started |

완료한 것:

- [ ] TBD

막힌 것:

- TBD

다음 액션:

- TBD

## Task Backlog

| Priority | Task | Owner | Related Milestone | Dependency | Status |
| --- | --- | --- | --- | --- | --- |
| P0 | TBD | TBD | TBD | TBD | Not Started |
| P1 | TBD | TBD | TBD | TBD | Not Started |
| P2 | TBD | TBD | TBD | TBD | Not Started |

우선순위 기준:

- `P0`: 프로토타입 한 판 성립에 직접 필요하다.
- `P1`: 테스트 품질과 플레이 감각에 중요하다.
- `P2`: 있으면 좋지만 MVP 실패 원인은 아니다.

## Risks

| Risk | Impact | Probability | Owner | Mitigation | Status |
| --- | --- | --- | --- | --- | --- |
| 서버 권한 전투 구현 지연 | High | Medium | TBD | 기본 공격 1종만 먼저 완성 | Open |
| GAS 학습 비용 증가 | High | Medium | TBD | Attribute, Ability, Effect 최소 세트로 제한 | Open |
| 맵 스케일 재작업 | Medium | Medium | TBD | 2라인 회색 박스로 먼저 플레이 테스트 | Open |

## Decisions

| Date | Decision | Reason | Follow-up |
| --- | --- | --- | --- |
| YYYY-MM-DD | TBD | TBD | TBD |

## Open Questions

- [ ] MVP 시점은 TPS 유지인가, 쿼터뷰 전환인가?
- [ ] 초기 MVP에 미니언을 포함할 것인가?
- [ ] 매치 내 성장 시스템을 포함할 것인가?
- [ ] 목표 플레이 타임은 몇 분인가?
- [ ] 첫 플레이 테스트 기준 인원과 환경은 무엇인가?

## Review Checklist

일정 리뷰 때 아래 항목을 확인한다.

- [ ] 이번 주 목표가 한 문장으로 명확한가?
- [ ] 각 작업에 담당자와 완료 기준이 있는가?
- [ ] P0 작업이 과도하게 많지 않은가?
- [ ] 리스크에 대응 액션이 있는가?
- [ ] 완료된 결정과 열린 질문이 분리되어 있는가?
- [ ] 다음 작업자가 바로 이어서 실행할 수 있는가?

## Change Log

| Date | Change | Reason | Author |
| --- | --- | --- | --- |
| 2026-06-08 | Initial draft | 일정 문서 작성을 위한 기본 템플릿 생성 | Codex |
| 2026-06-08 | 기획 및 개발 기간 반영 | 6월 25일까지 기획, 7월 22일까지 개발하는 일정 기준 적용 | Codex |
