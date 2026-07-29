# Day 2 강사 가이드 — AI와 대화하는 기술 (프롬프트 + 미니게임)

**오늘의 목표.** "같은 도구인데 왜 결과가 다를까"를 몸으로 깨닫는다. 모호한 프롬프트로 일부러 실패한 뒤 구체적 프롬프트로 성공하는 A/B 경험을 통해 Golden Rule 1(Be specific)·2(One thing at a time)를 체득한다. 되돌리기·중단·새 세션이라는 안전장치 3종을 익혀 "망쳐도 복구할 수 있다"는 자신감을 만든다.

**오늘의 산출물.** 학생 1인당 숫자 맞추기 게임(`number-game/index.html`) + 모호 vs 구체 비교 기록.

## 준비물

- [ ] `slides/day2.html` 투영, `handouts/day2-worksheet.md` 배포
- [ ] **`handouts/prompt-cheatsheet.md` 인쇄 배포 (오늘부터 상시 사용 — 가급적 인쇄물로)**
- [ ] 강사 시연용 빈 폴더 `demo-day2`
- [ ] 어제 결석자 파악 — 결석자는 워크시트 Day 1을 셀프 진행하도록 자리 배치(옆에 잘하는 학생)

## 타임라인 (120분)

| 시간 | 분량 | 내용 | 자료 |
|---|---|---|---|
| 00:00 | 10′ | 복습 퀴즈(손들기) + 오늘 예고 | 슬라이드 1–3 |
| 00:10 | 15′ | **A/B 라이브 시연**: 모호 vs 구체 + Golden Rule 1·2 | 슬라이드 4–8 + 시연 |
| 00:25 | 10′ | 안전장치 3종(Esc·`/undo`·새 세션) + 치트시트 투어 | 슬라이드 9–10 |
| 00:35 | 10′ | 실습 ①: 일부러 모호하게 — "Make a game." 실험 | 워크시트 Step 1 |
| 00:45 | 10′ | 실습 ②: 새 세션 → 구체 프롬프트로 다시 | 워크시트 Step 2 |
| 00:55 | 45′ | 실습 ③: FIX 라운드로 게임 완성 | 워크시트 Step 3 |
| 01:40 | 10′ | 비교 회고: 뭐가 달랐나 (2–3명 발표) | 슬라이드 13 |
| 01:50 | 10′ | Golden Rules 복창 + 내일 예고 | 슬라이드 14–15 |

## 진행 대본

### 1) 복습 퀴즈 (10′) — 슬라이드 2

손들기 퀴즈 3문항. ① "The 4 words of the loop?" (다 같이 외치기: TELL–WATCH–CHECK–FIX) ② "AI can be wrong. Who checks?" ("Me!") ③ "What did you build yesterday?" (어제 만든 페이지 자랑할 사람 1명 화면 공유).

### 2) A/B 라이브 시연 (15′) — 오늘의 승부처

`demo-day2` 폴더에서 opencode 실행. **1차: 일부러 모호하게.**

```text
Make a game.
```

- 중계 멘트. "What game? Card game? Racing? The AI doesn't know. Watch what happens." → AI가 임의의 게임을 만들거나 반문한다. 어느 쪽이든 교훈은 같다: "Vague in → random out."
- **2차: 구체적으로.** 새 세션(Ctrl+X 후 N — 화면으로 크게 보여주기) 후:

```text
Create index.html — a number guessing game.
The computer picks a secret number from 1 to 100.
I type a guess. The game tells me "higher" or "lower".
I have 7 tries. Show a win or lose message at the end.
Make it colorful with big buttons.
```

- 브라우저로 열어 2~3회 플레이. "Same AI. Same day. Different words. **The prompt is the program.**"
- 구체 프롬프트를 슬라이드 7로 해부한다: 무엇을(게임 종류) + 규칙(범위·기회·힌트) + 겉모습(colorful, big buttons).

### 3) 안전장치 3종 + 치트시트 (10′) — 슬라이드 9–10

- **Esc**: AI가 엉뚱한 방향으로 달리면 멈춘다.
- **`/undo`**: 방금 변경을 되돌린다. 여러 번 가능. "Time machine."
- **새 세션 (Ctrl+X, 그다음 N)**: 대화가 꼬였을 때 새 출발. opencode를 껐다 켜도 같은 효과.
- 치트시트 배포. 5개 섹션(시작/모양/기능/고치기/막혔을 때)을 30초씩 훑고, "매일 옆에 두라"고 안내.

### 4) 실습 운영 (총 65′)

- **Step 1 — 모호 실험 (10′)**: 새 폴더 `number-game` → opencode → 워크시트대로 `Make a game.` 전송. 결과를 워크시트 기록표에 적는다(AI가 뭘 만들었나 / 내가 원한 것인가). **이 실패는 오늘의 핵심 경험이므로 건너뛰지 못하게 한다.** 빨리 끝난 학생에게는 "옆 사람과 결과 비교 — 서로 다른 게 나왔죠? 그게 포인트"라고 짚어준다.
- **Step 2 — 구체 프롬프트 (10′)**: 새 세션(Ctrl+X N) 후 워크시트의 구체 프롬프트 전송(빈칸: 숫자 범위·시도 횟수·색). 브라우저 CHECK. 전원이 동작하는 게임을 가진 상태로 Step 3 진입이 목표.
- **Step 3 — FIX 라운드 (45′)**: 메뉴에서 **한 번에 하나씩**: 남은 시도 표시 → 이모지·색 스타일링 → Play Again 버튼 → 이긴 횟수 카운터. Stretch: 최고 기록 저장(localStorage), 난이도 선택(Easy 1–50 / Hard 1–500).

**순회 우선순위.** ① Step 2에서 게임이 아예 안 뜨는 학생(에러면 "다음 주 배울 것 미리 맛보기"라며 에러 복사→붙여넣기 시켜보기 — Day 4 내용의 예고편) ② `/undo`를 몰라서 꼬인 학생 ③ Stretch 안내.

### 5) 마무리 (20′)

- 회고 질문(슬라이드 13): "Step 1 and Step 2 — same AI. What was different?" 2~3명 답 듣기. 목표 답: "내 말이 달랐다."
- Golden Rules 복창: "Be specific! One thing at a time! You decide, AI builds!"
- 내일 예고. "Tomorrow, no more my missions. **YOUR idea.** Tonight, think: what app do YOU want to make?"

## 예상 질문·상황 대응

| 상황/질문 | 대응 |
|---|---|
| 모호 실험에서 AI가 되물음("어떤 게임?") | 훌륭한 소재. "AI도 정보가 부족하면 일을 못 한다 — 그래서 구체성이 필요" 정리. 반문에 답하지 말고 Step 2로 진행 |
| `/undo`가 안 먹는 것 같음 | 메시지 단위로 여러 번 입력 가능. 그래도 꼬이면 새 세션 + 치트시트 5번 재시작 프롬프트 |
| 게임 로직 버그(힌트 반대, 시도 수 안 줄어듦 등) | FIX 공식 연습 기회: "When I guess 50 and the number is 80, it says 'lower'. It should say 'higher'. Fix it." |
| 학생이 여러 요청을 한 문장에 몰아넣음 | Golden Rule 2 상기. "AI도 사람처럼 한 번에 하나를 잘한다" |
| 영어 부담 호소 | 치트시트 빈칸만 채우게. "문법 채점 아무도 안 한다" |
| 상위권 조기 완료 | Stretch 후 "가위바위보 게임을 처음부터 혼자 프롬프트 설계" 미션 |

## 화이트보드 백업 (정전·프로젝터 불능 시)

보드에: `Vague in → Random out` / Golden Rule 1·2 / 구체 게임 프롬프트 전문 / 안전장치 3종(Esc, /undo, Ctrl+X N).

## 슬라이드 구성 (slides/day2.html, 15장)

| # | 슬라이드 | 핵심 내용 |
|---|---|---|
| 1 | 타이틀 | Day 2: Talking to AI Like a Pro 🗣️ |
| 2 | Quiz | 복습 3문항(손들기): 4 words? / Who checks? / What did you build? |
| 3 | Today | Better words → better apps. And we build a GAME 🎮 |
| 4 | Experiment | "Make a game." — 시연 큐 슬라이드. "What will happen?" |
| 5 | Why? | Vague in → Random out. "AI cannot read your mind." |
| 6 | Golden Rule 1 | **Be specific**: what + how it looks + how it works. 나쁜/좋은 예 2열 |
| 7 | Anatomy | 구체 게임 프롬프트를 색깔로 분해(무엇/규칙/모양) |
| 8 | Golden Rule 2 | **One thing at a time** — 몰아 요청 vs 한 개씩 비교 |
| 9 | Safety tools | Esc = stop / `/undo` = time machine / Ctrl+X→N = fresh start |
| 10 | Cheat sheet | 치트시트 5개 섹션 안내 — "keep it next to you" |
| 11 | Mission | Number Guessing Game — Step 1 vague → Step 2 specific → Step 3 FIX |
| 12 | FIX ideas | tries counter / colors+emoji / Play Again / win counter (+Stretch) |
| 13 | Compare | "Same AI. What was different?" 회고 질문 슬라이드 |
| 14 | Recap | 3 Golden Rules 복창 |
| 15 | Tomorrow | "YOUR idea starts tomorrow 💡 — tonight, think about it" |

## 워크시트 매핑 (handouts/day2-worksheet.md)

Step 1 모호 실험+기록표(What did AI make? / What did YOU want?) → Step 2 새 세션+구체 프롬프트(빈칸: 범위·시도·색) → Step 3 FIX 메뉴 4종+Stretch 2종 → 안전장치 3종 참조 박스 → 체크포인트(게임 동작/비교 기록/FIX 3회) → 출구 티켓("내일 만들고 싶은 앱 아이디어 1줄" — Day 3 연결).
