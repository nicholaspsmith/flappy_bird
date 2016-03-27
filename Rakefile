# -*- coding: utf-8 -*-
$:.unshift("/Library/RubyMotion/lib")
require 'motion/project/template/ios'

begin
  require 'bundler'
  Bundler.require
rescue LoadError
end

Motion::Project::App.setup do |app|
  app.name = 'flappy'
  app.frameworks += ["SpriteKit"]
  app.interface_orientations = [:portrait]
  
  app.identifier = 'com.nicholaspsmith.flappy'
  app.codesign_certificate = 'iPhone Developer: Nick Smith (NJ3LQM3WW9)'
  app.provisioning_profile = '/Users/nick/Documents/Programming/Xcode/iOS_Team_Provisioning_Profile_.mobileprovision'
end

desc "Run simulator on iPhone"
task :iphone6sp do
    exec 'bundle exec rake device_name="iPhone 6s Plus"'
end

