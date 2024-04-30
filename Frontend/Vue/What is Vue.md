마지막 학습 날짜 : 2024.04.30.

</br></br>

# What is Vue
[공식문서](https://ko.vuejs.org/guide/introduction)를 참고하는 습관을 들이자!

### Vue가 뭐길래
: 사용자 인터페이스를 구축하기 위한 JavaScript 프레임워크

***[핵심기능]***
1. 선언적 렌더링(Declarative Rendering): Vue는 표준 HTML을 템플릿 문법으로 확장하여 JavaScript 상태(State)를 기반으로 화면에 출력될 HTML을 선언적(declaratively)으로 작성할 수 있음
2. 반응성(Reactivity): JavaScript 상태(State) 변경을 추적하고, 변경이 발생하면 DOM을 효율적으로 업데이트


</br>

### CDN에서 Vue 사용하기
[공식문서 참고](https://ko.vuejs.org/guide/quick-start.html#using-vue-from-cdn)

#### 1. 스크립트 태그

아래의 script 코드를 html의 <head> 태그 내에 삽입   

```
<script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
```

``` html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Vuejs</title>
  <!-- 아래에 삽입 -->
  <script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
</head>
<body>
  
</body>
</html>
```
