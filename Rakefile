desc 'outputs hello to the terminal'

namespace :greeting do

	desc 'outputs hello to the terminal'
	task :hello do
  		puts "hello from Rake!"
	end
	desc 'outpust hola to the terminal'
	task :hola do
		puts "hola de Rake!"
	end
end


namespace :db do 

  desc 'migrate changes into your database'
  task :migrate => :environment do 
    Student.create_table
  end
  desc 'ur mom lol'
  task :seed do
  	require_relative './db/seeds.rb'
  end
end

task :environment do
  require_relative './config/environment'
end

task :console => :environment do
	Pry.start
end