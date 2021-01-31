---
title: Ruby 설치 방법
date: 2021-01-31
categories: [Manual]
tags: [manual, github]
pin: true
math: false
toc: true
toc_sticky: true
---

※ 본 내용은 2021-01-29 기준으로 작성된 것으로 이 글을 읽는 시점에 따라 적용되지 않을 수 있음

## __1. 공식 사이트에서 설치 파일 다운로드__

아래 사이트에 접속한다.

<https://www.ruby-lang.org/ko/downloads/>

그럼 아래와 같은 화면이 나온다.

![RubyInstall1](/images/RubyInstall/RubyInstall1.PNG)

자신의 컴퓨터의 운영체제에 맞는 것을 선택한다. 보통은 Windows일 것이다.

***

![RubyInstall2](/images/RubyInstall/RubyInstall2.PNG)

Download 버튼을 클릭한다.

***

![RubyInstall3](/images/RubyInstall/RubyInstall3.PNG)

보면 다양한 버전의 Ruby가 있다. 자신이 사용하고자 하는 목적에 따라 적합한 버전을 선택한다.

다른 프로그램을 사용하기 위해서라면 보통 Readme나 manual 같은 설명서에 어느 버전을 써야 할지 명시해준다.

특별히 그런 게 없다면 오른쪽에 현재 추천하는 버전이 있음으로 그것을 다운받는다.

***

## __2.설치 프로그램 실행__

다운로드 받은 설치프로그램을 실행한다.

![RubyInstall4](/images/RubyInstall/RubyInstall4.PNG)

라이센스 동의를 하고 Next를 눌러서 다음으로 넘어간다.

![RubyInstall5](/images/RubyInstall/RubyInstall5.PNG)

설치경로를 설정한다. 체크 박스 3개는 PATH 설정, .rb, .rbw 확장명을 가지는 파일을 자동으로 연결해주는 것, UTF-8을 기본 외부 인코딩으로 설정한다는 것이다. 특별히 설정해야 하는 게 아니면 그냥 둬도 상관없다.

Install을 눌러서 다음으로 넘어간다.

![RubyInstall6](/images/RubyInstall/RubyInstall6.PNG)

어떤 것을 설치할지 선택한다. 마찬가지로 절대 사용할 일이 없을 거란 걸 확신할 수 있는 게 아니면 다 설치해준다.

![RubyInstall7](/images/RubyInstall/RubyInstall7.PNG)

그러면 다음과 같이 설치가 진행된다.

![RubyInstall8](/images/RubyInstall/RubyInstall8.PNG)

체크 박스에 체크가 되어있도록 하고 Finish 버튼을 누른다. MSYS2development toolchain을 설치하기 위함이다.

설령 여기서 모르고 넘어갔다면 설치경로로 들어가서 따로 설치를 할 수 있다.

![RubyInstall9](/images/RubyInstall/RubyInstall9.PNG)

해당 창이 열리면 3을 누르고 엔터를 친다. 3번 옵션인 MSYS 2 and MINGW development toolchain을 설치하는 것이다.

![RubyInstall10](/images/RubyInstall/RubyInstall10.PNG)

다음과 같이 설치가 진행되고 완료된다.
