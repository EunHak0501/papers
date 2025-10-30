# ComKD-CLIP: Comprehensive Knowledge Distillation for CLIP

- **원문**: `ComKD-CLIP.pdf`
- **저자**: Yifan Chen, Xiaozhen Qiao, Zhe Sun, Xuelong Li 외 (iOPEN, USTC, TeleAI)
- **주요 키워드**: CLIP, Knowledge Distillation, Multi-stage Alignment

## 핵심 요약

ComKD-CLIP은 대규모 CLIP 교사 모델에서 경량 학생 모델로 지식을 이전하는 포괄적인 증류 프레임워크입니다. 이미지/텍스트 인코더를 단계적으로 정렬하고, 프롬프트 최적화 및 attention 기반 증류 전략을 결합하여 작은 모델에서도 경쟁력 있는 멀티모달 표현을 얻습니다.

## 주요 아이디어

1. **다단계 정렬**: 교사 모델의 이미지·텍스트 표현을 분리해 각각 증류한 뒤, 최종적으로 대조 학습 로짓까지 정렬합니다.
2. **Prompt Distillation**: 학습 가능한 프롬프트를 도입해 텍스트 표현 공간을 교사와 학생 간에 가깝게 유지합니다.
3. **EduAttention**: attention 맵을 증류하여 학생 모델이 교사와 유사한 크로스모달 상호작용을 학습하도록 돕습니다.
4. **경량화 성능 검증**: 다양한 다운스트림 벤치마크에서 기존 경량 CLIP 대비 우수한 성능을 달성하며, 실환경 배포에 적합한 효율을 보여줍니다.

## 참고 자료

- CLIP (Radford et al., 2021) 원문.
- Knowledge Distillation 응용 사례.
