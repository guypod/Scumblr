source 'https://rubygems.org'

gem 'rails', '5.2.4.2'

gem 'zip'
gem 'lograge'
# Allow using posix-spawn for popen to save memory with multiple threads.
gem 'posix-spawn'

#For Tasks/Search Providers
gem 'google-api-client', '~> 0.8.6'
gem "github_api", require: false
gem 'colorize', require: false
gem 'twitter', '>= 6.0.0'
gem 'market_bot'
gem 'koala'
gem "brakeman", require: false
gem "bundler-audit"
gem 'rest-client'
gem 'chartkick'

gem 'redcarpet'

gem 'addressable'

gem 'jwt', '<= 1.5.2'

# Pretty file sizes
gem 'filesize'

# scott things
gem 'json-schema-generator'
gem 'zeroclipboard-rails', '>= 0.1.1'

gem 'activerecord-session_store', git: 'https://github.com/rails/activerecord-session_store'
#Database gems
gem 'sqlite3'
gem 'pg'

#git functionality
gem 'git'

#Workflow
gem 'workflowable', '>= 1.0.1'

#JIRA Integration
gem 'jiralicious', '>= 0.4.3'

#Authorization
gem 'cancan'

#Searching
gem 'ransack', '>= 1.7.0'

#Image processing/attachments
gem 'paperclip', '>= 4.2.0'
gem 'aws-sdk', '>= 1.52.0', '< 2.0'


# Time period parsing
gem 'chronic'

#Nice select fields
gem "select2-rails"

#Faster json parsing
gem 'oj'

#Bulk edits
gem 'activerecord-import', '>= 0.5.0'

#Used for task queueing
gem 'sidekiq'
gem 'sidekiq-status'

#Pagination
gem 'kaminari', '>= 0.16.1'

#Sidekiq UI
gem 'sinatra', require: false

#Templating language, not sure if used
gem 'slim'

#Performance gem that changes how links are handed
##gem 'turbolinks'
gem 'jquery-turbolinks', '>= 2.0.2'

#Allowing exporting/importing data into database
gem 'yaml_db', '>= 0.7.0'

#Authentication
gem 'devise', '>= 4.4.2'
gem 'responders', '>= 2.4.0'

#Comments
gem 'acts_as_commentable_with_threading', '>= 1.2.0'

#JSON API Calls
gem "active_model_serializers", ">= 0.10.2"

# Cron job generation
gem "whenever", ">= 0.9.2"

# Used for finding changes to serialized attributes
gem "hashdiff"

#gem 'active_scaffold'
gem "therubyracer"
gem "less-rails" , ">= 2.5.0" #Sprockets (what Rails 3.1 uses for its asset pipeline) supports LESS
gem 'simple_form', '>= 4.0.0'

gem 'ip'

gem 'stackprof'

gem 'faraday'
gem 'net-http-persistent'

gem 'minitest'

gem 'minitest-rails', '>= 3.0.0'

group :development, :test, :production do
  gem 'unicorn'
  gem 'unicorn-rails'
end

group :test, :production do
  #this doesn't get along with rack-mini-profiler
  gem 'oj_mimic_json'
end


group :development, :dirtylaundrydev do
  gem 'spring', group: :development
  gem "ruby-prof"
  gem 'meta_request', '>= 0.5.0'
  gem "binding_of_caller"
  gem "bullet", ">= 5.1.0"
  gem 'rack-mini-profiler', require: false
  gem 'flamegraph'
  gem 'rbtrace'
  #gem 'rails-footnotes'
  #gem 'rails-footnotes', github: 'josevalim/rails-footnotes', branch: 'release-4.0'
  gem 'rails-footnotes', '>= 4.0.2', '< 5'
  gem 'railroady'
  gem 'ruby_gntp'
  # gem 'rack-perftools_profiler', :require => 'rack/perftools_profiler'
end

group :development, :dirtylaundrydev, :profile do

  gem 'byebug'
  gem 'quiet_assets'
  gem "better_errors"
  gem 'pry'

end

#Testing
group :development, :test, :dirtylaundrydev do
  gem 'rspec-rails', '>= 3.0.2'
  gem 'factory_girl_rails', '>= 4.4.1'

end

group :test do
  gem 'database_cleaner'
  gem 'shoulda', '>= 3.5.0'
  gem 'activerecord-nulldb-adapter', '>= 0.3.1'
  gem 'minitest-reporters'
  gem 'shoulda-matchers', '~> 2.0'
  gem 'shoulda-callback-matchers', '~> 1.1.1'
  gem 'simplecov', :require => false, :group => :test
end

gem 'foundation-rails', '5.3.3.0'
gem 'sass-rails', '5.0.5'
gem 'sass', '3.2.19'
gem 'coffee-rails', '4.2.2'
gem 'sprockets', '2.11.0'


gem 'uglifier', '>= 2.5.3'

gem 'jquery-rails', '>= 4.0.1'

gem 'rb-readline'


# needed by  sidekiq
gem 'json', '>= 2.3.0'
gem 'ffi'


if File.exists?("custom/Gemfile")
  eval(IO.read("custom/Gemfile"), binding)
end
if File.exists?("../custom/Gemfile")
  eval(IO.read("../custom/Gemfile"), binding)
end
if File.exists?("./Gemfile.append")
  eval(IO.read("./Gemfile.append"), binding)
end
