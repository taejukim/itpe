=======================
MSA와 Monolithic Architecture(Microservices Architecture vs Monolithic)

#정보관리기술사 #프로젝트관리 #현대적아키텍처

- [ ] 1회
- [ ] 2회
- [ ] 3회
- [ ] 4회
- [ ] 5회

## 정의
작은 서비스 단위로 분해된 아키텍처와 통합된 구조의 비교, MSA vs Monolithic
- Monolithic: 모든 기능을 하나의 코드베이스와 DB에 통합하여 구축하는 전통적 방식
- MSA: 비즈니스 기능을 독립적인 서비스 단위로 쪼개어 배포하고 운영하는 현대적 방식

## 구성요소
- Monolithic 특징: 단일 프로세스, 단순한 구조, 배포 및 테스트 용이(초기), 기술 스택 고착
- MSA 특징: 독립 배포 가능, 폴리글랏 프로그래밍(다양한 언어/DB), 느슨한 결합, 서비스 간 통신(REST, gRPC)
- 데이터 관리: Monolithic(단일 DB/Shared), MSA(서비스별 DB/Polyglot)
- 조직 관리: Monolithic(계층형 조직), MSA(목적 중심의 Cross-functional 팀)

## 구성도 요소
* 아키텍처 비교:
    - Monolithic: [UI] -> [Application Core (All Functions)] -> [DB]
    - MSA: [UI] -> [API Gateway] -> [Service A/B/C (Each with DB)]
* 관계: 복잡도가 낮은 초기에는 Monolithic이 유리하나, 확장성과 민첩성이 필요한 경우 MSA로 전환
```
[Monolithic]              [MSA]
    [All]             [Svc A] [Svc B]
      |                  |       |
    [DB]               [DB A]  [DB B]
```

## 키워드
* 독립 배포, 폴리글랏, API 게이트웨이, 느슨한 결합, 인프라 자동화

## 암기법
* 모통엠독 (모놀리식 통합, MSA 독립)
* 폴독민확 (MSA: 폴리글랏, 독립배포, 민첩성, 확장성)
