# kotlin-blackjack

[게임 규칙](https://namu.wiki/w/%EB%B8%94%EB%9E%99%EC%9E%AD(%EC%B9%B4%EB%93%9C%EA%B2%8C%EC%9E%84)#s-4.1)

## 2단계

- [X] 블랙잭을 위한 덱을 구성한다
    - [X] 플레잉카드를 만든다 [참고](https://ko.wikipedia.org/wiki/%ED%94%8C%EB%A0%88%EC%9E%89_%EC%B9%B4%EB%93%9C)
        - [X] 플레잉카드는 4가지 중 하나의 슈트(suit)와, 끗수(denomination)를 가지고 있다.
        
- [X] 게임을 진행한 Player를 생성한다
    - [X] Player는 이름과, 자신이 받은 플레잉카드들을 가지고 있다.
    - [X] Player는 자신의 점수를 계산할 수 있다.
        - [X] Ace가 존재할 시의 계산법을 고려한다.
            - [X] 11을 더해도 `버스트`가 되지 않는다면 11을, 그렇지 않다면 1을 더한다.

- [X] 게임을 진행한다.
    - [X] 게임에 참여할 Player들을 입력받는다.
    - [X] 시작 시 Player들에게 2장의 패를 분배한다.
        - [X] BlackJack을 만족하는 유저가 존재하는지 확인하고, 만족한다면 게임을 종료한다.
    - [X] Player 순서대로 게임을 진행한다.
        - [X] 매번 카드를 draw 후 `버스트`가 됐는지 체크한다.
            - [X] `버스트`라면 게임을 끝낸다.
            - [X] `버스트`가 되지 않았다면 계속해서 카드를 뽑을지를 물어본다.
    - [X] 모든 Player가 게임을 종료했다면 결과를 출력한다.


- [ ] 딜러를 생성한다.
    - [ ] 딜러는 기본적으로 플레이어와 같다
    - [ ] 딜러는 자신이 16이하인지 여부를 확인하여 카드를 추가로 받아야하는지를 알려준다.

- [ ] Player 승,패 여부를 알 수 있다.
    - [ ] 딜러가 21보다 크면 버스트되지 않았던 Player들은 승리한다.
    - [ ] 딜러가 21보다 작으면 Player와의 점수를 비교한다.

- [ ] 최종 승패를 알려준다.
