---
title: Jekyll을 이용해서 깃허브로 블로그 만들기_4.서치 콘솔, 애널리틱스, 웹마스터 연동
date: 2021-02-07
categories: [Manual]
tags: [manual, github, blog, jekyll]
pin: true
math: false
toc: true
toc_sticky: true
description: 만든 블로그를 서치 콘솔, 애널리틱스, 웹마스터에 연동하는 법에 대해 알아봤다.
---

_※ 본 내용은 2021-02-07 기준으로 작성된 것으로 이 글을 읽는 시점에 따라 적용되지 않을 수 있음._

블로그를 만든 후 구글이나 네이버에 검색되기 위해서는 서치 콘솔, 웹마스터에 사이트맵에 등록해야 한다.

블로그에 유입되는 사람 수와 그 특징을 자동으로 조사해주는 애널리틱스를 연동하면 관리하기 좋다.

해당 기능을 이용하기 위해서는 각각 구글과 네이버에 계정이 있어야 한다.

***

## __구글 서치 콘솔__

구글 서치 콘솔에 접속한다. 왼쪽 위에 있는 창을 통해 속성을 추가한다.

![GSC1](/images/Jekyll4/GSC1.PNG)

도메인 이름이 있다면 왼쪽에 입력하면 된다. 그렇지 않다면 오른쪽에 블로그 주소 이름을 넣는다.

깃허브로 사이트를 제작했다면 기본적으로 오른쪽에 자신의 사이트 이름을 넣으면 된다. 계정이름.github.io를 입력하면 된다.

![GSC2](/images/Jekyll4/GSC2.PNG)

사이트 소유 확인을 위해 다양한 방법을 선택할 수 있다. HTML 파일을 업로드 하는 것이 가장 간편하다.

해당 파일을 다운로드하고 jekyll이 있는 폴더에 넣는다.

![GSC3](/images/Jekyll4/GSC3.PNG)

다음과 그림과 같이하면 된다.

![GSC4](/images/Jekyll4/GSC4.PNG)

확인을 눌러서 인증을 받는다.

![GSC5](/images/Jekyll4/GSC5.PNG)

정상적으로 인식이 됐다면 소유권이 확인된다. 문제가 생기면 다시 시도한다. 혹은 다른 방법을 선택해서 한다.

![GSC6](/images/Jekyll4/GSC6.PNG)

메인 화면에서 왼쪽 위의 속성 검색에 자신이 설정한 블로그 주소가 뜨고 다음과 같은 화면이 나온다.

![GSC8](/images/Jekyll4/GSC8.PNG)

사이트 맵을 추가하면 자동으로 사이트를 크롤링한다.

색인에 Sitemaps를 클릭하면 새 사이트맵을 추가할 수 있다. 이전 포스팅에서 sitemap.xml파일을 만드는 과정을 진행했다.

해당 파일을 제출하면 된다.

사이트에서 색인을 생성하고 실제 검색 결과가 나오기까지는 며칠 걸린다.

![GSC9](/images/Jekyll4/GSC9.PNG)

***

## __구글 애널리틱스__

구글 애널리틱스 사이트에 들어가서 계정을 만든다.

이름을 설정하고 필요한 옵션을 선택한다. 이후 다음 버튼을 클릭한다.

![GA1](/images/Jekyll4/GA1.PNG)

속성 이름을 자유롭게 정한다. 밑에 고급 옵션 보기를 누른다.

![GA2](/images/Jekyll4/GA2.PNG)

고급 옵션을 통해서 유니버설 속성을 만들 수 있다. 기존에 사용했던 유니버설 버전 사용법을 먼저 소개하고 최근에 나온 GA4 연동법을 소개하겠다.

선택 후 다음을 누른다.

![GA3](/images/Jekyll4/GA3.PNG)

본인에게 알맞게 선택하고 만들기를 누르면 된다.

![GA4](/images/Jekyll4/GA4.PNG)

구글 애널리틱스 4를 만들도록 설정했다면 스트림 설정 창이 뜬다. 지금 등록하고자 하는 건 웹 블로그이므로 웹을 선택한다.

![GA5](/images/Jekyll4/GA5.PNG)

블로그 주소를 입력하고, 이름을 정한다. 필요한 옵션도 선택하고 스트림을 만든다.

![GA6](/images/Jekyll4/GA6.PNG)

측정 ID가 나오고 이걸 이용해서 구글 애널리틱스를 사용할 수 있다. 하지만 앞에서 말했듯이 현재 사용 중인 Jekyll은 지원하지 않는 것 같다. 아이디를 적어도 연결이 되지 않는 문제가 있다.

![GA7](/images/Jekyll4/GA7.PNG)

창 왼쪽에 있는 설정을 들어가면 다음과 같이 창이 바뀐다. 보면 UA로 시작하는 속성이 있는데 이게 구버전인 유니버설 애널리틱스다. 해당 아이디를 사용하면 기록이 추적이 된다.

![GA8](/images/Jekyll4/GA8.PNG)

재킬 파일이 있는 곳에 가서 _config.yml에 들어간다. 보통 구글 애널리틱스와 연동할 수 있는 옵션이 미리 되어있다.

사용 중인 minimal-mistakes 테마에서는 다음과 같이 되어있다. provider에 "google-universal"을 적어주고 추적 아이디에 아까 웹에서 확인한 아이디를 넣는다.

![GA9](/images/Jekyll4/GA9.PNG)

만약 옵션이 없다면 다음과 같이 includes에 새로 파일을 만든다.

![GA10](/images/Jekyll4/GA10.PNG)

아래 코드를 복사해서 'UA-~~~~'를 자신의 추적 ID로 바꾼다. minimal-mistakes는 anonymizeIp를 설정하는 별도 코드가 있는데 계속 문제를 일으켜서 그 부분은 삭제했다.

minimal-mistakes는 설정한 애널리틱스를 사용할 수 있도록 별도의 html 파일을 제공한다. 굳이 필요한 파일은 아니다.

```html
<script>
  window.ga=function(){ga.q.push(arguments)};ga.q=[];ga.l=+new Date;
  ga('create','UA-~~~~','auto');
  ga('set', 'anonymizeIp');
  ga('send','pageview')
</script>
<script src="https://www.google-analytics.com/analytics.js" async></script>
```

![GA11](/images/Jekyll4/GA11.PNG)

설정한 html을 블로그 내에 추적하고자 하는 모든 곳에 코드를 넣어야 한다. 보통 _includes에 있는 head.html을 이용하면 된다. 사용 중인 테마는 사용자가 필요할 경우 별도로 사용할 수 있는 head.html에 있다. 거기에 다음과 같이 작성해서 넣어준다.

별도로 그런 게 없다면 이미 있는 head.html이나 default.html등 블로그 내에 공통으로 존재하는 html에 넣으면 된다.

만약 아까 만든 애널리틱스 추적 코드가 있는 html 파일의 이름이 google_analytics.html이라면

다음 예시의 analytics.html을 google_analytics.html로 바꾸면 된다.

![GA12](/images/Jekyll4/GA12.PNG)

블로그에 접속하고 애널리틱스에 기록이 나오는지 확인한다. 다음과 같이 현재 활성 사용자가 나온다면 연결이 된 것이다.

![GA13](/images/Jekyll4/GA13.PNG)

새로 나온 GA로 설계한다면 다음과 같이 하면 된다. 아까 웹 스트림을 등록했을 때 태글 구성할 수 있는 페이지가 있었다. 거기서 사이트 태그를 복사한다. 메인 화면에서 왼쪽 하단에 있는 관리로 들어가면 관리자 설정이 뜬다. 여기서 속성- > 데이터 스트림에 들어가면 기존에 만든 설정을 볼 수 있다.

![GA15](/images/Jekyll4/GA15.PNG)

설명에 나온 대로 모든 웹페이지의 \의 첫 번째 항목으로 넣으면 된다. 아까 했듯이 \_config.yml에 설정할 수 있는 조건이 있으면 사용한다. 없으면 _includes에 있는 head.html이나 default.html 혹은 footer.html과 같이 모든 페이지에 사용되는 곳에다가 붙여넣기 한다.

![GA16](/images/Jekyll4/GA16.PNG)

여기서는 analytucs-providers 폴더에 custom.html 파일을 만들어서 코드를 넣었다. 그리고 이것을 head.html에 삽입되는 head 폴더 내에 있는 custom.html에 include 했다.

애널리스틱의 실시간 페이지에 접속해서 인식되는지 확인한다.

***

## __네이버 웹마스터__

네이버에 로그인하고 웹마스터 사이트에 들어간다. 들어가면 오른쪽에 웹마스터 도구를 선택한다.

![NWM1](/images/Jekyll4/NWM1.PNG)

사이트 주소를 입력해서 등록한다.

![NWM2](/images/Jekyll4/NWM2.PNG)

사이트 소유확인을 해야 한다. html 파일을 다운로드 받아서 재킬 테마가 있는 폴더에 넣는다. 그리고 소유확인 버튼을 누른다.

![NWM3](/images/Jekyll4/NWM3.PNG)

사이트 등록이 완료됐다면 이렇게 등록된 사이트가 목록에 있다. 들어간다.

![NWM4](/images/Jekyll4/NWM4.PNG)

왼쪽 메뉴에서 요청->사이트맵에 들어간다.

![NWM5](/images/Jekyll4/NWM5.PNG)

만들어놓은 사이트맵을 제출한다.

![NWM6](/images/Jekyll4/NWM6.PNG)

RSS를 제출하고자 한다면 요청->RSS에 들어가서 feed.xml을 제출한다. 네이버가 사용하는 RSS는 Jekyll 플러그인으로 생성하는 것과는 다르므로 따로 만들어야 한다. 이전 포스트에서 해당 내용을 설명했다.

![NWM6](/images/Jekyll4/NWM7.PNG)

***

## __네이버 애널리틱스__

네이버 애널리틱스에 접속하고 바로 시작하기를 누른다.

![NA1](/images/Jekyll4/NA1.PNG)

사이트를 새로 등록해야 하므로 사이트 등록 버튼을 누른다.

![NA3](/images/Jekyll4/NA3.PNG)

설정할 사이트 이름을 적고 사이트 주소를 입력한다. 그리고 등록한다.

![NA4](/images/Jekyll4/NA4.PNG)

해당 html 내용을 복사한다.

![NA5](/images/Jekyll4/NA5.PNG)

_includes에 있는 default.html이나 head.html, footer.html 중 한 곳에 붙여넣는다. 블로그 페이지에 공통으로 들어가는 것이면 된다.

![NA6](/images/Jekyll4/NA6.PNG)

블로그에 접속하고 애널리틱스에서 실시간 분석에 들어가서 접속이 감지되는지 확인한다. 잘 된다면 연결이 된 것이다.

![NA7](/images/Jekyll4/NA7.PNG)
