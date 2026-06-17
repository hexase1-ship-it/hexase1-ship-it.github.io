# Dynasty Genetics Overhaul (CK3 Mod)

출생 시점(on_birth_child)에 스크립트 이벤트를 실행해 **부모의 선천 특성(congenital traits)**이 자식에게 전달될 확률을 조정하는 모드입니다.

## 변경 내용
- 선천 **긍정 특성**(지능/외모/체력 계열) 유전 확률 강화
- 선천 **부정 특성**(근친/허약) 유전 확률 완화

적용 방식은 바닐라 수치를 직접 덮어쓰는 define 수정이 아니라, 출생 후 이벤트로 trait를 보정하는 방식입니다.

## 구조
- `descriptor.mod`
- `common/on_action/dgo_on_actions.txt`
- `events/dgo_genetics_events.txt`
- `localization/english/dgo_l_english.yml`

## 설치 방법
1. 이 폴더(`dynasty_genetics_overhaul`)를 CK3의 `mod` 폴더로 복사합니다.
2. 런처에서 새 모드를 등록할 때 `descriptor.mod`를 사용합니다.
3. 플레이셋에 추가 후 게임 실행.

## 커스터마이징
`events/dgo_genetics_events.txt`의 각 `chance = N` 값을 바꿔서 난이도/밸런스를 조정할 수 있습니다.

예시:
- `genius` 45 → 30으로 낮추면 최상위 지능 특성 희귀화
- `inbred` 20 → 35로 올리면 근친 리스크 강화

