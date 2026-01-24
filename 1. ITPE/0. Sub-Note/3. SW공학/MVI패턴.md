=======================
MVI패턴(Model-View-Intent Pattern)

#SW공학 #디자인패턴 #아키텍처

- [ ] 1회
- [ ] 2회
- [ ] 3회
- [ ] 4회
- [ ] 5회

## 정의
단방향 데이터 흐름 UI 패턴, MVI
- Model-View-Intent로 구성되며, 사용자 의도(Intent)를 명시적으로 표현하는 반응형 아키텍처 패턴
- 단방향 데이터 흐름(Unidirectional Data Flow)을 통해 상태 예측 가능성과 디버깅 용이성 제공

## 특징
- 단방향 흐름: 예측 가능한 상태 관리
- 불변성: 상태 변경 추적 용이
- 명시적 의도: 사용자 액션 명확히 표현
- 디버깅 용이: 상태 변화 추적 가능

## 목적
- 단방향 데이터 흐름으로 상태 관리의 예측 가능성 확보
- 명시적 Intent 표현을 통한 디버깅 및 테스트 용이성 향상

## 구성요소
- Model(모델): 불변(Immutable) 상태 객체, 애플리케이션의 전체 상태
- View(뷰): 상태를 렌더링하여 UI 표현, 사용자 입력 수집
- Intent(인텐트): 사용자 의도/액션을 명시적으로 표현
- Unidirectional Flow(단방향 흐름): Intent → Model → View 순환
- State Management(상태 관리): 중앙 집중식 상태 관리
- Immutability(불변성): 상태 변경 시 새로운 객체 생성

## 구성도
```
┌──────────────────────────────────────────┐
│             MVI Pattern                  │
└──────────────────────────────────────────┘

         ┌──────────┐
         │   User   │
         └─────┬────┘
               │ 사용자 액션
               ▼
        ┌─────────────┐
        │    View     │
        │  (UI 렌더링) │
        └──────┬──────┘
               │
          Intent 전달
               │
               ▼
        ┌─────────────┐
        │   Intent    │
        │  (사용자 의도)│
        └──────┬──────┘
               │
          상태 변경 요청
               │
               ▼
        ┌─────────────┐
        │    Model    │
        │   (상태)     │
        └──────┬──────┘
               │
          새로운 상태
               │
               └─────► View (순환)

[단방향 데이터 흐름]
User Action → Intent → Model Update → View Render → User
                        ▲               │
                        └───────────────┘
```

## 키워드
- Model, View, Intent, Unidirectional Data Flow
- Immutable State, Reactive Programming, State Management
- Redux, RxJava, Cycle.js
- 예측 가능성, 디버깅 용이성, 테스트 용이성

## 암기법
- MVI: 모뷰인 (Model-View-Intent)
- 특징: 단방향 흐름 + 불변 상태 + 명시적 의도
- 데이터 흐름: 인모뷰 순환 (Intent→Model→View)

## 연관 토픽
- [[MVC패턴]] - 기본 UI 분리 패턴
- [[MVVM]] - 데이터 바인딩 패턴
