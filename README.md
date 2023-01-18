# leature5
## non-deterministic environment(sthochastic)
deterministic 환경: action을 했을 때, 그 action에 대해 기대되는 state가 확정적인, 결정적인 환경 -> 이 환경에서 Exploit & Exploration 방법을 적용할 경우 적어도 80%의 정확도를 얻음
non deterministic 환경: agent에게 운이 적용(무작위성 가짐) -> 확룰적인 환경

### sthochastic 환경에서 q learning
<img width="398" alt="스크린샷 2023-01-18 오후 11 47 29" src="https://user-images.githubusercontent.com/121830114/213204269-db611b44-85b5-47c6-9918-562af45c1fb4.png">
<img width="300" alt="스크린샷 2023-01-18 오후 11 47 19" src="https://user-images.githubusercontent.com/121830114/213204284-5673c436-362b-4d51-b948-0a35b1acd7cd.png">
정확도가 무척 낮음 stochastic한 환경에서는 아무리 지도(Q)가 정확하더라도 언제든지 도랑에 빠지거나 잘못된 길로 가버리기 쉽상이다.<br>
해결책: Q를 100% 신뢰하는 것이 아닌 어느 정도만 신뢰하는 전략 취함

