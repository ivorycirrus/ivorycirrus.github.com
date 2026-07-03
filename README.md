# IvoryCirrus'Lab

This is source repository for blog.<br>
Please visit this url. [https://ivorycirrus.github.io/](https://ivorycirrus.github.io/)

## Site Arch.
* Blog engine : [Jekyll](https://jekyllrb.com/)
* Blog theme : [jekyll-theme-EasyBook](https://github.com/laobubu/jekyll-theme-EasyBook)
* Profile management : [Gravatar](https://ko.gravatar.com/)
* Comment service : [Disqus](https://disqus.com/)

## Local Development (Dev Container)

이 저장소는 [Dev Container](https://containers.dev/) 설정을 포함합니다.
GitHub Pages 프로덕션 환경(Ruby 3.3, `github-pages` gem)과 동일한 조건에서
블로그를 빌드하고 미리볼 수 있습니다.

### 1. 컨테이너 열기
* VS Code + [Dev Containers 확장](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)에서
  `Reopen in Container` 실행 (또는 GitHub Codespaces에서 열기)
* 최초 실행 시 `bundle install`이 자동으로 수행됩니다 (`postCreateCommand`).

### 2. 블로그 실행 (미리보기)
컨테이너 셸에서 아래 중 하나를 실행합니다.

```bash
# 헬퍼 스크립트 (외부 접근 허용 + LiveReload)
IP=0.0.0.0 ./serve

# 또는 직접 실행
bundle exec jekyll serve --host 0.0.0.0 --livereload
```

* 브라우저에서 [http://localhost:4000](http://localhost:4000) 접속
* 포트 `4000`(사이트)과 `35729`(LiveReload)는 자동으로 포워딩됩니다.
* 파일을 수정하면 LiveReload로 브라우저가 자동 갱신됩니다.

### 3. 정적 사이트 빌드
```bash
# _site/ 디렉터리에 정적 파일 생성
bundle exec jekyll build
```

## License

[CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)
