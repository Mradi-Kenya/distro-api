# DISTRO - API

GOAL: Enable distribution campaigns to be more structured and help in empowering logistics of ensuring the right person and all beneficiaries get what they were promised.

## Development

The api is built using `Ruby` as the primary language, and `Rails` as the preferred framework.

## Key Dependencies to run this in your own local machine
- Docker
- Ruby: currently at version - `3.2.1`
- Rails: currently at version `7.0.4`
- Dip: A Docker compose wrapper, at version - `7.5`

### How to install **Dip**
- `gem install dip` in your local ruby.
- NB: Using a Ruby Version Manager is highly recommended: `rbenv` or `rvm`.

### How to setup the docker containers
From scratch you should first build the container images.
- `dip build`


When your local machine needs to setup the environment for the containers i.e. the volumes, network etc.
- `dip provision`


### How to start your services
```sh
# Rails Console
dip rails c

# Run Rails server with debugging capabilities i.e. `debugger` would work.
dip rails s

# Run Rails the web app (with all the dependencies)
dip up web


# Run migrations
dip rails db:migrate

# Launch bash within the app directlry (with dependencies up)
dip runner

# Run any command via bash
dip bash -c 'ls -al tmp/cache'

# Update gems or packages
dip bundle install

# Run psql console
dip psql

# Run tests
# NB: This commands is prefixed with `RAILS_ENV=test`
dip rspec
or
dip rspec spec/path_to_folder/path_to_individual_spec.rb:path_to_specific_line

# Run linter
dip rubocop

# Shutdown all containers
dip down
```

