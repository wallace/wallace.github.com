---
layout: post
title: "Weechat Bliss"
date: 2013-02-13 18:11
comments: true
categories: 
---

Back in [Weechat Karmageddon](http://blog.jonathanrwallace.com/blog/2013/01/17/weechat-karmageddon/), I spoke about a script I wrote to make giving hubot karma easy-peasy.  In this post, we'll talk about the rest of my weechat setup.

<a href="http://www.flickr.com/photos/superfantastic/50088733/" title="Buddha dog by SuperFantastic, on Flickr"><img src="http://farm1.staticflickr.com/32/50088733_58935531ce_m.jpg" width="240" height="160" alt="Buddha dog"></a>

<!-- more -->

## Overview

Weechat has two main ways to extend its stock functionality, scripts and plugins. Plugins are C programs that are dynamically loaded. Writing C programs to extend my IRC client is more work than I care for so I stick to scripts.

Since I use scripts from perl, python and ruby I make sure to install weechat with support for those languages.

```$ brew install weechat --ruby --python --perl```

## Scripts

Here's a quick list of scripts that I use regularly:

- [weechat-notification-center-rb](https://github.com/wallace/weechat-notification-center-rb) -- notifies you in Mac OS X Notification center
- [weechat-nerdbot-karma](https://github.com/wallace/weechat-nerdbot-karma) -- bestows karma, nerdbot style
- [buffers.pl](http://www.weechat.org/scripts/source/buffers.pl.html/) -- lists your current buffers
- [urlgrab.py](http://www.weechat.org/scripts/source/urlgrab.py.html/) -- quickly open up links of the cat images shared by coworkers

Once weechat has started, you may type ```/script help``` to get an interactive script manager.  Unofficial scripts will not be listed in the interactive script manager so you'll need to follow the installation instructions for [weechat-notification-center-rb](https://github.com/wallace/weechat-notification-center-rb) and [weechat-nerdbot-karma](https://github.com/wallace/weechat-nerdbot-karma).

## Startup

I currently run camper_van as a proxy to my work campfire rooms, so I run campfire in one terminal and then I set up a [custom profile with a handy shortcut and startup command in iTerm2 to start up weechat](https://www.evernote.com/shard/s2/sh/c42cd246-a62e-481f-abbe-883983ac1016/794e8070a80d96a8b0f2bdf9c2320dc9/res/84d089e9-0852-49c2-b3e6-2150411b51b6/skitch.png).  

## Configuration

Here's an example irc.conf for weechat.

{% gist 4949912 %}

I had to make a slight modification to how urlgrab worked so here's my urlgrab.conf file.  I believe it was adding quotes around %s for localcmd.

{% gist 4949942 %}

## Usage

I switch buffers with ```/b <buffer number```.  I bestow karma via ```/karma <name> <amount>```.  And examining urls is a snap with ```/url <ordinal position of url most recent first>``` e.g., ```/url 1``` opens up the most recent url in the current buffer.

## Coming up

You may look forward to what I had to do to install camper_van (war story!) and another plugin to start camper_van in the background as a hook_process on weechat so there's no need to run camper_van in its own terminal.

