---
layout: page
title: Instructions
permalink: /instructions/
---
![octocat][]

# Publishing Content with GitHub Pages

### Table of Contents
1. [Set up a GitHub Account](#step-1-set-up-a-github-account)
2. ['Fork' the site into your account](#step-2-fork-the-site-into-your-account)
3. [Set up your GitHub domain](#step-3-set-up-your-github-domain)

## Step 1: Set up a GitHub Account
***
Visit [https://github.com/join](https://github.com/join) and add your information. Choose the Free/Public plan, then activate your account by checking your email for the registration link.

__Note:__ Your username will also be part of your site's public URL, so choose one you can live with!

## Step 2: 'Fork' the site into your account
***
Visit the base site repository [https://github.com/mnyrop/nycdh-jekyll](https://github.com/mnyrop/nycdh-jekyll) in a new tab and click on the fork button near the top right corner.  ![fork button][fork]

This creates a [fork](https://help.github.com/articles/fork-a-repo/) (i.e. a diverging copy) of our base site for you to use and change however you want. Your fork/copy will start off looking something like this:

![](http://www.pixedelic.com/themes/geode/demo/wp-content/uploads/sites/4/2014/04/placeholder4.png)

This is the basic structure that will power your site!

## Step 3: Set up your GitHub domain
***
Before we start changing how things look, we'll need to see your site live at your own domain.
Click on the Settings tab and rename your repository to reflect your domain. This will be:

> your-username.github.io

For example, if your GitHub username is `bharkonnen`, your site will be `bharkonnen.github.io`.
<br><br>
![rename][]

Next, return back to the page with your files and find `_config.yml`. Click on it, then click the pencil button to edit. Replace `url` with your new url, and replace `baseurl` with "". Fill in other information (e.g. `title`, `description`, and `username` info) as you like. Scroll down and click "Commit" when you are ready.


[fork]: {{ site.baseurl }}/images/fork.png
[octocat]: {{ site.baseurl }}/images/octocat.gif
[rename]: {{ site.baseurl }}/images/rename.png
