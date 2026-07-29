# Day 4 강사 가이드 — 집중 개발 (기능 스프린트 + 4가지 탈출법)

**오늘의 목표.** 캡스톤의 MUST 기능 3개를 전부 동작시킨다. 그 과정에서 반드시 막히게 되는데, 그때 **4 Escape Moves**(에러 복붙 / `/undo` / 작게 쪼개기 / 새 세션)로 스스로 빠져나오는 경험을 한다. Save Point 습관(동작하는 버전 백업)을 심는다.

**오늘의 산출물.** MUST 3개가 동작하는 `my-app/index.html` + 스프린트 로그(워크시트) + Save Point 파일들.

## 준비물

- [ ] `slides/day4.html` 투영, `handouts/day4-worksheet.md` 배포
- [ ] 어제 계획서(승인 사인된 것) 지참 확인 — 없으면 워크시트에 다시 옮겨 적게
- [ ] Day 3 결석자 대응: 시작 전 10분 압축 기획(테마 중 단순한 것 배정 + 즉석 승인) 후 합류
- [ ] 신호등 운영 방식 결정: 색종이 3장 배포 or 손 신호(주먹=빨강/보=초록/반=노랑)

## 타임라인 (120분)

| 시간 | 분량 | 내용 | 자료 |
|---|---|---|---|
| 00:00 | 5′ | 오늘 목표 선언: "MUST 3 all working" | 슬라이드 1–2 |
| 00:05 | 10′ | 강의: 스프린트 리듬 + Save Point + 4 Escape Moves | 슬라이드 3–8 |
| 00:15 | 30′ | 스프린트 1: MUST 1 완성 | 워크시트 로그 |
| 00:45 | 3′ | 체크포인트 ①: 신호등 | 슬라이드 9 |
| 00:48 | 30′ | 스프린트 2: MUST 2 | 워크시트 로그 |
| 01:18 | 3′ | 체크포인트 ②: 신호등 | 슬라이드 9 |
| 01:21 | 24′ | 스프린트 3: MUST 3 (+빠른 학생은 NICE) | 워크시트 로그 |
| 01:45 | 15′ | 정리: DoD 확인 + 내일 발표 안내 | 슬라이드 11–12 |

강의를 10분에 끝내는 것이 중요하다. 오늘의 배움은 말이 아니라 90분의 스프린트 안에서 일어난다.

## 진행 대본

### 1) 오프닝 (5′)

"Yesterday you made a plan and v0. Today — **Build Day.** One goal: your 3 MUST features, all working. Tomorrow you present. Let's go."

### 2) 강의: 리듬과 탈출법 (10′) — 슬라이드 3–8

- **스프린트 리듬** (슬라이드 3): `ONE feature → TELL → CHECK → Save Point → ✔ → next`. 워크시트 로그에 기능마다 한 줄 기록.
- **Save Point** (슬라이드 4): 기능 하나가 잘 돌 때마다 파일 탐색기에서 `index.html` 복사 → `index-v1.html`, `v2`… "게임에서 보스전 앞 세이브처럼. 전부 깨져도 세이브로 돌아가면 된다."
- **4 Escape Moves** (슬라이드 5–8, 각 1분):
  1. **Paste the error** — 빨간 에러·이상한 메시지는 전체 복사해서 `I got this error. Please fix it:` 뒤에 붙여넣기. "에러는 나쁜 소식이 아니라 AI에게 주는 최고의 힌트."
  2. **`/undo`** — 방금 변경이 이상하면 타임머신. 여러 번 가능.
  3. **Ask smaller** — 한 번에 안 되면 쪼갠다. "Add a full expense tracker" → "Add ONE input box and a button that adds the number to a list."
  4. **Fresh start** — 대화가 완전히 꼬였으면 Ctrl+X N 새 세션 + 치트시트 5번 재시작 프롬프트(현재 상태 요약 + 다음 한 가지). "AI의 기억을 리셋하고 현재 파일에서 다시 출발."

### 3) 스프린트 운영 (90′)

- 각 스프린트 시작을 짧게 선언하고 타이머 표시(칠판에 종료 시각 써두기).
- **체크포인트 신호등**: 전원 동시에 신호. 초록=순항 / 노랑=질문 있음 / 빨강=막힘. 빨강 먼저, 노랑 다음 순회. 초록 학생 중 여유 있는 1~2명을 빨강 옆에 "helper"로 지정(가르치면 더 배운다고 명분 부여).
- **순회 시 개입 원칙**: 코드를 직접 봐주지 말 것. "어떤 Escape Move를 써봤어?"부터 묻고 학생이 스스로 4개 중 하나를 고르게 한다. 강사가 프롬프트를 대신 써주는 건 최후 수단.
- **진도 리스크 관리**: 스프린트 2가 끝났는데 MUST 1도 안 되는 학생 → 기능을 더 잘게 컷(합계 계산 → 목록 표시까지만). "발표는 완성된 부분만 보여주면 된다"고 안심시키기.
- 빠른 학생: MUST 3 완료 시 NICE 착수 전에 **전체 시나리오 테스트**(처음 열어서 끝까지 눌러보기) 먼저 → 발견한 버그 FIX → 그다음 NICE.

### 4) 마무리 (15′)

- **DoD 확인** (슬라이드 11): ① MUST 3 브라우저 동작 ② 앱 이름 + Made by 이름 표시 ③ 처음부터 끝까지 데모 가능. 워크시트 체크.
- 내일 안내 (슬라이드 12): 완성 안 됐어도 괜찮다 — 내일 50분 다듬기 시간이 있다. 발표는 1인 2분: 데모 + 3문장(앱 이름 / 뭘 할 수 있나 / 제일 어려웠던 것). "오늘 밤에 새 기능 추가하지 말 것 — 내일 아침에 깨진 앱으로 시작하는 지름길."
- 출구 티켓: "내일 다듬을 것 1가지" 적기.

## 예상 질문·상황 대응

| 상황/질문 | 대응 |
|---|---|
| AI가 응답을 안 하거나 한없이 김 | Esc로 중단 → 요청을 더 작게. 네트워크 문제면 페어 전환(리스크 표 참조) |
| 파일이 여러 개로 쪼개짐(css/js 분리) | `Put everything back into ONE file: index.html.` — 규칙 상기 |
| 전부 깨졌는데 `/undo`로도 복구 불가 | Save Point 등판: 탐색기에서 `index-v2.html` 복사 → `index.html`로 이름 변경 → 새 세션에서 재시작 프롬프트 |
| localStorage가 동작 안 함 | 대부분 브라우저는 file://에서도 동작. 안 되면 그 자리에서 판정: 저장 기능을 NICE로 강등하고 진행 (완성이 우선) |
| "AI가 만든 코드가 무슨 뜻인지 몰라도 되나요?" | 오늘은 된다. 단 "무엇을 해야 하는지"는 알아야 CHECK가 가능. 심화 학습 욕구는 Day 5 클로징에서 안내 예정 |
| 학생이 몰래 범위를 키움 | 계획서 사인 상기. "버전 2는 캠프 후에" |
| 헬퍼 학생이 대신 다 해줌 | 헬퍼 규칙: 키보드는 주인만. 헬퍼는 말로만 도움 |

## 화이트보드 백업 (정전·프로젝터 불능 시)

보드에: 리듬 한 줄(`ONE feature → TELL → CHECK → SAVE → next`) + 4 Escape Moves 번호 목록 + 종료 시각·체크포인트 시각 2개.

## 슬라이드 구성 (slides/day4.html, 12장)

| # | 슬라이드 | 핵심 내용 |
|---|---|---|
| 1 | 타이틀 | Day 4: Build Day 🔨 |
| 2 | Goal | "All 3 MUST features working — today." (내일 발표 카운트다운) |
| 3 | The rhythm | ONE feature → TELL → CHECK → Save Point → ✔ → next (리듬 다이어그램) |
| 4 | Save Point | index.html 복사 → index-v1.html. 게임 세이브 비유 🎮💾 |
| 5 | Escape 1 | Paste the error — 전체 복사 + `I got this error. Please fix it:` |
| 6 | Escape 2 | `/undo` = time machine (여러 번 가능) |
| 7 | Escape 3 | Ask smaller — 큰 요청 vs 쪼갠 요청 예시 |
| 8 | Escape 4 | Fresh start — Ctrl+X→N + 재시작 프롬프트(치트시트 5번) |
| 9 | Traffic light | 🟢 going well / 🟡 question / 🔴 stuck — 체크포인트에서 다 같이 |
| 10 | Sprint plan | 오늘의 시간표: Sprint 1·2·3 + 체크포인트 2회 |
| 11 | Definition of Done | MUST 3 동작 / 앱 이름+Made by / 데모 가능 |
| 12 | Tomorrow | Ship It! — 2-min demo + 3 sentences. "Do NOT add features tonight 😉" |

## 워크시트 매핑 (handouts/day4-worksheet.md)

상단 미니 참조: 4 Escape Moves + 리듬 한 줄 → 스프린트 로그 표(기능 / 사용한 프롬프트 / 동작 Y·N / Save Point 저장 ✔) 6행 → 신호등 설명 박스 → DoD 체크 3항목 → 출구 티켓("내일 다듬을 것 1가지"). 로그 표는 "FIX 루프를 스스로 돌린 흔적"으로 평가에 사용(curriculum.md 5절).
