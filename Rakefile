namespace :greeting do
desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end

desc 'outputs hola to the terminal'
  task :hola do
    puts "hola de Rake!"
  end

namespace :db do
  task :enviornment do
    require_relative './config/enviornment'
  end
  desc 'migrate changes to your database'
  task :migrate => :environment do
    Student.create_table
  end
end
