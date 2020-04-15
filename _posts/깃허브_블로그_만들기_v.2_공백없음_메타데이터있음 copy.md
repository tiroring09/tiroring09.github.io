---
layout: post
title:  "test post including metadata format!"
date:   2000-04-15 17:45:00 +0900
categories: jekyll update
---
깃허브 블로그 만들기 v.2

# 깃허브 블로그 만들기 v.2

[TOC]

## 실행환경
- 윈도우환경
- 깃 & 깃허브
- Jekyll

## 설치
### 1. 깃허브 레포 생성
### 2. 로컬에 지킬설치
[깃허브 공식문서: Creating a GitHub Pages site with Jekyll](https://help.github.com/en/github/working-with-github-pages/creating-a-github-pages-site-with-jekyll)
[지킬 윈도우 설치 공식문서](https://jekyllrb.com/docs/installation/windows/)
지킬을 사용하려면 아래 3가지가 필요하다.

1) Ruby
파이썬과 같은 프로그래밍 언어이다. 이것은 각 운영체제별로 설치절차가 살짝 다른데, 리눅스에서는 자체 패키지 관리 시스템(apt 등) 또는 서드파티 도구(rbenv & RVM)를 통해 설치가능하고, 맥에서는 서드파티 도구(rbenv & RVM)를 통해 설치가능하고, 윈도우에서는 RubyInstaller를 통해 설치할 수 있다.
[루비 공식 설치 안내 페이지](https://www.ruby-lang.org/ko/downloads/)에 다 나와있는 내용이니 이쪽 참고해서 본인 환경에 맞는 방법으로 루비를 설치하자.
이번 시도에서는 윈도우 환경에서 실행하므로, [RubyInstaller](https://rubyinstaller.org/downloads/)를 통해 설치하려고 했는데, With Devkit & Without Devkit 중에서 선택해야 했다. 지킬공식문서에서 아래와 같이 안내되어있는걸 보니 왠지 With Devkit으로 설치해야 할 것 같다. 버전은 현 시점에서 권장하는 `Ruby+Devkit 2.6.X (x64)`으로 설치.[^주석1]
	> Ruby version 2.5.0 or above, **including all development headers** (ruby version can be checked by running ruby -v)
	
	```
	$ ruby -v
	ruby 2.6.6p146 (2020-03-31 revision 67876) [x64-mingw32]
	```

[^주석1]: 왠지는 모르겠지만 `MSYS2 toolchain`까지 합하여 용량이 약 1GB에 육박하더라...왤까?!

2) RubyGems
RubyGems는 루비에서 동작하는 패키지 매니저이다. 파이썬의 pip와 대응하고, 음 리눅스에 비유한다면 apt와 비슷한 것 같다. 1)에서 진행한 방법으로 설치하니까 gem도 설치된 것을 아래와 같이 확인 하였다.
	```
	$ gem -v
	3.0.3
	```

3) Install Jekyll
gem이 설치된 것을 확인했으면, gem을 통해서 Jekyll을 설치하면 된다. [지킬 윈도우 설치 공식문서](https://jekyllrb.com/docs/installation/windows/)에서 안내가 좀 그지같이 되어있어서 햇갈렸는데, 그냥 `gem install jekyll bundler`명령어로 설치한 후, `jekyll -v`명령어를 통해서 설치를 확인하면 된다.
	```
	$ gem install jekyll bundler
	(중략)
	27 gems installed
	```
	```
	$ jekyll -v
	jekyll 4.0.0
	```











