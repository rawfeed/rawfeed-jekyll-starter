# frozen_string_literal: true

require "rawfeed"

namespace :create do
  desc "Create a post draft"
  task :draft do
    Rawfeed::CLI.run(["create:draft"])
  end

  desc "Create a page"
  task :page do
    Rawfeed::CLI.run(["create:page"])
  end

  desc "Create a pixel post"
  task :pixel do
    Rawfeed::CLI.run(["create:pixel"])
  end

  desc "Restore the resume page"
  task :resume do
    Rawfeed::CLI.run(["restore:resume"])
  end
end

namespace :restore do
  desc "Restore the resume page"
  task :resume do
    Rawfeed::CLI.run(["restore:resume"])
  end
end

namespace :post do
  desc "Publish a selected draft"
  task :draft do
    Rawfeed::CLI.run(["post:draft"])
  end
end

namespace :move do
  desc "Compatibility alias for publishing a selected draft"
  task :posts do
    Rawfeed::CLI.run(["post:draft"])
  end
end

namespace :home do
  desc "Set the home page to the profile"
  task :about do
    Rawfeed::CLI.run(["home:about"])
  end

  desc "Set the home page to the weblog"
  task :blog do
    Rawfeed::CLI.run(["home:blog"])
  end
end

namespace :blog do
  desc "Enable the weblog"
  task :enable do
    Rawfeed::CLI.run(["blog:enable"])
  end

  desc "Disable the weblog"
  task :disable do
    Rawfeed::CLI.run(["blog:disable"])
  end
end

namespace :pixels do
  desc "Enable the pixel gallery"
  task :enable do
    Rawfeed::CLI.run(["pixels:enable"])
  end

  desc "Disable the pixel gallery"
  task :disable do
    Rawfeed::CLI.run(["pixels:disable"])
  end
end
