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

## 1.5 – [데이터 구조](https://en.wikipedia.org/wiki/Data_structure)

모든 컴퓨터 과학자들과 프로그래머가 적어도 이것들을 알아야 합니다:

- [Array](http://en.wikipedia.org/wiki/Array_data_structure)
- [Tree](http://en.wikipedia.org/wiki/Tree_%28data_structure%29)
- [Stack](http://en.wikipedia.org/wiki/Stack_%28abstract_data_type%29)
- [Queue](http://en.wikipedia.org/wiki/Queue_%28abstract_data_type%29)
- [Graph](http://en.wikipedia.org/wiki/Graph_%28abstract_data_type%29)
- [Hash Table](http://en.wikipedia.org/wiki/Hash_table)
- [Linked List](http://en.wikipedia.org/wiki/Linked_list)
- [Heap](http://en.wikipedia.org/wiki/Heap_%28data_structure%29)

# Core Concept #2 – [인공 지능](http://en.wikipedia.org/wiki/Artificial_intelligence)

## 2.1 – [탐욕 알고리즘](https://en.wikipedia.org/wiki/Greedy_algorithm)

하이킹을 가고 있다고 상상해봅시다. 가능한 한 최고봉에 도달하는 것이 목표입니다. 올라가기 전에 지도를 펼쳐보지만 지도에 표시된 경로가 수천 가지입니다. 각각의 경로를 평가할 시간도 없고 너무 귀찮습니다. 지도를 버려버립시다! 탐욕스럽고 근시안적인 간단한 전략으로 하이킹을 시작합니다. 가장 위쪽으로 기울어진 경로를 따라 올라갑니다.

여행이 끝나고 몸 전체가 아프고 피곤합니다. 처음으로 지도를 펼쳐 봅니다. 세상에! 계속 위로만 올라갈것이 아니라 진흙강을 건넜어야만 했네요.

탐욕 알고리즘은 최고의 즉각적인 선택을 하고 선택에 대해 다시 생각해보지 않습니다.


## 2.2 – [언덕 오르기 알고리즘](https://en.wikipedia.org/wiki/Hill_climbing)

이번에는 다른 언덕을 오르고 있습니다. 당신은 가장 높은 봉우리로 갈수 있는 길을 찾으려합니다. 그러나 지도도 없고 안개가 자욱해서 앞을 분간하기 어렵습니다. 여행을 더 쉽게하기 위해 경로를 추적하고 현재 고도를 측정하는 등산 앱을 다운로드했습니다.

언덕을 오르고 또 오릅니다. 오를 때마다 가장 높은 고도로 기록된 경로를 따라 오릅니다. 하지만 여행 중간에 약가 다른 경로를 선택합니다.

또 매번 다른 시작점을 무작위로 선택해서 출발할 수도 있습니다. 그래서 매번 비슷한 지역에 머물러 맴돌 가능성이 줄어듭니다.

언덕 오르기 알고리즘은 주변 솔루션을 만들어서 더 나은 솔루션을 찾으려고 시도합니다. 각각의 주변 솔루션은 지금까지 최고인 솔루션을 기반으로 단일 요소들을 수정하여 만들어집니다.

## 2.3 – [담금질 기법 알고리즘](https://en.wikipedia.org/wiki/Simulated_annealing)

에베레스트산. 당신이 직면한 가장 큰 도전입니다. 정상에 오르는 것이 목표이지만, 에베레스트산을 여러번 오르는 것은 비현실적입니다. 오직 한번의 기회뿐입니다. 신중할 필요가 있습니다. 항상 위쪽으로 올라가는 대신 가끔 낮은 지점으로 이동해서 다른 길을 탐색하고 잘못된 길로 접어들 확률을 줄입니다. 높이 올라가면 올라갈수록 낮은 지점으로 이동하여 탐색할 확률이 낮아집니다.

## 2.4 – [동적 프로그래밍](http://en.wikipedia.org/wiki/Dynamic_programming)
```
아빠: *종이에 “1+1+1+1+1+1+1+1 =”이라 쓴다.*
아빠: 정답이 뭘까요?
아이: *세보더나 3초 후에* 8이요!
아빠: *왼편에 “1+”이라 쓴다.*
아빠: 이번에는?
아이: *즉시* 9요!
아빠: 와우! 어떻게 그렇게 빨리 계산했지?
아이: 1만 더 더하면 되잖아요!
아빠: 이전 답이 8이라는걸 알았으니까 다시 계산할 필요가 없었구나. 똑똑하군!
```
Jonathan Paulson / [Quora](http://go.skimresources.com/?id=80757X1532039&xs=1&isjs=1&url=http%3A%2F%2Fwww.quora.com%2FHow-should-I-explain-dynamic-programming-to-a-4-year-old%2Fanswer%2FJonathan-Paulson&xguid=62f2a82b862028b7bb904f718462b28f&xuuid=dc8b6fa4a3da275e357375821cb77f27&xsessid=&xcreo=0&xed=0&sref=http%3A%2F%2Fcarlcheo.com%2Fcompsci&xtz=-540&jv=13.20.0-stackpath&bv=2.5.1)

위의 예가 메모이제이션을 설명하고 있습니다. (메모리제이션 아니고 메모이제이션임) 동적 프로그래밍에서 탑-다운 접근 방식은 이전에 계산한 값을 저장해두었다가 다음에 사용합니다.

더보기: [Dynamic Programming – From Novice to Advanced (TopCoder)](https://www.topcoder.com/community/data-science/data-science-tutorials/dynamic-programming-from-novice-to-advanced/), [Tutorial for Dynamic Programming (CodeChef)](http://www.codechef.com/wiki/tutorial-dynamic-programming)

## 2.5 – [머신 러닝](http://en.wikipedia.org/wiki/Machine_learning)

Pararth Shah가 [여기](http://go.skimresources.com/?id=80757X1532039&xs=1&isjs=1&url=http%3A%2F%2Fwww.quora.com%2FHow-do-you-explain-Machine-Learning-and-Data-Mining-to-non-Computer-Science-people%2Fanswer%2FPararth-Shah&xguid=62f2a82b862028b7bb904f718462b28f&xuuid=dc8b6fa4a3da275e357375821cb77f27&xsessid=&xcreo=0&xed=0&sref=http%3A%2F%2Fcarlcheo.com%2Fcompsci&xtz=-540&jv=13.20.0-stackpath&bv=2.5.1)서 훌륭한 비유를 썼는데, 너무 길어서 옮기지는 않습니다.

## 2.6 – [P vs NP Problem](https://en.wikipedia.org/wiki/P_versus_NP_problem)

P vs NP 는 컴퓨터 과학계에서 가장 유명하고 중요한 풀지못한 문제중 하나입니다.

곱셈 문제가 있다고 합시다.
> Q1: 7 x 17 = p

정답은 119입니다. 풀기 너무 쉽죠? 그럼 거꾸로 이문제는 어떨까요?
> Q2: p x q = 119 (p & q cannot be 1 & 119)

두번째 문제를 풀기 위해서, Q1을 보지 않았다면, 아마 2부터 118까지 모든 숫자들을 넣어봐야 할것입니다. [소인수들](https://en.wikipedia.org/wiki/Integer_factorization)을 쉽게 찾을 수 있는 효율적인 알고리즘을 아직 찾아내지 못했습니다.

이 문제는 어떨까요: p가 7일수 있을까요? 아마 쉽게 답할수 있을겁니다. 그냥 119를 7로 나눠보면 되니까요!

곱셈은 쉽습니다. 하지만 소인수를 찾아내는 것은 어렵습니다.

Q1은 풀기 쉽기 때문에 P(다항식)문제입니다. 컴퓨터는 두 수가 엄청나게 크더라도 별로 시간을 들이지 않고 곱셈을 해낼수 있습니다.

Q2는 정의하기는 쉽지만 해결하기는 어렵기 때문에 NP(비 결정식 다항식)문제입니다. 119의 소인수를 찾는 것은 컴퓨터가 계산하기 쉽지만 500자리의 숫자는 어떨까요? 지금은 어떤 컴퓨터에서도 불가능합니다.

중요한 부분은 다음과 같습니다. NP문제 (예:분해) 또한 P문제(예:곱셈)아닐까요? 단지 NP문제를 풀기 위한 효율적인 방법을 찾지 못한것 아닐까요? 
NP문제는 정말 해결하기 어려울까요? 아니면 훌륭한 알고리즘을 가진 멋진 과학자 (혹시 당신?)의 "유레카!"가 필요합니까? 아니면 인간이 너무 어리석은걸까요? 인간보다 [훨씬 지능이 높은 기계나 생명](https://www.youtube.com/watch?v=aTZyVZBtP70&t=8m46s)이 있다고 상상해봅시다. 그들은 우리가 개미를 보듯이 우리를 볼것입니다. 우리의 지능 수준은 그들에게 너무 하찮을것 입니다. P vs NP 문제를 푸는 것은 그들에게 1 + 1을 푸는 것과 같습니다!

그럼 P vs NP 문제가 왜 중요할까요? 우리가 P = NP를 증명할 수 있다면, [모든 NP 문제](https://en.wikipedia.org/wiki/List_of_NP-complete_problems)가 컴퓨터가 계산할만한 시간 내에 쉽게 해결 될 수 있다는 것을 의미합니다. 우리는 암([단백질 접힘](http://en.wikipedia.org/wiki/Protein_folding))의 치료, 암호 ([RSA](http://en.wikipedia.org/wiki/RSA_%28cryptosystem%29)) 해독 등을 할수 있을 것입니다. 세상을 바꾸는것이죠!

P vs NP는 클레이 수학 연구소(Clay Mathematics Institute)의 [7가지 밀레니엄 상 문제들](http://www.claymath.org/millennium-problems) 중 한가지입니다. 첫번째 정답자에게 1백만 달러가 주어집니다.

더보기: [P vs. NP and the Computational Complexity Zoo (video)](https://www.youtube.com/watch?v=YX40hbAHx3s), [Simple Wikipedia](http://simple.wikipedia.org/wiki/P_versus_NP)

이것도 봅시다: [프로그래밍 언어의 반지의 제왕 비유 [인포그래픽]](http://carlcheo.com/startcoding)
