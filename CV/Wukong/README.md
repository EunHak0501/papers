# Wukong: Towards a Scaling Law for Large-Scale Recommendation

- **원문**: `Wukong.pdf`
- **저자**: Buyun Zhang 외 (Meta)
- **주요 키워드**: Recommendation Systems, Scaling Law, Factorization Machines

## 핵심 요약

Wukong은 추천 시스템에서 언어 모델과 유사한 스케일링 법칙을 구현하기 위해 고안된 팩터라이제이션 머신 기반 아키텍처와 업스케일링 전략입니다. 적절한 파라미터 증가와 데이터 확장을 결합해 모델 품질이 안정적으로 향상되도록 설계되었으며, 실제 대규모 데이터셋에서 성능-비용 곡선을 체계적으로 분석합니다.

## 주요 아이디어

1. **Stacked Factorization Machine**: 순환적으로 쌓은 팩터라이제이션 블록으로 복잡한 상호작용을 표현하면서도 계산 효율을 유지합니다.
2. **Synergistic Upscaling**: 네트워크 깊이/너비, 배치, 데이터 크기 등을 공동으로 스케일해 일정한 성능 향상 경향을 확보합니다.
3. **Scaling Law 관찰**: 모델 크기와 성능 사이의 로그-선형 관계를 정량화하여 향후 확장 계획 수립에 활용합니다.
4. **실전 적용성**: 온라인 추천 시나리오에 적용 가능한 추론 효율, 메모리 사용량을 분석하며 배포 전략을 제시합니다.

## 참고 자료

- 대규모 추천 모델 최적화 사례.
- Scaling law 연구 일반화 자료.
