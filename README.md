# 40easy

쉽게 설명하는 40가지 컴퓨터 과학 개념 (원문 - http://carlcheo.com/compsci)

컴퓨터 과학에 대한 이론과 개념을 [재미있고](https://www.youtube.com/watch?v=P2SsIYEbCio) [흥미롭게](https://www.youtube.com/watch?v=lhlBWlhS7Vg) 배울 수 있도록 비유와 최소한의 기술 용어를 사용해서 작성한 목록들입니다. 
일반적인 개념만 이해하면 누구나 쉽고 빠르게 딸 수있는 컴공 학위라고나할까요.

중요한점 :
- 출처가 없으면 제가 작성한것입니다. 잘못된 부분이 있으면 바로잡아주시고 제안해주세요.
- 제목은 각각의 위키피디아 글로 링크됩니다. 자세하고 진지한 설명은 위키피디아를 참고하세요.
- 비유는 이해하기 엄청 쉽지만, 완벽하게 이해하긴 어렵습니다. 개념을 완전히 이해하려면 [가장 기초적인것부터 공부해야 합니다.](https://www.youtube.com/watch?v=L-s_3b5fRd8&t=22m38s)

또한, 만약 프로그래밍을 지금 시작하시는거라면 [이 인포그래픽](http://carlcheo.com/startcoding)을 참고하세요.


# 주요 개념 #1 – 알고리즘과 자료구조

## 1.1 – [빅 O 표기법 (점근 표기법)](http://en.wikipedia.org/wiki/Big_O_notation)

[해리포터 전편 블루레이](http://amzn.to/1F2nDhh)를 아마존에서 주문하고 동시에 온라인에서 다운로드도 한다고 해봅시다.
어떤게 더 빠를지 생각해볼까요. 배송이 도착하려면 아마 몇일이 걸릴거고 다운로드는 30분만에 완료될겁니다. 너무 차이가 큰죠?

이번엔 몇개의 영화들을 더 많이 산다고 해보죠. 반지의 제왕, 트와일라잇, 다크나이트 트릴로지 등등.
그리고 동시에 이 영화들을 다 다운로드 하면 어떨까요? 배송은 마찬가지로 몇일 걸리겠지만 다운로드는 3일은 기다려야 완료될겁니다.
온라인으로 몇편을 구매하든 배송기간에 영향을 미치지 않습니다. 출력은 늘 동일합니다. 이걸 O(1)이라고 합니다.
다운로드 시간은 영화의 파일 사이즈에 비례해서 커지죠. 이걸 O(n)이라고 합니다.

확인해보니, 온라인 주문이 다운로드보다 더 확장이 쉬운걸 알 수 있습니다.
빅 O 표기법에 대해하는것은 알고리즘의 효율성과 확장성을 측정하는데 중요한 도움을 줍니다.

참고: 빅 O 표기법은 알고리즘에서 최악의 케이스를 나타냅니다. 위의 예제에서 O(1)과 O(n)이 최악의 케이스라고 가정합시다.

더보기: [Big O Notations (video)](https://www.youtube.com/watch?v=V6mKVRU1evU), [Plain English explanation of Big O](http://stackoverflow.com/questions/487258/plain-english-explanation-of-big-o), [A Beginner’s Guide to Big O Notation](http://rob-bell.net/2009/06/a-beginners-guide-to-big-o-notation/)

## 1.2 – [정렬 알고리즘](http://en.wikipedia.org/wiki/Sorting_algorithm)
[![https://youtu.be/kPRA0W1kECg](http://img.youtube.com/vi/kPRA0W1kECg/0.jpg)](https://youtu.be/kPRA0W1kECg)

더보기: [Sorting Algorithm Animations](http://www.sorting-algorithms.com/), [Beautiful and configurable visualizations of sorting algorithm](http://sorting.at/) 

## 1.3 – [재귀](http://en.wikipedia.org/wiki/Recursion_%28computer_science%29)

>영화관에 있는 누군가가 당신에게 몇번째 열에 앉아있냐고 묻습니다. 당신은 몇번째 열인지 세기 귀찮아서 앞사람에게 물어봅니다. 앞사람이 한 대답에서 1만 더하면됩니다. 똑똑하군요! 그치만 앞사람도 당신과 똑같이 행동했습니다. 마침내 제일 앞에 앉은 사람에게 질문이 도달했습니다. "나는 1번 열에 앉았어요!". 거기서부터 올바른 메시지가(1씩 증가하면서) 물어본 사람에게까지 전달됩니다.
Aaron Krolik/[Quora](http://go.skimresources.com/?id=80757X1532039&xs=1&isjs=1&url=http%3A%2F%2Fwww.quora.com%2FHow-should-I-explain-recursion-to-a-4-year-old%2Fanswer%2FAaron-Krolik&xguid=62f2a82b862028b7bb904f718462b28f&xuuid=4ac041a637bc9d05bb56b8d0a0d91658&xsessid=&xcreo=0&xed=0&sref=http%3A%2F%2Fcarlcheo.com%2Fcompsci&xtz=-540&jv=13.20.0-stackpath&bv=2.5.1)

[드로스테 효과](https://en.wikipedia.org/wiki/Droste_effect)로 알려진 다른 예가 있습니다.
간호사가 쟁반을 들고 있고 그 위에 컵과 작은 그림이 그려진 코코아 통이 있습니다. 코코아 통의 그림은 간호사가 같은 쟁반을 들고 서있는 그림이 계속해서 그려져 있습니다.

![드로스테효과](http://carlcheo.com/wp-content/uploads/2015/04/Droste.jpg)

드로스테 효과로 알려진 [다른 예제들](http://www.webdesignerdepot.com/2009/09/50-stunning-examples-of-the-droste-effect/)이 있습니다.

아직 재귀가 뭔지 모르시겠다면 [여기](https://github.com/serendip811/40easy#13--재귀)를 확인하시고... 아니면 계속 읽어내려갑시다.

## 1.4 – [Big Data](https://en.wikipedia.org/wiki/Big_data)

>정원의 수도관에 누수가 생겼다고 해봅시다. 문제를 해결하기 위해 양동이와 씰링 재료들을 가져왔습니다. 잠시 후에 누수가 더 커져서 더 큰 도구를 가지고올 배관공이 필요하다는 것을 알수 있습니다. 그 사이에 당신은 여전히 양동이를 이용해서 물을 퍼냅니다. 잠시 후, 지하에 엄청나게 많은 양의 물이 누수되어 흐르고 있다는 것을 깨닫게 됩니다. 매 초 10L의 물을 처리해야 합니다. 양동이로는 더는 감당할 수 없습니다. 물의 양과 속도가 증가했기 때문에 문제 해결을 위해 완전히 새로운 다른 방법의 접근이 필요합니다. 도시가 범람하는 것을 막으려면 막대한 토목 공학 전문 지식과 정교한 통제 시스템을 필요로하는 거대한 댐을 정부가 만들어야 할 수도 있습니다.
Balaji Viswanathan/[Quora](http://go.skimresources.com/?id=80757X1532039&xs=1&isjs=1&url=http%3A%2F%2Fwww.quora.com%2FWhat-is-Big-Data-16%2Fanswer%2FBalaji-Viswanathan-2&xguid=62f2a82b862028b7bb904f718462b28f&xuuid=41a28108e3b9bc3087637bbd35c0ce1c&xsessid=&xcreo=0&xed=0&sref=http%3A%2F%2Fcarlcheo.com%2Fcompsci&xtz=-540&jv=13.20.0-stackpath&bv=2.5.1)

빅 데이터는 기존의 데이터 처리 도구로는 관리 할 수없는 크고 복잡한 데이터 세트를 말합니다.

더보기: [Big Data by TED-Ed (video)](https://www.youtube.com/watch?v=j-0cUmUyb-Y), [What is Big Data and Hadoop (video)](https://www.youtube.com/watch?v=FHVuRxJpiwI)


