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

## 리액티브 데이터
Vue.js에서 추출했을 때(get)와 설정했을 때(set), 훅(hook) 처리가 등록되어 반응하는 데이터  
### 리액티브 시스템
단순한 DOM 변경뿐만 아니라 DOM 변경을 최적화하고, 데이터를 동기화하고, 변경을 감지하는 기능 등을 모두 포함한 것  
### 리액티브 데이터 정의
컴포넌트의 data 옵션에 문자열 또는 객체 등의 데이터를 정의하면, 인스턴스 생성 때 모두 리액티브 데이터로 변환됨
