# dam-operations · 운영 레이어 + 엔진 6서버

K-water 수자원 자동화 — **dam-operations** MCP 운영 레이어 아키텍처를 한눈에 보는 단일 페이지.

👉 **[페이지 보기 — eum-jium.github.io/dam-operations-map](https://eum-jium.github.io/dam-operations-map/)**

## 담긴 내용

- **운영 레이어 · 20 도구** — 3 영역(치수 / 이수 / 개발) × (분석 도구 + 조회 도구). 한국어 기능명 + 실제 함수명 보조 표기.
- **엔진층 · 6 서버 (82 도구)** — GIS(`dam-preprocessing`)가 상류에서 DEM→유역·하천·CN·제원 합성 → 강우-유출(`dam-hms`) → 저수지(`dam-reservoir`) → 하천 수리(`dam-ras`) 모델 체인 + 관측(`dam-observation`)·지식(`dam-knowledge`) 입력.
- **GIS 자료 Tier** — 한국: 정밀토양도(농진청)+토지피복도(환경부) / 글로벌: GCN250(HWSD 기반, 인증 불필요). 글로벌 자료만으로 합천 NSE 0.779로 정밀자료(0.740) 능가.

전부 결정론(AI 0), Qwen 오케스트레이션. 외부 의존성 없는 자기완결 HTML 1개.
