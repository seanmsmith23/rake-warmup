desc "Gives current time"
task :time do
  puts Time.now
end

desc "Gets name and says hi"
task :greet do
  puts "Whats your name?"
  name = STDIN.gets.chomp
  puts "Hello #{name}"
end

desc "Prints out your favorite food"
task :print_favorite_food do
  puts "Your favorite food is #{ENV["FAVORITE_FOOD"]}"
end

namespace :getting_ready do
  desc "wakes up"
  task :wakes_up do
    puts "I'm awake"
  end

  desc "gets dressed"
  task :gets_dressed => :wakes_up do
    puts "Now I'm clothed"
  end
end

task :default => "getting_ready:gets_dressed"