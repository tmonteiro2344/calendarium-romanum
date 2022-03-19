require 'rspec/core/rake_task'
RSpec::Core::RakeTask.new(:spec)

desc 'Run specs with each fully supported locale'
task :spec_all_locales do
  %w(en la cs fr it pt).each do |locale|
    sh "LOCALE=#{locale} rake spec"
  end
end
