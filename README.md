# 한국 전통무용 이미지 생성 AI 평가

이미지 생성 AI 8종이 한국 전통무용 22개 종목을 그릴 때 의상·소품·동작을 맞게 그리는지, 중국·일본 요소가 섞이는지 확인하는 측정입니다. 평가는 AI가 아니라 전통무용 전문가가 이미지마다 의견을 다는 방식으로 합니다.

**갤러리:** https://kloud80.github.io/korea-dance-image-eval/

## 측정 방법

- 종목 22개: 부채춤, 장고춤, 태평무, 일무(종묘제례), 승무, 살풀이춤, 처용무, 학무, 향발무, 교방굿거리춤, 춘앵전, 무산향, 진주검무, 한량무, 진도북춤, 소고춤, 강강술래, 입춤, 바라춤, 화관무, 삼고무, 오고무
- 프롬프트: 종목 이름만 넣은 한 문장 × 3개 언어(한국어·영어·중국어) = 66개
  - 예: "한국 전통무용 살풀이춤 공연" / "A performance of Salpuri-chum, a Korean traditional dance" / "韩国传统舞蹈 Salpuri-chum 的表演"
- 모델 8종: Google Nano Banana 2.1, OpenAI GPT Image 2.6, xAI Grok Imagine 2.0, Meta Muse Image, MiniMax H3, Alibaba Qwen Image 3 Pro, ByteDance Seedream 5.5, Black Forest Labs Flux 3
- 공통 조건: 가로 3:2, 약 1K 해상도, 프롬프트마다 1장, 프롬프트 자동 보강 끔
- 평가: 전통무용 전문가(박사과정 수료)가 이미지마다 전체 의견과 부분 의견(영역 표시)을 남김

## 진행 상황

- 2026-11-15: 22개 종목 × 3개 언어 × 8개 모델 이미지 공개. 전문가 검토 진행 예정.
- (이전 8개 종목·4개 언어 파일럿은 내렸습니다.)

## 파일

- `index.html`: 갤러리
- `data/images.json`: 이미지별 모델·프롬프트·언어·시드
- `images/`: 공개용 WebP (긴 변 1024px)

## 라이선스

프롬프트, 데이터, 페이지는 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.ko)입니다.
이미지는 각 회사의 AI가 생성한 것이며 실제 공연 사진이 아닙니다. 이미지 이용 조건은 생성한 각 회사의 약관을 따릅니다.
