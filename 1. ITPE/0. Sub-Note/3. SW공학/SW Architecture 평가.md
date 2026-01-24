=======================
SW Architecture 평가(Software Architecture Evaluation)

#SW공학 #아키텍처 #평가

- [ ] 1회
- [ ] 2회
- [ ] 3회
- [ ] 4회
- [ ] 5회

## 정의
아키텍처 품질속성 평가, 소프트웨어 아키텍처 평가
- 소프트웨어 아키텍처가 요구되는 품질속성(성능, 보안, 가용성 등)을 만족하는지 검증하는 프로세스
- 아키텍처 설계 초기에 위험요소를 식별하고 개선방안을 도출하여 프로젝트 리스크 최소화

## 특징
- 사전 예방: 구현 전 설계 단계에서 평가
- 정량화: 시나리오 기반 측정 가능한 평가
- 독립성: 제3자 관점의 객관적 평가
- 트레이드오프: 상충되는 품질속성 균형 분석

## 목적
- 아키텍처 설계의 품질 검증 및 위험 조기 발견
- 품질속성 간 트레이드오프 분석 및 최적 의사결정 지원

## 구성요소
- ATAM(Architecture Trade-off Analysis Method): 품질속성 간 트레이드오프 분석 방법
- SAAM(Software Architecture Analysis Method): 시나리오 기반 아키텍처 분석
- CBAM(Cost Benefit Analysis Method): 아키텍처 의사결정의 비용-편익 분석
- Quality Attribute(품질속성): 성능, 보안, 가용성, 확장성, 유지보수성
- Scenario(시나리오): 품질속성을 평가하기 위한 구체적 상황
- Trade-off(트레이드오프): 상충되는 품질속성 간 균형점

## 구성도
```
[아키텍처 평가 프로세스]

1. 준비단계
   └─ 이해관계자 식별, 평가목표 설정

2. 분석단계
   ├─ 아키텍처 이해
   ├─ 품질속성 시나리오 도출
   └─ 아키텍처 패턴/전략 분석

3. 평가단계
   ├─ ATAM: 트레이드오프 분석
   ├─ SAAM: 시나리오 기반 평가
   └─ CBAM: 비용-편익 분석

4. 결과단계
   └─ 위험요소 식별, 개선방안 도출


[ATAM 프로세스]
Stakeholder → Quality Attribute
      ↓
   Scenario
      ↓
Architecture Analysis
      ↓
Trade-off Analysis
      ↓
Risk & Sensitivity Point
```

## 키워드
- ATAM, SAAM, CBAM
- Quality Attribute, Scenario, Trade-off
- Risk, Sensitivity Point, Non-Risk

## 암기법
- 평가 3대 방법: 에이탐-삼-씨밤 (ATAM-SAAM-CBAM)
- ATAM 핵심: 시나리오로 품질평가, 트레이드오프 발견

## 연관 토픽
- [[SW Architecture]] - 아키텍처 기본 개념
- [[ISO-IEC-IEEE 42010]] - 아키텍처 표준
- [[ISO-IEC 25010]] - 품질 특성 표준
