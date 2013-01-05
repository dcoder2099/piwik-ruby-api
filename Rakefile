require 'rubygems'
require 'rake'

begin
  require 'jeweler'
  Jeweler::Tasks.new do |gem|
    gem.name        = "autometal-piwik"
    gem.summary     = %Q{A ruby client for the Piwik API.}
    gem.description = %Q{Provides simple access to the Piwik API.}
    gem.email       = "ac@humbuckercode.co.uk"
    gem.homepage    = "https://github.com/Achillefs/autometal-piwik"
    gem.authors     = ['Achillefs Charmpilas', 'mihael']
    gem.add_dependency "activesupport", ">= 3.0.9"
    gem.add_dependency "rest-client",   ">= 1.6.1"
    gem.add_dependency "json",          ">= 1.4.6"
    # gem is a Gem::Specification... see http://www.rubygems.org/read/chapter/20 for additional settings
  end
rescue LoadError
  puts "Jeweler (or a dependency) not available. Install it with: sudo gem install jeweler"
end

require 'rake/testtask'
Rake::TestTask.new(:test) do |test|
  test.libs << 'lib' << 'test'
  test.pattern = 'test/**/*_test.rb'
  test.verbose = true
end

task :test => :check_dependencies

task :default => :test


