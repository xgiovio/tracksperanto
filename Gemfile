# -*- ruby -*-
source 'http://rubygems.org'

gem "bundler"

gem "obuf", "~> 1.1"
gem "tickly", "~> 2.1.6"
gem "bychar", "~> 3"
gem "progressive_io", "~> 1.0"
gem "flame_channel_parser", "~> 4.0"
gem 'term-ansicolor', '<= 1.2.0' # Locked because newer versions require tins that do not work on 1.9.3 and less
gem 'tins', '< 0.9.0' # flame_channel_parser wants it via framecurve, but for Ruby 1.8.7 we have to ask for an older version
gem "progressbar", "0.10.0"
gem "update_hints", "~> 1.0"

group :development do
  gem "test-unit", '3.1.5'
  gem "approximately"
  
  gem "rake", '10.5.0'
  gem "linebyline"
  
  gem 'git', '< 1.3.0' # Later ones require 1.9 via nokogiri
  gem "jeweler", '1.8.4' # Last one without the stupid nokogiri dependency
  
  if RUBY_VERSION < "1.9"
    gem "flexmock", "~> 0.8", :require => %w( flexmock flexmock/test_unit ) # Max. supported on 1.8
  else
    gem "flexmock", "~> 1.3.2", :require => %w( flexmock flexmock/test_unit )
  end
  
  gem "cli_test", "~>1.0"
  gem "rake-hooks", '~> 1.2.3'
end