---
layout: post 
title: About
repository_url: http://github.com/dilawar/sniffer
---

## {{ page.title }} 

In following image, each node is a student, each edge shows how much copy has
been done between two students. Thicker the edge, larger the copy. There are \\(n\\)
files matching if there are \\(n\\) edges between two students. 

![Plagiarism in code]({{ site.url }}/images/copy_all.jpg).

This application is intended to use to check plagiarism in assignments. It has
some capabilities to check copying in pdf files also.

This is poor man [MOSS](http://theory.stanford.edu/~aiken/moss/). It is perhaps
not as fast as MOSS but I have great success with it as a teching assistant.

## Installation

You can install it using `python-setuptools`. It is also available on `pypi`. To
install, do

    $ pip install code-sniffer 

If you are behind proxy, check out how to use `pip` behind proxy. You can also
download the code from its [gihub repository]({{page.repository_url}}). Run the
following command

    $ python setup.py build 
    $ sudo python setup.py install 

Any of these two method will install code-sniffer to your system

## How to use it

First you need to create a configuration file `~/.config/sniffer/config`. You
can see a [sample file here]({{ page.repository_url }}/master/blob/snifferrc).
If you choose to save this file at some other location, you need to specify the
location using `--config` option at command line e.g.

    $ code-sniffer --config ~/.snifferrc 


