source "https://rubygems.org"

# GitHub Pages — this gem pins Jekyll and all plugins to the versions
# GitHub Pages runs, so what you see locally matches what GitHub builds.
gem "github-pages", group: :jekyll_plugins

# Plugins used by this site (also declared in _config.yml)
group :jekyll_plugins do
  gem "jekyll-feed"
  gem "jekyll-sitemap"
  gem "jekyll-seo-tag"
end

# Windows / JRuby compatibility shims
gem "tzinfo-data", platforms: [:mingw, :mswin, :x64_mingw, :jruby]
gem "wdm", "~> 0.1.1", platforms: [:mingw, :mswin, :x64_mingw]

# Faster file watching on macOS
gem "webrick"
