---
layout: post
title:  "Hosting a Website for Cheap Part 1"
date:   2017-01-21 8:39:51 -0600
categories: jekyll, github, aws, route 53, github pages
permalink: /hosting_for_cheap_part1/
---

## Why Jekyll

Building and hosting websites have come a long way over the years.  There are so many options, that it can be a little daunting starting out.  I am by far not a front-end web developer.  And if you are like me, you may be seeking an easy solution like a hosted platform that takes care of much of the labor such as Medium or Word Press for hosting a blog or simple website.

I'm going to provide a solution for those seeking to build a simple static website that can be used as a blog, portfolio, or what have you using a variety of tools.  In a series of posts, I'm going to outline how I put together this website and how I host my email for ~$0.53 per month.  

I use to pay $10 per month for DNS and virtual private server hosting.  Let's actually break down what I get now versus $10 per month paying before.  For $0.53 per month, I have a scalable website that can grow at demand with zero intervention or labor on my behalf.  Free https support enabled on this website where I do not have to renew any certificates for.  I have a free custom domain email address where I can generously send and receive way more emails than I will ever need.  Now I could cut the costs to $0, but that would take away any custom domain names I could assign to website and email hosting.  A very small price to pay.

Interested?  Let's dive into the real meat.  We are going to start from the ground up on how to get Jekyll going on our local machine.

## Linux Installation

I will be using [Xubuntu-16.10](http://mirror.us.leaseweb.net/ubuntu-cdimage/xubuntu/releases/16.10/release/) for now on.  Open up a terminal and install the following software packages with:

{% highlight bash %}
sudo apt-get install ruby2.3 ruby2.3-dev
sudo gem install jekyll bundler
jekyll new my-blog
{% endhighlight %}

What we did thus far is install Ruby 2.3(Ruby2.4 is the latest of this writing but is not supported in the latest Ubuntu Repos as of yet).  We also installed the development header files for ruby which are required for installing the gems jekyll and bundler.  Lastly, we created a default layout of "my-blog".

## Serving up our Jekyll web site

Now it's time to spin up what we have thus far.

{% highlight bash %}
jekyll serve
{% endhighlight %}

This in serve creates a local web server and creates our static html files (that are placed in _site folder)that can be viewed in our web browser at localhost:4000 by default.  

If you are wondering how do I navigate and figure out what does what, I would like to point you to https://jekyllrb.com/docs/structure/.

## Prettifying and Adding Content

The current default layout for our Jekyll site is bland.  A great way to overhaul our look is to browse at http://jekyllthemes.org/ where there are a number of free layouts that one can drag and drop into the _layouts folder.

Assuming the default layout, let's put together a post.  The easiest way is to examine our only example in the _posts folder.  Notice how the file name is dated as that is important for making more posts.

If you are not familiar with Markdown, I would recommend looking at https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet.

Try it for yourself and create a post in that directory.  See the results in the web browser by refreshing the home page.  Any errors will be displayed in the terminal.

## Conclusion of Part 1

Thus far, we have a simple Jekyll web site but we can't actually access it from the web.  In the next part, we will take a look at deploying it to Github Pages.  Our site will be managed and hosting on Github not a private web server like Amazon S3, Digital Ocean, etc.  Any changes or content we add, will be through Git.