source "https://rubygems.org"

# GitHub Pages gem - keeps dependencies in sync with GitHub Pages
gem "github-pages", group: :jekyll_plugins

# If you want to use Jekyll natively without GitHub Pages compatibility
# gem "jekyll", "~> 4.3"

# Jekyll plugins
group :jekyll_plugins do
  gem "jekyll-feed"
  gem "jekyll-seo-tag"
end

# Windows and JRuby does not include zoneinfo files
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1", :platforms => [:mingw, :x64_mingw, :mswin]

# Lock `http_parser.rb` gem to `v0.6.x` on JRuby builds
gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]
