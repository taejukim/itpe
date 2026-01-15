#정보관리기술사
## 정의
Disaster Recovery as a Service 의 정의
- DRP(Disaster Recovery Plan)의 DR 모델 중 클라우드 상에 DRS를 구성하는 재해복구 방식
특징) 데이터 복제, Fail over, Fail back

## 구성도
- 센터 : 온프레미스 >  오프프레미스
	- 서버, CDP
- 백업 : Fail Over > Fail Back
- 네트워크 : WAN (VPN)
- On-Premise Center와 DRaaS간 데이터 복제

## 기술요소
* CDP : 데이터 트랙 캡쳐, 복구 시점 저장
* Replication : 데이터 복제 분산 저장, 이중화
* Cloud : 가상화 기반 서비스
## 유형
* 관리형 : 재해 복구 전과정 아웃소싱, 높은 비용, 편리함
* 지원형 : 필요한 서비스만 위탁, 관리형/DIY 형의 중간
* DIY형 : HW만 위탁, 구성은 직접, 비용 낮은, 불편함

## 키워드
* 데이터 복제, Fail over/Fail back, CDP, Replication, Coud

## 암기법
- RCF
	- Replication
	- Cloud
	- Fail over, Fail back
- 관지디
	- 관리형
	- 지원형
	- DIY형
