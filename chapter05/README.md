## 컴포넌트
- Vue.js의 강력한 기능 중 하나는 컴포넌트  
- 기능을 가진 UI 부품별로 템플릿과 자바스크립트를 세트로 묶어, 다른 UI 부품과 분리해서 개발하거나 관리

### 컴포넌트는 설계도
컴포넌트 - 기능을 가지고 있는 HTML 요소의 설계도  
인스턴스 - 설계도를 기반으로 만들어진 실체

### 컴포넌트 정의 방법
- Vue.component 메서드로 전역으로 등록  
```
Vue.component('my-component', {
  template: '<p>myComponent</p>'
})
```

- 로컬에 등록하기
```
var myComponent = {
  template: '<p>myComponent</p>'
}

new Vue({
  el: '#app',
  components: {
    // <my-component>가 루트에서만 사용할 수 있게 됨
    'my-component': myComponent
  }
)}
```

- 컴포넌트의 옵션
```
Vue.component('my-component', {
  // 템플릿
  template: '<p>{{ message }}</p>',
  // 데이터는 객체를 리턴하는 함수로 지정하기
  data: function() {
    return {
      message: 'Hello Vue.js'
    }
  },
  methods: {
    // 메서드, 산출 속성, 워처의 정의 방법은 루트 생성자 객체와 같다
  }
})
```
