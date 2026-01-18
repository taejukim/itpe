=======================
CI, CD(Continuous Integration, Continuous Deployment)

#정보관리기술사 #프로젝트관리 #[[DevOps]]

- [ ] 1회
- [ ] 2회
- [ ] 3회
- [ ] 4회
- [ ] 5회

## 정의
자동화된 코드 통합과 신속한 배포 체계, CI/CD
- CI(지속적 통합): 개발자가 작성한 코드를 수시로 병합하고 자동 빌드 및 테스트 수행
- CD(지속적 서비스 제공/배포): CI를 통과한 결과물을 테스트 또는 운영 환경에 자동으로 배포

## 구성요소
- Code Repository: 소스 코드 관리 (Git, SVN 등)
- Build Automation: 코드 컴파일 및 패키징 자동화 (Maven, Gradle)
- Test Automation: 단위 테스트 및 통합 테스트 자동화 (JUnit, Selenium)
- Artifact Repository: 빌드 결과물 저장 및 관리
- Deployment Automation: 서버 배포 및 설정 자동화 (Jenkins, Ansible, Terraform)
- CD의 구분: Continuous Delivery(수동 승인 배포) vs Continuous Deployment(완전 자동 배포)

## 구성도 요소
* 파이프라인(Pipeline): Plan -> Code -> Build -> Test -> Release -> Deploy -> Operate
* 관계: 개발과 운영의 벽을 허무는 [[DevOps]] 실현의 기술적 핵심
```
[Dev] -> [Push] -> [Build] -> [Test] -> [Staging] -> [Prod]
 | <---------- (CI) ----------> | <------- (CD) --------> |
```

## 키워드
* 파이프라인, 자동화 테스트, 젠킨스(Jenkins), 릴리스 주력, 무중단 배포

## 암기법
* 통합배포 (CI는 통합, CD는 배포)
* 빌테배 (빌드, 테스트, 배포 자동화)
