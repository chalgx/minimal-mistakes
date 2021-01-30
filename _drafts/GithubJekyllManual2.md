---
title: Jekyll을 이용해서 깃허브로 블로그 만들기_2.robots.txt, sitemap, rss 생성 및 설정
date: 2021-01-29
categories: [Manual]
tags: [manual, github, blog, jekyll]
pin: true
math: false
toc: true
toc_sticky: true
---

![Test](/images/TestImage.png)

## __1.robots.txt 생성 및 설정__

robots.txt는 크롤러에게 웹페이지에서 가지는 접근권한에 대해 알려준다. 즉 크롤러가 웹페이지의 데이터를 가져가도 되는지를 알려주는 것이다.

sitemap.xml의 위치를 등록해서 크롤링하는데 도움을 줄 수 있다.

이미 파일이 있다면 이 과정을 굳이 할 필요가 없다.

1. Github Jekyll 블로그의 가장 상위 디렉토리인 루트에 robots.txt를 생성한다.

2. 자신이 원하는 대로 디자인 한다. 예시는 다음과 같다.

```
User-agent: *

Allow: /

Sitemap: https://chalgx.github.io/sitemap.xml
```

모든 크롤러에게 모든 접속을 허용한다는 내용이다. 아마 대부분은 이런식으로 하면 문제가 없을 것이다.

특정 크롤러를 차단하거나 디렉토리를 검색되지 않게 하려면 다음을 참고해서 작성하면된다.

<https://ko.wikipedia.org/wiki/%EB%A1%9C%EB%B4%87_%EB%B0%B0%EC%A0%9C_%ED%91%9C%EC%A4%80>

3. 원격 저장소에 업데이트 한다.

```
git add robots.txt
git commit -m "add robots.txt"
git push origin master
```

***

## __2.sitemap.xml(사이트맵) 생성__

사이트맵은 웹크롤러에게 해당 웹페이지의 접근가능한 페이지를 알려준다. 이를 통해서 검색엔진에 등록이 되는데 도움이 된다.

방법은 크게 두 가지가 있다. 플러그인을 만드는 방법과 수동으로 직접 작성하는 방법이다. 여기서는 플러그인을 활용하는 방법만 소개한다.

이미 파일이 있다면 이 과정을 굳이 할 필요가 없다.

1._config.yml에 아래 내용을 추가한다. minimal-mistakes 테마는 이미 되어 있다.

```
plugins :
   - jekyll-sitemap
```

2. 원격 저장소에 업데이트 한다.

```
git add _config.yml
git commit -m "add plugins jekyll sitemap"
git push origin master
```

***

## __3.rss.xml 생성__

RSS Feed는

이미 파일이 있다면 이 과정을 굳이 할 필요가 없다.

https://jekyllcodex.org/without-plugin/rss-feed/