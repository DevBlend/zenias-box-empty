# Empty Zenias box

This is a vagrant box with no specific package installed, but only zenias is accessible.

## Specs:
  - Box: minimal/trusty64

## Filesystem
This folder is a shared folder: so you will find its content on the _guest_ machine in the `/vagrant` folder.

## Packages
This virtual machine has been created with no specific package beside `git` and the `heroku-toolelt`.

## Pushing your commits to Heroku
A simple step by step method to push your website to heroku:

```bash
# You must be in the /vagrant/working_dir dir:
cd /vagrant/working_dir

# Init a git repo if not already done:
git init

# Commit your changes:
git add .
git commit -m 'Initial commit'

# Create a heroku app:
heroku create

# Push the site:
git push heroku master

# Test the heroku box :
heroku open
```