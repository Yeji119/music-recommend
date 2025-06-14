# 🎸 나만의 인공지능 서비스 과제2 - [ROCK IS MY LIFE]

## 🧠 프로젝트 개요

- **서비스명:** ROCK IS MY LIFE  
- **기능 설명:**  
  사용자가 기분이나 원하는 분위기를 입력하면,  
  🎸 락 음악 추천 전문 AI_가 어울리는 락 음악 3곡을 추천해줍니다.  
- **접속 링크:** [https://yeji119.github.io/music-recommend/](https://yeji119.github.io/music-recommend/)

---

## 🔌 인공지능 API 구성

본 서비스는 **Google Gemini API**를 활용하여 락 음악을 추천합니다.

- **사용 모델:** [Gemini 2.0 Flash](https://cloud.google.com/vertex-ai/generative-ai/docs/models/gemini/2-0-flash?hl=ko)
- **프롬프트 설계 전략:**
  - Gemini에게 **오랜 경력의 락 덕후** 역할을 부여
  - 입력된 분위기를 짧고 핵심적으로 요약
  - 추천 곡은 설명 없이 **제목 + 가수 이름만 간결하게** 안내

---

## 💻 프론트엔드 구성

- 서비스 페이지는 HTML과 CSS을 사용하여 구성되었습니다.
- 스타일 시트는 별도의 [`style.css`](style.css) 파일로 분리하였습니다.
- 사용자 입력 후 결과는 실시간으로 출력됩니다

---

## 🛠️ 서비스 구성 요소 (3) - 백엔드

- 프론트엔드에서 직접 Gemini API 키가 노출되지 않도록,  
  **사용자 입력을 받아 대신 Gemini API를 호출해주는 간단한 백엔드**를 구성했습니다.
- 해당 백엔드는 **Vercel의 Serverless Function** 기능을 이용해 배포하였습니다.
- 전체 구현 코드는 GitHub 저장소에서 확인할 수 있습니다:  
  🔗 [https://github.com/Yeji119/music-recommend-api](https://github.com/Yeji119/music-recommend-api)