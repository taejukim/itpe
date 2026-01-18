=======================
AOP(Aspect Oriented Programming)

#정보관리기술사 #SW공학 #관점지향

- [ ] 1회
- [ ] 2회
- [ ] 3회
- [ ] 4회
- [ ] 5회

## 정의
횡단 관심사를 분리하여 모듈성을 높이는 프로그래밍 패러다임, 관점지향 프로그래밍
- 비즈니스 로직(Core Concern)과 공통 기능(Cross-cutting Concern)을 분리하여 관리
- 로깅, 보안, 트랜잭션 등 여러 모듈에 흩어진 중복 코드를 별도의 '관점(Aspect)'으로 모듈화함

## 구성요소
- Aspect: 횡단 관심사를 모듈화한 것 (Advice + Pointcut)
- Join Point: Advice가 적용될 수 있는 지점 (메서드 호출, 필드 변경 등)
- Pointcut: Join Point 중 실제로 Advice가 적용될 지점을 선별한 것
- Advice: 특정 Join Point에서 실행되는 실제 액션 (코드)
- Weaving: 비즈니스 코드에 Aspect를 결합하여 실행 가능한 코드로 만드는 과정
- Target: Aspect가 적용되는 대상 객체

## 구성도 요소
* 아키텍처: 핵심 로직(수직)을 관통하는 횡단 관심사(수평)의 분리 구조
* 관계: OOP의 모듈화를 보완하여 코드의 가독성과 유지보수성 극대화
```
[Svc A] [Svc B] [Svc C]
   |       |       |
---+-------+-------+--- [Logging Aspect]
---+-------+-------+--- [Security Aspect]
```

## 키워드
* 횡단 관심사, 분리(Separation), Aspect, Weaving, 프록시(Proxy)

## 암기법
* 횡단관심사 (여러 모듈을 가로지르는 공통 기능)
* 애조포위 (Aspect, Joinpoint, Pointcut, Weaving)
