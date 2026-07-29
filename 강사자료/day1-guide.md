# Day 1 강사 가이드 — AI가 코드를 짠다 (개념 + 첫 웹페이지)

**오늘의 목표.** 학생이 바이브 코딩이 무엇인지 감을 잡고, opencode로 생애 첫 웹페이지를 직접 만들어 브라우저에서 열어본다. 핵심 루프 **TELL → WATCH → CHECK → FIX**를 몸으로 1회 이상 경험한다.

**오늘의 산출물.** 학생 1인당 자기소개 웹페이지(`my-profile/index.html`) + FIX 요청 3회 이상.

## 준비물

- [ ] `slides/day1.html` 프로젝터 투영 (오프라인 동작, ←/→/Space/클릭 넘김)
- [ ] `handouts/day1-worksheet.md` 배포 (인쇄 권장)
- [ ] 강사 PC에 라이브 시연용 **빈 폴더** (`demo-day1`) 준비, opencode 로그인 확인
- [ ] 학생 PC 전원·인터넷·opencode 동작 사전 점검 (세팅 자료 기준)

## 타임라인 (120분)

| 시간 | 분량 | 내용 | 자료 |
|---|---|---|---|
| 00:00 | 10′ | 인사 + 아이스브레이크 + 오늘 예고 | 슬라이드 1–3 |
| 00:10 | 8′ | **라이브 시연**: 말로 웹페이지 만들기 | 슬라이드 4 + 시연 |
| 00:18 | 12′ | 개념: 바이브 코딩, AI는 어떻게 일하나, 핵심 루프 | 슬라이드 5–10 |
| 00:30 | 15′ | 실습 ①: 폴더 만들기 → opencode 실행 → 첫 프롬프트 | 워크시트 Step 1–2 |
| 00:45 | 10′ | 실습 ②: 브라우저에서 열기 (CHECK) | 워크시트 Step 3 |
| 00:55 | 5′ | (모아서) FIX 요청하는 법 시범 1회 | 슬라이드 11 |
| 01:00 | 40′ | 실습 ③: FIX 라운드 3회+ (자기화) | 워크시트 Step 4 |
| 01:40 | 10′ | 짝과 화면 바꿔 구경 + 잘된 것 하나씩 소리내 말하기 | — |
| 01:50 | 10′ | 정리: 루프 복습, 내일 예고, 출구 티켓 | 슬라이드 12–14 |

시간이 밀리면 실습 ③을 줄이지 말고 아이스브레이크·공유를 줄인다. 첫날의 성패는 "내 손으로 FIX를 몇 번 돌렸나"에 달려 있다.

## 진행 대본

### 1) 오프닝 (10′)

- 팀 소개 후 질문 하나 던지기. "Have you ever wanted to make your own app or website?" (손 들게 하기)
- 오늘 약속을 말한다. "Today, you will make your first webpage. Not next week — **today, in this room.**"

### 2) 라이브 시연 (8′) — 오늘의 승부처

터미널을 프로젝터에 크게 띄우고(글자 크기 최대), `demo-day1` 폴더에서 `opencode` 실행. 아래 프롬프트를 **학생들이 보는 앞에서 천천히 타이핑**한다.

```text
Create index.html — a colorful webpage about Luang Prabang.
Add a big title, 3 famous places with short descriptions,
and a button that shows a fun fact about Laos when clicked.
```

- WATCH 동안 중계한다. "Look — the AI is writing HTML, CSS, JavaScript. I am not typing any code."
- 끝나면 `index.html`을 브라우저로 열고 버튼을 눌러 보인다. 환호 유도.
- 바로 FIX 1회 시연. `Change the colors to the colors of the Lao flag.` → 새로고침 → 달라진 화면.
- 마무리 멘트. "I did not write code. I **told** the AI what I want. This is **vibe coding**. Today you will do the same."

시연 실패 대비: 사전에 같은 프롬프트로 1회 생성해 둔 백업 폴더를 준비해 두고, API가 느리면 "AI is thinking — good time to explain" 하며 개념 슬라이드로 자연스럽게 넘어갔다가 돌아온다.

### 3) 개념 강의 (12′) — 슬라이드 5–10

전달할 것은 딱 세 가지다. 길게 하지 않는다.

1. **Vibe coding이란**: 코드를 한 줄씩 쓰는 대신, AI에게 원하는 것을 말하고 결과를 확인하며 방향을 잡는 개발 방식. (2025년 초 Andrej Karpathy가 이름 붙임 — "There's a new kind of coding… you fully give in to the vibes.")
2. **AI는 어떻게 일하나**: 아주 많은 글과 코드를 읽고 "다음에 올 말"을 잘 맞히도록 훈련된 프로그램(LLM). 매우 똑똑한 조수지만 **틀릴 수 있다** → 그래서 CHECK는 언제나 사람 몫.
3. **핵심 루프**: TELL(원하는 걸 말한다) → WATCH(AI가 만든다) → CHECK(브라우저에서 확인한다) → FIX(고칠 점을 말한다). 오늘부터 5일 내내 이 네 단어만 기억하면 된다.

### 4) 실습 운영 (총 70′)

워크시트 순서대로. 각 스텝 시작을 슬라이드로 알리고, 이후는 순회하며 개별 지원한다.

- **Step 1–2 (15′)**: 바탕화면에 `my-profile` 폴더 → 터미널에서 그 폴더로 이동 → `opencode` 실행 → 워크시트의 첫 프롬프트를 빈칸 채워 전송. 여기서 전원이 "AI가 뭔가 만들기 시작"하는 상태까지 도달해야 한다. 뒤처진 학생 최우선 지원.
- **Step 3 (10′)**: 파일 탐색기에서 `index.html` 더블클릭 → 브라우저 확인. 첫 화면이 뜨는 순간을 다 같이 축하한다 ("Everyone who can see their page — raise your hand!").
- **Step 4 (40′)**: FIX 라운드. 워크시트의 FIX 메뉴에서 골라 **한 번에 하나씩** 요청 → 새로고침 → 확인. 최소 3회, 빠른 학생은 Stretch 과제로.

**순회 우선순위.** ① opencode가 아예 안 도는 학생(세팅 자료로 복구, 안 되면 옆 학생과 페어) ② 첫 프롬프트를 못 보낸 학생(치트시트는 내일 배포지만, 워크시트의 예시를 그대로 쓰게 안내) ③ 잘하는 학생 Stretch 안내.

### 5) 마무리 (20′)

- 짝과 화면을 바꿔 서로의 페이지에서 "좋은 점 하나"를 말하게 한다 (영어 한 문장이면 충분: "I like your colors.").
- 루프 복습: 슬라이드 보며 다 같이 네 단어 소리내기. "TELL! WATCH! CHECK! FIX!"
- 출구 티켓(워크시트 마지막 칸): 오늘 배운 것 1가지 + 궁금한 것 1가지 적고 제출.
- 내일 예고. "Tomorrow: how to talk to AI like a pro — and we make a GAME."

## 예상 질문·상황 대응

| 상황/질문 | 대응 |
|---|---|
| "코드를 몰라도 정말 되나요?" | 된다. 다만 "뭘 원하는지"는 알아야 한다. 그게 이번 5일의 훈련. |
| "AI가 만든 코드는 누구 거예요?" | 이 수업 결과물은 여러분 것. 단, 실무에선 회사·라이선스 정책 확인이 필요하다고 짧게. |
| 영어 프롬프트를 겁냄 | "Short sentences. Wrong grammar is OK." 워크시트 예시를 그대로 복사해도 됨을 강조. |
| 생성이 너무 오래 걸림 | Esc로 중단하지 말고 기다리게 안내(첫날은 Esc 미도입). 전체적으로 느리면 페어로 전환. |
| AI가 파일을 여러 개 만듦 | 정상. 오늘은 `index.html`만 열면 된다고 안내. 원하면 "Put everything in ONE file index.html" 요청. |
| 이상한 결과/깨진 화면 | 첫날은 `/undo`를 가르치지 않았으므로: "It looks broken. Please fix it. I want ___." 로 FIX 요청 유도. |
| 학생이 코드를 이해하려고 멈춤 | 좋은 신호! 단 오늘은 "동작 확인"이 먼저. 코드 읽기는 과정 밖 심화로 안내. |

## 화이트보드 백업 (정전·프로젝터 불능 시)

보드에 이것만 그린다: `TELL → WATCH → CHECK → FIX` 순환 화살표 + Golden Rule 두 줄(Be specific / One thing at a time) + 첫 프롬프트 전문.

## 슬라이드 구성 (slides/day1.html, 14장)

| # | 슬라이드 | 핵심 내용 |
|---|---|---|
| 1 | 타이틀 | Vibe Coding Camp — Day 1: Your First Webpage. "You speak. AI builds. You decide." |
| 2 | Hello! | 팀 소개 자리 + 질문 "Ever wanted to make your own app?" |
| 3 | Today | 오늘 할 일 3줄: See it → Learn the loop → Build YOUR page |
| 4 | Live Demo | "Watch. I will not write code." (시연 큐 슬라이드) |
| 5 | What is Vibe Coding? | 정의 한 줄 + Karpathy 인용 한 줄 |
| 6 | Old way vs New way | 코드 한 줄씩 vs 말하고 확인하기 (2열 비교) |
| 7 | How does AI work? | LLM = "다음 말 맞히기"를 아주 잘하는 프로그램. 그림 수준 |
| 8 | AI can be wrong | 환각 개념 한 장 — "So YOU always check." |
| 9 | The Loop | TELL → WATCH → CHECK → FIX 다이어그램 (이후 매일 재등장) |
| 10 | You decide, AI builds | Golden Rule 3 소개 |
| 11 | How to FIX | FIX 요청 공식: what I SEE + what I WANT |
| 12 | Mission | 미션 요약: My Profile Page, FIX ×3 |
| 13 | Recap | 네 단어 복창 슬라이드 |
| 14 | Tomorrow | 내일 예고: Talk like a pro + make a GAME |

## 워크시트 매핑 (handouts/day1-worksheet.md)

Step 1 폴더·실행 → Step 2 첫 프롬프트(빈칸 채움) → Step 3 브라우저 CHECK → Step 4 FIX 메뉴 3회+ → Stretch(다크모드 토글 등) → 체크포인트 3개 → 출구 티켓.
