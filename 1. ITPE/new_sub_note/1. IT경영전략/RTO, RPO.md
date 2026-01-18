=======================
RTO, RPO(Recovery Time Objective, Recovery Point Objective)

#정보관리기술사 #IT경영전략 #비즈니스연속성

- [ ] 1회
- [ ] 2회
- [ ] 3회
- [ ] 4회
- [ ] 5회

## 정의
비즈니스 복구 수준을 결정하는 핵심 성과 지표, RTO/RPO
- RTO: 재해 발생 후 업무를 다시 시작할 때까지 허용되는 최대 중단 시간 (시간 관점)
- RPO: 재해 발생 시 데이터 손실을 감수할 수 있는 과거의 특정 시점 (데이터 관점)

## 구성요소
- RTO(Recovery Time Objective): 서비스 재개까지 걸리는 목표 시간 (0에 가까울수록 고비용)
- RPO(Recovery Point Objective): 백업 주기와 관련된 데이터 유실 허용 한도
- MTPD(Maximum Tolerable Period of Disruption): 업무 중단을 견딜 수 있는 한계점
- RSO(Recovery Scope Objective): 복구해야 할 업무의 범위 결정
- RCO(Recovery Communication Objective): 통신 및 네트워크 복구 목표

## 구성도 요소
* 타임라인: 과거(백업 시점) ← [재해 발생 시점] → 미래(서비스 재개 시점)
* 관계: RPO는 백업 기술(Snapshot, Mirroring)에 영향, RTO는 복구 인프라([[DRS]])에 영향
```
<--- [RPO] --- [재해 발생] --- [RTO] --->
(Data Loss)                  (Down Time)
```

## 키워드
* 복구 목표, 가용성, 백업 주기, [[BIA]] 연계, 서비스 중단

## 암기법
* 알티오는시간 (Recovery Time), 알피오는데이터 (Recovery Point)
