#연속성 #지표

## 정의
RTO / RPO (복구 목표 시간 및 시점)
재해 복구 및 비즈니스 연속성 계획의 핵심 지표인 목표 복구 시간과 시점, RTO/RPO
- RTO (Recovery Time Objective): 재해 발생 시점부터 서비스가 복구되어 재개될 때까지의 목표 시간
- RPO (Recovery Point Objective): 재해 발생 시 손실을 감내할 수 있는 데이터의 목표 복구 시점
특징) 복구 수준 결정의 기준, 비용과 트레이드 오프 관계, 비즈니스 영향 분석([[BIA]]) 결과 반영

## 개념 비교
- RTO: "얼마나 빨리 복구할 것인가?" (시간적 관점) / 목표: 운영 중단 최소화
- RPO: "데이터를 어느 시점까지 복원할 것인가?" (데이터 관점) / 목표: 데이터 손실 최소화

## 관련 지표
- RSO (Recovery Scope Objective): 복구해야 할 업무의 범위
- RCO (Recovery Communication Objective): 복구 시 필요한 네트워크 및 통신 확보 목표
- MTPD (Maximum Tolerable Period of Disruption): 업무 중단 최대 허용 기간

## DR 구축 유형별 수준
- Mirror Site: RTO=0, RPO=0 (실시간 동기화)
- Hot Site: RTO <= 수시간, RPO = 최신 백업 시점
- Warm Site: RTO <= 수일, RPO = 주기적 백업 시점
- Cold Site: RTO <= 수개월, RPO = 원격지 백업 시점

## 기대효과
- 서비스 중요도에 따른 차별화된 복구 전략 수립 가능
- IT 투자 비용 대비 효율적인 재해 복구 체계([[DRS]]) 구축 기반 마련

## 키워드
- [[BIA]], [[DRS]], MTPD, Resilience, 데이터 손실 허용 시점

## 암기법
- R데T시S업C네: RPO 데이터, RTO 시간, RSO 업무범위, RCO 네트워크
- 미핫웜콜: 미러, 핫, 웜, 콜드 사이트 (복구 수준)
