# SW공학 서브노트 작성 프로젝트 진행 상황

## 프로젝트 개요

**목표**: SW공학.pdf 기반 55개 토픽에 대한 정보관리기술사 시험 대비 서브노트 작성

**참조 문서**: 
- Reference: SW공학.pdf (바이너리 파일로 직접 읽기 불가)
- Target List: `3. SW공학/0. SW공학 추가 토픽 List.md` (55개 토픽)
- Template: `99. Reference/Prompt_1.md`

**저장 위치**: `/Users/tj.k/Library/CloudStorage/GoogleDrive-taejukim.me@gmail.com/내 드라이브/TJ PKM/1. ITPE/0. Sub-Note/3. SW공학/`

## 작업 완료 현황

### 1단계: 55개 서브노트 파일 생성 ✅ (완료)

모든 토픽에 대해 표준 템플릿 구조로 파일 생성 완료

**템플릿 구조**:
```markdown
=======================
토픽 이름(영문 Full name)

#정보관리기술사 #SW공학 #추가태그

- [ ] 1회
- [ ] 2회
- [ ] 3회
- [ ] 4회
- [ ] 5회

## 정의
리드문 + 토픽 (20자 미만)
- 정의 1줄
- 정의 2줄

## 구성요소
- 핵심 구성요소 리스트

## 구성도
* Text 기반 다이어그램

## 키워드
* 암기 필요 키워드

## 암기법
* 한글 두음법칙 활용 암기법
```

### 생성된 파일 목록 (55개)

#### Architecture & Design (10개)
1. SW Architecture.md
2. ISO-IEC-IEEE 42010.md
3. SW Architecture 평가.md
4. 아키텍처 모델-패턴.md
5. MVC패턴.md
6. MVVM.md
7. MVI패턴.md
8. 모듈화.md
9. 노코드.md
10. Vibe coding, AI 코딩.md

#### UML & Diagrams (7개)
11. UML-Diagram 전체.md
12. UML의 관계.md
13. Class diagram.md
14. Usecase diagram.md
15. 활동 다이어그램.md
16. 상태 머신 다이어그램.md
17. Sequence diagram.md

#### Open Source (2개)
18. 오픈소스 소프트웨어.md
19. 오픈소스 License 분류.md

#### Testing (9개)
20. Test 일반.md
21. 테스트 관리.md
22. 블랙박스 테스트.md
23. 화이트박스 테스트.md
24. 회귀 테스트.md
25. 경험기반 기법.md
26. 성능 테스트.md
27. ISO 29119.md
28. Test Coverage.md

#### Quality Management (7개)
29. 프로젝트 QM.md
30. ISO-IEC 25010.md
31. CMMI.md
32. SW 안정성-분석 개념.md
33. FTA.md
34. FMEA.md
35. HAZOP.md

#### Audit & Certification (13개)
36. SP 인증.md
37. 정보시스템 감리.md
38. 정보시스템 감리 Framework.md
39. 감리절차.md
40. 감리결과보고서 작성하기.md
41. 감리 PMO 비교.md
42. 클라우드 감리.md
43. 운영감리.md
44. 유지보수 감리.md
45. 빅데이터 감리.md

#### Cost Estimation (3개)
46. 간이법 계산.md
47. SW사업 대가 산정 가이드.md
48. AI 개발비 산정.md

#### Maintenance & Deployment (4개)
49. Lehman 소프트웨어 변화.md
50. 3R.md
51. 소프트웨어 리팩토링.md
52. 무중단 배포 기법.md

**기존 파일 (작성 전부터 존재)**:
53-55. AOP.md, 객체지향 관련 파일들 등

---

### 2단계: 특징 및 목적 섹션 추가 🔄 (진행 중)

**사용자 요청사항**:
> "지금까지 작성된 55개 토픽에 대해 각 특징을 정의 하단에 작성해주시고 그 아래 목적도 2가지 정도 적어주세요. 특징은 간단명료하게 적어주세요. 예를 들어 간결성, 유지보수성 등이요"

**추가되는 구조**:
```markdown
## 정의
...

## 특징
- 특징1: 간단명료한 설명
- 특징2: 간단명료한 설명
- 특징3: 간단명료한 설명
- 특징4: 간단명료한 설명

## 목적
- 목적1 설명
- 목적2 설명

## 구성요소
...
```

**완료된 파일 (약 30개)**:
- ✅ Architecture & Design (10개)
- ✅ UML & Diagrams (7개)
- ✅ Open Source (2개)
- ✅ Testing (9개)
- ✅ Quality Management 일부 (7개)

**진행 필요 파일 (약 25개)**:
- 🔄 Audit & Certification (13개)
- 🔄 Cost Estimation (3개)
- 🔄 Maintenance & Deployment (4개)
- 🔄 기타 기존 파일들

---

## 작성 원칙

### Ground Rules
1. Reference 기준 내용으로만 작성 (PDF 읽기 불가로 웹검색 활용)
2. 각 토픽별 독립된 .md 파일 생성
3. 통합 설명 가능 시 통합 생성
4. 모든 토픽에 태그 추가:
   - #정보관리기술사 (필수)
   - 각 도메인 Tag (e.g., #SW공학, #아키텍처, #테스트)
   - 카테고라이징 가능한 분류 태그
5. 핵심만 요약, 줄글 말고 불렛 포인트로 작성
6. Text 기반 구성도 작성

### 특징 작성 원칙
- 4가지 특징을 간단명료하게 (예: 간결성, 유지보수성, 확장성)
- 각 토픽의 고유한 특성 반영
- 기술적 특성 중심으로 기술

### 목적 작성 원칙
- 2가지 주요 목적
- 왜 이 기술/방법론이 필요한지 명확히 서술
- 실무적 가치 강조

---

## 다음 작업

### 즉시 처리 필요
1. 나머지 25개 파일에 "특징" 및 "목적" 섹션 추가
   - Audit & Certification (13개)
   - Cost Estimation (3개)  
   - Maintenance & Deployment (4개)
   - 기존 파일 업데이트 (AOP 등)

### 검토 사항
- ISO-IEC-IEEE 42010.md에 사용자가 "4+1 view" 추가한 것 확인됨
- 사용자 커스터마이징 존중 필요

---

## 참고 사항

### 기존 예시 파일 구조 (AOP.md)
```markdown
=======================
AOP(Aspect Oriented Programming)

#정보관리기술사 #SW공학 #관점지향

- [x] 1회
- [ ] 2회
...

## 정의
AOP(Aspect-Oriented Programming)
횡단 관심사를 분리하여 모듈성을 높이는 프로그래밍 패러다임, 관점지향 프로그래밍
- 비즈니스 로직(Core Concern)과 공통 기능(Cross-cutting Concern)을 분리하여 관리
- 로깅, 보안, 트랜잭션 등 여러 모듈에 흩어진 중복 코드를 별도의 '관점(Aspect)'으로 모듈화함

## 구성요소
- Core Concern: 필수요구사항
- Join Point: 핵심관심사 횡단위치 
...
```

### 작업 도구
- 파일 생성/수정: `write`, `search_replace` 도구 사용
- 배치 처리로 효율성 확보
- 각 섹션 사이에 적절한 줄바꿈 유지

---

## 완성 시 결과물

**총 55개의 체계적인 SW공학 서브노트**
- 정보관리기술사 시험 대비용
- 템플릿 기반 일관된 구조
- 암기법 및 키워드 포함
- 특징 및 목적 명시로 학습 효율성 향상
- Text 기반 구성도로 이해도 향상

**활용 방안**:
- 5회 반복 학습 체크리스트 제공
- 카테고리별 태그로 검색 용이
- 암기법으로 시험 대비 효율적
- 구성도로 개념 시각화
