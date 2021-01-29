---
title: 텀프로젝트의 추억_6.고행 그리고 기도
date: 2021-01-17 05:00:00
categories: [Essay]
tags: [essay, term project]
pin: true
use_math: true
toc: true
---

3학년 2학기. 마이크로프로세서 2. 대학 생활 중 가장 고생했던 기간을 만들어준 프로젝트.

***

## __소문__

마이크로프로세서 2 과목을 하는 교수님은 2분이 있으셨다. 둘 다 중간고사 이후에는 텀프로젝트를 준비하는 기간을 주시는 데 한 분은 자유주제고 다른 한 분은 정해진 주제가 있었다. 바로 자율주행 모형자동차를 만드는 것이었다.  
  
누구를 들어도 특별히 상관없다고 생각했다. 그래도 그동안의 경험을 통해 자유주제보다는 정해진 주제를 잘 만드는 것을 잘 할 수 있는 사람이라고 생각해서 그 교수님을 선택했다. 실습 시험을 보는 것도 마음에 들었다.  
  
자동차의 모든 부품을 직접 구매하고 만능기판에 납땜해야 했다. 이미 만들어져서 핀만 꽂으면 되는 모듈은 사용이 불가능했다. MCU는 Atmega 128을 사용했다.  모형은 DC 모터와 서보 모터가 같이 있는 RC카 프레임을 이용했다.  
  
자율주행은 초음파 센서와 적외선 센서로 했다. 트랙의 라인을 따라서 양옆에 벽이 세워져 있다. 초음파 센서를 좌, 우, 앞 3방향으로 달아서 벽에 부딪히지 않게 주행하는 것이다.  
  
또한 벽이 없는 대신 바닥에 검은색 라인이 있어서 초음파가 아닌 적외선 센서를 쓰는 구간도 있었다.  
  
이외에도 LCD에 총 주행시간을 정확하게 표시해야 했다.
  
***

## __팀 - 놀랍도록 정확하게__

중간고사가 있기 몇 주 전에 팀 배정을 했다. 랜덤 방식이었다. 같이 졸업작품을 하기로 한 인원들과 같은 팀이 되기를 바랐다. 실력이 제법 괜찮았기 때문이다. 하지만 팀 배정은 놀랍도록 정확하게 우리 사이를 갈라놓았다. 한 팀당 4명인데, 우리 팀은 남는 인원까지 합해져서 5명이 한 팀이었다.  

납땜해본 경험이나 소프트웨어 작성하는 것에 자신 있는지 물어봤다. 기댈 수 있을 만한 사람은 없었다.  
  
그래도 얼핏 들으니 성적 좋고, 열심히 하는 사람도 포함된 듯했다. 그 정도면 충분했다. 그래도 운이 좋았다고 생각했다.  

***

## __구매 - 뜻 밖의 난관__

팀이 정해지자마자 조교는 프로젝트를 소개했다. 무엇을 만드는지, 어떤 부품을 사야 하는지, 어느 사이트에서 구매할 수 있는지 상세하게 소개했다.  
  
그리고 지금 당장 구매를 하라고 했다. 특히 모형 자동차 프레임은 지금 주문하면 한 달 뒤에 온다고 했다.  

센서나 부품은 사이트에서 쉽게 구매할 수 있었는데 프레임이 문제였다. 중국에서 직구하는 것인데 통관배송 등 생소한 작업을 거쳐야 했다. 팀원 중에서 직구 경험이 있는 사람이 있는지 물어봤는데 아무도 없었다. 좀 헤매다가 며칠 늦게 주문을 완료했다.  

부품, 센서들은 금방 배송이 됐다. 프레임은 하필 검사 품목에 걸렸는지 가장 늦게 배송됐다. 우리보다 늦게 주문한 팀도 있었는데 더 늦은 것이다.  
  
그래도 아슬아슬하게 중간 평가받기 직전에 배송을 받을 수 있었다.

***

## __회로도 - 좋을 때__

OrCad로 회로도를 제출하는 게 첫 번째 과제였다. 하지만 바로 중간고사 기간이라 회로도를 그릴 시간이 많지 않았다.  
  
다행히도 학기 초에 작년 강의자료를 구해서 필요한 부품, 센서들이 무엇인지 파악했고 그것을 기반으로 틈틈이 준비를 해왔다. 제출할 때 즈음에는 거의 완성된 상태였다.  
  
미리 해놓는다는 철칙을 지킨 덕분에 편하게 넘어갈 수 있었다. 또 하드웨어를 만드는 작업을 빠르게 시작할 수 있었다.

***

## __하드웨어 제작 - 불행의 시작__

중간고사가 끝나자마자 바로 납땜에 돌입했다. 납땜이 처음인 사람에게는 어떻게 해야 하는지 일일이 시범을 보여주면서 알려줬다.  
  
주말, 공간 때마다 납땜했다. 각자 시간표에 맞게 일을 나누려 했는데 데이트, 다른 공모전 참여 등으로 바쁜 인원들이 있었고 그때는 그냥 내가 일을 맡아서 했다.  
  
전자회로 2 들을 때 납땜을 한 것 이후로 현장실습으로 PCB 기판에 SMD 타입의 소자를 납땜하면서 실력이 많이 늘었다고 생각했다. 어느 부분을 먼저 납땜해야 하는지 순서를 정하고, 중간 테스트를 수행하고, 깔끔하게 납땜하기 위해 노력했다. 확실히 현장실습 때의 경험이 도움이 됐다.
  
하지만 만능 기판은 차이가 있었고, 무엇보다 여러 명이 작업할 경우 고려해야 할 것이 있다는 것을 몰랐다.  
  
여러 명이 하다 보니 앞에 했던 사람이 어디서부터 어디까지 했는지 알기 힘들었다. 또 기존에 생각해놨던 배선 경로를 몰라서 자신에게 가장 편한 대로 선을 연결했다.
그래서 납땜 선로가 깨끗하지 않고 엉켰다. 또 실수로 잘못된 핀을 연결해서 수정하느라 고생하는 경우도 많았다.  

회로도는 스케치 형식이기 때문에 만능기판으로 납땜하는 실제 상황과는 다른 것이 많았다.  

만능기판에 회로를 그리는 프로그램을 이용해서 미리 그려놓을 필요가 있었다. 하지만 툴을 한 번도 사용한 적이 없어서 불편하고, 이미 상당히 진행해서 그냥 그대로 진행했다.  
  
회로도 대로 따라서 만들었는데 LCD가 작동하지 않는 문제가 있었다. 멀티 미터나 오실로스코프로 보면 전원은 정상적으로 들어가고 있었다. 다른 MCU로 테스트를 해봤는데 소스 코드, LCD 둘 다 문제가 없었다.  
  
바로 전 여름방학 때 중학생을 대상으로 아두이노를 가르쳤는데 그때도 LCD에 글자가 표시되지 않는 문제가 있었다. 강의가 끝나고 LCD에 있는 가변 저항을 바꾸니 그제야 글자가 제대로 보였다. 전류가 부족해서 생기는 문제였다.  
  
그래서 같은 문제일 것으로 생각하고 기존 LCD 부분 회로를 조금 바꿔서 가변 저항을 넣어서 납땜했다. 예상대로 가변 저항을 이용해서 저항값을 조절하니 잘 나왔다.  
  
다른 팀들도 마찬가지로 똑같은 문제를 겪었다. 조교에게 왜 안 되는 회로를 줬냐고 물었더니 작년에는 됐다고 했다.  

한 팀은 최종 평가 바로 전날까지 LCD 문제를 해결하지 못했다. 잘못 납땜한 것으로 생각하고는 계속 다시 납땜했다고 한다. 그렇게 1~2일 만에 모두 납땜할 수 있을 정도의 실력이 되었지만, LCD에 글자가 표시되지 않았다.  
  
잠깐 연구실에 들렀을 때, 그 팀의 사람들이 영혼이 빠져나간 채로 앉아 있는 것을 봤다. LCD에 문제가 있다고 해서 내가 아는 것을 알려줬다. 그 문제가 맞았다. 하지만 그들은 문제를 고칠 생각이 없어 보였다. 아마 너무 지쳤기 때문일 것이다.  
  
서보모터도 문제였다. 힘이 너무 약해서 방향 전환을 하지 못했다. 크기는 비슷하면서 토크는 충분히 강한 서보모터로 교체해서 사용했다. 전기를 많이 먹는다는 문제가 있었지만 이미 전원부 납땜을 다 해서 어떻게 할 도리가 없었다. 그냥 부족하게 사용했다.  
  
작년에 사용한 프레임은 힘이 충분한 서보모터를 사용했으나 해당 사이트의 판매가 중단돼서 다른 곳을 알려준 것이었다. 또 전원도 전에는 3.7V 리튬이온 배터리 2개를 이용했다고 했다.  
  
모든 공강 시간과 주말 시간을 쏟아부어서 작업하는 바람에 다른 공부와 과제 할 시간이 없어져 버렸다. 그래서 계속 뒤로 미루기 시작했다.  

***

## __기본 동작 소프트웨어 제작 - 마지막 웃음__

납땜과 소프트웨어 제작을 동시에 했다. 순조로웠다. 납땜도, 소프트웨어 제작도 한 번에 잘 진행됐다. 하드웨어 완성 평가가 얼마 안 남았는데도 아직 다 못한 팀이 많았다. 많은 팀이 평가 전날까지 밤을 새워가며 했다.
  
우리 팀은 날 한 번 새지 않고 하드웨어 및 기본 동작 테스트를 통과했다. 다만 동작 테스트에서 모터 드라이버가 말썽을 부려서 감점이 있었다.  
  
이전부터 불안정하긴 했었다. 그래서 급하게 납땜을 했었는데 발열이 심해지는 증상이 나타났다. 그날은 그렇게 마무리되고 끝났다.  

집으로 돌아가면서 모터 드라이버 과열 증상의 원인에 대해서 찾아봤다. 그러다 전압, 전류가 모자랄 경우 발생할 수 있는 문제라는 것을 알았다.  
  
급하게 수정한다고 회로도와 좀 다르게 납땜을 했는데 생각해보니 전원 공급이 부족하게 연결해 놨다.  
  
아쉬웠다. 평가하는 순간에 납땜을 제대로 했다면 충분히 모든 점수를 획득할 수 있었을 터이다.  

그래도 점수 면에서 다른 팀들을 많이 앞지른 것에 만족했다.

***

## __주행 알고리즘 - 절망의 늪__

본격적으로 트랙에서 돌 수 있게 주행하는 코드를 만들기 시작했다.  

이때 즈음 학부 연구생이 되었다.  
  
처음 목표는 트랙에 딱 맞춰서 구간별로 코딩하는 것이 아니라 트랙이 어떻든 돌 수 있는 코드를 만드는 것이었다.  
  
초음파 센서로 받는 데이터는 정확하지 않다. 그래서 알파-트림드 평균 필터를 넣어봤다. 작동은 더더욱 되지 않았다. 연산 문제인가 싶어서 미디언 필터를 사용했다.  

적외선 센서는 자동차의 그림자 때문에 오작동하는 경우가 많았다. 결국 사용을 포기하기로 했다. 조교에게 물어보니 굳이 사용할 필요 없고 트랙만 잘 돌면 된다고 했다. 초음파 센서로 감지되지 않는 구간을 대비해서 별도로 코드를 작성해서 넣었다.  
  
전원은 AA 건전지를 이용했다. 6개씩 2개, 총 12개의 건전지를 한 번에 사용했다. 어댑터를 이용해보려 했지만, 맞는 전압이 없었다.  
  
적정 전압보다 높은 전압의 어댑터는 있어서 그걸 이용해보기로 했다. 어댑터에 저항을 이용해서 전압분배 회로를 만들어봤다. 전원을 꽂으니 연기가 났다. 안정화하기 위해 커패시터를 달았다. 여전히 연기가 났다. 다이오드를 달았다. 괜찮은가 싶더니 연기가 났고 결국 포기했다.  
  
어댑터를 사용하면 선을 들고 차량을 따라다녀야 한다는 문제가 있고, 또 최종 평가는 건전지로만 동작해야 했기 때문에 그냥 건전지를 사용했다.  

그렇게 폐건전지가 쌓여갔다. 내 연구실 서랍 안 박스에는 폐건전지들이 나뒹굴었다.

아무리 해봐도 생각한 대로 동작하지 않았다. 차량은 절대 직선으로 가주지 않았다. 양옆의 벽은 너무 가까워서 조금씩 방향 전환하는 기준을 찾는 것도 힘들었다.  

건전지의 잔량에 따라 모터의 동력이 바뀌고 그에 따라서 모든 기준치 값이 바뀌어야 했다.  
  
무엇보다 초음파 센서가 문제였다. 문제가 있을 것이라고 쉽게 예상할 수 있는 센서였기에 LCD에 감지되는 값을 출력해서 계속 모니터링했다. 특정 부분에서 멀티패스 효과가 나타나는 것인지 문제를 일으켰다. 또 값이 제대로 출력되어도 방향 전환이 제대로 이루어지지 않았다.
  
원인을 파악할 수 없었다. 하지만 계속 매달렸다. 너무 늦어서 학교 연구실에서 자거나, 사우나에서 잠을 잤다. 날을 새기도 했다. 되지 않는 걸 되게 해야 했다. 정신이 피폐해져 갔다. 울고 싶었다.  
  
멘탈을 붙잡을 수 없었다. 팀장으로서 팀원들에게 동기를 부여하고 기운을 북돋아야 하는데 내가 가장 먼저 망가지기 시작했다. 이 길은 내 길이 아니라는 생각이 강하게 들었다.  
  
미뤄놓은 일들도 많았다. 하지만 이 텀 프로젝트 때문에 다른 건 할 수 없었다.  

트랙을 잘 주행하는 팀들이 나오기 시작했다. 초조해졌다. 도대체 우리가 만든 건 무엇이 문제일까. 저 사람들은 어떻게 한 것일까. 센서 탓, 환경 탓마저 하지 못 할 상황이 돼버렸다.  
  
빨리 들어오는 것을 포기하고 완주를 목표로 잡았다. 소스 코드도 구간에 맞춰서 코딩하는 것으로 바꿨다.

초음파가 값을 이상하게 받는 것 같으니 아예 조금 움직이고 멈추고 값을 받고 기다렸다가 다시 조금 움직이고 멈추고 값을 받고 하는 방식으로 바꿔버렸다. 근데 희망이 보였다. 생각한 대로 자동차가 움직여줬다.  
  
정지한 상태로 값을 받아서 초음파 센서 사용 시 발생하는 간섭이나 노이즈 문제가 해결되는 것이라고 생각했다.  
  
우스꽝스럽긴 하지만 되는 게 어디인가. 그렇게 그런 상태에 맞춰서 코딩했다.  
  
얼추 되기 시작하자 또 욕심이 생겼다. 중간에 멈추는 것을 그만두고 계속 굴러가도록 하는 식으로 바꿨다.  

***

## __수리 - 반복되는 악몽__

괜찮던 하드웨어가 문제를 일으키기 시작했고 다시 납땜하는 경우가 잦아졌다. 납땜했었는데 빠지고, 선이 끊어지는 등의 문제가 발생했다. 핀 소켓이 너덜너덜해지다 빠져버리는 문제도 발생했다.  
  
프로그램 짜는 것만 해도 시간이 없는데 그런 문제까지 겹치니 짜증이 솟구쳤다. 그래도 소프트웨어보다 하드웨어 고치는 건 훨씬 쉬었다.  
  
고치고, 고치고. 그러다 보니 더 손대기 힘든 지경까지 와버렸다. 평가받는 순간까지 버티길 바랄 뿐이었다.  

1학년 1학기 때 겪은 텀 프로젝트의 악몽이 몇 배나 증폭되어서 다가왔다. 움직이는 거 사용하지 말고, 불안정한 센서 사용하지 않아야 한다는 것을 알았지만, 프로젝트 주제가 정해져 있어서 어쩔 수 없었다.  

***

## __평가 - 오직 기도뿐__

다행히도 평가는 기말고사 기간 전이었다. 평가가 있기 바로 전날까지 날을 샜다. 하지만 더 한다고 나아질 것 같지는 않았다. 그래도 계속 매달려서 조금이라도 트랙을 더 주행한다면 가치가 있다고 생각했다.  
  
우리 팀 외에도 날을 새는 팀은 많았다.  

평가가 있기 불과 몇 시간 전부터 또 하드웨어가 말썽이었다. 그 무렵 난 소프트웨어에서 거의 손을 떼고 수리하는 일만 했다. 도저히 소프트웨어를 건드릴 엄두가 나지 않았기 때문이다.  
  
평가가 시작되었다. 이제 남은 건 기도뿐이었다. 우리와 함께 날을 샜던 팀은 트랙을 완주했다. 정말 부러웠다. 특히 하드웨어 버스 기사, 소프트웨어 버스 기사가 각각 1명씩 있는 팀이어서 더욱 그랬다. 내가 저 팀에 들어갔으면 하는 생각이 들었다.  

연습 때도 잘 되고 실전에서도 잘 된 팀도 있었다. 그런데 연습 때는 잘 돌다가 평가 당일에 문제가 발생한 팀들도 꽤 있었다. 모터가 타버리거나 운이 나빠서 벽에 부딪히는 경우였다. 기도가 부족했던 것이다.
  
우리 팀 차례가 됐을 때 난 보고 있을 수 없었다. 바깥으로 나갔다. 닫힌 문틈으로 흘러들어오는 환호성과 한숨을 들으며 대충 어느 정도 주행했을지를 가늠했다. 결과는 예상대로 좋지 않았다.  
  
너무 아쉬웠지만, 그래도 괜찮았다. 고생했으니까. 이제 끝났으니까. 그리고 많이 배웠으니까.  

내가 고민했던 다른 교수님의 수업은 달랐다. 학생 수가 너무 적어서 절대평가였다고 한다. 자유주제니까 대충해서 제출해도 교수님은 좋게 성적을 주셨다고 했다.  
  
그 말을 듣고 많이 억울했다.  
  
다행히 텀 프로젝트를 제외한 나머지 전부에서 점수를 좋게 받아서 커트라인으로 좋은 점수를 받을 수 있었다.  
  
팀원들에게 미안했다. 날 믿고 따라와 주고, 내가 요구하는 대로 해줬지만 좋은 결과를 주지 못했다.  

평가가 끝나고 연구실의 내 자리를 정리했다. 연구원들과 같이 밖으로 나가서 고기를 구워 먹었다.  
  
맛있는 것도 먹고, 잠도 푹 잤다.

***

## __문제의 원인__

지금 생각해보면 초음파 센서를 사용할 때 필터링 한다고 여러 번의 입력을 받고 그것을 처리하는 과정이 있다. 초음파 센서를 사용하기 위해 일정 시간 딜레이가 있어서 그동안은 아무 동작도 하지 않는다. 그런데 여러 번의 입력을 받고 게다가 3개를 사용하니 프로세스가 멈추는 시간이 엄청나게 늘어나는 것이다. 하지만 모터는 계속 돌아가고 있다.  
  
프로세스는 멈췄는데 모터는 돌아가니 원하는 대로 동작하지 않는 것은 당연했다. 초음파 센서로 얻은 값이 좀 튀더라도 그런 필터 설계는 하면 안 되는 것이었다. 아니면 다른 방법을 찾아야 했다.  
  
그래서 가고, 멈추고를 반복하는 방식으로 했을 때 잘 동작할 수 있었던 것이다. 그런 것도 모르고 초음파가 받아들이는 값 자체의 문제일 거라는 생각에 빠져서 이런 결과를 초래했다.  

***

## __교훈__

하드웨어는 균일하고 안정적이어야 한다. 외부 충격에 강해야 하고, 쇼트나 끊어질 염려가 없어야 한다. 하드웨어가 잘 돼야 소프트웨어가 의미가 있다.  
  
만능기판에 회로를 구성한다면 꼭 만능기판 툴로 그림을 그려놓자. 손으로 그리는 한이 있더라도 만능기판 모양에 맞춘 설계도가 필요하다.  
  
초음파 센서를 실시간성, 움직이는 것에 사용하려면 고려해야 할 것이 많다는 것을 명심하자.  
  
건전지 잔량에 따라 모터 속도가 달라진다. 즉 테스트할 때마다 주행하는 법이 달라진다. 안 된다고 계속 코드를 바꾸면 문제가 생긴다. 일반 건전지가 아닌 축전지나 성능 좋은 배터리를 사용해야 한다. 완충 상태일 때만 테스트를 한다면 일정한 모터 속도를 유지할 수 있다.  

코드에 딜레이는 최대한 없애야 한다.  
  
무엇보다 기도가 중요하다. 열심히, 간절히 기도해야 한다.  

***

## __텀 프로젝트의 추억 글__

- [1.움직이지마](https://chalgx.github.io/essay/MemoriesofTermProject1)
- [2.미루지마](https://chalgx.github.io/essay/MemoriesofTermProject2)
- [3.원래 한 번에 안 되는 거야](https://chalgx.github.io/essay/MemoriesofTermProject3)
- [4.안 배웠는데](https://chalgx.github.io/essay/MemoriesofTermProject4)
- [5.잘난척](https://chalgx.github.io/essay/MemoriesofTermProject5)
- [6.고행 그리고 기도](https://chalgx.github.io/essay/MemoriesofTermProject6)
- [7.에라 모르겠다](https://chalgx.github.io/essay/MemoriesofTermProject7)