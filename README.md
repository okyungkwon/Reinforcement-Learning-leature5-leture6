# leature 5
## non-deterministic environment(sthochastic)
deterministic 환경: action을 했을 때, 그 action에 대해 기대되는 state가 확정적인, 결정적인 환경 -> 이 환경에서 Exploit & Exploration 방법을 적용할 경우 적어도 80%의 정확도를 얻음
non deterministic 환경: agent에게 운이 적용(무작위성 가짐) -> 확룰적인 환경

### sthochastic 환경에서 q learning
<img width="398" alt="스크린샷 2023-01-18 오후 11 47 29" src="https://user-images.githubusercontent.com/121830114/213204269-db611b44-85b5-47c6-9918-562af45c1fb4.png">
<img width="300" alt="스크린샷 2023-01-18 오후 11 47 19" src="https://user-images.githubusercontent.com/121830114/213204284-5673c436-362b-4d51-b948-0a35b1acd7cd.png">
정확도가 무척 낮음 stochastic한 환경에서는 아무리 지도(Q)가 정확하더라도 언제든지 도랑에 빠지거나 잘못된 길로 가버리기 쉽상이다.<br>
해결책: Q를 100% 신뢰하는 것이 아닌 어느 정도만 신뢰하는 전략 취함
<img width="429" alt="스크린샷 2023-01-18 오후 11 58 47" src="https://user-images.githubusercontent.com/121830114/213205260-2ba5f2af-304f-4a0b-98c8-800002b4d4cd.png">

<img width="603" alt="스크린샷 2023-01-18 오후 11 58 56" src="https://user-images.githubusercontent.com/121830114/213205276-70ad356f-2987-4d6a-a035-c9a0ee1cd2a4.png">

learning rate를 반영했을 때 Q learning 정확률
<img width="548" alt="스크린샷 2023-01-19 오전 12 01 58" src="https://user-images.githubusercontent.com/121830114/213206026-bb25db92-594a-4c92-8faf-afb09a7d1eb4.png">
<img width="300" alt="스크린샷 2023-01-19 오전 12 02 06" src="https://user-images.githubusercontent.com/121830114/213206038-8c6e0005-a6d3-4b42-8da3-bbdada30d761.png">
learning rate에 따라 정확률은 차이가 남

# Leture 6
## Q network
예를 들어 80x80 픽셀의 grayscale 게임 화면을 입력으로 받는 경우

