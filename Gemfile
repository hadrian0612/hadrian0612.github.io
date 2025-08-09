# frozen_string_literal: true

source "https://rubygems.org"

gemspec

gem "html-proofer", "~> 5.0", group: :test

platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

gem "wdm", "~> 0.2.0", :platforms => [:mingw, :x64_mingw, :mswin]

gem "jekyll", "~> 4.4.1"
gem "jekyll-feed"
gem "jekyll-seo-tag"
gem "jekyll-include-cache"
gem "jekyll-archives"       # 如果使用分类/标签
gem "webrick"              # Ruby 3.0+ 必需
gem "logger"               # 消除 Ruby 3.4 警告
# gem 'bootstrap', '~> 5.3.2'
# ------- mark -------
