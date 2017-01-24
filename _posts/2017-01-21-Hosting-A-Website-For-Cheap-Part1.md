---
layout: post
title:  "Hosting a Website for Cheap Part 1"
date:   2017-01-21 8:39:51 -0600
categories: jekyll, github, aws, route 53, github pages
permalink: hosting_for_cheap_part1
---

## Intro

Building and hosting websites have come a long way over the years.  There are so many options, that it can be a little daunting starting out.  I'm going to provide a solution for those seeking to build a simple static website that can be used as a blog, portfolio, or what have you using a variety of tools.  In a series of posts, I'm going to outline how I put together this website and how I host my email for ~$0.53 per month.  

It's pretty outrageous actually.  Not long ago, I was ashamingly paying $5 per month for DNS and $5 per month for virtual server hosting and that's actually pretty good!  Now I only pay for DNS hosting and requests using Route 53 from Amazon.

Let's actually break down what I get now versus $10 per month paying before.  For $0.53 per month, I have a scalable website that can grow at demand with zero intervention or labor on my behalf.  Free https support enabled on this website where I do not have to renew any certificates for.  I have a free custom domain email address where I can generously send and receive way more emails than I will ever need.  Now I could cut the costs to $0, but that would take away any custom domain names I could assign to website and email hosting.  A very small price to pay.

Interested?  Let's dive into the real meat.  We are going to start from the ground up on how to get Jekyll going on our local machine.

## Linux Installation

I will be using [Xubuntu-16.10](http://mirror.us.leaseweb.net/ubuntu-cdimage/xubuntu/releases/16.10/release/) for now on.  Open up a terminal and install the following software packages with:

{% highlight bash %}
sudo apt-get install ruby2.3
{% endhighlight %}

