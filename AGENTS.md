# FieryTale Codex Working Guide

## 목적

이 저장소는 Unreal Engine 기반 게임 `FieryTale`의 기획 및 프로토타입 준비 문서를 관리한다.

Codex가 이 폴더에서 실행되면 먼저 이 문서를 읽고, 아래 기준에 따라 즉시 기획 작업을 이어간다.

## 프로젝트 요약

`FieryTale`은 전 세계의 동화, 설화, 민담 속 인물과 공간을 하나의 세계관으로 통합한 멀티플레이 대전 게임이다.

초기 기획 기준은 다음과 같다.

- 장르: AOS 구조 기반 팀 PvP
- 초기 매치 규모: 2 vs 2
- 엔진: Unreal Engine
- 네트워크: Dedicated Server 또는 서버 권한 기반 구조
- 전투/능력 시스템: Gameplay Ability System, GAS
- 초기 전장: 2개 라인, 팀별 넥서스 1개, 넥서스 타워 2개
- 초기 MVP 목표: 한 판이 서버 권한으로 끝까지 돌아가는 얇은 프로토타입

## 먼저 읽을 문서

새 작업을 시작하기 전에 다음 문서를 우선 확인한다.

1. `Docs/InitialConcept.md`
2. `Docs/SubDocuments/WorkspaceStatusAndStartup.md`
3. `Docs/SubDocuments/MVPScopeDecision.md`
4. `Docs/SubDocuments/CameraViewpointComparison.md`
5. `Docs/SubDocuments/Week1_TeamPlan.md`
6. `ConceptArt/StorybookWorld_ConceptGuide.md`
7. 관련 작업이 동화 원전, 캐릭터 후보, 세계관 소재를 다루는 경우 `Docs/FairyTales/` 하위 문서

## 실행 시작 절차

Codex가 이 폴더에서 새로 실행되면 다음 순서로 작업 준비를 한다.

1. `git status --short`로 현재 변경 상태를 확인한다.
2. `rg --files` 또는 가능한 빠른 파일 목록 명령으로 폴더 전체 산출물을 훑는다.
3. Trello를 사용할 수 있으면 기본 활성 보드를 아래 "Trello 기본 보드" 기준으로 설정한다.
4. 위 "먼저 읽을 문서" 목록을 읽고 현재 결정, 열린 질문, 다음 액션을 확인한다.
5. 사용자가 구체적인 작업을 주지 않았다면 `WorkspaceStatusAndStartup.md`의 "가장 가까운 다음 액션" 중 하나를 선택해 기획 산출물로 좁힌다.
6. 문서 변경 전에는 기존 문서와 중복되는지 확인하고, 변경 후에는 수정 파일과 핵심 결정을 짧게 보고한다.

## Trello 기본 보드

이 작업폴더에서 Trello 작업을 할 때는 다음 보드를 기본 활성 보드로 사용한다.

- 보드 이름: `FieryTale`
- 짧은 보드 ID: `Zx9zFR6a`
- 내부 보드 ID: `6a3a21b44eb622271cb44349`
- URL: `https://trello.com/b/Zx9zFR6a`

Trello 카드, 리스트, 라벨, 체크리스트를 조회하거나 생성할 때 사용자가 다른 보드를 명시하지 않으면 이 보드를 기준으로 처리한다.

## 현재 기획 상태

확정에 가까운 기준:

- 게임의 핵심 매력은 동화/설화 캐릭터 크로스오버다.
- 초기 제작 범위는 2 vs 2 소규모 프로토타입이다.
- 초기 개발 리스크는 멀티플레이, GAS, 서버 권한 전투, AOS 승패 흐름 검증이다.
- 첫 번째 전장의 시각 콘셉트는 특정 동화 하나가 아니라 "책과 이야기 자체로 이루어진 세계"다.

아직 결정이 필요한 쟁점:

- MVP 시점을 TPS로 유지할지, 낮은 쿼터뷰/쿼터뷰 AOS로 리스크를 줄일지
- 미니언 또는 라인 병력을 초기 MVP에 포함할지
- 매치 내 성장 방식을 사용할지, 초기에는 제외할지
- 캐릭터 역할군을 전통적 탱커/딜러/서포터로 나눌지
- 한 매치의 목표 플레이 타임
- 동화 원전의 퍼블릭 도메인/저작권 관리 기준

## 작업 우선순위

기획 작업은 다음 순서로 진행한다.

1. 핵심 플레이 정체성 결정: AOS 전략성 우선인지, TPS 액션성 우선인지
2. MVP 매치 규칙 확정: 팀, 스폰, 라인, 구조물, 승패, 리스폰
3. 전장 구조 문서화: 2라인 블록아웃, 구조물 위치, 교전 공간
4. 캐릭터 역할군과 초기 캐릭터 2종 설계
5. GAS 기준 전투 규칙 정리: Attribute, Ability, Effect, GameplayTag
6. 4주 프로토타입 범위와 주차별 산출물 정리
7. 테스트 체크리스트와 구현 우선순위 정리

## 문서 작성 규칙

- 기획 문서는 기본적으로 한국어로 작성한다.
- 파일명은 기존 패턴처럼 영어 PascalCase 또는 명확한 영어 이름을 사용한다.
- 문서는 `Docs/` 하위에 둔다. 세부 보조 문서는 `Docs/SubDocuments/`를 우선 사용한다.
- 원전 동화/설화 개별 정리는 `Docs/FairyTales/`에 둔다.
- 컨셉아트 가이드와 이미지 산출물은 `ConceptArt/`에 둔다.
- 구현 계획과 실제 개발 산출물이 생기면 `Dev/` 하위를 사용한다.
- 새 문서를 만들 때는 목적, 현재 결정, 열린 질문, 다음 액션을 명확히 남긴다.
- 기획 결정은 "재미있을 것 같다"보다 구현 가능성, MVP 범위, 테스트 가능성을 기준으로 쓴다.

## Codex 작업 방식

사용자가 별도 지시 없이 "기획 이어서 하자", "다음 단계 진행", "정리해줘"처럼 요청하면 다음 흐름을 따른다.

1. 관련 기존 문서를 확인한다.
2. 폴더 전체 상태가 오래되었거나 불명확하면 `WorkspaceStatusAndStartup.md`를 갱신한다.
3. 현재 쟁점 중 하나를 좁혀서 산출물로 만든다.
4. 막연한 아이디어보다 프로토타입에 바로 영향을 주는 규칙, 표, 체크리스트를 우선 작성한다.
5. 문서 변경 후 변경 파일과 핵심 내용을 짧게 보고한다.

사용자가 아이디어 검토를 요청하면 코드나 파일을 바로 수정하기보다, 먼저 장단점과 추천안을 정리한다.

사용자가 문서 생성을 요청하면 기존 문서의 톤과 구조를 맞추고, 과도한 마케팅 문구를 피한다.

## 다음에 하면 좋은 작업

가장 가까운 다음 기획 산출물 후보:

1. `Docs/SubDocuments/MVPViewpointDecision.md`
   - TPS 유지와 쿼터뷰 전환 중 MVP 기준 결정을 정리한다.
2. `Docs/SubDocuments/CoreMatchRules.md`
   - 2 vs 2 한 판의 시작, 진행, 종료 규칙을 확정한다.
3. `Docs/SubDocuments/InitialCharacterRoles.md`
   - 초기 캐릭터 역할군과 2종 캐릭터 초안을 만든다.
4. `Docs/SubDocuments/GASCombatPlanning.md`
   - GAS 기준 Attribute, Ability, Effect, Tag 초안을 정리한다.
5. `Docs/SubDocuments/PrototypeBacklog.md`
   - 4주 프로토타입의 기능 백로그와 우선순위를 정리한다.
