=======================
ISO/IEC 25010(ISO 9126, Software Product Quality)

#SW공학 #품질모델 #표준

- [ ] 1회
- [ ] 2회
- [ ] 3회
- [ ] 4회
- [ ] 5회

## 정의
소프트웨어 품질 특성 국제 표준, ISO/IEC 25010
- 소프트웨어 제품의 품질 특성과 평가 모델을 정의한 국제 표준 (ISO 9126의 후속)
- 사용 품질(Quality in Use)과 제품 품질(Product Quality)의 2가지 품질 모델 제시

## 특징
- 포괄성: 8대 품질 특성 정의
- 계층성: 특성-부특성 구조
- 표준화: 국제 표준 품질 모델
- 측정성: 평가 가능한 품질 정의

## 목적
- 소프트웨어 품질 특성의 체계적 분류 및 평가 기준 제공
- 제품 및 사용 품질의 측정 및 개선 지원

## 구성요소
### 제품 품질 모델 (8대 특성)
- Functional Suitability(기능 적합성): 기능 완전성, 정확성, 적절성
- Performance Efficiency(성능 효율성): 시간 행동, 자원 활용, 용량
- Compatibility(호환성): 공존성, 상호운용성
- Usability(사용성): 인식성, 학습성, 운용성, 오류방지, 심미성, 접근성
- Reliability(신뢰성): 성숙성, 가용성, 결함 허용성, 회복성
- Security(보안성): 기밀성, 무결성, 부인방지, 책임추적성, 인증성
- Maintainability(유지보수성): 모듈성, 재사용성, 분석성, 수정성, 시험성
- Portability(이식성): 적응성, 설치성, 대체성

### 사용 품질 모델 (5대 특성)
- Effectiveness(효과성): 목표 달성도
- Efficiency(효율성): 자원 대비 성과
- Satisfaction(만족성): 유용성, 신뢰감, 즐거움, 편안함
- Freedom from Risk(위험 회피): 경제적, 건강/안전, 환경 위험 완화
- Context Coverage(범위 포괄성): 상황 완전성, 유연성

## 구성도
```
┌──────────────────────────────────────┐
│       ISO/IEC 25010 품질 모델        │
└──────────────────────────────────────┘

[제품 품질 - 8대 특성]

1. Functional Suitability (기능 적합성)
2. Performance Efficiency (성능 효율성)
3. Compatibility (호환성)
4. Usability (사용성)
5. Reliability (신뢰성)
6. Security (보안성)
7. Maintainability (유지보수성)
8. Portability (이식성)

[사용 품질 - 5대 특성]

1. Effectiveness (효과성)
2. Efficiency (효율성)
3. Satisfaction (만족성)
4. Freedom from Risk (위험 회피)
5. Context Coverage (범위 포괄성)

[ISO 9126 vs ISO 25010 비교]

ISO 9126 (구버전, 6대 특성)
- 기능성, 신뢰성, 사용성
- 효율성, 유지보수성, 이식성

ISO 25010 (신버전, 8대 특성)
- 기능 적합성, 성능 효율성
- 호환성, 사용성, 신뢰성
- 보안성, 유지보수성, 이식성

변경점:
- 기능성 → 기능 적합성
- 효율성 → 성능 효율성
- 보안성 추가 (독립 특성)
- 호환성 추가 (독립 특성)
```

## 키워드
- Functional Suitability, Performance, Compatibility
- Usability, Reliability, Security
- Maintainability, Portability
- ISO 9126, SQuaRE, 품질 특성

## 암기법
- 제품 품질 8대: 기성호사신보유이
  (기능-성능-호환-사용-신뢰-보안-유지-이식)
- 사용 품질 5대: 효효만위범
  (효과-효율-만족-위험-범위)
- 9126→25010: 6개→8개 (보안, 호환 추가)

## 연관 토픽
- [[프로젝트 QM]] - 품질 관리
- [[SW Architecture 평가]] - 품질 평가
