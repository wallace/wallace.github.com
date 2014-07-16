---
layout: post
title: "my first haskell"
date: 2014-07-15 15:18
comments: true
categories: 
---

Last week I shared my [secrets to an amazing code retreat](/blog/2014/07/06/my-code-retreat-syllabus/index.html). Since then [Big Nerd Ranch](http://bignerdranch.com) held an internal code retreat (thanks [Stafford](https://twitter.com/srbiv)) and although I was only able to participate for a couple of sessions due to client work, I learned a couple of things and got to play with a new language. Can you guess which one?!? Read on to found out.

<a href="https://www.flickr.com/photos/rockandracehorses/3783326324" title="Born To Run! Rachel Alexandra and Calvin Borel win the $1.25 million Haskell Invitational by Sarah K. Andrew, on Flickr"><img src="https://farm4.staticflickr.com/3110/3783326324_154fe1441d_m.jpg" width="240" height="180" alt="Born To Run! Rachel Alexandra and Calvin Borel win the $1.25 million Haskell Invitational"></a>

<!-- more -->

Though I've stated many times how valuable I find code retreats to be, I'm still impressed at how I continue to learn at a consistent rate each time I attend or facilitate. Lucky for me, this time I was able to participate which is so much fun.

I had three experiences that I'd like to share.

1. Way way back when, I shared [what I learned at my first code retreat](http://www.bignerdranch.com/blog/lessons-learned-at-global-day-of-coderetreat/). Knowing how equality works in Ruby is a little tricky and understanding the importance of the hash and eql methods is key. But you can also get away with using the Comparable module (thanks [Steven Harman](http://stevenharman.net/)).

{% gist 4a0d0f0403a2b85b383f point.rb %}

1. As I mentioned above, I only experienced two full sessions. I was interuppted in the third session where we were constrained to using mute ping-pong TDD. But what was interesting is how in the few minutes we did share, I started with a full integration test. This stumped my partner. And to be honest, it was a little unfair as there's no way he could write a passing test without resorting to some nefarious behaviors. I later found out that we weren't the only ones who found starting with a high level integration test challenging when we weren't able to vocally coordinate with our partner. There's got to be some profound insight related to documentation, abstraction and code rot over time.

1. Finally, what I'm most excited about is that I was able to pair with [Bree Stanwyck](https://twitter.com/letsbreelhere) and we used Haskell. This was the first time I was exposed to Haskell other than via a presentation and we managed, with tests, to get a [functioning Haskell GoL implementation](https://gist.github.com/breestanwyck/479faa4a274f7278b5fb) within the session. I was very impressed with Haskell and look forward to exploring it more in the near future. The elegance and simplicity allows the intent of the GoL algorithm to shine through. 


For my next step, I'm planning on working through [http://learnyouahaskell.com/](http://learnyouahaskell.com/).
