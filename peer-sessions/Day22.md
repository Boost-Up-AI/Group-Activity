## 피어세션 16:00 ~ 17:30

# 공통 논문 리뷰
- Dropout
    - 기존에 사용하던 Model Combination은 DNN의 규모와 연산량 증가
    - Dropout의 효과는 여러 개의 "Thinned Network"를 학습시키는 것과 같음
    - Thinned Network == Dropout 과정에서 생략되지 않는 뉴런들로만 구성
    - 학습에서 Dropout Rate으로 활용되는 확률 p를 테스트 단계에서 가중에 곱해 approximate averaging method를 제안
    - General Technique, not specific to any domain
    - (정리된 PDF 파일은 attachment 폴더에 있습니다)

- ADAM Optimization
    - 메모리 요구사항이 적으며, 데이터/파라미터 차원이 클 경우에 적합
    - 노이즈가 크거나 기울기가 sparse할 때 적합
    - 하이퍼파라미터가 직관적이며 거의 조정하지 않아도 됨
    - 1차 gradient만 필요한 최적화 방법이며, 잡음이 높은 목적함수에 적용이 잘 되지 않는 SGD의 보완책
    - Adagrad + RMSprop의 장점을 종합해서 설계