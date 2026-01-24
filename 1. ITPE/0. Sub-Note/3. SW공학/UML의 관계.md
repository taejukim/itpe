=======================
UML의 관계(UML Relationship)

#SW공학 #UML #모델링

- [ ] 1회
- [ ] 2회
- [ ] 3회
- [ ] 4회
- [ ] 5회

## 정의
UML 요소 간 연결 관계, UML Relationship
- UML 다이어그램에서 클래스, 객체, 컴포넌트 등의 요소들 간의 의미적 연관성을 표현하는 관계
- 연관, 의존, 일반화, 실체화 등의 관계로 시스템 구조와 상호작용을 명확히 표현

## 특징
- 명확성: 요소 간 관계 명시적 표현
- 구조화: 시스템 구조 체계적 표현
- 강도 구분: 관계의 강도 차별화
- 방향성: 단방향/양방향 관계 표현

## 목적
- 클래스 및 객체 간 관계의 명확한 표현
- 시스템 구조와 의존성의 시각화 및 설계 의사결정 지원

## 구성요소
- Association(연관): 클래스 간 구조적 관계, 실선으로 표현
- Aggregation(집합): 전체-부분 관계, 빈 다이아몬드 (부분이 독립적 존재)
- Composition(합성): 강한 집합, 채운 다이아몬드 (부분이 전체에 종속)
- Dependency(의존): 일시적 사용 관계, 점선 화살표
- Generalization(일반화): 상속 관계, 빈 삼각형 화살표
- Realization(실체화): 인터페이스 구현, 점선 + 빈 삼각형
- Multiplicity(다중성): 관계의 개수 (0..1, 1, *, 1..*)
- Directionality(방향성): 단방향/양방향 관계

## 구성도
```
[UML 관계 표기법]

1. Association (연관) - 실선
   ClassA ───────── ClassB

2. Aggregation (집합) - 빈 다이아몬드
   Whole ◇───────── Part
   (자동차 ◇─── 바퀴: 바퀴는 독립적 존재 가능)

3. Composition (합성) - 채운 다이아몬드
   Whole ◆───────── Part
   (집 ◆─── 방: 집이 없으면 방도 없음)

4. Dependency (의존) - 점선 화살표
   ClassA ·········> ClassB
   (ClassA가 ClassB를 일시적 사용)

5. Generalization (일반화/상속) - 빈 삼각형
   Parent △───────── Child
          │
   (동물 △─── 고양이)

6. Realization (실체화) - 점선 + 빈 삼각형
   Interface △·········· Implementation
   (인터페이스를 구현)

[다중성 표기]
1      : 정확히 1개
0..1   : 0개 또는 1개
*      : 0개 이상
1..*   : 1개 이상
m..n   : m개 이상 n개 이하
```

## 키워드
- Association, Aggregation, Composition
- Dependency, Generalization, Realization
- Multiplicity, Directionality
- 연관, 집합, 합성, 의존, 일반화, 실체화

## 암기법
- 관계 6가지: 연집합의일실 (연관-집합-합성-의존-일반화-실체화)
- 강한 순서: 합성 > 집합 > 연관 > 의존
- 집합(◇ 빈것) vs 합성(◆ 꽉찬것)

## 연관 토픽
- [[UML-Diagram 전체]] - UML 전체 개요
- [[Class diagram]] - 클래스 다이어그램에서의 관계 활용
