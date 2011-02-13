# Rukoreh
This is a bare Ruby on Rails 3 app that has been configured for deployment on Heroku.  The steps below were all that was needed.

On Heroku, the app lives at [http://hollow-cloud-468.heroku.com](http://hollow-cloud-468.heroku.com)
## Heroku Documentation

  - [http://devcenter.heroku.com/](http://devcenter.heroku.com/)
  - [http://docs.heroku.com/quickstart](http://docs.heroku.com/quickstart)

## Create Heroku account
  - [http://heroku.com/signup](http://heroku.com/signup)

## Create new app
    rails myapp  
    cd myapp

## Install Heroku gem - add to Gemfile
    gem 'heroku'  
    bundle install

## Add ssh keys for Heroku
    heroku keys:add

## Regularly update Heroku gem
    gem update heroku

## Initialize with git
    git init  
    touch .gitignore
### add appropriate entries to .gitignore
    git add .  
    git commit -m 'Initial commit'

## Create app on Heroku
    heroku create

## Deploy app to Heroku
    git push heroku master

## Setup database
    heroku rake db:migrate

## Next steps
  - Develop and test changes locally.
  - Commit code to git.
  - Push your changes to Heroku with `git push heroku`.
