#정보관리기술사
## 정의
DRS(Disaster Recovery System)
IT 업무 연속성을 유지하는 체계, DRS의 정의
- 자연재해, 시스템 장애, 사이버 공격등으로 메인센터가 마비된 경우 서비스의 연속성을 확보하기 위해 대체 센터(Backup/DR Center)에서 신속하게 서비스를 복구/운영할 수 있도록 구축한 IT 복구 시스템

## 목적
* IT 인프라의 데이터 손실([[RPO]]) 최소화, 복구 시간 단축([[RTO, RPO]])
## 구성도
* 메인센터 <> DR센터
	* HW/SW
	* 스토리지
	* 네트워크
* DWDM, 전용선
* 센터 전환 
	* Fail-over, Fail-back
* 네트워크
	* 전용선 VPN, CDP, DWDM
* 백업
	* IP-SAN, DWDM
* 가용성확보
	* RAID, FTS
- 메인/DR 센터간 이중화, 가용성 보장

## 기술요소
* HA(High Avaliability) : HW 클러스터링, Stand-by
* FT(Falut Tolerant) : 실시간 복구, Dual 형태
* IP-SAN : SAN 트래픽, IP 패킷 전송
* DWDM : 고속 데이터 전송을 위한 통신

## 구축 유형
- Mirror Site : 메인센터와 동시 반영  > RTO = 0
- Hot Site : 메인센터와 거의 동시 > RTO <= 2H
- Warm Site : 메인센터와 장비/기술 보유 > RTO <=1W
- Cold Site : 메인센터 데이터만 보유 > RTO 수개원

## 운영형태
- 상호계약형, 공동계약형, 외주위탁형, 독립구축형

## 키워드
- RPO, RTO, RSO, RCO

## 암기법
* 전네백가
	* 센터 전환
	* 네트워크
	* 백업
	* 가용성
* 상공외독
	* 상호 계약
	* 공동 계약
	* 외주 위탁
	* 독립 구축


