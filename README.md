
# Welcome

This is a repository for documentation and scripts related to specimen digitization in the Natural History Museum of Los Angeles invertebrate paleontology collections (LACMIP).

## Scripts

Data cleaning and processing scripts to use with [OpenRefine](http://openrefine.org) are available in the [scripts](/scripts/) directory. Please see the [documentation website](https://lacmip.github.io/lacmip/) for how to use.

## Documentation

User-friendly documentation can be found at [https://lacmip.github.io/lacmip/](https://lacmip.github.io/lacmip/).

Content for this site is maintained in the [docs](/docs/) directory and hosted by GitHub Pages. Please see below for information about contributing to the documentation. You must be logged into GitHub and have the correct permissions to directly edit anything in this repository.

### How to edit an existing page

Find the page you wish to edit. Most should be located in the [docs/_documentation](docs/_documentation) directory.

Click on the filename, e.g. *access.md*, and then click on the pencil icon in the upper right corner to "Edit this file."

Edit whatever content and formatting you need to in the browser window. When you are ready to save, type a brief description in the "Commit Changes" box and click "Commit Changes." If you are making extensive edits, please refer to our [style guide](styleguide.md) to maintain consistency with headings and other formatting.

### How to create a new page

Creating a new page is easy, and the documentation website should automatically adjust its navigation to reflect your entry.

Begin by creating a new file ("Create new file") in the [docs/_documentation](docs/_documentation) directory. Name your file something short yet descriptive, and give it the *.md* extension, e.g. *loans.md*.

Include the following header at the very top of your new page:
```
---
title:
navcat:
tags:
---
```
This header contains "front matter" that the website uses to set itself up. It is important not only that you include the header but also that the information you include is appropriate. Here is what should go in each line:
- **title**: used to sort the sidebar navigation and as the first line of the page, e.g. "How to do a Loan"
- **navcat**: used to group pages into navigation categories for the sidebar navigation, e.g. "Workflows"
- **tags**: used to group pages into functional categories, e.g. "quick start"

## How to make bigger changes to the website:

The documentation website is hosted by GitHub Pages and based on the [Minimal Mistakes](mistakes.github.io/minimal-mistakes) remote theme. Please read up on both of these before diving into structural edits.

### Initial set-up on your local machine

You'll probably want to make bigger changes in a local environment vs. the GitHub website. To set up your local workspace...

1. Install [GitHub Desktop](https://desktop.github.com/) and clone this repository to your local machine.
1. Open a command line interface (e.g. Terminal for Macs) and check whether you have Ruby 2.1.0 or higher installed by running the command `ruby --version`. If you don't have Ruby installed, [install Ruby 2.1.0 or higher](https://www.ruby-lang.org/en/documentation/installation/).
1. Install Bundler by running `gem install bundler` in your command line.
1. Install Jekyll and other dependencies by running `bundle install` in your command line.

### Any time you want to work locally

1. In your command line interface, navigate to the GitHub Desktop instance of */lacmip/docs*, and run the command `bundler`. In Terminal, navigating to this directory might involve a command e.g. `cd Documents/GitHub/lacmip/docs`. You can check that you are in the folder you think you're in by entering `ls` to list the directory contents.
1. Edit website files as you wish in a text editor, e.g. [Atom](https://atom.io/).
1. When you want to preview the website locally, run the command `bundle exec jekyll serve` in your command line and open the link it returns in your browser. You will need to exit and re-run this command if you edit the *_config.yml* file, but other files should refresh automatically.
1. When you are ready to commit the changes you've made locally, open GitHub Desktop and push them to the master.
1. Keep your local dependencies current by occassionally running `bundle update` in your command line.
