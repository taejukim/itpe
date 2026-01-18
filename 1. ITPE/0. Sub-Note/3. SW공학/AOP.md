#정보관리기술사
#SW공학 #프로그래밍

- [ ] 1회
- [ ] 2회
- [ ] 3회
- [ ] 4회
- [ ] 5회

## 정의
AOP(Aspect-Oriented Programming)
횡단 관심사를 분리하여 모듈화하는 프로그래밍 패러다임, AOP
- 로깅, 보안, 트랜잭션 등 여러 모듈에 걸쳐 반복되는 횡단 관심사를 별도로 분리하는 기법
- 핵심 비즈니스 로직과 횡단 관심사를 분리하여 코드의 재사용성과 유지보수성을 향상

## 구성요소
- Aspect: 횡단 관심사를 모듈화한 단위
- Join Point: Aspect를 적용할 수 있는 프로그램 실행 지점
- Pointcut: Join Point를 선택하는 표현식
- Advice: Join Point에서 실행될 코드
- Weaving: Aspect를 대상 코드에 적용하는 과정
- 횡단 관심사: 로깅, 보안, 트랜잭션, 예외 처리 등 여러 모듈에 공통으로 필요한 기능

## 구성도
핵심 비즈니스 로직 + 횡단 관심사 → AOP 적용 → Aspect 분리 → Weaving → 통합된 코드

## 키워드
- Aspect, Join Point, Pointcut, Advice, Weaving, 횡단 관심사

## 암기법
- 아조포어위횡: Aspect, Join Point, Pointcut, Advice, Weaving, 횡단 관심사

핵심관심사 Core concern
횡단 관심사 crosscutting concern
위빙
126p.
![[Pasted image 20260117191942.png]]