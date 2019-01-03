
This is a repository for...

## How to create a new page

title: Accessing EMu
navcat: Basic Info (this is what sets a page in a navigation section)
tags: onboard (and on the top bar)

## To update the documentation website:
Simply run bundle update if you’re using Bundler.
Use Git
If you want to get the most out of the Jekyll + GitHub Pages workflow, then you’ll need to utilize Git. To pull down theme updates you must first ensure there’s an upstream remote. If you forked the theme’s repo then you’re likely good to go.

To double check, run git remote -v and verify that you can fetch from origin https://github.com/mmistakes/minimal-mistakes.git.

To add it you can do the following:

git remote add upstream https://github.com/mmistakes/minimal-mistakes.git
Pull down updates
Now you can pull any commits made to theme’s master branch with:

git pull upstream master
Depending on the amount of customizations you’ve made after forking, there’s likely to be merge conflicts. Work through any conflicting files Git flags, staging the changes you wish to keep, and then commit them.

## To work on the documentation website locally (on your computer):

1. Clone the GitHub repository
1. install
1. run the command `bundle exec jekyll serve` in your command line interface (e.g. Terminal for Macs)


mistakes.github.io/minimal-mistakes
