## RAILS VERSION
Puts rails version
```
rails --version
```

## CREATE RAILS APP ONLY API
Creates a new rails api
```
rails new apiName -T --api
```
-T parameter ommits test folder.
<br>
--api parameter will generate a rails only api app

# INSTALL GEMS WITH GEMFILE
Add gem to gemfile
```
gem 'rspec-rails', '~> 5.0.0'
```
Then run de bundle command from the command line
```
bundle
```

# RUN RAILS SERVER
Runs Rails server on localhost at port 3000
```
rails s
```
# RUN RSPEC TESTS
Runs Rspec tests
```
rspec
```
