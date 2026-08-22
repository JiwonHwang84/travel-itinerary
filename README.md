# travel-itinerary

단일 HTML 파일로 만든 정적 페이지를 GitHub Pages로 호스팅하는 저장소입니다.
빌드 도구나 의존성 설치가 필요 없습니다.

## 호스팅

https://jiwonhwang84.github.io/travel-itinerary/

`main` 브랜치 루트를 그대로 배포합니다. push하면 1~2분 내에 반영됩니다.

## 구성

| 경로 | 설명 |
|---|---|
| `index.html` | 배포되는 페이지. 이 파일 하나에 마크업·CSS·스크립트가 모두 들어 있습니다 |
| `archive/` | 이전 버전 보관 |
| `source/` | 작업용 원본 파일 |

외부 리소스는 CDN에서 불러옵니다 — Leaflet(지도), Font Awesome(아이콘), Google Fonts.
지도 타일 요청이 실패하면 대체 타일 서버로 순차 폴백하고, 모두 실패하면 안내 배너를 띄웁니다.

## 수정 방법

```bash
git add index.html
git commit -m "..."
git push
```

반영이 안 보이면 브라우저 강력 새로고침(`Cmd+Shift+R)
