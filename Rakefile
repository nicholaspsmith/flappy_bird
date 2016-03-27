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
  app.frameworks += ["SpriteKit", "GameController"]
  app.interface_orientations = [:portrait]
end

desc "Run simulator on iPhone"
task :iphone6sp do
    exec 'bundle exec rake device_name="iPhone 6s Plus"'
end