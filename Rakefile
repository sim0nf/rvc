require 'rake/testtask'

begin
  require 'jeweler'
  Jeweler::Tasks.new do |gem|
    gem.name = "rvc"
    gem.summary = "vSphere console UI"
    #gem.description = ""
    gem.email = "rlane@vmware.com"
    #gem.homepage = ""
    gem.authors = ["Rich Lane"]
    gem.add_dependency 'rbvmomi', '>= 1.1.5'
    gem.add_dependency 'trollop', '>= 1.16.2'
    gem.add_dependency 'backports', '>= 1.18.2'
  end
rescue LoadError
  puts "Jeweler not available. Install it with: gem install jeweler"
end

Rake::TestTask.new do |t|
  t.libs << "test"
  t.test_files = FileList['test/test_*.rb']
  t.verbose = true
end
