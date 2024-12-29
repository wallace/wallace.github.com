# frozen_string_literal: true

source 'https://rubygems.org'

# Use a newer version of github-pages
gem 'github-pages', '~> 228', group: :jekyll_plugins

# Add csv gem to fix Ruby 3.4.0 compatibility
gem 'csv'

# If you have any plugins, put them here!
group :jekyll_plugins do
  gem 'jekyll-feed'
  gem 'jekyll-github-metadata'
  gem 'jekyll-paginate'
  gem 'jekyll-sitemap'
end

# Windows and JRuby does not include zoneinfo files
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem 'tzinfo', '>= 1', '< 3'
  gem 'tzinfo-data'
end

# Performance-booster for watching directories on Windows
gem 'wdm', '~> 0.1', platforms: %i[mingw x64_mingw mswin]

# Lock webrick to ensure compatibility
gem 'webrick', '~> 1.7'

# Add faraday-retry gem
gem 'faraday-retry'
