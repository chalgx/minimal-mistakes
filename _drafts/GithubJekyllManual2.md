---
title: Jekyll을 이용해서 깃허브로 블로그 만들기_2.robots.txt, sitemap, feed 생성 및 설정
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

   ```txt
   User-agent: *

   Allow: /

   Sitemap: https://chalgx.github.io/sitemap.xml
   ```

   모든 크롤러에게 모든 접속을 허용한다는 내용이다. 아마 대부분은 이런식으로 하면 문제가 없을 것이다.

   특정 크롤러를 차단하거나 디렉토리를 검색되지 않게 하려면 다음을 참고해서 작성하면된다.

   <https://ko.wikipedia.org/wiki/%EB%A1%9C%EB%B4%87_%EB%B0%B0%EC%A0%9C_%ED%91%9C%EC%A4%80>

3. 원격 저장소에 업데이트 한다.

   ```bash
   git add robots.txt
   git commit -m "add robots.txt"
   git push origin master
   ```

***

## __2.sitemap.xml(사이트맵) 생성__

사이트맵은 웹크롤러에게 해당 웹페이지의 접근가능한 페이지를 알려준다. 이를 통해서 검색엔진에 등록이 되는데 도움이 된다.

방법은 크게 두 가지가 있다. 플러그인을 만드는 방법과 수동으로 직접 작성하는 방법이다. 여기서는 플러그인을 활용하는 방법만 소개한다.

이미 파일이 있다면 이 과정을 굳이 할 필요가 없다.

1. _config.yml에 아래 내용을 추가한다. minimal-mistakes 테마는 이미 되어 있다.

   ```yml
   plugins :
      - jekyll-sitemap

   whitelist:
      - jekyll-sitemap
   ```

   _config.yml 내부에서 plugins, whitelist 항목이 있으면 그 부분에 - jekyll-sitemap만 추가해준다.

2. 원격 저장소에 업데이트 한다.

   ```bash
   git add _config.yml
   git commit -m "add plugins jekyll sitemap"
   git push origin master
   ```

***

## __3.feed 생성__

Feed는 업데이트되는 정보를 자동으로 xml 형식으로 만들어준다. 이걸 이용해서 구독과 같이 바뀌는 정보를 받아서 볼 수 있다.

이미 파일이 있다면 이 과정을 굳이 할 필요가 없다.

Jekyll-feed 플러그인으로 자동으로 생성해줄 수 있는데 이때는 atom feed가 생성된다.

네이버 웹마스터에 등록하는 RSS feed는 따로 만들어야 한다.

### __3.1 Atom feed 생성__

1. _config.yml 안에 plugins와 whitelist에 다음과 같이 추가한다.

   ```yml
   plugins :
      - jekyll-feed

   whitelist:
      - jekyll-feed
   ```

2. 수정 내용을 원격 저장소에 업로드 한다.

   ```bash
   git add _config.yml
   git commit -m "add plugins jekyll feed"
   git push origin master
   ```

### __3.2 RSS feed 생성__

네이버 웹마스터에 등록하기 위해 필요한 RSS Feed는 직접 만들어도 되지만, Jekyll에서 제공하는 예시가 있다. 다음 사이트에 들어가면 확인할 수 있다.

<https://jekyllcodex.org/without-plugin/rss-feed/>

1. 기존에 feed 파일이 있다면 제거한다. _config.yml에 가서 plugins에 있는 것도 삭제하거나 주석 처리를 한다.

   ![RssFeed1](/images/GithubJekyll2/RssFeed1.PNG)

2. 새로 feed.xml을 생성하고 다음 내용을 넣는다. 혹은 위의 사이트에서 다운받아서 Jekyll 폴더가 있는 곳에 넣는다. 같은 것이다.

   ```xml
   <?xml version="1.0" encoding="UTF-8"?>
   <rss version="2.0" xmlns:atom="http://www.w3.org/2005/Atom">
   <channel>
      <title>{% raw %} {{ site.title | xml_escape }} {% endraw %} </title>
      <description>{% raw %}{{ site.description | xml_escape }}{% endraw %}</description>
      <link>{% raw %}{{ site.url }}{{ site.baseurl }}{% endraw %}/</link>
      <atom:link href="{% raw %}{{ "/feed.xml" | prepend: site.baseurl | prepend: site.url }}{% endraw %}" rel="self" type="application/rss+xml"/>
      <pubDate>{% raw %}{{ site.time | date_to_rfc822 }}{% endraw %}</pubDate>
      <lastBuildDate>{% raw %}{{ site.time | date_to_rfc822 }}{% endraw %}</lastBuildDate>
      <generator>Jekyll v{% raw %}{{ jekyll.version }}{% endraw %}</generator>
      {% raw %}{% for post in site.posts limit:10 %}{% endraw %}
         <item>
         <title>{% raw %}{{ post.title | xml_escape }}{% endraw %}</title>
         <description>{% raw %}{{ post.content | xml_escape }}{% endraw %}</description>
         <pubDate>{% raw %}{{ post.date | date_to_rfc822 }}{% endraw %}</pubDate>
         <link>{% raw %}{{ post.url | prepend: site.baseurl | prepend: site.url }}{% endraw %}</link>
         <guid isPermaLink="true">{% raw %}{{ post.url | prepend: site.baseurl | prepend: site.url }}{% endraw %}</guid>
         {% raw %}{% for tag in post.tags %}{% endraw %}
         <category>{% raw %}{{ tag | xml_escape }}{% endraw %}</category>
         {% raw %}{% endfor %}{% endraw %}
         {% raw %}{% for cat in post.categories %}{% endraw %}
         <category>{% raw %}{{ cat | xml_escape }}{% endraw %}</category>
         {% raw %}{% endfor %}{% endraw %}
         </item>
      {% raw %}{% endfor %}{% endraw %}
   </channel>
   </rss>
   ```

3. head.html에 다음 내용을 넣는다. 보통 _includes 폴더 안에 있다.

   ```html
   <link> {% raw %}rel="alternate" type="application/rss+xml" href="{{ site.url }}/feed.xml"{% endraw %}<\link>
   ```

4. 원격 저장소에 바꾼 내용을 업로드한다.

   ```bash
   git rm feed.xml
   git add feed.xml
   git add _config.yml
   git commit -m "add RSS feed"
   git push origin master
   ```

여기까지 했으면 생성이 완료된 것이다.

네이버 웹마스터에서 RSS를 제출하는 건 필수가 아니다. 번거롭다면 생략해도 된다.
