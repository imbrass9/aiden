<picture>
  <source media="(prefers-color-scheme: dark)" srcset="docs/banner.svg">
  <img src="docs/banner.svg" alt="AIDEN Skills" width="100%">
</picture>

<p align="center">
  <strong>클로드 코드(AI 코딩·업무 조수)로 1인 사업을 굴리는, 에이든의 실전 스킬 모음</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/for-Claude_Code-blueviolet?style=for-the-badge" alt="Claude Code">
  <img src="https://img.shields.io/badge/언어-한국어-2ea44f?style=for-the-badge" alt="한국어">
  <img src="https://img.shields.io/badge/by-트리오브에이와-1f2328?style=for-the-badge" alt="트리오브에이와">
</p>

<p align="center">
  <a href="#-이게-뭔가요">이게 뭔가요?</a> &bull;
  <a href="#-스킬-지도">스킬 지도</a> &bull;
  <a href="#-무슨-스킬이-있어요">스킬 목록</a> &bull;
  <a href="#-어떻게-써요">사용법</a> &bull;
  <a href="#-누가-만들었어요">만든 곳</a>
</p>

---

## 🧭 이게 뭔가요?

**클로드 코드**를 처음 켜면, 시키는 일은 잘하지만 "내 사업을 어떻게 굴려야 하는지"는 모르는 똑똑한 신입과 같습니다.

이 저장소는 에이든이 **1인 콘텐츠 사업을 실제로 굴리면서 만든 스킬들**을 한자리에 모아, 클로드 코드가 그 사업 감각을 그대로 익히게 하는 지도입니다. 스킬 하나하나가 "이럴 땐 이렇게 하라"는 작업 절차예요 — 방향 잡기, 고객 반응 검증, 화면 설계, 반복 작업 자동화까지.

> 💡 **스킬(skill)이란?** 클로드 코드가 특정 상황에서 꺼내 쓰는 작업 설명서입니다. "코어 잡아줘"라고 말하면 코어를 세우는 절차가 자동으로 로드돼요. 외우게 하는 게 아니라, **필요할 때 펼쳐 보게** 하는 방식입니다.

이 링크는 에이든이 **클로드 코드를 멘토링할 때 멘티에게 건네는 한 장짜리 자료**입니다. 각 스킬 페이지는 입문자도 따라 읽을 수 있게 한글로 풀어 썼습니다.

---

## 🗺 스킬 지도

스킬들은 **하나의 흐름**으로 이어집니다. 생각을 명료하게 만드는 데서 시작해, 코어를 세우고, 반응을 검증하고, 채널로 내보내는 순서입니다.

```mermaid
flowchart LR
    subgraph 방향잡기
        CLR["aiden-clarify<br/><sub>생각 명료화</sub>"]
        CORE["aiden-core<br/><sub>코어 잡기</sub>"]
    end
    subgraph 검증·설계
        RXN["reaction-lab<br/><sub>가상 고객 반응</sub>"]
        CONV["conversion-architect<br/><sub>전환 설계</sub>"]
    end
    subgraph 생산·발행
        OSMU["osmu · channel-composer<br/>newsletter-engine<br/><sub>채널 분화·발행</sub>"]
        SEO["search-optimizer<br/><sub>검색·AI 노출</sub>"]
    end

    CLR --> CORE --> RXN --> CONV --> OSMU --> SEO

    HT["humantouch-writing<br/><sub>사람이 쓴 글로</sub>"] -.글 검수.-> OSMU
    WF["wireframe-first<br/><sub>화면 설계</sub>"] -.화면 작업.-> OSMU

    style CLR fill:#2ea44f,color:#fff
    style CORE fill:#2ea44f,color:#fff
    style RXN fill:#e3b341,color:#1f2328
    style CONV fill:#e3b341,color:#1f2328
    style OSMU fill:#d1584f,color:#fff
    style SEO fill:#d1584f,color:#fff
```

<sub>🟢 이 저장소에 페이지가 있는 공개 스킬 &nbsp;·&nbsp; 🟡 검증·설계 &nbsp;·&nbsp; 🔴 발행 엔진(코호트에서 전체 제공)</sub>

---

## 📦 무슨 스킬이 있어요?

각 이름을 누르면 그 스킬의 한글 설명 페이지로 갑니다.

### 방향을 잡는다
| 스킬 | 한 줄 | 이럴 때 |
|---|---|---|
| [**aiden-clarify**](skills/aiden-clarify/README.md) | 흐릿한 생각·요청·결정을 명료하게 | "머릿속이 복잡해", "이거 어떻게 말하지" |
| [**aiden-core**](skills/aiden-core/README.md) | 사업의 코어(재료 + 본질)를 인터뷰로 세움 | "뭘 팔지 모르겠어", "코어 잡아줘" |

### 만들기 전에 점검한다
| 스킬 | 한 줄 | 이럴 때 |
|---|---|---|
| [**virtual-customer-feedback-qa**](skills/virtual-customer-feedback-qa/README.md) | 가상 고객 100만 명에게 미리 반응·사용성 점검 | "이 가격이면 살까", "어디서 막힐까" |
| [**wireframe-first**](skills/wireframe-first/README.md) | 화면 작업은 살아있는 와이어프레임 승인부터 | "대시보드 만들자", "화면 설계" |

### 반복 작업을 자동화한다
| 스킬 | 한 줄 | 이럴 때 |
|---|---|---|
| [**shorts-factory**](skills/shorts-factory/README.md) | 롱폼 1개를 세로 쇼츠로 잘라 예약 업로드까지 | "쇼츠로 잘라줘" |
| [**search-optimizer**](skills/search-optimizer/README.md) | 검색·AI가 내 글을 찾고 인용하게 만드는 구조 | "SEO", "AI 검색에 뜨게" |

### 스킬 자체를 다룬다 (멘토용)
| 스킬 | 한 줄 | 이럴 때 |
|---|---|---|
| [**skill-forge**](skills/skill-forge/README.md) | 스킬을 만들·다이어트·평가하는 메타 스킬 | "이거 스킬로 만들어줘" |
| [**skill-scrap**](skills/skill-scrap/README.md) | 깃허브에서 본 스킬을 스크랩·검색·공유 | "이 스킬 저장해줘" |
| [**finalize-propagate**](skills/finalize-propagate/README.md) | "이걸로 확정"하면 관련 문서 전부에 반영 | "최종으로 저장해" |

### 맛보기
| 스킬 | 한 줄 | 비고 |
|---|---|---|
| [**humantouch-writing**](skills/humantouch-writing/README.md) | AI 티를 지우고 사람이 쓴 글로 | 원리 공개, 엔진은 코호트 |

> 🔴 **발행 엔진**(osmu · channel-composer · newsletter-engine · conversion-architect)은 실제 사업의 수익 구조라, 공개 대신 **부트캠프·컨설팅 코호트에서 전체를 제공**합니다.

---

## 🚀 어떻게 써요?

### 1. 스킬을 클로드 코드에 넣습니다
쓰고 싶은 스킬 폴더를 스킬 폴더(`~/.claude/skills/`) 아래에 두면 끝입니다. 아래는 `aiden-core` 예시이고, 폴더 이름만 바꾸면 다른 스킬도 같습니다.

**Mac / Linux** <sub>(Apple Silicon·Intel 공통 — 파일 복사라 칩과 무관)</sub>
```bash
mkdir -p ~/.claude/skills
git clone https://github.com/imbrass9/aiden.git
cp -r aiden/skills/aiden-core ~/.claude/skills/
```

> 칩(Apple Silicon / Intel)이 실제로 갈리는 스킬은 `shorts-factory` 하나입니다 — 전사 엔진이 다릅니다. 나머지는 파일을 복사하는 것뿐이라 칩과 무관합니다.

**Windows (PowerShell)**
```powershell
New-Item -ItemType Directory -Force "$env:USERPROFILE\.claude\skills" | Out-Null
git clone https://github.com/imbrass9/aiden.git
Copy-Item -Recurse aiden\skills\aiden-core "$env:USERPROFILE\.claude\skills\"
```

각 스킬 페이지에도 같은 Mac·Windows 설치법이 들어 있습니다.

### 2. 그냥 말을 걸면 됩니다
스킬은 상황을 알아서 감지합니다. "코어 잡아줘"라고 하면 `aiden-core`가 켜져요. 각 페이지의 **"이렇게 부르면 됩니다"** 부분을 참고하세요.

---

## 👤 누가 만들었어요?

**에이든** — 콘텐츠 사업화 컨설턴트. 자기 이야기로 혼자서도 굴러가는 사업을 설계하고, 그 사업이 스스로 돌아갈 시스템까지 직접 만듭니다. 이 스킬들은 전부 그 과정에서 실제로 쓰던 것들입니다.

- 트리오브에이와

> 내 것을 꺼낼수록, 더 많은 것이 돌아옵니다.

---

## 라이선스

각 스킬 폴더의 라이선스를 따릅니다. 별도 표기가 없으면 MIT.
