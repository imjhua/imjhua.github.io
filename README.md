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
$ rvm use <version>
$ rvm install <version> # ruby 특정 버전 설치
$ ruby -v # ruby 버전 확인

$ gem install jekyll bundler # jekyll과 ruby 의존성 선언 및 의존성 분리 도구인 bundler 설치
$ bundle clean --force
$ bundle
$ jekyll serve
```

## test page

### config.yml

- /docs/test

```
# Collections
collections:
  docs:
    output: true
    permalink: /:collection/:path/
  portfolio:
    output: true
    permalink: /:collection/:path/
```

## layout

### ex

```
title: "Layout: Post with Table of Contents"
header:
  overlay_image: assets/images/sky.jpg
categories:
  - Layout
gallery:
  - url: /assets/sky.jpg
    image_path: assets/images/sky.jpg
    alt: "placeholder image 1"
  - url: /assets/sky.jpg
    image_path: assets/images/sky.jpg
    alt: "placeholder image 2"
  - url: /assets/sky.jpg
    image_path: assets/images/sky.jpg
    alt: "placeholder image 3"
```

### header

```
header:
  image: assets/images/sky.jpg # 배경
  overlay_image: /assets/images/unsplash-image-1.jpg # 상단 영역만
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)" # 캡션(이미지 정보)
```

### toc

```
toc: true
toc_sticky: true
toc_label: "Unique Title"
toc_icon: "heart"
```
