# -SBAR-
담낭절제술 후 임상간호 판단 및 SBAR 보고 시뮬레이션

## Room of Errors — WebXR 프로토타입

시뮬레이션테크놀로지Ⅱ 2조 (오선영 · 이새롬 · 황인경) 중간보고서 기반.

| 파일 | 설명 |
|---|---|
| `RoomOfErrors_WebXR.html` | 실행용 전체 소스 (HTML + CSS + JavaScript 모듈). Three.js 0.160.0을 jsDelivr CDN에서 불러옴 |
| `artifact-index.html` | Claude 아티팩트 게시용 본문 (doctype/head 없는 버전, 내용 동일) |

### 실행
- PC: `RoomOfErrors_WebXR.html`을 브라우저로 열기
- VR(HMD): HTTPS로 호스팅(GitHub Pages 등) 후 Quest 브라우저에서 열고 상단 "VR 시작"
  - 트리거: 선택·바닥 순간이동 / 스틱 좌우: 회전 / 그립: 메뉴

### 구현 범위
- E1~E8 오류 탐지(근거 선택)·교정, 위양성 감점
- 시간 앵커 2·3·5·8·10분: 보호자 등장, 통증 트랙, 출혈 트랙, 8분 중증 악화·낙상 위험, Time-out
- NPC: 환자·보호자·담당의(전화)·인계 간호사, 음성(TTS) 선택
- SBAR 보고 → 구두처방 read-back → 수액 bolus → 부분 회복
- 6-1 정량 평가(65+35점, 가산·감점, 통과 조건), 4-2 탐색 지표, 로그 JSON
