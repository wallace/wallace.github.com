---
layout: post
title: "Quickly create a Google hangout with Alfred"
date: 2013-10-08 20:40
comments: true
categories: 
---

At [Big Nerd Ranch](http://bignerdranch.com), we set up our [lita clone](https://github.com/jimmycuadra/lita) (a ruby based chat bot similar to [hubot](https://github.com/github/hubot)) so that it would generate Google hangout links for us that would allow us to quickly share the URL with a co-worker or client. But times, they be a changin'.

<a href="http://upload.wikimedia.org/wikipedia/commons/9/97/Barack_Obama_hangout.jpg" title="President Obama Google Hangout"><img src="http://upload.wikimedia.org/wikipedia/commons/9/97/Barack_Obama_hangout.jpg" width="240" height="73" alt="president_obama_google_hangout"></a>

<!-- more -->

Our bot functionality was ultimately based on a hack of Google hangout URLs...
which no longer works.

From [Jay](http://iamvery.com/)[Hayes](https://twitter.com/iamvery): 

> The "old" implementation of nerdbot hangouts depended on the fact that G+
> hangouts attached to events have static URLs. The "trick" was to create a G+
> event far in the future and copy the URL to the attached hangout to a list
> maintained in the Nerdbot's environment.
>
> Now it seems that G+ event hangout links expire just like "regular" hangouts
> after some time. :sob:

We have a few ideas floating around about how to recreate the bot functionality
but they are a bit involved. One of the key challenges is that you must be
authenticated with Google to request a hangout.

Today, I realized that [one of my favorite tools, Alfred,](http://blog.jonathanrwallace.com/blog/2013/02/02/quickr-flickr-search/)
should be able to help out.

A few shaved yaks later and :boom:, a [new alfred workflow for creating a google hangout](https://github.com/wallace/google_hangout_workflow). [Download it directly](https://github.com/wallace/google_hangout_workflow/raw/master/Google%20Hangout.alfredworkflow). Enjoy!
