# Ruby

## How configure env for ruby project

see [this](https://www.honeybadger.io/blog/rbenv-rubygems-bundler-path/)

## rbenv 

a new lightweight Ruby version management tool built. an alternative for RVM.

you can switch a version of Ruby based on the requirement.

much simpler version of RVM.

installation guide: https://gorails.com/setup/ubuntu/20.04#ruby-rbenv

## RVM

same as rbenv, it is more powerful and complicated.

## Bundler 

Bundler helps us easily specify all our project dependencies and optionally specify a version for each.

## RubyGems

a Ruby packaging system designed to facilitate the creation, sharing, and installation of libraries.

## Commands



## Questions

### diff btw 'gem install' and 'bundle install'

The main difference is that Rubygems (invoked with the command gem) manages all the gems (gemsets if you are using RVM) for a single machine, whereas Bundler (bundle) manages a gem set for a single application (its purpose being to deploy on multiple machines).

ref: [this](https://stackoverflow.com/questions/20224855/what-is-the-difference-between-bundle-update-and-gem-update/20224856)

## Errors

### gem install mysql2 failed on ubuntu

answer: https://stackoverflow.com/questions/37240720/how-to-install-mysql2-on-ubuntu-16-04-error-error-installing-mysql2-error-f

### 
