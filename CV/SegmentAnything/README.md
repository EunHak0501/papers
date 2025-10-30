# Segment Anything

- **원문**: `SegmentAnything.pdf`
- **저자**: Alexander Kirillov, Eric Mintun, Nikhila Ravi 외 (Meta AI)
- **주요 키워드**: Promptable Segmentation, SAM, SA-1B Dataset

## 핵심 요약

Segment Anything 프로젝트는 프롬프트 기반 세그멘테이션 태스크 정의, SAM 모델, 그리고 11M 이미지에서 10억 개 이상의 마스크를 포함한 SA-1B 데이터셋으로 구성된 비전 파운데이션 모델 접근입니다. SAM은 포인트, 박스, 마스크 등 다양한 프롬프트에 대응하여 제로샷으로 새로운 세그멘테이션 태스크에 빠르게 적응할 수 있습니다.

## 주요 아이디어

1. **Promptable Segmentation Task**: 사용자 입력(포인트, 박스, 텍스트 등)에 따라 다양한 세그멘테이션 결과를 생성하는 범용 태스크 정의.
2. **SAM 모델 설계**: 이미지 인코더, 프롬프트 인코더, 마스크 디코더로 구성된 아키텍처로, 고효율 인코딩과 마스크 생성 속도를 확보합니다.
3. **SA-1B 데이터 엔진**: 모델을 활용한 데이터 수집 루프를 통해 1B 마스크를 자동 주석화하여 대규모 학습 데이터를 확보합니다.
4. **제로샷 전이**: 의료, 영상 편집 등 다운스트림 작업에 프롬프트를 제공하면 별도 재학습 없이 활용 가능합니다.

## 참고 자료

- 공식 Segment Anything 웹사이트 및 데모.
- Zero-shot segmentation 관련 후속 연구.
