<template>
  <router-view />
</template>

<script>
export default {
  name: 'App',
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;300;400;500;700;900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@100;300;400;500;700;900&display=swap');

html,
body,
#app {
  font-family: 'Noto Sans KR', 'Roboto', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  width: 100%;
  height: 100%;
}

/* reset css */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
button {
  background-color: transparent;
  border: none;
  cursor: pointer;
}
a,
img,
fieldset {
  text-decoration: none;
  vertical-align: top;
  outline: 1;
  border: none;
}
ul,
ol,
li {
  list-style: none;
}
textarea {
  resize: none;
}

/* 전역 공통 클래스 */
/* 하이라이팅 */
mark {
  background-color: #00ffc2 !important;
  color: #006850 !important;
  font-weight: bold;
  padding: 0 2px;
}

/* 한 줄 생략 (...) */
.ellipsis__1 {
  display: -webkit-box !important;
  -webkit-line-clamp: 1; /* 줄 수를 여기서 조절 */
  -webkit-box-orient: vertical;
  overflow: hidden;
  text-overflow: ellipsis;
}

/* 여러 줄 생략 (...) — 기본 두 줄 */
.ellipsis__2 {
  display: -webkit-box !important;
  -webkit-line-clamp: 2; /* 줄 수를 여기서 조절 */
  -webkit-box-orient: vertical;
  overflow: hidden;
  text-overflow: ellipsis;
}

/* scroll reset */
.scroll_area::-webkit-scrollbar-thumb {
  background-color: #babac0;
  border-radius: 16px;
}
/* 스크롤바 막대 설정*/
.scroll_area::-webkit-scrollbar-thumb {
  background-color: #babac0;
  border-radius: 16px;
}
.scroll_area::-webkit-scrollbar-thumb:hover {
  background-color: #a0a0a5;
}

/* 스크롤바 뒷 배경 설정*/
.scroll_area::-webkit-scrollbar-track {
  border-radius: 10px;
  background-color: transparent;
}
.scroll_area::-webkit-scrollbar-track:hover {
  background-color: transparent;
}
.scroll_area::-webkit-scrollbar-button {
  display: none;
}
</style>
