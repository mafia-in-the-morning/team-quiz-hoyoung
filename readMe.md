# 선풍기 틀기
-사용자가 
# 시스템요구사항
1. 선풍기는 전원이 연결되어 있을 때만 작동한다.
2. 선풍기는 켜고 끌 수 있다.
3. 선풍기는 회전하는 바람 날개를 가지고 있으며, 회전 속도를 조절할 수 있다.
4. 회전 속도는 낮음, 중간, 높음으로 구분된다.
5. 선풍기는 회전 방향을 바꿀 수 있다.
6. 회전 방향은 왼쪽, 오른쪽으로 구분되며, 중앙 위치는 정지 상태이다.
7. 선풍기는 자동으로 일정한 시간이 지나면 자동으로 꺼지도록 설정할 수 있다.
8. 선풍기는 사용자가 원하는 시간까지 작동할 수 있도록 타이머 기능을 제공한다.
9. 선풍기는 작동 중인 상태에서 날개가 막혔을 경우 자동으로 정지하도록 되어 있다.


#커뮤니케이션 디이어그램 정보
┌─────────────────┐
│    User         │
└─────────────────┘
│
│
│ 1. 전원 연결
│
│
┌─────────────────┐
│    선풍기       │
└─────────────────┘
│
┌─────────────┬─────────────┬─────┴────┐
│ 2. 켜기/끄기  │ 3. 회전 속도 조절 │ 5. 회전 방향 변경
│              │               │         │
│              │               │         │
▼              ▼               ▼         ▼
┌─────────────────┐ ┌─────────────────┐ ┌─────────────────┐
│   Power ON/OFF  │ │  Rotation Speed  │ │ Rotation Direction│
└─────────────────┘ └─────────────────┘ └─────────────────┘
│              │               │         │
│              │               │         │
│              │               │         │
4. 자동 종료 │     7. 종료 안내    │    6. 방향 변경 안내  │
│              │               │         │
│              │               │         │
▼              ▼               ▼         ▼
┌─────────────────┐ ┌─────────────────┐ ┌─────────────────┐
│  Auto Shutdown  │ │    Shutdown     │ │ Direction Change │
└─────────────────┘ └─────────────────┘ └─────────────────┘
