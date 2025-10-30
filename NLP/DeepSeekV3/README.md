# DeepSeek-V3

- **원문**: `DeepSeekV3.pdf`
- **저자**: DeepSeek-AI
- **주요 키워드**: Mixture-of-Experts, MLA, Multi-Token Prediction, RLHF

## 핵심 요약

DeepSeek-V3는 총 671B 파라미터(토큰당 37B 활성) 규모의 Mixture-of-Experts 언어 모델로, Multi-head Latent Attention(MLA)과 DeepSeekMoE 아키텍처를 결합해 추론 효율과 성능을 동시에 높였습니다. 학습 과정에서는 14.8T 토큰 사전학습 후 감독 미세조정과 강화학습 단계를 통해 성능을 극대화하며, 보조 손실 없이 로드 밸런싱을 달성하고 다중 토큰 예측 목표를 도입해 생성 품질을 향상시킵니다.

## 주요 아이디어

1. **효율적인 MoE 설계**: DeepSeekMoE는 토큰당 제한된 전문가만 활성화하는 라우팅과 MLA 기반 압축 어텐션을 사용하여 추론 비용을 크게 줄이면서 품질을 유지합니다.
2. **보조 손실 없는 로드 밸런싱**: 기존 MoE에서 사용하던 로드 밸런싱 보조 손실 없이도 균형 잡힌 전문가 사용을 달성해 안정적 학습을 구현합니다.
3. **Multi-Token Prediction (MTP)**: 다음 토큰 예측을 다중 토큰 예측으로 확장하여 장거리 의존성을 포착하고 생성 정확도를 개선합니다.
4. **단계적 학습 파이프라인**: 대규모 사전학습 이후 SFT 및 RLHF를 포함한 다단계 파이프라인으로 실전 태스크 성능을 최적화합니다.

## 참고 자료

- DeepSeek 공식 블로그 및 발표 자료.
- MLA, MoE 관련 선행 연구 비교.
