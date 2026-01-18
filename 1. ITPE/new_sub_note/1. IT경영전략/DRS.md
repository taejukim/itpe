=======================
DRS(Disaster Recovery System)

#정보관리기술사 #IT경영전략 #재해복구

- [ ] 1회
- [ ] 2회
- [ ] 3회
- [ ] 4회
- [ ] 5회

## 정의
재해 복구 계획을 실현하기 위한 기술적 시스템, DRS
- 정보시스템의 안정성을 보장하기 위해 주 센터와 떨어진 지역에 구축한 복구 시스템
- 구축 수준에 따라 [[RTO, RPO]]가 결정되며 무중단 서비스를 지향함

## 구성요소
- Mirror Site: 실시간 동기 복제, RTO=0 (Active-Active)
- Hot Site: 실시간 비동기 복제, RTO=수시간 이내 (Active-Standby)
- Warm Site: 주기적 백업 데이터 전송, RTO=수일 이내
- Cold Site: 장소만 확보 및 장비 미설치, RTO=수주 이내
- 백업 센터: 데이터 보관 및 시스템 복원을 위한 물리적 거점

## 구성도 요소
* 아키텍처: 데이터 복제 기술(Storage mirroring, Database replication) 중심
* 관계: 거리와 대역폭에 따라 동기(Synchronous)/비동기(Asynchronous) 방식 선택
```
[주 센터] <---- (Sync/Async Replication) ----> [복구 센터]
    |                                              |
 [스토리지] <----------------------------------> [스토리지]
```

## 키워드
* 미러 사이트, 핫 사이트, 웜 사이트, 콜드 사이트, 동기/비동기 복제

## 암기법
* 미핫웜콜 (Mirror, Hot, Warm, Cold)
