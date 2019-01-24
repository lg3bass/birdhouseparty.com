+++
date = 2019-01-22T14:09:42-05:00
title = "creating a blog post"
writer = "Bob White"
draft = false
image = "header.png"
showonlyimage = false
categories = ["blog"]
keywords = ["hugo"]
topics = ["organization"]
tags = ["hugo", "work"]
weight = 1
description = "Creating a new blog post in gohugo.io"
+++

###Quick steps to create a blog post:

* create new blog post from template
* edit the .md file
* check with hugo server -D (drafts enabled)
* push to git
	

<!--more-->

###Detailed Instructions

1. Check the <https://www.birthouseparty.com> to make sure your is has been updated. 
2. Start the local server at <http://localhost:1313> to see the local changes and determine where you left off. 

		hugo server -D

3. Navigate to [http://localhost:1313/](http://localhost:1313/)

4. All good? OK, now let's create a new blog post.  To do so you will need exit the localhost mode.  To exit back to the terminal prompt type command-key(mac) + "C".

5. Create a new blog post using standard template

		hugo new --kind post-bundle post/<date>_<title-no-spaces>
		
	For my blog I will be using the convention:
	<date> = 20190122 
	<title-no-spaces> = title should be all lowercase separated y hyphens.  for instance:  "my-new-blog-post".
	
	example: **20190122_my-new-blog-post**
	
6. By default a blog post folder will be created in the post/ folder. Inside the "20190122_my-new-blog-post" folder will be folder called "work_new" and markdown file called "work_new.md".   Change the name of the folder and .md file to match.  Generally I would use the second part of the name you used to create the post.  e.g. "my-new-blog-post".

7. Edit your blog post to your heart's content.  Here is a [markdown cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet). I use [macdown](https://macdown.uranusjr.com/) to create and edit posts. 

8. Happy? Well then...Time to test. For reference here is a list of hugo commands.  See [basic usage](https://gohugo.io/getting-started/usage/) at gohugio.io.  Generally you want to use "hugo server" this will rebuild your blog at <http://localhost:1313>.  You can add flags like including drafts or publish to a dev or public directory.

		//starts a localhost:1313 server and writes 
		//content to /dev with drafts(-D) and watch (-w).
		hugo server -wD -d dev
		
		//create localhost:1313 (only) with drafts enabled
		hugo server -D
		
		//publish files to the /public directory with drafts enabled.
		hugo -D
		
		//create a localhost:1313 
		hugo server

9. Finally, let's publish to git.  I have setup birdhouseparty.com so that once you publish to git it will automatically regenerate the site on birdhouseparty.com.  Easy.

		//commit to github instructions
		git status -S
		

