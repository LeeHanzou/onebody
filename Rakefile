# Add your own tasks in files placed in lib/tasks ending in .rake,
# for example lib/tasks/capistrano.rake, and they will automatically be available to Rake.

require File.expand_path('../config/application', __FILE__)
require 'rake'
#require 'rake/testtask'
#require 'rake/rdoctask'

require Rails.root.join('lib/rake_abandon')

OneBody::Application.load_tasks

Dir["#{Rails.root}/plugins/*/**/tasks/**/*.rake"].sort.each { |ext| load ext }

