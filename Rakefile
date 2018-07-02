namespace :greeting do
desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

desc 'outputs hola to the terminal'
  task :hola do
    puts "hola de Rake!"
  end
end

namespace :db do
#  desc 'run before the migrate task'
  task :environment do
    require_relative './config/enviornment'
  end
  desc 'migrate changes to your database'
  task :migrate => :environment do
    Student.create_table
  end
end
