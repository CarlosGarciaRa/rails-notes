# RVM RUBIES
RVM basics commands
- [rvm list](https://github.com/CarlosGarciaRa/rails-notes/blob/main/rvm-basics.md#rvm-list)
- [rvm use](https://github.com/CarlosGarciaRa/rails-notes/blob/main/rvm-basics.md#rvm-use)
- [rvm uninstall](https://github.com/CarlosGarciaRa/rails-notes/blob/main/rvm-basics.md#rvm-uninstall)
- [rvm list gemsets](https://github.com/CarlosGarciaRa/rails-notes/blob/main/rvm-basics.md#list-all-gemsets)
- [rvm gemset list](https://github.com/CarlosGarciaRa/rails-notes/blob/main/rvm-basics.md#list-gemsets-for-current-interpreter)
- [rvm gemset use](https://github.com/CarlosGarciaRa/rails-notes/blob/main/rvm-basics.md#use-gemset)
- [rvm gemset create](https://github.com/CarlosGarciaRa/rails-notes/blob/main/rvm-basics.md#create-gemset)
- [rvm gemset delete](https://github.com/CarlosGarciaRa/rails-notes/blob/main/rvm-basics.md#delete-gemset)
- [gem list](https://github.com/CarlosGarciaRa/rails-notes/blob/main/rvm-basics.md#list-gems)
- [gem list](https://github.com/CarlosGarciaRa/rails-notes/blob/main/rvm-basics.md#list-gems)
- [gem install](https://github.com/CarlosGarciaRa/rails-notes/blob/main/rvm-basics.md#gem-install)

## RVM LIST
List Ruby interpreters you've already installed
```
rvm list

=* ruby-2.7.2 [ x86_64 ]
=* ruby-2.7.3 [ x86_64 ]
=* ruby-2.7.4 [ x86_64 ]
```

## RVM USE
Use a particular Ruby.
```
rvm use 2.7.2

Using /home/.rvm/gems/ruby-2.7.2
```
## RVM UNINSTALL
Uninstall a particular Ruby.
```
rvm uninstall 2.0.0
```
# RVM GEMSETS

## LIST ALL GEMSETS
To list all gemsets

```
rvm list gemsets

ruby-2.7.2 [ x86_64 ]
ruby-2.7.2@global [ x86_64 ]
ruby-2.7.2@rails-api [ x86_64 ]
```
## LIST GEMSETS FOR CURRENT INTERPRETER
To list all named gemsets for the current ruby interpreter

```
rvm gemset list

=> (default)
   global
   rails-api
```

## USE GEMSET
To use a specific gemset

```
rvm gemset use rails-api

Using ruby-2.7.2 with gemset rails-api
```

## CREATE GEMSET
To create a specific gemset

```
rvm gemset create rails-api

Gemset 'rails-api' created.
```

## DELETE GEMSET
To delete a specific gemset

```
rvm gemset delete rails-api
```

# RVM GEMS

## LIST GEMS
To list gems in a specific gemset

```
gem list

*** LOCAL GEMS ***

actioncable (6.1.4)
actionmailbox (6.1.4)
actionmailer (6.1.4)
actionpack (6.1.4)
actiontext (6.1.4)
actionview (6.1.4)
activejob (6.1.4)
activemodel (6.1.4)
```

## INSTALL GEMS
To install gems in a specific gemset

```
gem install rails -v 4.1.0
```
