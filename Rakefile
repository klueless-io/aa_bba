# frozen_string_literal: true

require 'bundler/gem_tasks'
require 'rspec/core/rake_task'

RSpec::Core::RakeTask.new(:spec)

require 'rake/extensiontask'

task build: :compile

Rake::ExtensionTask.new('aa_bba') do |ext|
  ext.lib_dir = 'lib/aa_bba'
end

task default: %i[clobber compile spec]
