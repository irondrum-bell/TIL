# 큐

## 개요
- 양 방향에서 모두 데이터에 접근 가능한 선형 자료구조이다.
- 한 쪽에선 삽입연산만 가능하고 다른 쪽에서는 삭제 연산만 가능하다.
- 삽입과 삭제가 서로 다른 위치에서 일어나기 때문에 먼저 저장된 데이터가 먼저 출력되는 선입선출(FIFO: First In First Out) 방식이다.
- enqueue: 큐에 새로운 데이터를 저장. 지원하는 언어에 따라 pop이라고도 한다.
- dequeue: 큐에서 가장 먼저 저장된(오래된) 데이터를 반환하고 삭제.  
![큐 삽입/삭제 연산 예시](https://upload.wikimedia.org/wikipedia/commons/d/d3/Fifo_queue.png)  
(출처: Wikipedia - https://en.wikipedia.org/wiki/FIFO_(computing_and_electronics))
- 큐의 변형된 형태로 양 방향 모두에서 삽입/삭제 연산이 가능한 데크(Deque: Double-ended queue)가 있다.  
![데크 예시](https://www.tutorialandexample.com/wp-content/uploads/2019/09/Deque-in-Java.png)  
(출처: Tutorial And Example - <https://www.tutorialandexample.com/deque-in-java/>)

### 장점
1. 데이터의 순차적인 접근
    - 선입선출 구조이기 때문에 저장된 순서대로 접근이 가능하다.

### 단점
1. 추가 메모리 필요
    - 양 방향에서 모두 데이터를 관리하기 위해 두 개의 포인터가 필요하다.
2. 메모리 낭비
    - 직접 구현하거나 배열 형태로 구현된 큐의 경우 생성할 때 크기를 지정해야 하므로 사용하지 않는 저장공가니 낭비될 수 있다.

## 정리
- 운영체제의 프로세스 작업 스케쥴링에 주로 사용된다.
