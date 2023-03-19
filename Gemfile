source 'https://rubygems.org'
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

ruby '3.2.1'

gem 'bootsnap', require: false
gem 'pg', '~> 1.1', '>= 1.4.6'
gem 'puma', '~> 6.1', '>= 6.1.1'
gem 'rails', '~> 7.0.4', '>= 7.0.4.3'
gem 'sidekiq', '~> 7.0', '>= 7.0.7'
gem 'tzinfo-data', platforms: %i[ mingw mswin x64_mingw jruby ]



group :development, :test do
  # See https://guides.rubyonrails.org/debugging_rails_applications.html#debugging-with-the-debug-gem
  gem 'debug', platforms: %i[ mri mingw x64_mingw ]
end

group :development do
  # Speed up commands on slow machines / big apps [https://github.com/rails/spring]
  # gem 'spring'
end

