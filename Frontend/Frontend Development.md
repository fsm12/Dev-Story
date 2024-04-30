마지막 학습 날짜 : 2024.04.30.

</br></br>

# Frontend Development

### keyword 정리부터

***SFC (Single File Component)*** : Vite를 이용한 CLI 환경  

</br>

***SPA (Single Page Application)*** : 페이지 하나로 구성된 웹 어플리케이션
ㄴ 화면이 바뀌는 것이 아닌, 미리 화면을 만들어놓고(Component) 특정 부분에 바꿔서 보여줌
ㄴ 화면은 만들어져 있는데 데이터가 없는 형태이므로, 비동기통신인 Axios

***참고) 비동기 HTTP 통신 종류***  
- XHR을 이용한 Ajax 비동기 통신
- Fetch
- 서브파티 라이브러리 중 Axios, jQuery  

</br>

***Router*** : 페이지를 이동 X, 주소에 해당하는 Component를 특정 위치에 시각화   

***Pinia*** : 중앙저장소  

</br></br>
<hr/>

### vue.js 세팅하자

***[vscode]***  
visual studio code Version 1.88.1 이상 설치    
(`Help` - `About` - `Version` 1.88.1 이상인지 확인)   

</br>

***[Extension]***  
Vue - Official
Vue 3 Snippets (자동완성)

</br>

`File` - `Preference` - `Configure User Snippets` - `vue 검색` + Enter - 아래 코드를 가장 바깥 중괄호 안에 작성
``` vue
"Generate Vue3 Option API Code": {
  "prefix": "vue3-option",
  "body": [
    "<script>\nexport default {\n\tname: \"\",\n\tcomponents: {},\n\tdata() {\n\t\treturn {\n\t\t\tmessage: '',\n\t\t};\n\t},\n\tmethods: {},\n};\n</script>\n\n<template>\n\t<div>\n\n\t</div>\n</template>\n\n<style scoped>\n\n</style>"
  ],
  "description": "Generate Option Vue3 Code"
  },
  "Generate Vue3 Composition API script setup Code": {
  "prefix": "vue3-<script setup>",
  "body": [
    "<script setup>\n\n</script>\n\n<template>\n\t<div>\n\t\t\n\t</div>\n</template>\n\n<style scoped>\n\n</style>"
  ],
  "description": "Generate Composition Vue3 <script setup> Code"
  },
  "Generate Vue3 Composition API script() Code": {
  "prefix": "vue3-setup()",
  "body": [
    "<script>\nexport default {\n\tname: \"\",\n\tcomponents: {},\n\tsetup() {\n\t\t\n\t\treturn {};\n\t}\n};\n</script>\n\n<template>\n\t<div>\n\n\t</div>\n</template>\n\n<style scoped>\n\n</style>"
  ],
  "description": "Generate Composition Vue3 setup() Code"
  }
```
`.vue` 확장자인 파일에서 `vue`를 입력하면 자동완성이 될 것.

***[nodejs.org]***

- nodejs.org 검색창에 입력 후 LTS 버전 다운로드 (기본설정)   
- Window + R(cmd) -> `node -v`, `npm -v` 두 명령어 입력시 버전이 나오면 환경 세팅 Success




