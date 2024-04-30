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

</br></br>
<hr/>

### 프론트엔드는 뭘 하나?

***Frontend Development*** : 웹사이트와 어플리케이션의 사용자 인터페이스(UI; 디자이너)와 사용자 경험(UX; 퍼블리셔)을 만들고 디자인 하는 것으로, 개발자는 HTML, CSS, JavaScript 등을 활용해 사용자가 직접 상호작용하는 부분을 개발한다.

***Client-side frameworks*** : Vue.js나 React.js, Angular는 클라이언트 측에서 UI와 상호작용을 개발하기 위해 사용되는 JavaScript 기반 프레임워크
ㄴ Spring은 Server-side framework라 함

</br></br>
<hr/>

### 그런데 HTML, CSS, JS도 있는데 굳이 Client-side frameworks가 필요한가?  
필요한 이유에 대해서는 아래 몇가지가 있다.

1. 웹에서 하는 일이 전에비해 많아짐. (정보를 얻기만 했던 곳이 아님)
2. 웹에서 다루는 데이터가 많아짐. => 애플리케이션의 상태를 변경할 때마다 일치하도록 UI를 업데이트 해야함

</br>

***SPA (Single Page Application)*** : 페이지 하나로 구성된 웹 어플리케이션으로, 웹 애플리케이션의 초기 로딩 후 새로운 페이지 요청 없이 동적으로 화면을 갱신하여 사용자와 상호작용하는 웹 어플리케이션 

</br>

***CSR; Client Side Rendering 방식*** : Server로부터 Client는 모든 HTML코드를 받고, Client가 데이터 변경이 필요하면 Server에게 Ajax 통신을 하고 JSON 형태로 응답값을 받아 페이지 일부를 갱신

참고) SPA의 반대인 MPA(Multi Page Application)은 SSR 방식으로 통신함

***[CSR 장점]***  
1. 속도가 빠름 bc) 서버로 전송되는 데이터의 양을 최소화   
2. 네이티브 앱과 유사한 사용자 경험을 제공   
3. FE와 BE의 명확한 분리  

***[CSR 단점]***  
1. 초기 구동속도가 느림 : JavaScript가 다운, 분석 및 실행될 때까지 페이지가 완전히 렌더링 되지 않음  
2. SEO(Search Engine Optimize) 문제 : 페이지를 나중에 만들기도 해서 검색에 노출이 쉽지 않을 수 있음   


