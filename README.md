# GDGoC INHA 팀 프로젝트 핸드북

부원들에게 공유하는 핸드북 사이트입니다. Vercel로 자동 배포됩니다.

## 구조

| 파일 | 내용 |
|---|---|
| `index.html` | 핸드북 본문 전체 (6개 파트 · 28개 장) |
| `script.html` | 1~3파트 발표 대본 (85분 기준) |
| `img/` | 본문에 들어가는 스크린샷 |

## 고치는 법

1. 이 레포를 clone 하거나, GitHub 웹에서 바로 편집합니다.
2. `index.html`을 엽니다. 한 장(chapter)은 `<article class="chapter" id="c-...">` 하나입니다.
   - 예: 깃허브 파트의 브랜치 장은 `id="c-g-branch"`
   - 장 안의 한 절은 `<section class="csec" id="g-branch-1">` 입니다.
3. 고친 뒤 **새 브랜치에서 PR**을 올립니다. main에 직접 push 하지 않습니다.
4. main에 머지되면 Vercel이 자동으로 다시 배포합니다.

## 스타일 규칙

본문에서 자주 쓰는 클래스입니다. 새 문단을 넣을 때 그대로 따라 쓰면 디자인이 유지됩니다.

- `<p class="lead">` — 장 도입 문단
- `<ul class="bullets">` — 점 목록
- `<div class="callout">` — 강조 박스 (`callout warn` 주의, `callout ok` 권장)
- `<div class="g-step">` — 따라 하기 단계 (번호 + 설명 + 스크린샷)
- `<span class="ic">` — 버튼·메뉴 이름, `<code>` — 명령어·코드

## 이미지 추가

`img/` 에 넣고 `<img src="img/파일명">` 으로 참조합니다.
