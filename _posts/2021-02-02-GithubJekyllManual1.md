---
title: Jekyll을 이용해서 깃허브로 블로그 만들기_1.Jekyll 설치 및 github 연동
date: 2021-02-02
categories: [Manual]
tags: [manual, github, blog, jekyll]
pin: true
math: false
toc: true
toc_sticky: true
---

## __0.전제 조건__

본 과정을 수행하기 위해서는 깃허브 계정이 있어야 한다. 로컬에서 관리하려면 git과 ruby가 설치되어 있어야 한다.

[Github 가입 방법](https://chalgx.github.io/Manual/GithubManual1/)

[Ruby 설치 방법](https://chalgx.github.io/Manual/RubyInstallManual/)  

***

## __1.Jekyll 테마 선택__

Jekyll 순정 버전에서 본인이 원하는 대로 수정해서 사용할 수 있다. 아니면 무료 Jekyll theme 사이트에서 원하는 것을 선택해도 된다.

설치 방법은 기본적으로 해당 테마가 있는 github에 가보면 Readme.md에 자세하게 설명되어 있고 그것을 따르면 된다.

본 내용은 minimal-mistakes를 기준으로 작성했고 fork 하는 방식을 사용했다.

***

## __2.설치 과정__

![GithubJekyll1](/images/GithubJekyll1/Jekyll1.PNG)

깃허브로 원하는 Jekyll theme에 들어가면 상단에 Fork가 있다. 해당 버튼을 누르고 잠시 기다리면 fork가 완료된다.

![GithubJekyll2](/images/GithubJekyll1/Jekyll2.PNG)

제대로 됐다면 앞쪽 이름이 자신의 이름으로 바뀐다. 오른쪽에 있는 Settings에 들어간다.

![GithubJekyll3](/images/GithubJekyll1/Jekyll3.PNG)

Repository name을 자신의 계정명.github.io로 바꾼다.

여기서 계정명은 chalgx이므로 chalgx.github.io로 바꿨다.

바꾼 이후 Rename을 클릭한다.

Repository는 Public으로 공개되어 있어야 한다.

다시 Code로 돌아간다.

![GithubJekyll4](/images/GithubJekyll1/Jekyll4.PNG)

_config.yml에서 자신에게 맞게 수정해야 한다. 들어간다.

![GithubJekyll5](/images/GithubJekyll1/Jekyll5.PNG)

들어가면 다음과 같이 내용을 읽을 수 있다. 오른쪽의 수정 버튼을 눌러서 내용을 수정한다.

![GithubJekyll6](/images/GithubJekyll1/Jekyll6.PNG)

이중에서 url은 반드시 바꿔야 한다. 앞서서 바꾼 Repository명으로 바꾼다. "https://계정명.github.io"가 된다. 예시로는 "https://chalgx.github.io"다.

이외에도 Title 등 다양한 것들을 자신에게 맞게 수정한다.

창을 아래로 내려서 commit해서 저장한다.

***

## __3.로컬에서 Ruby 연동__

로컬에서 루비를 연동하면 로컬서버로 사이트를 확인할 수 있다. 수정한 내용을 바로 확인할 수 있고, 다양한 에러를 직접 확인할 수 있어서 매우 편리하다.

먼저 cmd, bash와 같은 터미널을 연다. 여기서는 git bash를 사용했다.

로컬에서 관리하기 위해 관련 파일을 저장할 곳을 정하고 깃허브에 있는 파일들을 다운로드한다.

```bash
git clone https://github.com/계정명/계정명.github.io
```

다음은 예시 화면이다.

![GithubJekyll8](/images/GithubJekyll1/Jekyll8.PNG)  

jekyll bundle을 설치해준다.

```ruby
gem install jekyll bundler
```

![GithubJekyll10](/images/GithubJekyll1/Jekyll10.PNG)

필요한 bundle도 설치해준다.

```ruby
gem install bundler
```

![GithubJekyll12](/images/GithubJekyll1/Jekyll12.PNG)

이제 로컬에서 사용할 수 있게 빌드한다.

```ruby
bundle install
```

![GithubJekyll13](/images/GithubJekyll1/Jekyll13.PNG)

완료되면 준비가 다 된 것이다.

터미널에 다음과 같이 입력하면 로컬 서버가 생성된다.

```ruby
jekyll serve
```

컴퓨터 내부 네트워크인 127.0.0.1:4000에 접속하면 생성된 페이지를 볼 수 있다. 크롬이나 익스플로러 같은 웹브라우저 주소창에 입력하면 된다.

_drifts의 폴더 안 내용도 테스트하고 싶다면 다음과 같은 옵션을 붙인다.

```ruby
jekyll serve --drifts
```
