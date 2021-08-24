# RAILS MODEL
- [creating rails model](https://github.com/CarlosGarciaRa/rails-notes/new/main#creating-a-rails-model)
- [running migrations](https://github.com/CarlosGarciaRa/rails-notes/new/main#running-migrations)

## CREATING A RAILS MODEL
> A Rails Model is a Ruby class that can add database records

In order to create a Rails Model we run the following command on the shell
```
rails generate model ModelName ColumnOneName:ColumnOneType ColumnTwoName:ColumnTwoType
```
It will generate this output
```
Running via Spring preloader in process 3719
      invoke  active_record
      create    db/migrate/20210824164447_create_articles.rb
      create    app/models/ModelName.rb
      invoke    rspec
      create      spec/models/ModelName_spec.rb
      invoke      factory_bot
      create        spec/factories/ModelNames.rb
```

## RUNNING MIGRATIONS
> A Rails migration is a tool for changing an application’s database schema. 
In order to run migrations we run the following command on the shell
```
rails db:migrate
```

It will generate this output
```
== 20210824164447 CreateArticles: migrating ===================================
-- create_table(:articles)
   -> 0.0030s
== 20210824164447 CreateArticles: migrated (0.0037s) ==========================
```
