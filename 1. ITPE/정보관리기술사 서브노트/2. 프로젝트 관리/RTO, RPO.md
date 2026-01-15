
## 정의
RTO (Recovery Time Objective) : 목표 복구 시간
RPO (Recovery Point Objective) : 목표 복구 시점
[[DRS]] 핵심지표 RTO, RPO의 개념

## 개념도
* RTO
	- 재정 > 시간
		- 한계재정
	- 목표 복구 시간
	- 개념 : 서비스를 복구하는데 필요한 서용 시간
	- 목표 : 복구시간 최소화
	- 적용분야 : 증권, 은행 등 금융권
- RPO
	- 데이터 손실 > 시간
		- 데이터 손실 허용
	- 목표 복구 시점
	- 개념 : 감내할 수 있는 데이터 손실 허용 시점
	- 목표 : 데이터 손실 최소화
	- 적용 분야 : 제조, 연구, 고객관리 분야
- 사업 분야에 따라 RTO, RPO 최적화
## DR 유형
- Mirror Site : 메인센터와 동시 반영  > RTO = 0
- Hot Site : 메인센터와 거의 동시 > RTO <= 2H
- Warm Site : 메인센터와 장비/기술 보유 > RTO <=1W
- Cold Site : 메인센터 데이터만 보유 > RTO 수개원
- 시스템 중요도에 따라 DR 유형 선택

## BCP와 관계도
* 목표
	- RTO (시간) 
	- RPO (데이터)
	-  RSO (업무범위)
	- RCO (네트워크)
- BCP (Business Continunity Plan)
- 기대 효과
	- 업무 연속성 보장
	- 시스템 데이터 보호
	- Resilience (복원력)
	- ISO 22301 준수
- 적절한 목표(RTO, RPO) 설정으로 비스지스 연속성 보장


## 키워드
- MTPD(Maximum Tolerable Period Of Distruption) : 운영중단 회대 허용 기간
- MBCO(Minmum Business Continunity Objectives) : 사업 연속성 최소 목표
- 

## 암기법
- R데T시S업C네
	- RPO 데이터
	- RTO 시간 
	- RSO 업무 범위
	- RCO 네트워크
- 미핫웜콜
	- 미러 사이트
	- 핫 사이트
	- 웜 사이트
	- 콜드 사이트

