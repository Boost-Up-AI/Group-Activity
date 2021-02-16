## Day16 피어세션 16:00~17:30

- 알고리즘 코드 리뷰
- BFS
    - 구슬 탈출4: [https://www.acmicpc.net/problem/15653](https://www.acmicpc.net/problem/15653) \
    queue에는 원소를 적게 담을수록 좋다. (메모리 초과 주의) \
    처음에 R,B의 위치를 파악한 뒤 '.'으로 바꿔주기 \
    move : O,#을 만날 때까지 이동하는 함수, 이 때 distance도 같이 저장하기 \
    move를 적용한 후에 R=B 이면 이동거리가 더 긴 공을 한 칸 이동시켜준다. \
    - 달이 차오른다, 가자: [https://www.acmicpc.net/problem/1194](https://www.acmicpc.net/problem/1194) \
    비트마스킹을 이용하여 키와 문을 6자리 이진수로 표현한 후 대조한다. \
    a=1, b=10, c=100, d=1000, e=10000, f=100000 \
    키가 6개밖에 없으므로 비트마스킹을 사용하면 좋다. 하지만, 키가 더 많으면 비추. \

- DFS
    - 알파벳: [https://www.acmicpc.net/problem/1987](https://www.acmicpc.net/problem/1987) \
    visited에 알파벳을 append하면 시간초과. \
    ASCII 코드를 이용하여 visited를 26개짜리 리스트로 만들어놓기 \
    dfs 재귀를 돌고 나서 상위노드로 백트래킹을 할 수 있게 False로 바꿔주기!! \
    - 숫자고르기: [https://www.acmicpc.net/problem/2668](https://www.acmicpc.net/problem/2668) (cycle 찾기) \
    DFS는 기저조건을 어떻게 설정하는지(언제 return할지)가 핵심이다. \
    DFS의 특징: 가지치기(pruning) → 필요없는 방향으로 탐색하지 않으므로 while문보다 시간 단축됨. \
    - 텀 프로젝트: [https://www.acmicpc.net/problem/9466](https://www.acmicpc.net/problem/9466) (cycle 찾기) \
    subcycle을 발견하면 걸러내야 시간초과에 안 걸린다. \

- Further Question: 이분탐색
    - 배열에서 이동: [https://www.acmicpc.net/problem/1981](https://www.acmicpc.net/problem/1981) \
    최소~최대 구간을 반씩 나눠 둘 중 어느 쪽인지 선택 → 반복 \
