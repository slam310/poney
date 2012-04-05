# Project script

This script provide simple method to handle a Symfony2 poney, it help you to run task

## Installation

    cd ~/bin
    git clone git://github.com/benji07/poney.git poney

Add the poney script inside your `PATH`

    export PATH=~/bin/poney/bin:$PATH

## Usage

Display help using this command

    $ poney

Install a poney (create parameters file, chmod cache dir, install vendors, create database, load fixtures and install assets)

    $ poney install

Update a poney (update the database and install assets)

    $ poney update

Update vendors of a poney

    $ poney vendors

Install git hooks (you need to create directories named after git hooks inside bin/hooks directory, ie: bin/hooks/pre-commit/phplint).

I bundle this script with 2 hooks i used on each of my Symfony2 poney (PHPCS and PHP Lint).

    $ poney hooks

Reload fixtures for a poney

    $ poney fixtures

If something went wrong while using these script, you can find log inside the file app/logs/poney.log

## Disclamer

This script use helpers from [Ciboulette](https://github.com/knplabs/ciboulette).