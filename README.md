# Project script

This script provide simple method to handle a Symfony2 project, it help you to run task

## Installation

    cd ~/bin
    git clone git://github.com/benji07/project.git project

Add the project script inside your `PATH`

    export PATH=~/bin/project/bin:$PATH

## Usage

Display help using this command

    $ project

Install a project (create parameters file, chmod cache dir, install vendors, create database, load fixtures and install assets)

    $ project install

Update a project (update the database and install assets)

    $ project update

Update vendors of a project

    $ project vendors

Install git hooks (you need to create directories named after git hooks inside bin/hooks directory, ie: bin/hooks/pre-commit/phplint).

I bundle this script with 2 hooks i used on each of my Symfony2 project (PHPCS and PHP Lint).

    $ project hooks

Reload fixtures for a project

    $ project fixtures

If something went wrong while using these script, you can find log inside the file app/logs/project.log

## Disclamer

This script use helpers from [Ciboulette](https://github.com/knplabs/ciboulette).