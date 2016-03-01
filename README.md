#Ruby Starter Kit
This is a Ruby app boilerplate with conventional code structure and basic dev env to start some console mode utility app with (Bundler, Guard, ActiveSupport Logger, Rubocop, RSpec, WebMock, Travis, CodeClimate).

[![Travis build status](http://img.shields.io/travis/artemv/ruby-starter-kit.svg?style=flat)](https://travis-ci.org/artemv/ruby-starter-kit)
[![Code Climate](https://codeclimate.com/github/artemv/ruby-starter-kit/badges/gpa.svg)](https://codeclimate.com/github/artemv/ruby-starter-kit)
[![Test Coverage](https://codeclimate.com/github/artemv/ruby-starter-kit/badges/coverage.svg)](https://codeclimate.com/github/artemv/ruby-starter-kit/coverage)
[![Dependency Status](https://gemnasium.com/artemv/ruby-starter-kit.svg)](https://gemnasium.com/artemv/ruby-starter-kit)

#App code structure
Place your app-specific code in app/ dir, and utility code that you'd like to extract to gems later to lib/ dir. Files in both of them are autoloaded from app.rb (via lib/environment.rb).

#Installation
* Clone the repo: `git clone https://github.com/artemv/ruby-starter-kit.git my-app`
* Install Ruby 2.3.0 from https://www.ruby-lang.org/en/downloads/ or via RVM (https://rvm.io/)
* Install Bundler and dependencies:
```
cd my-app
gem install bundler
bundle install
```

#Usage
Run the app entry point script:
```
bin/app.rb
```

Run the guard dev env tool:
```
guard
```
It will run rubocop on start, will run rubocop inspections on changed files and will re-run all RSpecs and rubocop
inspections if you hit Enter in guard window.
