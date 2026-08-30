## breath024

로컬 LLM과 자동화 도구를 주로 만듭니다. 웹·안드로이드·데이터 파이프라인까지
필요한 만큼 직접 짭니다.

아래 프로젝트는 대부분 저장소를 열어뒀습니다. 업무로 만든 것과
개인 데이터가 섞인 것만 비공개입니다.

---

### AI 시스템

[COMET](https://github.com/breath024/comet) · 2026-03 ~ · Python · 10,300줄
로컬에 상주하는 개인 비서. 질문마다 큰 모델을 부르면 느리고 아까워서
앞에 문지기 모델을 두고 등급을 나눠 보냅니다(12b / 26b MoE).
무거운 등급은 쓰고 나면 바로 VRAM에서 내려서 16GB 한 장을 돌려씁니다.
웹검색·종목분석·재무·시세·화면인식·텔레그램·상주 데몬까지 붙어 있습니다.

**MMOFM** · 2026-08 ~ · Python · 6,600줄
대화가 쌓여서 인격이 되는 기억 시스템. 요약으로 압축하지 않고 노트로 쌓아 태그로 분류합니다.
만들면서 제일 오래 붙잡은 건 AI 티였는데, 원인이 말투가 아니라 리듬이었습니다.
노트 373장을 세보니 지시문은 바로 밑에 깔린 자기 직전 답 6개한테 지고 있었고,
프롬프트 대신 출력 쪽에 길이·지문·어휘 반복 게이트를 달아서 잡았습니다.

[PROMETHEUS](https://github.com/breath024/prometheus) · 2026-08 ~ · Python
위 엔진을 복사하지 않고 환경변수로 갈라 쓰는 두 번째 인격체.
시간이 지나면 혼자 상태가 변하고, 돌보지 않으면 그게 말투에 실립니다.

### 도구

[HELM](https://github.com/breath024/helm) · 2026-08 · Python, JS · 4,800줄
Claude Code 세션 여러 개를 한 창에서 탭·분할로 다루는 데스크톱 앱.
앞서 만든 버전은 conhost 창을 띄워 Win32로 겹쳐놓는 방식이라 계속 싸웠는데,
ConPTY로 직접 물고 xterm.js로 그리게 바꿔서 찾을 창도 벗길 테두리도 없앴습니다.

[QALens](https://github.com/breath024/qalens) · 2026-08 · Python · 2,700줄
파일 종류를 판별해 정적 분석과 브라우저 런타임 검사를 같이 돌리는 QA CLI.

[ContentForge](https://github.com/breath024/contentforge) · 2026-06 ~ · Python · 2,200줄
주제 한 줄을 넣으면 카드뉴스를 만들어내는 앱.

[에이전트 관리 콘솔](https://github.com/breath024/claude-agent-console) · 2026-06 ~ · Python · 3,100줄
AI 콘솔 여러 개를 한 화면에서 만들고 전환하는 tkinter 앱. HELM의 전신입니다.

### 트레이딩

**coin-bot** · 2026-06 ~ · Python · 5,100줄
손으로 하던 선물 매매 규칙을 코드로 옮긴 것. 진입은 되는데 청산 규율이 안 지켜져서,
나가는 일을 봇에게 맡기는 쪽으로 만들었습니다. 백테스트와 모의투자 포함.

[stock-bot](https://github.com/breath024/stock-bot) · 2026-05 ~ · Python
국내 주식 자동매매와 가상매매.

### 웹

[Only Money](https://github.com/breath024/only-money) · 2026-06 ~ · 단일 HTML · 10,600줄 — 투자 대시보드
[중국어 SRS](https://github.com/breath024/chinese-srs) · 2026-05 ~ · 단일 HTML · 5,100줄 — 회화 중심 학습앱, 데이터 팩 분리
[AURA](https://github.com/breath024/aura) · 2026-06 · Three.js — 스크롤에 따라 카메라가 전진하는 3D 데모

---

라이브러리와 빌드 산출물을 뺀 순수 작성 코드 기준입니다.
업무로 만든 것들은 여기 없습니다.
