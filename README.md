# KOGAMES 브랜드 페이지

GitHub Pages로 무료 상시 호스팅되는 정적 웹사이트입니다. 서버가 필요 없습니다.

- 주소: https://spicerpon.github.io/
- 수정한 파일을 이 저장소에 커밋하면 1~2분 뒤 자동으로 반영됩니다.

## 파일 구성

| 파일 | 주소 | 내용 |
|---|---|---|
| `index.html` | `/` | KOGAMES 회사 홈 — 영어(기본) |
| `star-miner/index.html` | `/star-miner/` | Star Miner 앱 홈페이지 (**OAuth 동의 화면의 홈페이지 URL**) |
| `privacy/index.html` | `/privacy/` | 개인정보처리방침 — 영어 |
| `terms/index.html` | `/terms/` | 이용약관 — 영어 |
| `ko/…` | `/ko/…` | 위 4개 페이지의 한국어판 (같은 구조) |
| `ja/…` | `/ja/…` | 위 4개 페이지의 일본어판 (같은 구조) |
| `assets/style.css` | | 전체 디자인 (색상은 맨 위 `:root` 변수만 바꾸면 됨) |
| `404.html` | | 없는 주소 접속 시 화면 |

## 수정하는 법

**가장 쉬운 방법 (웹에서 바로):** GitHub 저장소에서 파일을 열고 ✏️(Edit) 버튼 → 수정 → `Commit changes`.

**언어별 파일:** 영어는 최상위 폴더, 한국어는 `ko/`, 일본어는 `ja/` 폴더에 같은 이름으로 있습니다. 내용을 고칠 때는 세 언어 파일을 함께 고쳐주세요.

**자주 바꿀 곳**
- 게임 추가: 각 언어의 `index.html`에서 `<article class="game">` 블록 하나를 복사해 내용만 변경
- 색상: `assets/style.css` 맨 위 `--accent`, `--bg` 등
- 개인정보처리방침: 실제로 쓰지 않는 SDK(Firebase, Unity Ads 등)는 표에서 행 삭제, 시행일 변경
- 이메일 변경: 모든 파일에서 `spicerpon@gmail.com` 검색 후 교체

## Google OAuth 브랜딩 인증 입력값 (star-miner-464706)

| 항목 | 값 |
|---|---|
| 앱 이름 | `Star Miner` (← `star-miner/index.html`의 `<title>`, `<h1>`과 일치해야 함) |
| 사용자 지원 이메일 | `spicerpon@gmail.com` |
| 애플리케이션 홈페이지 | `https://spicerpon.github.io/star-miner/` |
| 개인정보처리방침 링크 | `https://spicerpon.github.io/privacy/` |
| 서비스 약관 링크 | `https://spicerpon.github.io/terms/` |
| 승인된 도메인 | `spicerpon.github.io` |

승인된 도메인은 Google Search Console에서 `https://spicerpon.github.io/` (URL 접두어 속성)로 소유권 확인이 되어 있어야 하며,
확인한 Google 계정이 Cloud 프로젝트의 소유자/편집자여야 합니다.
HTML 파일 인증을 쓰면 Google이 준 `googleXXXX.html` 파일을 이 저장소 최상단에 올리면 되고, 이 파일은 지우면 안 됩니다.
