---
layout: post
title: "Octopress love; twitter update"
date: 2013-09-21 16:12
comments: true
categories: 
---

Tweets in the sidebar for your health!

<a href="http://www.flickr.com/photos/ken_c_lo/8097545949/" title="octopress by ken_c_lo, on Flickr"><img src="http://farm9.staticflickr.com/8335/8097545949_7d3cb17900_m.jpg" width="240" height="73" alt="octopress"></a>

<!-- more -->

I have finally addressed the lack of tweets in the sidebar.

A goodly open source contributer [created a pull request](https://github.com/imathis/octopress/pull/1311) that updates the octopress twitter aside to [handle twitter's API changes](https://dev.twitter.com/blog/api-v1-is-retired).

You have to [create your own twitter widget](https://twitter.com/settings/widgets) and extract the data-widget-id.

<img src="http://note.io/17Shlyn" />

[Drop that widget id into your _config.yml file.](https://github.com/wallace/wallace.github.com/commit/91d97778feaba757e867fbd39fb912f7b947555e)

I've also ported that fix over to the
[justin-kelly-theme](https://github.com/wallace/justin-kelly-theme/commit/5d84658bcc74adfee974cdbd2c4e64ec90b0baf1)
too. You'll want to remove the old justin-kelly-theme and reinstall it.

```
$ rm -rf .themes/justin-kelly-theme/
$ bundle exec rake install['justin-kelly-theme']
```
