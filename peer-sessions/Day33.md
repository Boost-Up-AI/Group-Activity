### 피어세션 16:00~17:30

1. 논문리뷰: YOLO by 지호님 \
YOLO가 나오기 전에는 분류기를 써서 탐색했으나, 이 논문은 bounding boxes와 관련된 회귀문제로 해결을 했다. \
인간의 object detection 능력은 매우 뛰어난 편이다. 

- YOLO의 이점
    - Bounding box와 classification을 동시에 수행함으로써 학습 속도가 매우 빠르다.
    - Detection을 regression 문제로 간주하기 때문에 복잡한 파이프라인을 구축할 필요가 없다. 
    - 복잡한 이미지에 대해 globally 추론을 한다. train과 test 시, 전체적인 이미지를 보므로 클래스에 대한 문맥적인 정보와 object appearance가 모두 담겨 있다.
    - Object의 일반화 가능한 특징들을 학습한다.

- 저자는 모든 걸 C++로 구현....WOW... 군용 목적으로 이용되는 것을 원치 않아 지금은 손을 뗀 상태!


2. 과제3 질문 by 지영님 \
    Q. num of params는 무엇을 의미하는지?? \
    A. 각 layer마다 # of trainable parameters의 총합 = tensor 원소 개수 \
    convolution layers는 filter(3d tensor)의 width * height * channels 을 의미. \
    linear layer는 W, b의 원소 개수.
    - ex) a = torch.zeros(4, 4) \
        torch.numel(a) = 16   (numpy의 size)
        a.size() = [4, 4]     (numpy의 shape)


3. LINE 채용설명회 후기 by 누리님
- 인재상 \
기본적인 개발실력 + 신입공채의 경우 기대치가 높지 않음 + 빠르게 습득하고 적응하는 능력 \ + 서류도 개발자가 검토 (HR팀은 관여하지 않음)
- 현직자들을 위한 내부 교육.성장 프로그램이 있다. (유투브 채널에 재직자 인터뷰 영상 참고)
- 라인의 강점: 글로벌 회사. 수평적 문화

4. 조교님 멘토링 질문 정하기  \
이번주 과제2의 torch tensor를 copy하는 5가지 방법, weight를 assign하는 2가지 방법에 대해 설명해주시면 감사하겠습니다. \
또한, 조교님께서 주로 사용하는 방법이 있는지, 각 방법마다 어떤 차이가 있는지 궁금합니다.