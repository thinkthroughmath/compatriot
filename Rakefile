#!/usr/bin/env rake
require "bundler/gem_tasks"
require 'rake/testtask'

desc "Run tests"
task :test do
  test_task = Rake::TestTask.new("tests") do |t|
    t.test_files = Dir.glob(File.join("spec", "**", "*_spec.rb"))
  end
  task("tests").execute
end

desc "Run tests"
task :spec do
  task("test").execute
end
