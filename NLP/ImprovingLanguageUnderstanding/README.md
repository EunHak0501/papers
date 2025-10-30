# Improving Language Understanding by Generative Pre-Training

- **원문**: `ImprovingLanguageUnderstanding.pdf`
- **저자**: Alec Radford, Karthik Narasimhan, Tim Salimans, Ilya Sutskever (OpenAI)
- **주요 키워드**: Generative Pre-Training, Transfer Learning, GPT-1

## 핵심 요약

본 논문은 대규모 비지도 언어 모델을 생성 방식으로 사전학습한 후, 태스크별로 지도 미세조정을 수행하면 적은 라벨 데이터만으로도 다양한 NLP 과제에서 우수한 성능을 얻을 수 있음을 보였습니다. 사전학습은 BooksCorpus 등을 활용해 일반 언어 패턴을 습득하며, 이후 태스크 특화 입력 변환과 함께 미세조정하여 문서 분류, 질문응답, 의미 유사도 등에서 큰 성능 향상을 달성했습니다.

## 주요 아이디어

1. **Generative Pre-Training (GPT)**: 언어 모델을 순방향 생성 방식으로 사전학습해 다양한 언어 지식을 내재화합니다.
2. **Task-Aware Fine-Tuning**: 태스크 입력을 모델이 익숙한 형식으로 변환하고, 소량의 라벨 데이터로 미세조정하여 전이 효율을 극대화합니다.
3. **Few-Shot Generalization**: 일부 태스크에서는 예시를 입력에 포함시키는 것만으로도 추가 학습 없이 성능 향상이 가능합니다.
4. **범용성 검증**: entailment, QA, 감성 분석 등 여러 벤치마크에서 동일 모델이 일관된 개선을 보여 범용 사전학습 접근의 가치를 입증합니다.

## 참고 자료

- GPT-2, GPT-3 등 후속 연구와의 비교.
- Transfer learning in NLP 관련 튜토리얼.
