namespace :greeting do

desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end

desc 'outputs hello to the terminal'
task :hola do
  puts "hola de Rake!"
end

end

desc 'opens console'
task :console do
  Pry.start
end


namespace :db do
  desc "you know about that environment"
  task :migrate => :environment do
    Student.create_table
  end

  desc "Seed that DB"
  task :seed do
    require_relative './db/seeds.rb'
  end

  task :environment do
  require_relative './config/environment'
end
end
