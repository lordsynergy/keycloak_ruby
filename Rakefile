# frozen_string_literal: true

require "bundler/gem_tasks"
require "rspec/core/rake_task"

RSpec::Core::RakeTask.new(:spec) do |task|
  task.verbose = false
end

require "rubocop/rake_task"
RuboCop::RakeTask.new

require "reek/rake/task"
Reek::Rake::Task.new

task default: %i[spec rubocop reek]
