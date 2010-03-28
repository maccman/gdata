# Copyright (C) 2008 Google Inc.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

require 'rubygems'
require 'rake/rdoctask'
require 'rake/testtask'

task :default => [:test]

task :test do
  ruby "test/ts_gdata.rb"
end

task :doc do
  system "rdoc -U --title 'gdata module documentation' -m README README lib/"
end

begin
  require "jeweler"
  Jeweler::Tasks.new do |gemspec|
    gemspec.name = "gdata"
    gemspec.summary = "Google GData API"
    gemspec.email = "info@eribium.org"
    gemspec.homepage = "http://github.com/maccman/gdata"
    gemspec.authors = ["Alex MacCaw"]
  end
rescue LoadError
  puts "Jeweler not available. Install it with: sudo gem install jeweler"
end