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

### composite primary keys on table (many-to-many)

0. install [this](https://rubygems.org/gems/composite_primary_keys) to your bundle
1. add self.primary_keys = :YOUR_KEY1, :YOUR_KEY2 (model)
2. add bleongs_to to each column (model)
3. add add_foreign_key to each column (migration)
4. add execute 'alter table xxx add primary key (key1, key2) (migration)

ref: [this](https://stackoverflow.com/questions/12746280/define-a-unique-primary-key-based-on-2-columns)

### :destory vs :delete on Active Record

The easiest way to sum it up is to use delete if you want records to be deleted quickly. However, if you care about models callbacks, referential integrity, or validations (for example, setting a criteria to not destroy a record unless a certain condition is “true”), then use destroy.

- destory

  1. all callbacks are called.
  2. refererntial integrity matters (if you break the constraint, you receive the error)
  3. validation matters (if you failed a validation, you receive the error)

- delete

  1. none of them above matters

## Errors

### gem install mysql2 failed on ubuntu

answer: https://stackoverflow.com/questions/37240720/how-to-install-mysql2-on-ubuntu-16-04-error-error-installing-mysql2-error-f

### Use the new Ruby 1.9 hash syntax. (convention:Style/HashSyntax)

previous: 

```
:id => value
```

new:

```
id: value
```

see [this](https://stackoverflow.com/questions/44005410/need-to-refactor-to-the-new-ruby-1-9-hash-syntax/44005425)
