---
layout: post
title: "bugs be gone"
date: 2013-01-07 21:19
comments: true
categories: 
---

NO MOAR BUGZ!  One down, an infinite more to go.  

<a href="http://www.flickr.com/photos/staflo/7697379948/" title="fly session by staflo, on Flickr"><img src="http://farm8.staticflickr.com/7261/7697379948_59b2b0d828_m.jpg" width="240" height="240" alt="fly session"></a>

<!-- more -->

At [Big Nerd Ranch](http://bignerdranch.com), many of us use [campfire](http://campfirenow.com/).  And many of us also use [IRC](http://en.wikipedia.org/wiki/Internet_Relay_Chat).  We also dislike having unnecessary programs running so when we found [camper_van](https://github.com/aniero/camper_van) we got excited.

Unfortunately, we found a [bug](https://github.com/aniero/camper_van/issues/22).
But no longer fear, the bug has been [cleared](https://github.com/aniero/camper_van/pull/23).

In fact, if you can't wait for the pull request to be accepted and a new version
to be released you can do the following:

```
    $ gem install specific_location
    $ gem specific_install -l https://github.com/bignerdranch/camper_van.git
```

Enjoy!
