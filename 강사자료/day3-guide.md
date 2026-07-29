# Day 3 강사 가이드 — 아이디어를 설계로 (캡스톤 기획 + v0)

**오늘의 목표.** "앱 = 작은 기능들의 목록"이라는 설계 사고를 익힌다. 자기 아이디어를 MUST 3 + NICE 2 기능 목록으로 쪼개고, Plan 모드로 AI와 계획을 다듬은 뒤, v0(첫 화면 + 첫 기능)까지 만든다. **오늘 강사의 가장 중요한 일은 범위 승인(스코프 다이어트)이다.**

**오늘의 산출물.** 학생 1인당 캡스톤 계획서(워크시트, 강사 승인 사인 포함) + v0 (`my-app/index.html`).

## 준비물

- [ ] `slides/day3.html` 투영, `handouts/day3-worksheet.md` 배포 (계획서 양식 포함 — 인쇄 강력 권장)
- [ ] 치트시트 여분 (잃어버린 학생용)
- [ ] 어제 출구 티켓의 "만들고 싶은 앱" 훑어보기 — 위험한 범위(채팅·로그인 등) 미리 파악
- [ ] Day 1–2 결석자용 압축 안내 준비: "루프 4단어 + Golden Rule 2개 + 치트시트" 5분 브리핑 후 바로 합류

## 타임라인 (120분)

| 시간 | 분량 | 내용 | 자료 |
|---|---|---|---|
| 00:00 | 8′ | 복습 + "오늘부터 네 앱" 선언 | 슬라이드 1–3 |
| 00:08 | 17′ | 강의: 기능 쪼개기, MUST/NICE, 캡스톤 규칙 | 슬라이드 4–7 |
| 00:25 | 10′ | 테마 갤러리 + 선택 가이드 | 슬라이드 8 |
| 00:35 | 15′ | 실습 ①: 종이 계획서 작성 (+스케치 2분) | 워크시트 Step 1 |
| 00:50 | 15′ | 실습 ②: Plan 모드로 AI와 계획 다듬기 + **강사 범위 승인 순회** | 워크시트 Step 2 |
| 01:05 | 35′ | 실습 ③: Build 모드 전환 → v0 생성 → CHECK/FIX | 워크시트 Step 3 |
| 01:40 | 20′ | 30초 피치(계획 공유) + 내일 예고 | 슬라이드 14–15 |

## 진행 대본

### 1) 오프닝 (8′)

- 복습 한 번: Golden Rules 3개 복창.
- 선언. "For two days, you built MY missions. From today — **your app, your idea.** On Friday, you present it."

### 2) 강의: 앱은 기능 목록이다 (17′) — 슬라이드 4–7

- **분해 시연**: "Food Menu App"을 보드/슬라이드에서 해부한다. 겉보기엔 마법 같지만 실은: ① 메뉴+가격 보여주기 ② 카테고리로 거르기 ③ 담은 것 합계 내기. "Every app = a list of small features."
- **기능 문장 공식**: "User can ___." 한 문장으로 안 써지면 아직 기능이 아니라 소원이다. 나쁜 예: "User can do everything about food"(너무 큼) → 좋은 예: "User can see 10 menu items with prices."
- **MUST 3 + NICE 2**: 왜 제한하나 — 남은 시간은 이틀이고, "small and FINISHED beats big and broken."
- **캡스톤 규칙** (슬라이드 7을 그대로 읽기): 파일은 `index.html` 하나 / 서버·로그인·외부 API 금지 / localStorage(브라우저 저장)는 허용 / 금요일에 2분 데모.

### 3) 테마 갤러리 (10′) — 슬라이드 8

6개 테마를 한 줄씩 소개(여행 가이드 / 음식 메뉴판 / 동아리 소개 / 라오스 퀴즈 / 용돈 기록장 / 플래시카드). 선택 기준 제시: "**Pick something your family or friends could actually use.** 그게 발표 때도 제일 재밌다." 자유 주제는 규칙(단일 파일·서버 금지) 안에서 허용 — 단, Step 2에서 강사 승인 필수.

### 4) 실습 운영 (총 65′)

- **Step 1 — 종이 계획서 (15′)**: 워크시트에 앱 이름 / 누가 쓰나 / MUST 3("User can ___" 형식 강제) / NICE 2 / 화면 스케치(네모와 글자면 충분, 2분). 종이에 먼저 쓰게 하는 이유: AI에게 말 걸기 전에 자기 생각이 있어야 대화가 산으로 안 간다.
- **Step 2 — Plan 모드 (15′)**: **Tab을 눌러 Plan 모드로** (우하단 표시 확인시키기 — 화면 크게 보여줄 것). Plan에서는 AI가 파일을 만들지 않고 대화만 한다. 워크시트 프롬프트로 계획 검증: 

```text
I want to build ___ (app name) for ___ (who).
It is ONE file: index.html. No server, no login.
MUST features:
1. User can ___
2. User can ___
3. User can ___
Is this a good plan for 2 days? What should I build first?
```

  AI의 제안(순서·주의점)을 워크시트에 메모. **이 시간에 강사는 전원 순회하며 계획서에 승인 사인**을 한다(아래 스코프 다이어트 참고). 사인 없이 Step 3 진입 금지.
- **Step 3 — v0 생성 (35′)**: **Tab으로 Build 모드 복귀 확인 후** v0 요청: 앱 이름·레이아웃·MUST 1번 기능 하나만. 워크시트 템플릿 제공. CHECK → FIX 1~2회. 목표 상태: "제목이 보이고, 첫 기능이 어설프게라도 동작한다."

### 5) 30초 피치 (20′)

전원 기립, 순서대로 30초: "My app is ___. It is for ___. It can ___, ___, and ___." 인원이 많으면 4인 조 내 공유 후 조별 1명 전체 발표. 박수 필수. 마무리: "Tomorrow is Build Day. 2 hours, 3 features. Sleep well."

## 스코프 다이어트 (범위 승인 기준) — 오늘의 핵심 업무

| 학생이 가져온 것 | 문제 | 다이어트 처방 |
|---|---|---|
| 친구와 채팅 앱 | 서버 필요 | "메시지 메모 보드(내 브라우저에만 저장)"로 전환 |
| 로그인/회원가입 | 서버·보안 | 시작 화면에서 이름만 입력받아 "Hello, ___!" 표시로 대체 |
| 실시간 지도/날씨 | 외부 API | 고정 이미지+목록, 또는 도시별 정보 카드로 대체 |
| 쇼핑몰(결제까지) | 결제 불가 | 장바구니 담기 + 합계 표시까지로 컷 |
| 사진 업로드 공유 | 서버 필요 | 이모지/기본 이미지 선택으로 대체 |
| MUST가 4개 이상 | 시간 부족 | 3개로 컷, 나머지는 NICE로 강등. "NICE는 못 해도 수료" |

판정 기준 한 줄: **"단일 index.html + localStorage로 이틀 안에 되는가?"** 애매하면 줄인다. 학생이 아쉬워하면 "버전 2는 캠프 끝나고 만들자"로 명분을 준다.

## 예상 질문·상황 대응

| 상황/질문 | 대응 |
|---|---|
| Plan 모드인 채 "파일이 안 만들어져요" | 우하단 모드 표시 확인 → Tab으로 Build 복귀. 오늘 가장 흔한 사고 — 순회 시 첫 확인 항목 |
| 아이디어가 없다는 학생 | 테마 6개 중 "가족이 쓸 만한 것" 고르게. 그래도 막히면 음식 메뉴판(구조가 가장 단순) 배정 |
| AI가 Plan 대화에서 기능을 잔뜩 불려놓음 | "AI는 신나서 부풀린다. 결정은 네가. MUST 3개만 남겨" — Golden Rule 3 연결 |
| 두 학생이 같은 테마 | 문제없음. "같은 테마, 다른 앱이 나오는 게 바이브 코딩의 재미" |
| v0부터 화려하게 꾸미려 함 | "내일 기능 먼저, 꾸미기는 금요일 오전에 시간 따로 있다" |
| Day 1–2 결석자 | 5분 브리핑(루프·규칙 2개·치트시트) 후 바로 계획서부터. 테마는 단순한 것 권장 |

## 화이트보드 백업 (정전·프로젝터 불능 시)

보드에: `App = list of features` / `User can ___.` / `MUST 3 + NICE 2` / 규칙 3줄(one file / no server·login·API / localStorage OK) / 테마 6개.

## 슬라이드 구성 (slides/day3.html, 15장)

| # | 슬라이드 | 핵심 내용 |
|---|---|---|
| 1 | 타이틀 | Day 3: From Idea to Plan 💡 |
| 2 | Recap | 3 Golden Rules 복창 슬라이드 |
| 3 | Big news | "Today we start YOUR app." (Mon–Tue: my missions → Wed–Fri: YOUR app, Friday: present) |
| 4 | Apps = features | Food Menu App 분해 그림: ①see menu ②filter ③total |
| 5 | Feature sentence | "User can ___." 공식 + too big vs just right 예시 |
| 6 | MUST 3 + NICE 2 | "Small and finished beats big and broken." |
| 7 | The rules | ONE file index.html / no server·login·external API / localStorage OK / 2-min demo Friday |
| 8 | Theme gallery | 6테마 카드 + "or your own idea (within the rules)" + "pick what family/friends could use" |
| 9 | Step 1 | Paper plan: name / who / MUST 3 / NICE 2 / sketch |
| 10 | Plan mode | NEW TOOL: press Tab → Plan. "AI talks, does not build." 우하단 표시 그림 |
| 11 | Plan talk | Plan 대화 프롬프트 템플릿 (워크시트와 동일) |
| 12 | Back to Build | "Press Tab again!" → v0 = title + layout + first MUST feature |
| 13 | v0 mission | v0 요청 템플릿 + "CHECK in browser before anything else" |
| 14 | Pitch | 30-second pitch 공식: My app is _ / for _ / it can _,_,_ |
| 15 | Tomorrow | Build Day 예고: "2 hours. 3 features. You can do it." |

## 워크시트 매핑 (handouts/day3-worksheet.md)

Step 1 계획서 양식(앱이름/누가/MUST 3 "User can" 빈칸/NICE 2/스케치 박스/**강사 승인 사인란**) → Step 2 Plan 모드 안내(Tab)+대화 프롬프트+AI 제안 메모칸 → Step 3 Build 복귀+v0 프롬프트 템플릿 → 체크포인트(사인 받음/v0 브라우저 동작/피치 완료) → 출구: 내일 첫 스프린트에서 만들 기능 1개 적기.
