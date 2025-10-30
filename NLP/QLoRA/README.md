# QLoRA: Efficient Finetuning of Quantized LLMs

- **원문**: `QLoRA.pdf`
- **저자**: Tim Dettmers, Artidoro Pagnoni, Ari Holtzman, Luke Zettlemoyer
- **주요 키워드**: 4-bit Quantization, LoRA, Parameter-Efficient Fine-Tuning

## 핵심 요약

QLoRA는 4비트 NormalFloat(NF4) 양자화와 저랭크 어댑터(LoRA)를 결합해 대형 언어 모델을 단일 48GB GPU에서도 미세조정할 수 있도록 하는 방법입니다. 양자화된 본체를 고정한 채 LoRA 모듈만 학습하면서도 16비트 정밀도와 유사한 성능을 유지하며, Guanaco 모델 패밀리를 통해 챗봇 벤치마크에서 기존 공개 모델을 상회합니다.

## 주요 아이디어

1. **NF4 데이터 타입**: 정보이론적으로 최적인 4비트 분포를 정의해 양자화 오차를 줄입니다.
2. **Double Quantization & Paged Optimizers**: 옵티마이저 상태까지 4비트로 압축하고, GPU 메모리 부족을 방지하기 위해 페이징 전략을 도입합니다.
3. **LoRA Backpropagation**: 양자화된 가중치를 고정한 채 LoRA 모듈로만 기울기를 역전파하여 학습 안정성을 확보합니다.
4. **Guanaco 평가**: Vicuna 등 대화형 벤치마크에서 65B 모델이 ChatGPT의 99% 수준 성능을 달성함을 실험으로 검증합니다.

## 참고 자료

- LoRA, NF4 관련 구현 예시.
- Guanaco 공개 체크포인트.
