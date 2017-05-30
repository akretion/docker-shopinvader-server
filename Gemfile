source 'https://rubygems.org'

# Use https for github source
git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
  "https://github.com/#{repo_name}.git"
end

# Bundle edge Rails instead: gem 'rails', github: 'rails/rails'
gem 'rails', '4.2.8'
# Use SCSS for stylesheets
gem 'sass-rails', '~> 5.0'
# Use Uglifier as compressor for JavaScript assets
gem 'uglifier', '>= 1.3.0'
# Use CoffeeScript for .coffee assets and views
gem 'coffee-rails', '~> 4.1.0'
# See https://github.com/rails/execjs#readme for more supported runtimes
# gem 'therubyracer', platforms: :ruby

# Use jquery as the JavaScript library
gem 'jquery-rails'
# Turbolinks makes following links in your web application faster. Read more: https://github.com/rails/turbolinks
gem 'turbolinks'
# Build JSON APIs with ease. Read more: https://github.com/rails/jbuilder
gem 'jbuilder', '~> 2.0'
# bundle exec rake doc:rails generates the API under doc/api.
gem 'sdoc', '~> 0.4.0', group: :doc

# Use ActiveModel has_secure_password
# gem 'bcrypt', '~> 3.1.7'

# Use Unicorn as the app server
# gem 'unicorn'
# Use Puma as the app server
gem 'puma'

# Use Capistrano for deployment
# gem 'capistrano-rails', group: :development

# Shopinvader / Locomotive gems
gem 'custom_fields', github: 'locomotivecms/custom_fields', ref: '36b79ea91b896abdc5c863f898b16dd1e9ae9756'
gem 'locomotivecms_steam', github: 'locomotivecms/steam', ref: '0b2fab03029872cf3b4f73336ae8fc2d241e06af', require: false
gem 'locomotivecms', github: 'locomotivecms/engine', ref: '71f0b0c5c42b6d35751e81ca9d66ac1317b115e4'
gem 'shop_invader', github: 'akretion/shopinvader', ref: 'bce7865fff3e8d6abd670e4215889969da89f466', branch: 'add-erp-proxy'


group :development, :test do
  # Call 'byebug' anywhere in the code to stop execution and get a debugger console
  gem 'byebug'
end

group :development do
  # Access an IRB console on exception pages or by using <%= console %> in views
  gem 'web-console', '~> 2.0'

  # Spring speeds up development by keeping your application running in the background. Read more: https://github.com/rails/spring
  gem 'spring'
end

group :production do
  gem 'carrierwave-aws'
  gem 'rails_12factor'
end