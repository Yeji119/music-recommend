# 🎸 나만의 인공지능 서비스 과제2 - [ROCK IS MY LIFE]

## 🧠 프로젝트 개요

- **서비스명:** ROCK IS MY LIFE  
- **기능 설명:**  
  사용자가 기분이나 원하는 분위기를 입력하면,  
  🎸 _락 음악 추천 전문 AI_가 어울리는 락 음악 3곡을 추천해줍니다.  
- **접속 링크:** [👉 바로가기](여기도똑같은주소)

---

## 🔌 인공지능 API 구성

본 서비스는 **Google Gemini API**를 활용하여 락 음악을 추천합니다.

- **사용 모델:** [Gemini 2.0 Flash](https://cloud.google.com/vertex-ai/generative-ai/docs/models/gemini/2-0-flash?hl=ko)
- **프롬프트 설계 전략:**
  - Gemini에게 **60년 경력의 락 덕후** 역할을 부여
  - 입력된 분위기를 짧고 핵심적으로 요약
  - 추천 곡은 설명 없이 **제목 + 가수 이름만 간결하게** 안내

---

## 💻 프론트엔드 구성

- UI는 순수 HTML과 CSS만으로 구성되었습니다.
- 스타일 시트는 별도의 [`style.css`](style.css) 파일로 분리하여 관리합니다.
- 사용자 입력 후 결과는 실시간으로 출력되며, 아래 이미지처럼 **락 스피릿이 가득한 시각적 포인트**를 제공합니다:

| ![](MusicIsMyLife.jpg) | ![](RockForYourSoul.jpeg) |
|------------------------|---------------------------|
| Jazz is my life        | Rock for your soul        |

```css
.image-box {
  display: flex;
  justify-content: center;
  gap: 24px;
}
