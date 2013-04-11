---
layout: post
title: "Living in a camper_van down by the river"
date: 2012-12-05 16:26
comments: true
categories: 
published: false
---

<a href="http://www.youtube.com/watch?v=3nhgfjrKi0o">Not that type of van</a>

At [Highgroove Studios](http://www.highgroove.com), we used
[campfire](http://campfirenow.com) as our primary chat tool and I specifically
used [propane](http://propaneapp.com/).  Propane worked great but since merging
with [Big Nerd Ranch](http://www.bignerdranch.com), we also use IRC.  Having too
many programs open is annoying so a while back [Andy
Lindeman](http://alindeman.github.com/) spearheaded using
[camper_van](https://github.com/aniero/camper_van) as a campfire bridge.

Today, I finally started shaving this yak while waiting for tests to complete
and I ran into a strange issue.

~ ruby-1.9.3 $ camper_van
2012-12-05 15:32:28   932  INFO CamperVan : starting server on 127.0.0.1:6667
2012-12-05 15:32:33   932  INFO CamperVan : got connection from 127.0.0.1
2012-12-05 15:32:33   932  INFO CamperVan : performing request to https://bignerdranch.campfirenow.com/users/me.json
dyld: lazy symbol binding failed: Symbol not found: _yajl_set_static_value
  Referenced from: /Users/jonathanwallace/.rvm/gems/ruby-1.9.3-p194/gems/yajl-ruby-0.7.9/ext/yajl/yajl.bundle
  Expected in: flat namespace

dyld: Symbol not found: _yajl_set_static_value
  Referenced from: /Users/jonathanwallace/.rvm/gems/ruby-1.9.3-p194/gems/yajl-ruby-0.7.9/ext/yajl/yajl.bundle
  Expected in: flat namespace

Trace/BPT trap: 5

With the help of [Jeremy W. Sherman](), I tracked down

https://github.com/aniero/camper_van/issues/20
which leads to 
https://github.com/defunkt/resque/issues/600
which leads to
https://github.com/defunkt/resque/issues/600#issuecomment-9315183

short answer, rebuild ruby with gcc instead of clang and it'll work

or you can edit the gem directly, http://tom.meinlschmidt.org/2011/11/01/cucumber-yajl-troubles-osx-lion/

http://clang.llvm.org/compatibility.html#inline

https://github.com/brianmario/yajl-ruby
