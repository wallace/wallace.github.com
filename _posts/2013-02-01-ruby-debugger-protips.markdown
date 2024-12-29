---
layout: post
title: "ruby debugger protips"
date: 2013-02-01 22:05
comments: true
categories: 
---

I've been a big fan of debuggers ever since my first gig, an internship with
Cisco Systems in 2000, where I became very familiar with
[gdb](http://www.gnu.org/software/gdb/).

But I've had my complaints about the state of debugging in ruby.  Read on to
find how I've put my foot in my mouth.

<a href="http://www.flickr.com/photos/charlottemorrall/3850109985/" title="Foot in mouth by {Charlotte.Morrall}, on Flickr"><img src="http://farm3.staticflickr.com/2436/3850109985_ec24eef5f3_m.jpg" width="240" height="163" alt="Foot in mouth"></a>

<!-- more -->

I covered the basics in a [previous blog post](http://blog.bignerdranch.com/1565-debugging-best-practices/) but one thing I've not stopped complaining about is the lack of debugger sessions.  And by that I mean the ability to save a set of break points in a running process, quit that process, and restart it again restoring the previous break points and watches.

[ruby-debug19 is abandonware](https://github.com/cldwalker/debugger#reason-for-fork) and [debugger](https://github.com/cldwalker/debugger) has taken over.  I was all set to dive into the source to determine how to hack in this functionality but imagine my surprise when I found its already available!  Checkout ```save``` and ```source```.

{% gist 4696064 %}

Oh man, do I ever love open source.
