# FieryTale Working Notes

## 현재 작업 기준

- 작업 폴더: `C:\Users\njh10\Documents\PW\FieryTale`
- Git 상태: 최초 커밋 이후 현재 변경사항 없음
- 핵심 문서:
  - `Docs/InitialConcept.md`
  - `Docs/FairyTales/00_SelectionCriteria.md`
  - `ConceptArt/StorybookWorld_ConceptGuide.md`

## 현재 기획 요약

FieryTale는 전 세계 동화, 설화, 민담 속 인물과 공간을 하나의 세계관으로 통합한 TPS 기반 2 vs 2 멀티플레이 AOS 게임이다.

초기 MVP는 데디케이트 서버 기반 멀티플레이, GAS 기반 캐릭터 능력 시스템, TPS 전투, 2개 라인, 넥서스와 넥서스 타워, 구조물 파괴와 승패 판정을 검증하는 데 초점을 둔다.

첫 번째 배경 컨셉은 특정 동화 하나가 아니라 책, 종이, 이야기 자체를 상징하는 "스토리북 월드"다. 책으로 된 성, 펼쳐진 책 광장, 종이 구조물, 악기 실루엣의 원경을 사용한다.

## 확정된 방향

- 장르: TPS 시점의 팀 기반 AOS
- 초기 규모: 2 vs 2
- 엔진: Unreal Engine
- 네트워크: 데디케이트 서버, 서버 권한 구조
- 전투/능력: Gameplay Ability System
- 전장: 2개 라인, 팀별 넥서스 1개와 넥서스 타워 2개
- IP 방향: 퍼블릭 도메인 원전 기반, 현대 스튜디오 고유 디자인 회피

## 아직 정해야 할 핵심 질문

- 전체 톤을 밝은 동화풍, 다크 판타지, 혼합형 중 어디에 둘 것인가?
- 미니언 또는 라인 병력을 둘 것인가?
- 매치 내 성장 방식을 레벨업, 아이템, 카드, 스킬 강화 중 무엇으로 할 것인가?
- 캐릭터 역할군을 탱커, 딜러, 서포터 등으로 명확히 나눌 것인가?
- 한 매치의 목표 플레이 타임을 몇 분으로 잡을 것인가?
- 조준 방식을 순수 TPS 슈터에 가깝게 할 것인가, 액션 AOS 보조 조준에 가깝게 할 것인가?

## 다음 작업 추천 순서

1. `Docs/Worldbuilding.md` 작성: 세계관 기본 설정, 왜 동화들이 한 전장에 모였는지, 넥서스의 의미 정리
2. `Docs/CoreGameLoop.md` 작성: 플레이어가 매치 중 반복하는 핵심 행동 루프 정의
3. `Docs/MatchRules.md` 작성: 승리 조건, 리스폰, 구조물, 라인, 미니언 여부 정리
4. `Docs/BattlefieldLayout.md` 작성: 2 vs 2 전장 구조, 라인 배치, 엄폐물, 시야 포인트 정리
5. `Docs/CharacterRoles.md` 작성: 초기 캐릭터 역할군과 스킬 설계 기준 정리
6. `Docs/GASCombatFramework.md` 작성: Attribute, Ability, Effect, Cue, 서버 권한 판정 기준 정리
7. `Docs/MVPProductionScope.md` 작성: 실제 프로토타입 제작 범위와 일정 정리

## 바로 이어서 하기 좋은 작업

가장 먼저 `Worldbuilding.md`를 작성하는 것이 좋다. 이유는 캐릭터, 맵, 구조물, 넥서스, 중립 오브젝트의 명칭과 분위기가 세계관 기준에 따라 달라지기 때문이다.

권장 시작 주제:

- 세계의 이름
- 넥서스의 정체
- 전장에 소환되는 규칙
- 동화 원전의 인물들이 전투 캐릭터가 되는 이유
- 밝은 동화성과 전장 긴장감을 동시에 유지하는 톤
