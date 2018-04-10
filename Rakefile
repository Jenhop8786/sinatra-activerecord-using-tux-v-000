require_relative './config/environment'
require 'sinatra/activerecord/rake'
require 'my-sinatra-app'

desc "run irb console"
task :console, :environment do |t, args|
ENV["SINATRA_ENV"] = args[:environment] ||= "development"

exec "irb -r/completion -r my-sinatra-app"

# Type `rake -T` on your command line to see the available rake tasks
end