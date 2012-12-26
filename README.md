# Engineering

## Local setup

### Dependencies

+ [plovr](http://plovr.com/)
+ [Rails 3.2.3](https://rvm.io/)
+ [Java](http://www.java.com/en/download/index.jsp)   // needed to run plovr

### Getting started

To get started developing locally we need to do two things:

Run the Rails web/asset server on port 3000 via:

    cd server
    bundle install
    rake db:create:all
    rake db:migrate
    rake db:fixtures:load   # Only if you want the fixtures data
    rails s

Run the plovr build server on port 9810 via:

    cd client
    java -jar tools/plovr-eba786b34df9.jar serve plovr.json

### Running the tests

To run the tests do:

    cd server
    rake db:migrate
    rake db:test:prepare  # Loads the test fixtures
    rspec -c -f d spec/*spec.rb
