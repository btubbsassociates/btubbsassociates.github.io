source "https://rubygems.org"

# Use GitHub Pages gem which includes all compatible versions
gem "github-pages", "~> 231", group: :jekyll_plugins

# Or use standalone Jekyll (comment out github-pages above if using this)
# gem "jekyll", "~> 3.9.5"
# gem "minima", "~> 2.5"

group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
  gem "jekyll-seo-tag", "~> 2.8"
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

# For macOS - webrick is needed for Ruby 3.0+
gem "webrick", "~> 1.8"
