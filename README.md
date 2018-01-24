# Publishing Content with GitHub Pages
# Instructions

__Table of Contents__
1. [Set up a GitHub Account](#step-1-set-up-a-github-account)
2. ['Fork' the sample site into your account](#step-2-fork-the-sample-site-into-your-account)
3. [Set up your GitHub domain](#step-3-set-up-your-github-domain)
4. [View your site](#step-4-view-your-site)
5. [Edit a post](#step-5-edit-a-post)
6. [Add a new page](#step-6-add-a-new-page)

__Advanced:__ [Learn about Liquid](../advanced-liquid/)

![octocat][]

## Step 1: Set up a GitHub Account
***
Visit [https://github.com/join](https://github.com/join) and add your information. Choose the Free/Public plan, then activate your account by checking your email for the registration link.

*__Note:__ Your username will also be part of your site's public URL, so choose one you can live with!*

## Step 2: 'Fork' the sample site into your account
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

Return back to the page with your files and find `_config.yml`. Click on it, then click the pencil button to edit. Replace the `baseurl` value with empty single quotes: `''`. (This will serve your site at your domain instead of `yourdomain.github.io/nycdh-jekyll/`.)

Next, fill in other information (e.g. `title`, `description`, and `username`) as you like. Scroll down and click "Commit" when you are ready.

You can always change these later, so don't worry!
<br><br>
![config][]

## Step 4: View your site
***
Open up a new tab, and navigate to your domain. It may take a minute or so, but should look like something like this:
<br><br>
![screen][]

## Step 5: Edit a post
***
 While still on your live site, click on "Writing My Own Post." (It should be at `yourdomain.github.io/2018/01/22/my-own-post/`.)

 Open the [Markdown Cheatsheet](../markdown-cheatsheet/) in another tab. And in one more tab, open your site repository on GitHub, navigate into `_posts`, open `2018-01-22-my-own-post.md`, and click edit.

 Skim through the Markdown Cheatsheet and rewrite the contents of the post with headers, lists, and links. Commit the edits and refresh the live post to see your changes.

 *__Note:__ Jekyll is very picky about post titles and dates. If you want to change them, make sure you keep the same date format! Titles cannot have `:` characters unless you wrap the entire title in quotes (`title: "My Tile: My Subtitle"`). Lastly change the file name (up top) to reflect your new title and date.*


## Step 6: Add a new page
***
Now that we've edited an existing post with Markdown, we can add a brand new page with text and images. Navigate to the home of your site repository on GitHub, and click __"Create New File"__.

Enter the name of your file up top. It **cannot** have spaces or special characters, **must** be lowercase, and must end in **.md** (for Markdown).

__Good:__  
- `my-project-name.md`  
- `test-page.md`  
- `really-long-but-still-okay-name.md `  

__Bad:__
- `has spaces .md`
- `badextension.doc`
- `too-$pec!al.md`

Add metadata to the top of your file, between two lines with three hypthens, like so:
```yaml
---
layout: page
title: <Your Title>
permalink: /<your-permalink>
---
```
Underneath the metadata, add info to your page just like with the post. This time, try to add at least one image! The syntax for an image is:

`![label][http://link-to-full-image.jpg]`



[octocat]:  https://github.com/mnyrop/nycdh-jekyll/blob/master/images/octocat.gif?raw=true
[fork]:     https://github.com/mnyrop/nycdh-jekyll/blob/master/images/fork.png?raw=true
[rename]:   https://github.com/mnyrop/nycdh-jekyll/blob/master/images/rename.png?raw=true
[config]:   https://github.com/mnyrop/nycdh-jekyll/blob/master/images/config.png?raw=true
[screen]:   https://github.com/mnyrop/nycdh-jekyll/blob/master/images/screen.png?raw=true
