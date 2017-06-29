---
layout: post
title:  "TODO"
date:   2017-06-29 13:10:00 -0600
categories: how, to, install, jekyll, xubuntu, ubuntu
permalink: installing_jekyll_xubuntu
---

## Installation

Ubuntu repo as of this date uses less than Ruby2.  So we will have to retrieve from Ruby website the latest and setup our operation system environment.

Install Ruby higher than 2.1 from https://www.ruby-lang.org/en/downloads/

**Using 2.4.1 for this tutorial.**

```bash
cd ~
wget https://cache.ruby-lang.org/pub/ruby/2.4/ruby-2.4.1.tar.gz
tar -xzvf ruby-2.4.1.tar.gz
rm ruby-2.4.1.tar.gz
```

Now to configure default settings and install.

```bash
cd ~/ruby-2.4.1
./configure
sudo make install
```

Hopefully all is well at this point.  If using a different Xubuntu or Ubuntu version, you may have to install a bajillion dependencies.  Good luck on your internet search results!

The ruby source version will be installed in /usr/local/lib/ruby by default

Time to install Jekyll and dependencies.  Installing Jekyll 3.5.0 as of this writing.

```bash
sudo gem install jekyll bundler minima jekyll-feed
```

## Running Jekyll

To test out the default jekyll website by creating one...

```bash
mkdir my_jekyll_website
cd my_jekyll_website
jekyll new .
```

If error messages appear, install the missing gems it requires until you finally see that the new jekyll site is installed.


To see our default Jekyll website

```bash
jekyll s
```

Open up a web browser and go to localhost:4000

