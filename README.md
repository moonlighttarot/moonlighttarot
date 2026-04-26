# 🌙 달빛 타로 · Moonlight Tarot

웹 기반 타로 카드 리딩 PWA. 3개의 덱을 지원합니다.

## 🃏 덱 구성

- **유니버설 웨이트** (78장) — 정/역방향 해석
- **심볼론** (78장) — Problem/Way/Outcome 3단계 해석
- **로맨스 엔젤** (44장) — 사랑과 관계의 오라클

## ✨ 기능

- 1장·2장·3장 카드 뽑기
- 3D 카드 플립 애니메이션
- PWA 지원 (홈 화면에 추가, 오프라인 사용 가능)
- 카드 데이터를 외부 JSON 파일로 분리하여 실시간 수정 가능

## 📁 폴더 구조

```
.
├── index.html          사이트 본체
├── manifest.json       PWA 매니페스트
├── sw.js               서비스 워커 (캐시 관리)
├── README.md           이 파일
├── data/
│   ├── waite.json      웨이트 78장 데이터
│   ├── symbolon.json   심볼론 78장 데이터
│   └── romance.json    로맨스 엔젤 44장 데이터
└── icons/
    ├── icon-192.png    PWA 아이콘 192x192
    └── icon-512.png    PWA 아이콘 512x512
```

## 🛠 카드 해석 수정 방법

**방법 1 — GitHub 웹사이트에서 직접 편집 (가장 쉬움)**

1. GitHub에 접속해서 이 저장소로 이동
2. `data/` 폴더 클릭
3. 수정하고 싶은 파일 클릭 (예: `symbolon.json`)
4. 오른쪽 위 연필 아이콘(✏️ Edit) 클릭
5. 원하는 카드 해석 텍스트 수정
6. 페이지 아래 "Commit changes" 버튼 클릭
7. 1~2분 후 사이트에 자동 반영됨

사용자는 같은 주소로 새로고침만 하면 최신 내용이 보입니다.

**방법 2 — 컴퓨터에서 편집**

1. JSON 파일을 다운로드
2. 메모장이나 VS Code 등으로 열어 수정
3. GitHub에 다시 업로드

## 📜 출처

- **심볼론 카드 해석**: Peter Orban · Ingrid Zinnel · Thea Weller (Switzerland) 공식 가이드북
- **한글 번역**: 클림 트윈스타 · 박은영 (blog.naver.com/twinstar430)

본 프로젝트는 위 한글 번역본을 기반으로 재구성한 학습·상담 보조 도구입니다.
