---
layout: post
title: Developing a proper help environment
---

In order to test out changes to the site I need a page seperate to the main group for testing purposes. For this reason the Test page was created. To store all the various notes and practice before rolling out across the site.

<img src="/public/images/green_blog_test.png">

To remove the test page from the automatic sidebar, I added an AND statment determining any post titled "Test" should be removed from the sidebar {% raw %}"{% if node.title != null <span style="color:blue">and node.title != "Test"</span> %}".{% endraw %} Leaving the Test page seperate from sidebar and reachable only if searching for it.
