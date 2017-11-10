namespace :greeting do
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

  desc 'outputs hola to the termal'
  task :hola do
    puts "hola de Rake!"
  end
end

namespace :db do
  desc "migrate changes to your database"
  task :migrate => :environment do
    Student.create_table
  end

  desc "require environment"
  task :environment do
    require_relative './config/environment.rb'
  end

  desc "seeds database"
  task :seed do
    require_relative './db/seeds.rb'
  end
end
