#CBR rates fetcher
A command line tool to fetch [CBR](http://cbr.ru) currency rate as of given date. A wrapper over CBR XML API method.

#Installation
* Clone the repo: `git clone https://github.com/artemv/cbr-rates.git`
* Install Ruby 2.3.0 from https://www.ruby-lang.org/en/downloads/ or via RVM (https://rvm.io/)
* Install Bundler and dependencies:
```
cd cbr-rates
gem install bundler
bundle install
```
* Run the currency rate fetching script: `date="2015-09-16" code=BRL ./cbr_rate.rb`
By default it fetches USD rate: `date="2015-09-16" ./cbr_rate.rb`
