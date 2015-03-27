#!/usr/bin/env rake
require "bundler/gem_tasks"

module Bundler
  class GemHelper
    GEM_HOST = "http://prod-rubygems1-ep.tops.gdi"

    protected
    def rubygem_push(path)
      sh("gem push '#{path}' --host #{GEM_HOST}")
      Bundler.ui.confirm "Pushed #{name} #{version} to #{GEM_HOST}."
    end
  end
end
