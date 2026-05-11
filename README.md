# 🏋️ TRAINER SIMULATOR

> 현실 기반 퍼스널 트레이너 & 러닝 코치 인터랙티브 시뮬레이션 게임

Claude AI가 게임 마스터가 되어 실제 현장처럼 까다롭고 현실적인 회원들과 함께하는 트레이너 시뮬레이터입니다.

---

## 스크린샷

| 메뉴 | 게임 진행 |
|------|--------|
| 모드 & 난이도 선택 | 회원 상황 & 선택지 |

---

## 게임 모드

| 모드 | 설명 |
|------|------|
| 💪 PT 회원 모드 | 체지방 감량, 근력, 통증 회원 관리 |
| 🏃 러닝 코칭 모드 | 케이던스, 심박수, 레이스 전략 코칭 |
| 🦴 체형 교정 모드 | 자세 교정, 불균형, 재활 케어 |
| 🔥 컴플레인 대응 모드 | 환불, 불만, 감정적 회원 처리 |

## 난이도

- 🟢 **EASY** — 협조적인 회원
- 🟡 **NORMAL** — 현실적인 반응
- 🟠 **HARD** — 예민하고 까다로운 회원
- 🔴 **EXTREME** — 최악의 시나리오

---

## 실행 방법

### 방법 1: GitHub Pages (추천)

1. 이 저장소를 **Fork** 합니다
2. 저장소 `Settings` → `Pages` → **Branch: main / folder: / (root)** 설정
3. 몇 분 후 `https://<username>.github.io/<repo-name>/` 접속

### 방법 2: 로컬 실행

```bash
git clone https://github.com/<username>/trainer-simulator.git
cd trainer-simulator

# Python으로 로컬 서버 실행
python3 -m http.server 3000

# 브라우저에서 열기
open http://localhost:3000
```

> **주의:** `index.html`을 파일로 직접 열면 (`file://`) CORS 오류가 발생합니다. 반드시 서버를 통해 접속하세요.

---

## API 키 설정

게임 실행 시 Anthropic API 키가 필요합니다.

1. [console.anthropic.com](https://console.anthropic.com) 에서 키 발급
2. 게임 첫 화면에서 `sk-ant-...` 형식으로 입력
3. 키는 **브라우저 메모리에만 저장**되며 외부로 전송되지 않습니다

---

## 기술 스택

- **Frontend:** Vanilla HTML / CSS / JavaScript (의존성 없음)
- **AI Engine:** Anthropic Claude claude-sonnet-4-20250514 API
- **배포:** GitHub Pages (정적 호스팅)

---

## 파일 구조

```
trainer-simulator/
└── index.html     # 게임 전체 (단일 파일)
└── README.md      # 이 파일
```

---

## 라이선스

MIT License
