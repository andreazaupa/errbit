$:.unshift(File.expand_path('./lib', ENV['rvm_path']))
require 'rvm/capistrano'
load 'deploy/assets'
load 'deploy' if respond_to?(:namespace) # cap2 differentiator
Dir['vendor/plugins/*/recipes/*.rb'].each { |plugin| load(plugin) }

load 'config/deploy' # remove this line to skip loading any of the default tasks