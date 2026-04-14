# jiuk-portfolio

송지욱(Jiuk Song)의 Unity 게임 개발자 포트폴리오 사이트.

## 프로젝트 개요

- **타입**: 단일 파일 HTML 포트폴리오 (`index.html`)
- **호스팅**: GitHub Pages (`SongJiUk/jiuk-portfolio`)
- **언어**: HTML / CSS / Vanilla JS (빌드 도구 없음)
- **이미지**: `images/` 폴더 (GitHub raw URL로 로드)

## 파일 구조

```
jiuk-portfolio/
├── index.html      # 전체 사이트 (CSS + JS 인라인)
├── images/         # 프로젝트 스크린샷
│   ├── IdleRPG/
│   ├── TopDownShooting/
│   ├── 3DRPG_Solo/
│   └── ...
└── README.md
```

## 주요 섹션

| 섹션 | 설명 |
|------|------|
| `#hero` | 이름, 역할, 기술 칩, 버튼 |
| `#explorer` | 픽셀맵 인터랙티브 캔버스 (WASD 이동, 구역별 패널) |
| `#works-section` | 프로젝트 카드 그리드 (`PROJECTS` 배열 기반 렌더링) |
| `#skills-section` | 기술스택 바 (`SKILLS` 배열 기반 렌더링) |
| `#about-section` | 자기소개 + 터미널 스타일 profile.json |
| `#contact-section` | 이메일 / GitHub / Notion 링크 |

## 콘텐츠 수정 가이드

### 프로젝트 추가/수정

`index.html` 내 `PROJECTS` 배열 (약 470번째 줄)에서 수정:

```js
{
  id: 'project-id',       // 고유 ID
  name: '프로젝트명',
  emoji: '⚔️',
  subtitle: '기간 설명',
  color: '#f5c842',        // 카드 포인트 색상
  zoneColor: 0xd4a800,     // 픽셀맵 구역 색상
  year: '2025',
  platform: 'Android / iOS',
  duration: '5개월',
  isLatest: true,          // 최신 배지 여부
  shortDesc: '한 줄 설명',
  desc: '상세 설명',
  systems: [               // 핵심 시스템 목록
    { icon: '🔐', name: '시스템명', desc: '설명' }
  ],
  codeSnippets: [          // 코드 스니펫 (HTML 태그 포함)
    { title: '제목', file: 'File.cs', code: `...` }
  ],
  tags: ['Unity', 'C#'],  // 기술 태그
  github: null,            // 또는 URL
  youtube: 'https://...',
  images: ['https://raw.githubusercontent.com/...'],  // GitHub raw URL
  zoneX: 4, zoneY: 4, zoneW: 8, zoneH: 7,            // 픽셀맵 구역 위치
  tileTheme: 'castle'     // 픽셀맵 타일 테마
}
```

### 스킬 추가/수정

`SKILLS` 배열에서 수정:

```js
{ name: 'Unity', pct: 90, color: '#a78bfa' }
```

### 이미지 추가

1. `images/{프로젝트폴더}/` 에 파일 추가
2. GitHub에 push
3. `PROJECTS` 배열의 `images` 필드에 GitHub raw URL 추가

## 디자인 토큰

```css
--bg: #080814       /* 가장 어두운 배경 */
--gold: #f5c842     /* 강조 골드 */
--cyan: #00d4ff     /* 시안 */
--purple: #a78bfa   /* 보라 (주 포인트) */
--coral: #ff6b6b    /* 코랄 */
```

폰트: `Press Start 2P` (픽셀), `Inter` (본문), `JetBrains Mono` (코드)

## 개발 시 주의사항

- 빌드 도구 없음 — 브라우저에서 직접 열어서 확인
- 모든 CSS·JS가 `index.html` 한 파일에 인라인으로 존재
- 픽셀맵은 `<canvas>` 기반, 순수 JS로 렌더링
- 이미지는 GitHub raw URL 사용 (로컬 경로 사용 시 GitHub Pages에서 깨짐)
- 모바일 대응: 900px 이하 미디어쿼리로 처리됨

## 연락처

- Email: wldnr1014@naver.com
- GitHub: https://github.com/SongJiUk
