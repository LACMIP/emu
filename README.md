
This is a repository for...

## How to create a new page

title: Accessing EMu
navcat: Basic Info (this is what sets a page in a navigation section)
tags: onboard (and on the top bar)

`{% include figure image_path="/assets/images/unsplash-image-10.jpg" alt="this is a placeholder image" caption="This is a figure caption." %}`

`{% include video id="XsxDH4HcOWA" provider="youtube" %}`

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

### Initial set-up

1. Install [GitHub Desktop](https://desktop.github.com/) and clone this repository to your local machine.
1. Open a command line interface (e.g. Terminal for Macs) and check whether you have Ruby 2.1.0 or higher installed by running the command `ruby --version`. If you don't have Ruby installed, [install Ruby 2.1.0 or higher](https://www.ruby-lang.org/en/documentation/installation/).
1. Install Bundler by entering `gem install bundler` into your command line.

### Any time you want to work locally

1. In your command line interface, navigate to the GitHub Desktop instance of */lacmip/docs*, and run the command `bundler`. In Terminal, navigating to this directory might involve a command e.g. `cd Documents/GitHub/lacmip/docs`. You can check that you are in the folder you think you're in by entering `ls` to list the directory contents.
1. Edit website files as you wish in a text editor, e.g. [Atom](https://atom.io/).
1. When you want to preview the website locally, run the command `bundle exec jekyll serve` in your command line and open the link it returns in your browser. You will need to exit and re-run this command if you edit the *_config.yml* file, but other files should refresh automatically.
1. When you are ready to


mistakes.github.io/minimal-mistakes
