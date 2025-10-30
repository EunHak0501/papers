# 자연어 처리 (NLP)

대규모 언어 모델과 자연어 이해, 파인튜닝 기법에 관한 논문들을 정리합니다. 각 논문 폴더에는 PDF 원문과 핵심 내용을 정리한 요약 파일이 포함되어 있습니다.

## 포함된 논문

| 논문 | 핵심 주제 | 간단 소개 |
| --- | --- | --- |
| [DeepSeek V3](DeepSeekV3/README.md) | 초거대 Mixture-of-Experts LLM | 671B 파라미터 MoE 구조에 MLA/DeepSeekMoE와 다중 토큰 예측을 결합하여 개방형 모델 최고 수준 성능 달성 |
| [DeepSeek R1](DeepSeekR1/README.md) | RL 기반 추론 강화 | 대규모 RL만으로 추론 능력을 끌어올린 DeepSeek-R1-Zero와 다단계 학습을 적용한 DeepSeek-R1 소개 |
| [Improving Language Understanding by Generative Pre-Training](ImprovingLanguageUnderstanding/README.md) | GPT-1 | 생성 사전학습 후 태스크별 미세조정을 통해 다양한 NLP 벤치마크에서 성능 향상 |
| [QLoRA](QLoRA/README.md) | 양자화 기반 효율적 파인튜닝 | 4비트 양자화된 LLM에 LoRA를 적용하여 메모리 사용량을 줄이면서 성능 유지 |

## 향후 추가 아이디어

- 다국어/멀티모달 LLM 논문 추가 (예: Speech-to-Text, Vision-Language).
- 평가 벤치마크 및 실험 설정 비교 표 확장.
