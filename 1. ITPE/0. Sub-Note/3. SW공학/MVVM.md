=======================
MVVM(Model-View-ViewModel Pattern)

#SW공학 #디자인패턴 #아키텍처

- [ ] 1회
- [ ] 2회
- [ ] 3회
- [ ] 4회
- [ ] 5회

## 정의
데이터 바인딩 기반 UI 패턴, MVVM
- Model-View-ViewModel로 구성되며, 데이터 바인딩을 통해 View와 로직을 완전히 분리하는 패턴
- MVC의 발전형으로, ViewModel이 View의 상태와 동작을 추상화하여 테스트 용이성과 재사용성 향상

## 특징
- 양방향 바인딩: View와 ViewModel 자동 동기화
- 테스트 용이: ViewModel 단독 테스트 가능
- 완전 분리: View와 로직의 명확한 분리
- 재사용성: ViewModel 여러 View에서 재사용

## 목적
- 데이터 바인딩을 통한 View와 로직의 완전한 분리
- UI 로직의 테스트 용이성 및 유지보수성 향상

## 구성요소
- Model(모델): 데이터와 비즈니스 로직, 도메인 로직
- View(뷰): 사용자 인터페이스, 화면 표현 (XAML, XML)
- ViewModel(뷰모델): View의 추상화, 프레젠테이션 로직
- Data Binding(데이터 바인딩): View와 ViewModel 간 자동 동기화
- Command(커맨드): 사용자 액션을 ViewModel 메서드로 바인딩
- Observer Pattern(관찰자 패턴): 변경 자동 통지

## 구성도
```
┌──────────────────────────────────────────┐
│             MVVM Pattern                 │
└──────────────────────────────────────────┘

         ┌──────────┐
         │   User   │
         └─────┬────┘
               │
               ▼
        ┌─────────────┐
        │    View     │
        │  (UI Layer) │
        └──────┬──────┘
               │
        Data Binding
        (양방향 동기화)
               │
               ▼
        ┌──────────────┐
        │  ViewModel   │
        │(Presentation)│
        └──────┬───────┘
               │
          참조/호출
               │
               ▼
        ┌──────────────┐
        │    Model     │
        │ (Business)   │
        └──────────────┘

[데이터 흐름]
View ◄──Data Binding──► ViewModel ◄──► Model
     (자동 동기화)           (명시적 호출)
```

## 키워드
- Model, View, ViewModel, Data Binding
- Command, Observer Pattern, Presentation Logic
- WPF, Xamarin, Angular, Vue.js
- 테스트 용이성, 재사용성, 유지보수성

## 암기법
- MVVM: 모뷰뷰모 (Model-View-ViewModel)
- MVC와 차이점: 컨트롤러(Controller) → 뷰모델(ViewModel) + 데이터바인딩
- 핵심: 데이터 바인딩으로 View와 로직 완전 분리

## 연관 토픽
- [[MVC패턴]] - 기본 UI 분리 패턴
- [[MVI패턴]] - 단방향 흐름 패턴
