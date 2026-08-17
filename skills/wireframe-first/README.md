<p align="center">
  <a href="../../README.md">← 전체 스킬 모음으로</a>
</p>

<h1 align="center">wireframe-first</h1>

<p align="center">
  <strong>화면이 나오는 작업은 구조 먼저, 픽셀 나중</strong><br>
  레퍼런스 → 살아있는 반응형 와이어프레임 승인 → 아웃풋 제작 순서를 강제합니다.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/유형-Claude_Skill-blueviolet?style=for-the-badge" alt="Claude Skill">
  <img src="https://img.shields.io/badge/대상-SaaS·웹·대시보드-2ea44f?style=for-the-badge" alt="화면 작업">
</p>

---

## 한 줄로

> **색이 촌스러운 건 토큰만 바꾸면 되지만, 정보 위계가 틀리면 처음부터입니다.**

그래서 가장 비싼 실수(구조 오류)를 막는 승인 게이트를 맨 앞에 둡니다. 예쁜 화면을 서둘러 만들기 전에, **회색 뼈대**로 구조부터 맞추고 넘어갑니다.

---

## 「살아있는 와이어프레임」이란

일반 목업과 구분되는 형식입니다. 무채색·저충실도까지는 같고, 아래가 다릅니다.

| # | 특징 | 왜 |
|---|---|---|
| 1 | **정지 그림이 아니라 동작한다** | 폭마다 그리지 않고 실제 미디어쿼리 1벌로 짭니다. 그린 그림은 주장, 동작하는 것은 검증 가능한 사실 |
| 2 | **회색인 이유가 다르다** | 예쁘면 구조를 안 보고 통과시키기 때문입니다 |
| 3 | **상태를 형태로 인코딩** | 정상=얇은 실선 / 경고=굵은 테두리 / 미측정=점선. 나중에 시맨틱 컬러의 뼈대가 됩니다 |
| 4 | **더미 데이터로 밀도 표시** | 빈 박스는 표가 8행인지 40행인지 알려주지 않습니다 |
| 5 | **블록마다 질문을 단다** | `요약 타일 ×4 — "오늘 장사 잘 됐나?"`. 답하는 질문을 못 쓰는 블록은 삭제 |

---

## 순서 (건너뛰지 않습니다)

```mermaid
flowchart LR
    R["① 레퍼런스<br/>3~5개 직접 찾아<br/>왜 맞는지 한 줄씩"]
    W["② 와이어프레임<br/>살아있는 반응형·무채색<br/><b>승인받고 넘어감</b>"]
    T["③ 토큰<br/>색 4~6 · 서체 2~3<br/>간격 스케일"]
    B["④ 구현<br/>토큰에서 전부 파생"]
    C["⑤ 검수<br/>375 / 834 / 1440<br/>세 폭 각각 확인"]
    R --> W --> T --> B --> C
    style W fill:#2ea44f,color:#fff
    style C fill:#1f2328,color:#fff
```

②에서 승인이 나기 전에는 코드로 넘어가지 않습니다. 구조가 틀리면 다시 짜는 비용이 가장 큰 지점이기 때문입니다.

---

## 핵심 규칙

- **판단 기준은 생성 비용이 아니라 상대방의 판단 비용입니다.** 그래서 글 목록이 아니라 그림으로 냅니다.
- **0순위는 모든 폭에서 동일해야 합니다.** 폭마다 가장 먼저 읽힐 것이 다르면 같은 화면이 아니라 다른 제품입니다.
- **검수는 눈이 아니라 값으로.** 축소 스크린샷으로 본 것은 "의심"까지고, 판정은 실측(정렬·폭·줄길이·대비·오버플로)으로 합니다.
- **한 벌에서 여러 아웃풋이 파생됩니다.** 웹·HTML·앱·노션이 같은 와이어프레임에서 갈라져 나옵니다.

---

## 설치

**Mac / Linux**
```bash
mkdir -p ~/.claude/skills
git clone https://github.com/imbrass9/aiden.git
cp -r aiden/skills/wireframe-first ~/.claude/skills/
```

**Windows (PowerShell)**
```powershell
New-Item -ItemType Directory -Force "$env:USERPROFILE\.claude\skills" | Out-Null
git clone https://github.com/imbrass9/aiden.git
Copy-Item -Recurse aiden\skills\wireframe-first "$env:USERPROFILE\.claude\skills\"
```

설치 후 클로드 코드를 다시 시작하면 스킬이 로드됩니다.

---

## 이렇게 부르면 됩니다

```
대시보드 만들자
이 화면 구조부터 잡아줘
상세페이지 설계
관리자 화면 UI
와이어프레임 먼저
```
