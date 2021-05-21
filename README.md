# https://imjhua.github.io

- https://mmistakes.github.io/minimal-mistakes/
- https://github.com/mmistakes/minimal-mistakes
- https://unsplash.com/t/nature

## 환경구성

```sh
$ curl -L https://get.rvm.io | bash -s stable --ruby # rvm 설치
$ source ~/.bash_profile # 설치 경로 적용
$ rvm -v  # rvm 설치 확인
$ rvm list
$ rvm use <version> # ruby-2.6.0
$ rvm install <version> # ruby 특정 버전 설치
$ ruby -v # ruby 버전 확인

$ gem install jekyll bundler # jekyll과 ruby 의존성 선언 및 의존성 분리 도구인 bundler 설치
$ bundle clean --force
$ bundle
$ jekyll serve
```

## navigation.yrm

- GNB 메뉴 정의
- Sidebar 메뉴 정의

```
# local links
local:
  - title: "Resume"
    url: /resume/

# sidebar links
resume:
  - title: 목록
    children:
      - title: "메인"
        url: /resume/main/
      - title: "학력"
        url: /resume/학력/
```

## config.yml

- collection 디렉토리와 permalink 정의 (_로 시작하는 dir)
- 추가로 collection 으로 정의되는 파일들의 상세 레이아웃을 포함한 설정 기본값 정의 (대상은 _로 시작하는 dir)
- collection 의 index 페이지는 _page에서 레이아웃을 정의한다.

```
# Collections
collections:
  resume:
    output: true
    permalink: /:collection/:path/
```

### Layout

- 콜렉션: main(+archive), collection(+wide), categories ..
- 페이지: single, wide ..


```
---
title: "Resume"
permalink: /resume/
layout: main
collection: resume
---
```

### Markdown file

```
---
title: "Layout: Post with Table of Contents"
header:
  overlay_image: assets/images/sky.jpg
categories:
  - Layout
gallery:
  - url: /assets/sky.jpg
    image_path: assets/images/sky.jpg
    alt: "placeholder image 1"
---

{% include gallery %}

- [Twitter Cards](https://dev.twitter.com/cards/overview)
```

#### header

```
header:
  image: assets/images/sky.jpg # 배경
  overlay_image: /assets/images/unsplash-image-1.jpg # 상단 영역만
  overlay_color: "#333"
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)" # 캡션(이미지 정보)
```
#### categories
```
categories:
  - Layout
  - Uncategorized
```
#### tags
```
tags:
  - edge case
  - image
  - layout
```

#### toc

```
toc: true
toc_sticky: true
toc_label: "Unique Title"
toc_icon: "heart"
```

