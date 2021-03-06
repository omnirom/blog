![logo](https://github.com/omnirom/Docs/blob/master/images/omnirom_logo-big_layout_transparent-250px-150x150.png)
# OmniROM blog
## Introduction
The blog for Omni is setup using [Jekyll](https://jekyllrb.com/), allowing for quick and easy deployment of news for the Community. The below will give you the information you need to contribute to the Omni Community.

## Getting Started
### Setup Jekyll
In order to begin contributing, you need to setup Ruby and Jekyll on your local machine. To do so, perform the following:
```
$ sudo apt-get install ruby bundler
$ gem install jekyll
$ sudo gem install bundler **you may need to do this with MacOS**
$ sudo gem update
```
For more information on setup, see the [Jekyll Install Guide](https://jekyllrb.com/docs/installation/).

### Fork and Clone the Blog
In order to contribute you will need to create a fork to your own Github account and then clone that repo. The command to clone to your local machine would be something like (with <yourusername> replaced with your Github username):
```
$ git clone git@github.com:<yourusername>/blog.git
```
Navigate to the cloned folder, in this case `blog`, and then type the following:
```
sudo bundle update
sudo bundle install
jekyll serve
```
You will now be able to see a local copy of the blog on your machine at http://localhost:4000. Make any changes you would like and then push them to your fork, and then initiate a pull request and describe your changes.


## Contributing to the blog
### Post Format
The following needs to be at the top of each post with the `title`, `date`, `exceprt`, `categories`, and `tags` filled out:
```
---
layout: post
title: ""
date: YYYY-MM-DD HH:MM:SS -GMTOFFSET
excerpt:
categories:
-
tags:
-
author:
  display_name: name_to_be_displayed
---
```
All posts need to be placed into the `_posts` folder and the file name following the below convention:
```
YYYY-MM-DD-title-of-post.MARKUP
```
The file extension can be `.md` if you're doing a post using [Markdown](https://guides.github.com/features/mastering-markdown/) code, or `.html` if you decide to do an HTML post.
