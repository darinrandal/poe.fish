# poe.fish

poe.fish - Path of Exile Fishing Wiki website!

# Contributing

Anyone is welcome to contribute change requests via Pull Requests. If you're not familiar with GitHub, you'll need to read a couple guides but ultimately making changes to the wiki isn't to complex. You'll need a GitHub account and you'll need to follow the steps below to get it running on your computer. 

The majority of the wiki pages are written solely in [Markdown](https://www.markdownguide.org/basic-syntax/). The syntax is pretty straightforward. There is a few pages that have HTML that is required for some formatting but if you're interested in just changing text you'll be able to do that without knowing any HTML.

If you're uncomfortable with GitHub you can request changes with me on Discord at `darin#0001` or email your request to `updates@poe.fish`. Any changes will need to have supporting documentation/proof and be approved by a member of the Fishcord.

## Installation on Windows

Follow the Jekyll installation document [here](https://jekyllrb.com/docs/installation/windows/).

TL;DR: 
- Download the latest version of RubyInstaller.
- Choose all defaults for any options during the installation procedure.
- After the installation has finished open up a command prompt and run `gem install jekyll bundler` to install the website builder and bundler

After installation has completed

- Clone this GitHub repository to: `Documents\GitHub\poe.fish`.
- In command prompt change directories to your cloned repo: `cd Documents\GitHub\poe.fish`
- Run `bundle install` to install all the dependencies
- Run `jekyll serve --livereload` to start the web server
- Access the website at [127.0.0.1:4000](http://127.0.0.1:4000)

## Installation on Mac OS

- Install [homebrew](https://brew.sh/) if you don't have it already
- In your terminal run `brew install chruby ruby-install`
- Run `ruby-install ruby`
- Run the following in Terminal to add chruby to your path to change Ruby versions like so:

```
echo "source $(brew --prefix)/opt/chruby/share/chruby/chruby.sh" >> ~/.bash_profile
echo "source $(brew --prefix)/opt/chruby/share/chruby/auto.sh" >> ~/.bash_profile
echo "chruby ruby-3.1.2" >> ~/.bash_profile
```

- Quit and relaunch your terminal and run `ruby -v` you should see: 3.1.2 or higher
- Run `gem install jekyll bundler` to install Jekyll the website builder and bundler
- Clone this GitHub repository to `~/Documents/GitHub/poe.fish`
- In command prompt change directories to your cloned repo: `cd Documents/GitHub/poe.fish`
- Run `bundle install` to install all the dependencies
- Run `bundle exec jekyll serve --livereload` to start the web server
- Access the website at [127.0.0.1:4000](http://127.0.0.1:4000)

## File Structure

Currently the structure of the site consists of a few files in the root which are base pages that don't fit into a category.

Base pages:

 - `index.md` - home page
 - `anglers-mate-issues.md` - a list of every Angler's Mate edition on Reddit
 - `frequently-asked-questions.md` - FAQ
 - `scourge-modifiers-fishing` - ccourge modifiers
 - `fishing-items` - master list of all fishing items
 - `fishing-items/` - main folder which contains individual fishing item pages
   - `albino-rhoa-feather.md` - page dedicated to the albino rhoa feather
   - `anglers-plait.md` - page dedicated to angler's plait
   - ... the pages continue
 - `zones/` - folder containing every zone-specific pages
   - `areas-are-alluring.md` - areas are alluring sextant
   - `krillson-master-fisherman.md` - krillson info
   - ... other zone pages continue

## Adding a new page

Add a new page by putting it in the respective directory, either the root for base pages which don't fit in a category like `zones/` or `fishing-items/`, or create a new directory. A new page for a hypothetical fishing item named Bucket of Water would be: `fishing-items/bucket-of-water.md`. The final URL of this file would be `https://poe.fish/fishing-items/bucket-of-water`.

**Every page needs front matter. This lets the site builder know how to handle the new file.**

Front matter is seen at the top of each page file in this repository it follows this format:

```
---
layout: page
title: Angler's Plait
description: How to find Angler's Plait, Unset Ring in Path of Exile and how it relates to fishing
permalink: /fishing-items/anglers-plait/
image: /assets/img/anglers-plait.png
---

[ page content here ]
```

Properties - every property is required except `image` 
- `layout` - will always be `page`
- `title` - title of the page, shows up in the browser tab and the first h1 of the page automatically
- `description` - describe the page content in 255 characters or less
- `permalink` - URI of the page **with** a beginning slash *and* and **ending** slash with no domain or protocol such as `fishing-items/bucket-of-water`
- `image` - optional URI for an associated image for the image. typically used as a preview in search engines or discord
