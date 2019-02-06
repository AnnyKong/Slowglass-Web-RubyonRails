<!-- # README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ... -->

## Slowglass Web App


## start
```
rails new blog

bundle install
```

## basic rundown on the function of each of the files and folders that Rails created by default:
Directory structure
```
app/	controllers/models/views/helpers/mailers/channels/jobs/assets

bin/	rails script/ setup/update/deploy/run scripts

config/	Configure routes/database

config.ru	Rack configuration

db/	database schema/migrations

Gemfile
Gemfile.lock	needed gem dependencies(Bundler gem)

lib/	Extended modules

log/	log files.

package.json	needed npm dependencies by Yarn

public/	static files/compiled assets.

Rakefile	locates and loads tasks (for command line)

README.md	instruction manual/ how to set it up

test/	Unit tests/fixtures/test apparatus

tmp/	Temporary files (like cache/pid files).

vendor/	third-party code. i.e. vendored gems

.gitignore	which files should ignore.

.ruby-version	This file contains the default Ruby version.
```

Detailed version:
```
File/Folder	Purpose
app/	
Contains the controllers, models, views, helpers, mailers, channels, jobs and assets for your application.

bin/	
Contains the rails script that starts your app and can contain other scripts you use to setup, update, deploy or run your application.

config/	
Configure your application's routes, database, and more. This is covered in more detail in Configuring Rails Applications.

config.ru	
Rack configuration for Rack based servers used to start the application. For more information about Rack, see the Rack website.

db/	
Contains your current database schema, as well as the database migrations.

Gemfile
Gemfile.lock	
These files allow you to specify what gem dependencies are needed for your Rails application. These files are used by the Bundler gem. For more information about Bundler, see the Bundler website.

lib/	
Extended modules for your application.

log/	
Application log files.

package.json	
This file allows you to specify what npm dependencies are needed for your Rails application. This file is used by Yarn. For more information about Yarn, see the Yarn website.

public/	
The only folder seen by the world as-is. Contains static files and compiled assets.

Rakefile	
This file locates and loads tasks that can be run from the command line. The task definitions are defined throughout the components of Rails. Rather than changing Rakefile, you should add your own tasks by adding files to the lib/tasks directory of your application.

README.md	
This is a brief instruction manual for your application. You should edit this file to tell others what your application does, how to set it up, and so on.

test/	
Unit tests, fixtures, and other test apparatus. These are covered in Testing Rails Applications.
tmp/	Temporary files (like cache and pid files).

vendor/	
A place for all third-party code. In a typical Rails application this includes vendored gems.
.gitignore	This file tells git which files (or patterns) it should ignore. See GitHub - Ignoring files for more info about ignoring files.

.ruby-version	This file contains the default Ruby version.
```

## view all commands
```
rails new -h.
```

## start app
```

$ bin/rails server


$ bin/rails generate controller Welcome index
```


## view routes
`bin/rails routes`

## generate more controller and models
`rails generate controller Articles`
`rails generate model Article title:string text:text`

## run migration
`rails db:migrate`
`bin/rails db:migrate RAILS_ENV=production.`
