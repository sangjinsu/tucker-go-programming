# 25장 채널과 컨텍스트

## 채널

- 채널은 고루틴끼리 메시지를 전달할 수 있는 메시지 큐
- 채널 기본 크기는 0이다

### close()

- 채널을 닫아준다
- 좀비 고루틴: 채널을 닫아주지 않아서 무한 대기를 하는 고루틴을 좀비 고루틴 또는 고루틴 릭(누수)이라고 한다.

### Select 문

- 여러 채널에서 동시에 데이터를 기다릴 때 사용한다

### 채널로 생산자/소비자 패턴 구현

### 컨텍스트

- 작업을 지시할 때 작업 가능 시간, 작업 취소 등의 조건을 지시할 수 있는 작업 명세서 역할

### 채널로 발행/구독 패턴 구현

- 옵저버 패턴
- 구독 패턴 pub/sub