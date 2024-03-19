---
layout: post
title: Developing a proper testing environment
---
In order to test any changes made to my site I have two methods:

1. Test page:
A page alongside "about" that contains various features that I have yet to spread across the site. 
<img src="/public/images/green_blog_test.png">
To remove the test page from the automatic sidebar, I added an AND statment determining any post titled "Test" should be removed from the sidebar {% raw %}"{% if node.title != null <span style="color:blue">and node.title != "Test"</span> %}".{% endraw %} Leaving the Test page seperate from sidebar and reachable only if searching for it.

2. Local host:
Hosting the site locally allows for changes not pushed to the Git repositiory to be previewed in a browser. Specifically with the inbuilt Jekyll command 'serve', that hosts the site locally.