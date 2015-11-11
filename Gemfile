# Gemfile
source "https://rubygems.org"

# Platform helpers
def windows_only(require_as)
  RbConfig::CONFIG['host_os'] =~ /mingw|mswin/i ? require_as : false
end
def linux_only(require_as)
  RbConfig::CONFIG['host_os'] =~ /linux/ ? require_as : false
end
def darwin_only(require_as)
  RbConfig::CONFIG['host_os'] =~ /darwin/ ? require_as : false
end

# GEMS
gem 'awestruct', '0.5.7.RC1'
gem 'slim', '~> 3.0'
gem 'kramdown', '~> 1.0.1'
gem 'asciidoctor', '~> 1.5.0'
gem 'uglifier', '~> 2.0.1'
gem 'htmlcompressor', '~> 0.0.6'
gem 'curb', '~> 0.8.5'
gem 'oauth', '~> 0.3.6'
gem 'git', '~> 1.2.5'
gem 'oily_png', '~> 1.1.1'
gem 'nokogiri', '~> 1.5.10'
gem 'therubyracer', platforms: :ruby, require: linux_only('therubyracer')
gem 'parallel', '~> 1.1'
gem 'mime-types', '2.1'
gem 'google-api-client', '~> 0.8'
gem 'signet', '~> 0.6'
gem 'gpgme', '~> 2.0'
gem 'ruby-duration', '~> 3.1'
gem 'daybreak'
gem 'sass', '~> 3.4', '< 3.4.6'
gem 'activesupport', '> 3.1', '< 4.2.0' # Used in aweplug by ruby-duration
gem 'compass', '~> 1.0'
gem 'rake', '~>10.4'

# To use Aweplug code from a different location:
#
# From a specific GitHub branch. Ommit the 'branch' parameter for 'master'
#    gem 'aweplug', github: '<github_id>/aweplug', :branch => '<branch_name>'
#
# From a location on your disk:
#    gem 'aweplug', path: '<path_to_aweplug_on_your_disk>'
#
gem 'aweplug', github: 'Dantheman720/aweplug', :branch => 'FullDescription'

group :test do
  gem 'climate_control'
  gem 'guard'
  gem 'guard-minitest'
  gem 'launchy', '~>2.4'
  gem 'rubocop', '~> 0.34.2'
  gem 'cucumber', '~>2.0'
  gem 'poltergeist', '~> 1.7.0'
  gem 'minitest-reporters'
  gem 'rspec', '~>3.3'
  gem 'capybara', '~>2.5'
  gem 'selenium-webdriver', '~> 2.48.0'
  gem 'parallel_tests', '~> 1.9.0'
  gem 'cuke_sniffer', '~> 0.0.8'
  gem 'require_all', '~> 1.3.2'
  gem 'chromedriver-helper', '0.0.6'
  gem 'capybara-screenshot', '~> 1.0.11'
  gem 'site_prism', '~> 2.7'
 end

group :development do
  gem 'rb-inotify', require: false
  gem 'rb-fsevent', require: false
  gem 'rb-fchange', require: false
  gem 'pry', require: false
  gem 'pry-byebug', require: false
end

group :vdiff do
  gem 'wraith', '~> 1.3.0'
end

group :health do
  gem 'blinkr', '~> 0.3'
end

