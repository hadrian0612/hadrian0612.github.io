# frozen_string_literal: true

source "https://rubygems.org"

gemspec

gem "html-proofer", "~> 5.0", group: :test

platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

gem "wdm", "~> 0.2.0", :platforms => [:mingw, :x64_mingw, :mswin]

# Jekyll 核心
# gem "jekyll", "~> 4.4.1"  # 版本需与你的本地一致（通过 `jekyll -v` 查看）

# Chirpy 主题依赖
# gem "jekyll-theme-chirpy"  # 如果使用 remote_theme 可删除此行
gem "jekyll-paginate"      # 解决 pagination 警告
gem "webrick"              # Ruby 3.0+ 必需
gem "logger"               # 消除 Ruby 3.4 的警告