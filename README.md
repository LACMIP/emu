
# Welcome

This is a repository for documentation, lookups, and scripts related to specimen digitization in the Natural History Museum of Los Angeles invertebrate paleontology collections (LACMIP). Please see below for an overview of the repository structure and how to use/contribute. You must be logged into GitHub and have the correct permissions to directly edit anything in this repository.

```
Repository Structure

lacmip
  |-- docs                  # DOCUMENTATION WEBSITE FILES
      |-- _data             
        |-- navigation.yml  # edit to create top bar navigation (currently unused)
        |-- ui-text.yml     # edit to affect labels for certain website elements
      |-- _documentation    # edit or create files in this collection to update documentation website content
        |--[example.md]
        |--[example.md]
        |--[example.md]
        |--...  
      |-- _includes         
        |-- head            # snippet to include custom favicon
        |-- nav_list        # overwrite for theme code to create dynamic left sidebar navigation
        |-- posts-tag.html  # overwrite for theme code to make tags on collection items function
        |-- tag-list.html   # overwrite for theme code to make tags on collection items function
      |-- _layouts          
        |-- single.html     # overwrite for theme layout to get rid of default pagination
      |-- _tag              # add files in this collection to add a new documentation set/category
        |--[example.md]
        |--[example.md]
        |--[example.md]
        |--...  
      |-- assets            
        |-- images          # single folder for any images related to the site
      |-- script            # default theme scripts related to website design
      |-- _config.yml       # configuration file; edit to change certain site defaults
      |-- Gemfile           # file to manage Ruby/Jekyll dependencies
      |-- index.html        # homepage for the documentation site
  |-- lookups               # LOOKUP FILES
  |-- scripts               # DIGITIZATION AND DATA CLEANING SCRIPTS

```

## Documentation

User-friendly documentation can be found at [https://lacmip.github.io/lacmip/](https://lacmip.github.io/lacmip/). Content for this site is maintained in the [docs](/docs/) directory and hosted by GitHub Pages.

Documentation is written with markdown formatting. If you are unfamiliar with markdown, this is a good [brief introduction](https://guides.github.com/features/mastering-markdown/). If you are making extensive edits, please refer to our [style guide](styleguide.md) to maintain consistency across documentation.

### How to edit an existing page

1. Find the page you wish to edit. Most should be located in the [docs/_documentation](docs/_documentation) directory.
1. Click on the filename, e.g. *access.md*, and then click on the pencil icon in the upper right corner to "Edit this file."
1. Edit the content and formatting as you wish in the browser window. Change the *last_modified_at* date in the header to reflect today's date.
1. When you are ready to save, type a brief description in the *Commit Changes* box and click "Commit Changes."

### How to create a new page

Creating a new page is easy, and the documentation website should automatically adjust its navigation to reflect your entry. Begin by creating a new file ("Create new file") in the [docs/_documentation](docs/_documentation) directory. Name your file something short yet descriptive, and give it the *.md* extension, e.g. *loans.md*.

Include the following header at the very top of your new page:
```
---
title:
navcat:
tags:
---
```
This header contains "front matter" that the website uses to set itself up. It is important not only that you include the header but also that the information you include is appropriate. Here is what should go in each line:
- **title**: used to alphabetically sort the sidebar navigation and as the first line of the page, e.g. "How to do a Loan"
- **navcat**: used to group pages into navigation categories for the sidebar navigation, e.g. "Basics" or "Modules" or "Workflows"
- **tags**: used to group pages into functional categories, e.g. "quick start"

Once you have added the header, the rest of your new page should be formatted in markdown. Please refer to our [style guide](styleguide.md) to maintain consistency across documentation. When you have finished writing your new page, commit the changes and refresh the documentation website to make sure everything looks as you expected.

### How to make bigger changes to the website

The documentation website is hosted by GitHub Pages and based on the [Minimal Mistakes](mistakes.github.io/minimal-mistakes) remote theme. Please read up on both of these before diving into structural edits. Most theme files are hosted remotely by Minimal Mistakes; any defaults that are being overwritten should be listed in the repository structure figure at the top of this page.

#### Initial set-up on your local machine

You'll probably want to make bigger changes in a local environment vs. the GitHub website. To set up your local workspace...

1. Install [GitHub Desktop](https://desktop.github.com/) and clone this repository to your local machine.
1. Open a command line interface (e.g. Terminal for Macs) and check whether you have Ruby 2.1.0 or higher installed by running the command `ruby --version`. If you don't have Ruby installed, [install Ruby 2.1.0 or higher](https://www.ruby-lang.org/en/documentation/installation/).
1. Install Bundler by running `gem install bundler` in your command line.
1. Install Jekyll and other dependencies by running `bundle install` in your command line.

#### Any time you want to work locally

1. In your command line interface, navigate to the GitHub Desktop instance of */lacmip/docs*, and run the command `bundler`. In Terminal, navigating to this directory might involve a command e.g. `cd Documents/GitHub/lacmip/docs`. You can check that you are in the folder you think you're in by entering `ls` to list the directory contents.
1. Edit website files as you wish in a text editor, e.g. [Atom](https://atom.io/).
1. When you want to preview the website locally, run the command `bundle exec jekyll serve` in your command line and open the link it returns in your browser. You will need to exit and re-run this command if you edit the *_config.yml* file, but other files should refresh automatically.
1. When you are ready to commit the changes you've made locally, open GitHub Desktop and push them to the master.
1. Keep your local dependencies current by occasionally running `bundle update` in your command line.

## Lookups

 Commonly used lookups, e.g. for collector names or for EMu taxonomy, are available in the [lookups](/lookups/) directory. Please see the [documentation website](https://lacmip.github.io/lacmip/) for how to use.

## Scripts

Data cleaning and processing scripts to use with [OpenRefine](http://openrefine.org) are available in the [scripts](/scripts/) directory. Please see the [documentation website](https://lacmip.github.io/lacmip/) for how to use.
