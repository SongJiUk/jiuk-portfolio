# 송지욱 (Jiuk Song) — Unity 게임 개발자 포트폴리오

> **GitHub Pages:** https://songjiuk.github.io/jiuk-portfolio
> **Notion CV:** https://www.notion.so/273ea58668dd80769e87e65dcd3aca42
> **Email:** wldnr1014@naver.com

---

## 소개

Unity / C# 기반 게임 클라이언트 개발자입니다.
모바일 방치형 RPG 1인 개발 경험, 도담게임즈 실무 경험, UniTask · ObjectPool · ScriptableObject 등 현대적인 Unity 패턴을 적용한 프로젝트들을 포트폴리오로 정리했습니다.

---

## 프로젝트

### ⚔️ 모바일 방치형 RPG `2025.11 ~ 2026.03` · 1인 개발
Firebase Auth, UniTask, IAP/AdMob 등 실서비스 수준 SDK를 직접 연동한 1인 개발 방치형 RPG.
자동 전투·강화·던전·가챠 등 핵심 콘텐츠 구현.

- **기술:** Unity C#, Firebase, UniTask, IAP, AdMob, Data-Driven(구글시트→JSON)
- **플랫폼:** Android / iOS

---

### 🔫 탑다운 슈팅게임 `2025.05 ~ 06` · 1인 개발
탕탕특공대 모작. 오브젝트 풀링, 데이터 기반 설계, 로그라이크 스킬 진화 시스템 구현.

- **기술:** Unity C#, ObjectPool, Data-Driven, ITickable 커스텀 Update
- **플랫폼:** PC / Mobile
- **GitHub:** https://github.com/SongJiUk/likeTangTang

---

### 🤝 3D RPG 협업 프로젝트 `2023.09 ~ 11` · 3인 팀
3인 팀 협업 3D RPG. 몬스터 AI를 제외한 게임 시스템 전반 담당(기여도 약 90%).
GameManager·SceneManager·SoundManager 등 핵심 매니저 구현, 팀 통합 관리.

- **기술:** Unity C#, Singleton, PlayerPrefs, JSON, Git 협업
- **플랫폼:** PC
- **GitHub:** https://github.com/SongJiUk/Project

---

### 🎯 도담게임즈 · 실무 `2022.03 ~ 2023.05`
모바일 매치3 퍼즐 게임 클라이언트 개발. Unity 기반 신규 콘텐츠 기획·개발 및 유지보수 담당.

- **기술:** Unity C#, 모바일 최적화
- **플랫폼:** Android / iOS

---

### 🏢 Prison Life `2026.03 ~ 04` · 1인 개발 ★ LATEST
광석 채굴부터 수감자 수용까지 자동화되는 아이들 경영 시뮬레이션.
UniTask async/await 기반 NPC 자동화, IHandCuff 인터페이스 설계, DOTween 스폰 연출.

- **기술:** Unity C#, UniTask, DOTween, ScriptableObject, ObjectPool
- **플랫폼:** PC
- **GitHub:** https://github.com/SongJiUk/AssignmentGame
- **Notion:** https://www.notion.so/341ea58668dd819fa009eec04dd07362

---

### 🏰 3D RPG 개인 프로젝트 `2021.05 ~ 10` · 1인 개발
로그라이크 형식의 3D RPG. 퀘스트·상점·인벤토리·씬 전환 시스템 구현.

- **기술:** Unity C#, ObjectPool, 퀘스트 시스템, PlayerPrefs
- **플랫폼:** PC

---

## 기술 스택

| 분야 | 기술 |
|------|------|
| 엔진 | Unity 2022.3 LTS |
| 언어 | C# 9.0+ |
| 비동기 | UniTask |
| 외부 SDK | Firebase, IAP, AdMob |
| 데이터 | ScriptableObject, Data-Driven (구글시트→JSON) |
| 최적화 | ObjectPool, ITickable 커스텀 Update |
| 연출 | DOTween |
| 버전관리 | Git / GitHub |

---

## 포트폴리오 구조

```
jiuk-portfolio/
├── index.html      # 전체 사이트 (CSS + JS 인라인)
├── images/         # 프로젝트 스크린샷
│   ├── IdleRPG/
│   ├── TopDownShooting/
│   ├── 3DRPG_Solo/
│   └── 3DRPG_Team/
└── README.md
```

- 빌드 도구 없음 — 단일 HTML 파일
- Canvas 기반 픽셀맵 인터랙티브 (WASD 이동)
- GitHub Pages 호스팅
