desc 'Generate Guides'
task 'docs' do
  system 'rm -rf neo4j'
  ruby 'neo4j_guides.rb'
end

desc 'Upload documentation to RubyForge.'
task 'upload' do
  sh "scp -r neo4j/* " +
    "ronge@rubyforge.org:/var/www/gforge-projects/neo4j"
end
