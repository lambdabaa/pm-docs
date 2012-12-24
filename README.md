# Engineering

## Local setup

### Dependencies

+ [plovr](http://plovr.com/)
+ [Rails 3.2.3](https://rvm.io/)
+ [Java](http://www.java.com/en/download/index.jsp)   // needed to run plovr

### Getting started

To get started developing locally:

    cd client && java -jar tools/plovr-eba786b34df9.jar serve plovr.json
    cd server && rails s

This runs the plovr build server on port 9810 and the rails web/asset server  
on port 3000.  
