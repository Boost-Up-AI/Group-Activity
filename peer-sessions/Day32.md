### 피어세션 16:00~17:30 

- 논문리뷰
1. 동현님, 지영님: ResNet \
MS COCO: object detection에 사용되는 벤치마크 데이터셋 \
CNN layer를 여러개 거칠수록 receptive field가 커지기 때문에 high-level feature를 뽑을 수 있다. \
반대로, 얕은 층(입력 초반)에서는 low-level feature만 뽑아낼 수 있다. \
수식 (2)에서 W_s의 역할: 출력과 x의 dimension을 맞춰준다. \
identity mapping vs projection  (identity가 효과적) \
skip connection = LSTM의 cell state = Transformer에서 encoder의 hidden vector를 가져오는 것

2. 누리님: 강화학습 \
Environment가 agent에게 state를 주면 agent는 그에 대한 action을 취하고 env는 agent에게 reward를 준다. 
이러한 상호작용을 통해 reward를 최대화하는 policy를 찾는 것이 강화학습의 목표이다. \
특징: Trial and Error & Delayed reward (게임화면 외에 게임의 우승전략 같은 어떠한 정보도 입력하지 않는다.)

- 내일 LINE 채용설명회 참여시간 \
15:00~15:30 : 누리님 \
17:00~17:30 : 지영님, 지호님 \
- 스타트업 채용설명회에서 바로 면접보고 뽑을 수도 있다.

- 과거 피어세션 내용 정정 "Transfer learning과 앙상블 훈련은 서로 무관합니다."
1. Ensemble learning: [https://bkshin.tistory.com/entry/머신러닝-11-앙상블-학습-Ensemble-Learning-배깅Bagging과-부스팅Boosting](https://bkshin.tistory.com/entry/%EB%A8%B8%EC%8B%A0%EB%9F%AC%EB%8B%9D-11-%EC%95%99%EC%83%81%EB%B8%94-%ED%95%99%EC%8A%B5-Ensemble-Learning-%EB%B0%B0%EA%B9%85Bagging%EA%B3%BC-%EB%B6%80%EC%8A%A4%ED%8C%85Boosting) \
여러 개의 모델을 독립적으로 훈련시킨 뒤 출력결과를 투표 형식으로 합친다.
2. Transfer learning: [https://jeinalog.tistory.com/13](https://jeinalog.tistory.com/13)  \
pre-trained net (resnet, vgg16 등)을 불러와서 마지막 layer를 제외한 모든 layers의 parameters를 그대로 활용한다. 즉, 마지막 fully connected layer만 내가 풀고자 하는 데이터셋의 클래스 수에 맞게 바꾸어 학습시킨다.