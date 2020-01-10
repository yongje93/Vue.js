# Vue.js 공부
고양이도 할 수 있는 Vue.js 책 참고  
https://rintiantta.github.io/jpub-vue/

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

1. el : 애플리케이션 인스턴스를 적용할 요소 (선택자 형태로 지정)
2. data : 애플리케이션에서 사용할 데이터 (객체 또는 배열로 지정)
3. computed : 함수로 인해 산출되는 데이터
4. created : 라이프 사이클 훅 중 하나. 인스턴스가 생성되고, 리액티브 초기화가 일어난 후 자동 호출
5. methods : 애플리케이션에서 사용할 메서드
