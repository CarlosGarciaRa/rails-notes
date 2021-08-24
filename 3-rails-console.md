# RAILS CONSOLE
> The console command lets you interact with your Rails application from the command line. This is useful for testing out quick ideas with code and changing data server-side without touching the website.
- [running rails console](https://github.com/CarlosGarciaRa/rails-notes/new/main#runniing-rails-console)
- [exit rails console](https://github.com/CarlosGarciaRa/rails-notes/new/main#exit-rails-console)
- [database commands](https://github.com/CarlosGarciaRa/rails-notes/new/main#database-commands)
  * [number of records](https://github.com/CarlosGarciaRa/rails-notes/new/main#number-of-records)
  * [create new record](https://github.com/CarlosGarciaRa/rails-notes/new/main#create-new-record)
  * [first record](https://github.com/CarlosGarciaRa/rails-notes/new/main#first-record)
  * [record attribute](https://github.com/CarlosGarciaRa/rails-notes/new/main#record-attribute)


## RUNNIING RAILS CONSOLE
```
rails c
```
## EXIT RAILS CONSOLE
```
quit
```
## DATABASE COMMANDS
### NUMBER OF RECORDS
Returns the number of records in a table.
```
ModelName.count
```
### CREATE NEW RECORD
Creates records in a table.
```
ModelName.create
```
### FIRST RECORD
Returns the first record in a table.
```
ModelName.first
```
### RECORD ATTRIBUTE
Returns attribute of a record.
```
ModelName.first.attribute
```


