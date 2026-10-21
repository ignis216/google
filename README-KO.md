# 학회 포스터 실험 자극 시연 페이지 (정적 HTML)

## 구성
실험 1: Google AI Overview 6개, Gemini 6개 (총 12개)
실험 2: Google AI Overview 3개, Gemini 3개 (총 6개)
총 18개 자극과 QR 연결용 선택 페이지 4개, 전체 메뉴 1개.

## GitHub Pages 배포
1. GitHub에서 공개 저장소를 새로 만들고 이 ZIP을 컴퓨터에서 정상적으로 검사한 뒤 압축을 해제합니다.
2. 폴더 `poster_demo_clean_2026` 안의 **내용 전체**를 새 저장소의 최상단(root)에 업로드합니다. (폴더 한 겹을 더 만들지 않습니다.)
3. 저장소의 Settings → Pages → Build and deployment → Deploy from a branch → main / (root)를 선택합니다.
4. 배포 주소 `https://계정명.github.io/저장소명/`가 활성화되면 아래 네 URL을 각각 QR로 변환합니다.

- 실험 1 Google AI Overview: `https://계정명.github.io/저장소명/experiment1/google/`
- 실험 1 Gemini: `https://계정명.github.io/저장소명/experiment1/gemini/`
- 실험 2 Google AI Overview: `https://계정명.github.io/저장소명/experiment2/google/`
- 실험 2 Gemini: `https://계정명.github.io/저장소명/experiment2/gemini/`

* 사용자명과 저장소명이 아직 제공되지 않아 실제 QR 이미지는 포함하지 않았습니다.
* URL을 실제 배포 후 확인하고 QR을 생성하세요. QR의 링크는 인쇄하기 전에 반드시 실물 스마트폰으로 검사하세요.

## 보안 · 구현 정보
- 이전 ZIP 아카이브, 이전 빌드 스크립트 및 그 자산을 재사용하지 않았습니다.
- 업로드된 HTML 자극을 바탕으로 18개 모두 새로 생성했습니다.
- 원본에 포함된 실험 로그 수집, PsychoJS 연동, 부모 창 postMessage, iframe 제거 스크립트는 제거했습니다.
- 사용자가 보는 자극의 본문과 정·오답 차이, 검색/추천어/결과 인터랙션은 유지하도록 재구현했습니다.
- Gemini 원본의 중복 Base64 PNG는 별도의 검증된 정적 PNG 파일 하나로 추출했습니다.
- 실험 자극 화면에는 시연용 `자극 목록` 링크와 모바일 레이아웃 수정만 추가했습니다.
- HTML, CSS, JS(HTML 내부), PNG, README, SHA256SUMS.txt 파일만 포함합니다. 실행 파일이나 빌드 스크립트는 없습니다.
- 악성코드 탐지 소프트웨어로 검증한 결과는 아닙니다. 안전성을 보장하지 않으며, 탐지 경고가 다시 표시되면 열거나 배포하지 말고 격리하세요.

## 모바일 확인
- iPhone Safari, Android Chrome 등 실제 기기에서 검색어 입력 → 결과 표시 → `자극 목록` 복귀를 점검하세요.
- QR과 모바일 기기의 화면 차이로 원래 데스크톱 실험 화면과 시각적 배치가 달라질 수 있습니다.
- 각 데모는 실제 AI 모델과 통신하지 않고 미리 정해진 응답을 보여줍니다.
