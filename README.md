# Vue.js 공부
고양이도 할 수 있는 Vue.js 책 참고

## 기본적인 옵션 구성
```
var app = new Vue({
  1. el - 마운트할 요소
  el: '#app',         
  
  2. data - 데이터 
  data: {             
    message: 'Vue.js'
  },
  
  3. computed - 산출 속성
  computed: {
    computedMessage: function() {
      return this.message + '!'
    }
  },
  
  4. created - 라이프 사이클 훅
  created: function() {
    하고 싶은 처리
  },
  
  5. methods - 메서드
  methods: {
    myMethod: function() {
      하고 싶은 처리
    }
  }
})
```
