# 한국사 4,000년

**v1.0.0** · Last updated 2026-05-19

중학생을 위한 한국사 통사 학습 사이트. GitHub Pages 배포용 정적 HTML 사이트.

> 한 아버지가 자녀에게 물려주려고 만든 학습 자료입니다.
> 사실의 정확성, 균형 잡힌 시각, 학습자의 호기심을 자극하는 깊이를 모두 갖추도록 만들고 있습니다.

## 사이트 보기

**🌐 https://messfilm.github.io/korean-history/**

로컬에서 보려면 `index.html`을 브라우저로 열거나, 디렉토리에서 간단한 정적 서버를 띄우면 됩니다.

```bash
# 예: Python 3 내장 서버
cd korean-history
python3 -m http.server 8080
# 그리고 http://localhost:8080 접속
```

## 구성

- **9개 시대로 나눈 한국사 통사** — 선사·고조선 → 삼국·가야 → 남북국 → 고려 → 조선 전기 → 조선 후기 → 개항기 → 일제강점기 → 분단과 대한민국
- **사이트 내 검색** — 인물·사건·제도·유물을 한글·한자로 부분일치 검색
- **용어집 hover 팝업** — 본문의 점선 단어 위에 마우스를 올리면 작은 카드 설명
- **SVG 시각 자료** — 통합 연표, 시대별 시기 도식 등
- **한국 전통 미감** — 한지·먹·오방색 기반 디자인 시스템, Noto Serif KR·Cormorant Garamond 조판

## 진행 상황

- [x] 메인 페이지 (`index.html`)
- [x] 시대 페이지 — § I 선사·고조선 (`eras/01-prehistoric.html`)
- [x] 시대 페이지 — § II 삼국·가야 (`eras/02-three-kingdoms.html`)
- [x] 시대 페이지 — § III 남북국 (`eras/03-north-south.html`)
- [x] 시대 페이지 — § IV 고려 (`eras/04-goryeo.html`)
- [x] 시대 페이지 — § V 조선 전기 (`eras/05-joseon-early.html`)
- [x] 시대 페이지 — § VI 조선 후기 (`eras/06-joseon-late.html`)
- [x] 시대 페이지 — § VII 개항기·대한제국 (`eras/07-modern-opening.html`)
- [x] 시대 페이지 — § VIII 일제강점기 (`eras/08-japanese-colonial.html`)
- [x] 시대 페이지 — § IX 분단과 대한민국 (`eras/09-republic.html`)
- [x] **9개 시대 모두 1차 완성** (2026.5)
- [ ] 시대 페이지 — § VI 조선 후기
- [ ] 시대 페이지 — § VII 개항기·대한제국
- [ ] 시대 페이지 — § VIII 일제강점기
- [ ] 시대 페이지 — § IX 분단과 대한민국

## 학설 처리

논쟁점이 있는 부분(예: 묘청의 난 평가, 식민지 근대화론 vs 수탈론, 단군 신화의 역사성 등)은 한쪽으로 단정하지 않고
주요 학설 갈래를 양립 서술합니다. 각 시대 페이지의 **§.9 학설 갈래** 섹션에서 확인할 수 있습니다.

## 파일 구조

```
korean-history/
├── index.html                       메인 (Hero + 통합 연표 + 9개 시대 카드)
├── README.md                        이 파일
├── eras/
│   ├── 01-prehistoric.html          § I 선사·고조선
│   ├── 02-three-kingdoms.html       § II 삼국·가야
│   ├── 03-north-south.html          § III 남북국
│   ├── 04-goryeo.html               § IV 고려
│   ├── 05-joseon-early.html         § V 조선 전기
│   ├── 06-joseon-late.html          § VI 조선 후기
│   ├── 07-modern-opening.html       § VII 개항기·대한제국
│   ├── 08-japanese-colonial.html    § VIII 일제강점기
│   └── 09-republic.html             § IX 분단과 대한민국
└── assets/
    ├── styles.css                   디자인 시스템 (한지·먹·오방색)
    ├── search.js                    사이트 내 검색
    ├── glossary.js                  용어집 hover 팝업
    ├── glossary-data.json           용어 데이터
    └── search-index.json            검색 인덱스
```

외부 의존성은 **Google Fonts CDN뿐**입니다. 모든 경로는 상대경로로 작성되어 서브디렉토리 배포에서도 동작합니다.

## 참고 출처

- [국사편찬위원회 한국사데이터베이스](https://db.history.go.kr/)
- [한국학중앙연구원 한국민족문화대백과사전](https://encykorea.aks.ac.kr/)
- [우리역사넷](https://contents.history.go.kr/) (국사편찬위원회 대중용)
- [동북아역사재단](https://www.nahf.or.kr/)

## 면책

이 사이트는 학습 보조 자료입니다. 학술적·법적 인용은 원전을 직접 참고하시기 바랍니다.
콘텐츠는 검정 교과서와 위 출처를 종합해 정리한 것이며, 시대마다 학설 갈래가 다양함을 함께 기억해 주세요.

## 라이선스

- 콘텐츠 — [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) (학습 자료 공유 목적)
- 코드 — MIT
