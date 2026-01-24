=======================
Test Coverage(테스트 커버리지)

#SW공학 #테스트 #품질측정

- [ ] 1회
- [ ] 2회
- [ ] 3회
- [ ] 4회
- [ ] 5회

## 정의
테스트 완전성 측정 지표, 테스트 커버리지
- 테스트가 소프트웨어의 어느 정도를 검증했는지 정량적으로 측정하는 지표
- 코드, 기능, 요구사항 등의 테스트 수행 정도를 백분율로 표현하여 테스트 품질 평가

## 특징
- 정량화: 백분율로 측정 가능
- 객관성: 명확한 기준 제공
- 추적성: 미검증 영역 식별
- 다차원: 다양한 커버리지 유형

## 목적
- 테스트 완전성의 정량적 측정 및 품질 평가
- 미검증 영역 식별로 테스트 계획 개선

## 구성요소
### 코드 커버리지(Code Coverage)
- Statement Coverage(구문): 실행된 코드 라인 비율
- Decision/Branch Coverage(결정/분기): 실행된 분기 비율
- Condition Coverage(조건): 참/거짓 실행된 조건 비율
- Path Coverage(경로): 실행된 경로 비율
- Function Coverage(함수): 호출된 함수 비율

### 기능 커버리지(Functional Coverage)
- Requirement Coverage(요구사항): 검증된 요구사항 비율
- Feature Coverage(기능): 테스트된 기능 비율
- Use Case Coverage(유스케이스): 실행된 시나리오 비율

### 기타 커버리지
- API Coverage: 호출된 API 비율
- UI Coverage: 테스트된 화면 비율
- Data Coverage: 처리된 데이터 케이스 비율

## 구성도
```
[커버리지 계산 공식]

Coverage = (실행된 항목 수 / 전체 항목 수) × 100%

[코드 예시]
1: function divide(a, b) {
2:   if (b === 0) {           ← Decision Point
3:     return "Error";        ← Branch 1
4:   } else {
5:     return a / b;          ← Branch 2
6:   }
7: }

Test Case 1: divide(10, 2)
- Statement Coverage: 4/5 = 80% (2, 4, 5행)
- Branch Coverage: 1/2 = 50% (else만 실행)

Test Case 2: divide(10, 0)  
- Statement Coverage: 3/5 = 60% (2, 3행)
- Branch Coverage: 1/2 = 50% (if만 실행)

Combined Coverage:
- Statement Coverage: 5/5 = 100%
- Branch Coverage: 2/2 = 100%

[커버리지 목표]

┌─────────────────────────────────┐
│  산업별 권장 커버리지            │
├─────────────────────────────────┤
│  일반 웹/앱: 70-80%             │
│  금융/의료: 90% 이상            │
│  안전 필수: 100% (항공, 원자력) │
└─────────────────────────────────┘

[커버리지 도구]

- Java: JaCoCo, Cobertura, Emma
- JavaScript: Istanbul, NYC
- Python: Coverage.py
- C/C++: gcov, lcov
```

## 키워드
- Statement, Branch, Condition, Path Coverage
- Requirement, Feature, Use Case Coverage
- 정량적 측정, 테스트 완전성, 품질 지표
- JaCoCo, Istanbul, Coverage.py

## 암기법
- 코드 커버리지 5종: 구결조경함 
  (구문-결정-조건-경로-함수)
- 기능 커버리지 3종: 요기유 (요구사항-기능-유스케이스)
- 목표: 100% 커버리지 = 완벽 아님 (품질 보장 X)

## 연관 토픽
- [[테스트 관리]] - 테스트 관리
- [[화이트박스 테스트]] - 화이트박스 기법
