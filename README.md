# 인터넷 기초[04] 과제2 - 나만의 인공지능 서비스

## 개요
 - 서비스 명 : <span style="background-color:rgb(182,0,80)">ROCK IS MY LIFE</span>
 - 서비스 설명 : 사용자로부터 **기분**이나 듣고 싶은 노래의 **분위기**를 입력받으면, <span style="background-color:rgb(182,0,80)">ROCK IS MY LIFE</span>는 해당 곡을 추천해준다.
 - 서비스 접속 주소 : [주소압력](여기도똑같은주소)


## 서비스 구성 요소(1) - Gemini API
- <span style="background-color:rgb(182,0,80)">ROCK IS MY LIFE</span>가 추천하는 곡들은 구글의 LMM 모델인 Gemini의 API를 활용해 생성한다.
- 활용 모델 : [Gemini-2.0-flash](https://cloud.google.com/vertex-ai/generative-ai/docs/models/gemini/2-0-flash?hl=ko)
- 시스템 프롬프트 주안점
  - 인공지능에게 오랜 락덕후라고 역할을 부여했다.
  - 입력 받은 분위기를 짧게 요약하게 함.
  - 곡 설명은 하지 않고 가수와 제목만 간단히 말하게 했다.

## 서비스 구성 요소(2) - 프론트엔드
- <span style="background-color:rgb(182,0,80)">ROCK IS MY LIFE</span> 서비스 페이지는 HTML, CSS을 사용하여 간단하게 구성하였다.
- CSS 스타일 시트는 [style.css](style.css)파일로 따로 분리하였다.
- 평소에 좋아하던 이미지를 병렬로 배치하였다.<br>
<div class="image-box">
  display: flex;
  justify-content: center;
  gap: 1.5rem;
  <img src="MusicIsMyLife.jpg" alt="Jazz is my life" />
  <img src="RockForYourSoul.jpeg" alt="Rock for your soul" />
</div>