source "https://rubygems.org"

branch = ENV.fetch('SOLIDUS_BRANCH', 'v2.8')
gem "solidus", github: "solidusio/solidus", branch: branch

if branch == 'master' || branch >= "v2.0"
  gem "rails-controller-testing", group: :test
else
  gem "rails_test_params_backport"
end

gem 'sqlite3'
gem 'pg', '~> 0.21'

group :development, :test do
  gem 'pry-rails'
end

gemspec
