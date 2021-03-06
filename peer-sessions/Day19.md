## 피어세션 16:00~17:30

### PyTorch vs TF2
- PyTorch는 초기화 같은 것들을 많이 해야 하는데 TF2는 layer만 쌓으면 되므로 직관적이고 쉽다. \
하지만, pytorch가 lower-level이므로 조금 더 자유도가 높을 것이다.

### 논문 리뷰: Batch Normalization
1. 세부적인 수식은 강의에서 설명해주므로 모두 이해하려고 부담갖지 않아도 된다. 기존 방법의 한계점, 어떤 부분을 개선하기 위해 어떤 변화를 주었는지,\
어떤 식으로 활용될 수 있는지 등에 대한 이해를 목표로 하면 좋을 것 같다.

2. Batch Normalization의 성능이 잘 나오는 이유 \
![](https://user-images.githubusercontent.com/76163168/108344210-347c1880-7220-11eb-8498-b99c2be03e1e.png)


3. 6p  Accelerating learning rate decay의 의미
- 딥러닝 학습 시 초반에는 학습률을 높게 시작했다가 오버피팅을 방지하기 위해 점점 천천히 학습해야 하므로 학습률을 점차 줄여야 한다.
- Batch Norm을 사용하면 초기 학습률을 크게 설정할 수 있으므로 사용하지 않았을 때보다 더 빠르게 같은 lr로 줄일 수 있다.

4. 반박논문: How Does Batch Normalization Help Optimization? (2018)
- Batch norm을 사용했을 때 ICS가 커지는 실험을 근거로 반박함. 성능을 올릴 수 있었던 내부적인 요인은 loss smoothing이다.
- 추후 진행: Adam, 위의 반박논문 읽어보기


### 강의내용 질문 (강의록 8p)
|Q|=3  !=  |K|=|V|=4  ->  왜 쿼리벡터를 3개를 사용한걸까?? \
오늘은 강의를 다 듣지 못해서 내일 디스커션을 이어가겠습니다.


### 앙상블 모델
- 여러 가지 딥러닝 모델을 독립적으로 훈련시킨 뒤 각각 테스트한 결과를 투표하듯이 합친다.
- 여러 훈련된 net에서 특정 layer들을 선택한 뒤 feature를 추출하여 합친다. \
  (앙상블이라고 부르는게 맞는지는 모르겠습니다. 저희 교수님은 feature extraction이라고 표현하셨습니다.)


### 스몰토크
- 하이퍼커넥트 채용공고 https://career.hyperconnect.com/job/f2f89c67-fe43-4fbb-8df5-5a286723bfd3 \
채용공고에서 job description을 보면 경쟁사에게 기술스택을 노출하지 않기 위해 두루뭉술하게 나오는데 \
여기는 매우 자세하게 나와있어 참고하면 도움이 될 것 같다.

- 자신의 장점은 무엇인가? \
동현님: 무대뽀 정신!! 도전할 때 겁내지 않는 마인드!! \
지호님: 무언가 시작하면 끝까지 마무리지어 결과를 내는 성격, 꼼꼼한 공부 칭찬합니다:) \
지영님: 다른 사람의 장점을 잘 캐치하고 배우려는 자세 \
누리님: 잡다한 일이어도 나에게 주어진 것은 완벽하게 처리하려고 노력하는 편

- 오늘의 명언: 인생의 작은 성공을 많이 경험하는 것이 중요하다.

- 지영님이 꼽아주신 우리의 장점 \
동현님: 말할 때 ~해도 될까요? 정중 + 겸손 (절대로 을의 자세가 아닙니다 배려왕이십니다) \
지호님: 추진력 + 주도적인 성격, 독일에서 생활한 경험 (정말 멋진 도전이군요 부럽습니다!) \
지영님: 웃음장벽이 낮은 리액션 퀸!! (어제 장난친 거였습니다 주접 대환영ㅋㅋㅋ) \
누리님: 모르는 문제를 철저하게 공부해서 팀원들에게 공유 + 피어세션 분위기메이커 나야나^_^ 

- 제가 꼽은 지영님의 장점 \
저는 다른 캠퍼들의 발표를 들었을 때 웹개발과 연관지어 생각하는 지영님의 습관이 장점이라고 생각합니다. \
다양한 분야에 대해 배우고 흡수해서 본인의 프로젝트에 어떻게 활용할 수 있을지 생각해보는 게 중요한 태도인 것 같습니다. \
항상 관심있게 경청해주시고 정말 사소하더라도 질문해주시는 호기심 자체가 열정이 있다는 거니까요ㅎㅎㅎ
