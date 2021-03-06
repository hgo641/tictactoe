# tictactoe

Git 을 활용한 tic tac toe 게임입니다.

우선 선공/후공을 정하세요.
이후, 게임을 진행합니다.


repository를 살펴보면 다음과 같은 파일이 있습니다.

**board.md**

이 파일을 열어보면 다음과 같이 보여집니다.

```
| - | - | - |
|---|---|---|
|   |   |   |
|   |   |   |
|   |   |   |
```

하지만 markdown viewer를 이용해서 보시게 되면 아래와 같이 표로 보여지게 됩니다.

| - | - | - |
|---|---|---|
|   |   |   |
|   |   |   |
|   |   |   |

이건 markdown 문법이라는 건데 나중에 따로 보시면 될것 같고요,
우리는 이 markdown 표를 이용해서 게임을 진행할 예정입니다.

```
| - | - | - |
|---|---|---|
| 1 | 2 | 3 |
| 4 | 5 | 6 |
| 7 | 8 | 9 |
```

위를 보시면 1부터 9까지 적혀져 있는 공간이 있습니다. 이 가로 3칸, 세로 3칸의 표 안에서 번갈아가면서 o,x 를 자신의 차례대로 두면서 
가로, 세로, 대각선 방향 중 한칸이라도 자신의 표식이 일렬이 되면 승리인 게임입니다.

### 승리조건 

| - | - | - |
|---|---|---|
| o | x | x |
|   | o | x |
|   |   | o |

이 경우는 o가 승리


| - | - | - |
|---|---|---|
| x | x | x |
|   | o |   |
| o |   | o |

이 경우는 x가 승리

간단하시죠?

## 게임방법

자신의 차례에 
1. git pull로 최신 데이터를 내려받은 후
2. o 혹은 x 를 한 개 입력하고 
3. git commit을 해줘서 수정내역을 반영한 후
4. git push를 통해 서버에 올려주시면 됩니다.

이 1~4의 과정을 번갈아가면서 진행해보시면 됩니다.
