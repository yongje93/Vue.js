## 가상돔 (Virtual DOM)
브라우저는 html을 읽어서 DOM 트리, CSS 트리를 만들고 DOM이 화면에 있어야할 위치를 잡고 내용을 채운다.  
브라우저는 실시간 DOM 수정요청으로 그림을 다시 그리는데, 그닥 효율적이지 못하다.  
-> 이러한 브라우저의 단점을 도와주는 것이 **가상돔 (Virtual DOM)**  

### 특징
- HTML DOM의 추상화 개념
- 바인딩한 데이터를 기반으로 만들어짐
- DOM 노드와 마찬가지로 '가상노드'라고 부르는 노드로 이루어진 트리구조
- 변경사항을 가상의 위치에서 처리하고 실제 DOM의 조작을 최소화
- 웹페이지의 변경 속도를 매우 빠르게 해줌
