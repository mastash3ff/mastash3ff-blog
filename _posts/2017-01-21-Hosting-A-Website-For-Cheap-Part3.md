---
layout: post
title:  "Hosting a Website for Cheap Part 1"
date:   2017-01-23
categories: jekyll, github, aws, route 53, github pages
---

In a series of posts, I'm going to outline how I put together this website and how I host my email for ~$0.53 per month.

Building and hosting websites have come a long way over the years.  There are so many options, that it can be a little daunting starting out.  I'm going to provide a solution for those seeking to build a simple static website that can be used as a blog, portfolio, or what have you using a variety of tools.

It's pretty outrageous actually.  Not long ago, I was ashamingly paying $5 per month for DNS and $5 per month for virtual server hosting and that's actually pretty good!  Now I only pay for DNS hosting and requests using Route 53 from Amazon.

For that $0.53, I have a scalable website that can grow at demand with zero intervention or labor on my behalf.  Free https support enabled on this website where I do not have to renew any certificates for.  I have a free custom domain email address where I can generously send and receive way more emails than I will actually ever need.  I could cut the costs to $0 but that would take away any custom domain names I could assign to website and email hosting.  A very small price to pay.



{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
