=======================
CPM(임계경로 관리)(Critical Path Method)

#정보관리기술사 #프로젝트관리 #일정관리

- [ ] 1회
- [ ] 2회
- [ ] 3회
- [ ] 4회
- [ ] 5회

## 정의
프로젝트의 전체 기간을 결정하는 가장 긴 경로를 분석하는 기법, CPM
- 프로젝트 네트워크 다이어그램에서 활동의 여유 시간(Float)이 0인 경로를 식별
- 임계 경로 상의 활동이 지연되면 프로젝트 전체 일정이 지연되므로 집중 관리가 필요함

## 구성요소
- 주공정(Critical Path): 여유 시간이 0인 가장 긴 경로 (프로젝트 최소 소요 시간 결정)
- 여유 시간(Float/Slack): 전체 여유(Total Float)와 자유 여유(Free Float)
- 전진 계산(Forward Pass): 활동의 조기 시작일(ES)과 조기 종료일(EF) 산정
- 후진 계산(Backward Pass): 활동의 늦은 시작일(LS)과 늦은 종료일(LF) 산정
- PDM(Precedence Diagramming Method): 선후 관계를 표현하는 네트워크 도식화법

## 구성도 요소
* 계산 공식:
    - EF = ES + Duration
    - LS = LF - Duration
    - Float = LS - ES 또는 LF - EF
* 관계: 임계 경로가 여러 개일 경우 프로젝트 위험도가 높아짐
```
[A: 3d] -- [B: 5d] -- [C: 2d]  => Path 1: 10d (Critical)
      \              /
       -- [D: 4d] ---          => Path 2: 7d (Float: 3d)
```

## 키워드
* Critical Path, Float(여유), 전진/후진 계산, PDM, 일정 단축 대상

## 암기법
* 전후여주 (전진계산, 후진계산, 여유시간, 주공정)
