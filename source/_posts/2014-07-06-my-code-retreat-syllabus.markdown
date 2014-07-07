---
layout: post
title: "my code retreat syllabus"
date: 2014-07-06 21:39
comments: true
categories: 
---

You may have heard about [my adventures](/blog/2013/07/04/quick-recap/index.html) with [code retreats](/blog/2014/06/12/year-in-review/index.html). I greatly enjoy facilitating and participating and over the years I've come up with a base itinerary. You can find the official structure [here](http://coderetreat.org/facilitating/structure-of-a-coderetreat). This is more of my specific predilections. The day won't follow this exactly and will vary according to skill level and participants interest but read on to see what I enjoy.

<a href="https://www.flickr.com/photos/auteurdecinema/6157383349" title="Self-improvement in progress! by Kenneth Law, on Flickr"><img src="https://farm7.staticflickr.com/6199/6157383349_77ef7d33dd_m.jpg" width="240" height="240" alt="Self-improvement in progress!"></a>

<!-- more -->

1. Breakfast (8am) 
    The start of any good day begins with a good breakfast. I open the doors to the location around 8am for the early risers. 

1. Introduction (~ 8:30am)
    The first thing I do is introduce myself. Then I'll
      * talk about the itinerary of the day and the purpose of the code retreat. The importance of coding without pressure and seeking only to practice and improve.
      * Talk about the difference between perfection and reality (the how much we suck gap).
      * Talk about the 4 rules of simple design.
         * Passing tests.
         * Good names (reveal intent).
         * DRY - Don't repeat yourself (not just code but more imporant, concepts).
         * Small. Methods, classes, parameters lists, etc.
      * Encourage people to pair with others of different skill levels and platforms and the importance of communication and collaboration.
      * Introduce GoL.

1. 1st session (~ 9am)
    Let people pair up and practice on the problem.
    Review the approaches used.
    Help the group reflect on what was done, why and the limitations of the approaches chosen.
    Remind them of the problem constraints, "infinite grid".

1. 2nd session (~ 10am)
    Ping pong TDD.

1. 3rd session (~ 11am)
    Mute ping pong TDD (remind them to speak only about language details if they don't know the language they've agreed upon, not implementation questions)

1. Lunch break (~ 12pm)

1. 4th session (~ 1:30pm)
    No loops, no if statements (secretly forcing functional programming paradigms and moving away from array based solutions)

    At this point, take stock of the groups energy level. Determine by asking them whether they're up for one or two more sessions. Also by examining the excitement level in the room. If they're tired and interest is waning, I'll make the 5th session the last one. No one is at events like this for punishment purposes. :)

    For the last session, I encourage people to have the freedom to make their own choices, no constraints.

1. 5th session (~ 2:30pm)
     I often like to pretend that this session has no constriants only to stop them about 15-25 minutes in and add a constraint. Assuming this is the 2nd to last session, the constraint will be add a third state to a cell. You now have live, dying and dead cells. It now takes two ticks for a cell to die but once it starts dying it will die no matter what the generation after the next. While it is alive, it is considered alive for evaluating the state of other neighboring cells.

1. 6th session (~ 3:30pm)
    Pair up with no constraints. About 15-25 minutes in, ask everyone to switch stations/ computers. In other words, you start with your own code base as a pair and finish with someone else's. It doesn't matter if you know the language or not, that's part of the fun. I call these last two sessions consultant sessions as they mimic what happens with a consultant. 5th session is changing requirements. 6th session is rescue code.

1. Closing circle: Here's where we recap and give everyone a chance to share three things.
    * What're you going to do differently going forward?
    * What most surprised you?
    * What did you learn?




There's lots of other session idea out there too. Check out [the code retreat website for more.](http://coderetreat.org/facilitating/activity-catalog)
