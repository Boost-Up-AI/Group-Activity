## 피어세션 16:00 ~ 17:30

# 알고리즘 문제풀이 (카카오 인턴쉽 - 동굴탐험)
- 양방향 그래프를 단방향 그래프로 만들어서 계산을 효율적으로 수행
- Order에 있는 정보들을 단방향 그래프에 추가해야 함
- BFS로 그래프를 설계하고, DFS로 그래프를 탐색하면서 Cycle이 발생하면 False Return

# 알고리즘 기초 다지는 방법
- 지영님
    - 처음에는 백준에서 실버 문제부터 풀이
    - 기초적인 문제를 10문제씩 풀이 (DFS, BFS, 다익스트라, 이진탐색 -> 카테고리 존재)
    - 모르는 문제는 혼자 고민하지 않고 구글링, 남의 코드라도 한 번 코딩 해보는 경험이 중요
    - 문제를 풀면서 모르는 개념은 그때마다 찾는 것도 추천
- 지호님
    - 코딩테스트의 핵심은 접근법이 생각 나는지 or 안 나는지
    - 백준 골드문제 다 풀어보기
    - 처음 알고리즘 개념을 접할 때는 시간을 투자해서 이해
    - 접근법이 떠오르지 않으면 구글링, 남의 코드를 따라하면서 익히는 것도 좋은 학습
    - 알고리즘의 흐름과 데이터가 바뀌는 플로우를 따라가는데 시간을 투자해서 공부
    - 한 번에 한 유형만 집중적으로 하는 것이 효율적

# 논문 리뷰 (개인 관심 도메인)
- 누리님 (Parametric ReLU)
    - ReLU가 유행이 되면서 어느 정도 안정이 되었고, 발전을 위해 PReLU가 제안됨
    - PReLU를 Layer 별로, Channel 별로 다르게 설정할 수 있음
    - 적은 수의 Parameter를 추가해서 성능이 훨씬 좋아질 수 있음
    - 추가되는 Cost는 무시 가능한 정도임을 강조
    - Channel-Wise, Channel-Shared 방법 제시
    - Weight Decay를 사용하지 않은 이유는 ReLU와 같아지기 때문
- 지호님 (Image Super-Resolution Using Deep Convolutional Networks)
    - 저해상도 이미지를 고해상도로 바꾸는 Super-Resolution에 처음으로 딥러닝 적용
    - SRCNN 모델 설명
    - 이전에는 Sparse Coding 기반으로 Super Resolution 적용
    - CNN Layer를 더 늘려도 성능이 좋아지지 않음 -> Training의 어려움 때문
- 지영님 (Training Very Deep Networks)
    - Layer 층수가 깊어지면 학습이 어려워짐 -> Back-Propagation의 Gradient 손실
    - Highway Networks를 소개
    - LSTM에서 Cell-State가 하는 Method를 Motivation으로 설정
    - Depth가 깊은 Architecture에서 성능 향상
    - B_T라는 bias를 음수로 설정