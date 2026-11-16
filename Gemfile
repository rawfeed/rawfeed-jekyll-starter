source "https://rubygems.org"

gem "rubyzip", "~> 2.3"

group :jekyll_plugins do
  gem "jekyll-polyglot", "~> 1.14"
end

if ENV["RAWFEED_DEV_PATH"] && File.directory?(ENV["RAWFEED_DEV_PATH"])
  gem "rawfeed", path: ENV["RAWFEED_DEV_PATH"]
else
  gem "rawfeed", "~> 2.0.0"
end

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
platforms :windows, :jruby do
  gem "tzinfo", "~> 1.2"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1.1", :platforms => [:windows]
