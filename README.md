# https://imjhua.github.io

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
