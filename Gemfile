# encoding: utf-8

source 'https://rubygems.org'

gemspec

gem 'rake', '~> 10.1'
gem 'rspec', '~> 3.3.0'
gem 'yard', '~> 0.8'
gem 'simplecov', '~> 0.10'
gem 'concurrent-ruby'
gem 'concurrent-ruby-edge'

group :development, :test do
  gem 'byebug'
  gem 'pry'
  gem 'pry-byebug'
end

group :test do
  gem 'codeclimate-test-reporter', require: false
  gem 'safe_yaml', require: false
  gem 'webmock', require: false
end

local_gemfile = 'Gemfile.local'

if File.exist?(local_gemfile)
  eval(File.read(local_gemfile)) # rubocop:disable Lint/Eval
end
