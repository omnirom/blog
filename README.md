![logo](https://github.com/omnirom/Docs/blob/master/images/omnirom_logo-big_layo
ut_transparent-250px-150x150.png)
# OmniROM blog
## Introduction
The blog for Omni is setup using [Jekyll](https://jekyllrb.com/), allowing for quick and easy deployment of news for the Community. The below will give you the information you need to contribute to the Omni Community.

## Getting Started
### Setup Jekyll
In order to begin contributing, you need to setup Ruby and Jekyll on your local machine. To do so, perform the following:
```
$ sudo apt-get install ruby bundler
$ gem install jekyll
$ sudo gem update
```

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
---
```
