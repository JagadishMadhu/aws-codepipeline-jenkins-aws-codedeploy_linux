#!/usr/bin/env ruby

require 'rake/testtask'
require 'rubygems'
require 'rake'

task default: :compile

task :compile do
  puts "JagadishM: compiled ....."
end

task :clean do
  FileUtils.rm_r(Dir.glob("./*.html"), force: true)
end

task :test do 
  Rake::TestTask.new do |t|
    t.test_files = FileList['test/jenkins_sample_test.rb']
  end
end
