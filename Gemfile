source "https://rubygems.org"

# GitHub Pages 프로덕션 환경과 동일한 Jekyll 및 플러그인 버전을 고정합니다.
# (jekyll 3.10.0, jekyll-paginate, jekyll-gist, jemoji, kramdown, rouge 등
#  _config.yml에서 사용하는 모든 의존성은 github-pages gem에 포함되어 있습니다.)
# 참고: https://pages.github.com/versions/
gem "github-pages", "~> 232", group: :jekyll_plugins

# Ruby 3.0+ 에서 webrick이 기본 gem에서 제외되어,
# `jekyll serve` 로컬 서버 구동을 위해 명시적으로 추가합니다.
gem "webrick", "~> 1.8"

# Windows / JRuby 환경 호환용 (macOS/Linux devcontainer에서는 설치되지 않음)
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end
gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]
