Website for Palindrome Day
==========================

# Install

This uses Jekyll which is wonderful, but unfortunately requires Ruby on a mac, which is not.

Install the xcode command line tools for your flavour of MacOS from: https://developer.apple.com/download/more/

Install rvm:

    curl -sSL https://get.rvm.io | bash -s

Install ruby:

    bash # to get your newly installed rvm
    rvm install 3.0.0
    
Clone:

    git clone https://github.com/joesparrow/palindromeevents.git
    cd palindromeevents

Run:

    touch Gemfile
    gem install eventmachine -- --with-openssl-dir=/usr/local/opt/openssl@1.1
    gem install bundler
    bundle add webrick
    bundle add jekyll --version '~>3.9.0'
    bundle install
    
# Develop

Run jekyll with:

    bundle exec jekyll serve --incremental --watch

See the site locally: http://127.0.0.1:4000/

Or via domain name: https://palindromeday.co.uk
