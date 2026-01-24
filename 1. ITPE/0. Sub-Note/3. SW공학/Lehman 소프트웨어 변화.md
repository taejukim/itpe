=======================
Lehman 소프트웨어 변화(Lehman's Laws of Software Evolution)

#SW공학 #유지보수 #소프트웨어진화

- [ ] 1회
- [ ] 2회
- [ ] 3회
- [ ] 4회
- [ ] 5회

## 정의
소프트웨어 진화 법칙, Lehman의 법칙
- Meir Lehman이 제시한 소프트웨어 시스템의 진화와 유지보수에 관한 8가지 법칙
- 실세계에서 사용되는 E-type 시스템의 변화 패턴과 특성을 설명

## 구성요소
### Lehman의 8가지 법칙

1. **Continuing Change(지속적 변화)**
   - 시스템은 사용되는 동안 지속적으로 변경되거나 유용성 감소
   - 환경 변화에 적응하지 않으면 만족도 저하

2. **Increasing Complexity(복잡도 증가)**
   - 시스템 변경 시 구조가 복잡해짐
   - 리팩토링 없이 변경만 하면 복잡도 증가

3. **Self Regulation(자기 규제)**
   - 시스템 진화 과정은 자기 규제적
   - 변경 속도와 규모가 일정 패턴 유지

4. **Conservation of Organizational Stability(조직 안정성 보존)**
   - 시스템 생명주기 동안 평균 활동률(변경률) 일정
   - 조직의 작업 속도는 거의 변하지 않음

5. **Conservation of Familiarity(친숙도 보존)**
   - 각 릴리스의 증분 변화는 거의 일정
   - 사용자 적응 능력 한계로 변화량 제한

6. **Continuing Growth(지속적 성장)**
   - 사용자 만족 유지 위해 기능 지속 추가
   - 시스템 크기가 지속적으로 증가

7. **Declining Quality(품질 저하)**
   - 적극적 품질 관리 없으면 품질 저하
   - 변경 누적으로 설계 무결성 감소

8. **Feedback System(피드백 시스템)**
   - 진화 프로세스는 다단계 피드백 시스템
   - 이전 변경이 다음 변경에 영향

### 소프트웨어 유형 분류
- S-type(Specification): 정형 명세에 의해 정의
- P-type(Problem): 문제 해결 중심
- E-type(Embedded): 실세계에 내장된 시스템

## 구성도
```
[Lehman의 8가지 법칙]

1. Continuing Change
   └─ 변화 OR 유용성 감소

2. Increasing Complexity
   └─ 변경 → 복잡도 ↑

3. Self Regulation
   └─ 진화 속도 일정 패턴

4. Conservation of Organizational Stability
   └─ 평균 활동률 일정

5. Conservation of Familiarity
   └─ 릴리스당 변화량 일정

6. Continuing Growth
   └─ 기능 계속 추가

7. Declining Quality
   └─ 품질 관리 없으면 ↓

8. Feedback System
   └─ 이전 → 다음 영향

[시간에 따른 변화]

복잡도
   │      ╱
   │    ╱
   │  ╱        (지속 증가)
   │╱
   └──────────────> 시간

품질
   │╲
   │  ╲
   │    ╲      (관리 없으면 감소)
   │      ╲
   └──────────────> 시간

[E-type 시스템 특징]

실세계 ─────> E-type 시스템
환경 변화      │
사용자 요구    │ 적응 필요
기술 발전      │
규제 변경      ▼
             지속적 진화

[대응 전략]

1. 리팩토링: 복잡도 관리
2. 품질 관리: 품질 저하 방지
3. 점진적 변경: 친숙도 유지
4. 아키텍처 관리: 구조 무결성
```

## 키워드
- Continuing Change, Increasing Complexity
- Self Regulation, Conservation, Declining Quality
- E-type, 진화, 유지보수
- Lehman, 소프트웨어 노화

## 암기법
- 8가지 법칙: 변복자조친성품피
  (변화-복잡도-자기규제-조직-친숙도-성장-품질-피드백)
- 핵심 3개: 변화·복잡도·품질
- 유형: SPE (Specification-Problem-Embedded)

## 연관 토픽
- [[3R]] - 리엔지니어링 기법
- [[소프트웨어 리팩토링]] - 코드 개선
