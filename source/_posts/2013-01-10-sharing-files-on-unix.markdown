---
layout: post
title: "Sharing Files On Unix"
date: 2013-01-10 13:16
comments: true
categories: 
---

Here's a task I've had to do many times and I'm always looking one or two (or
all) of the commands up on the interwebz.

<a href="http://www.flickr.com/photos/emrank/3291247985/" title="Sharing is caring - Oasis 21 by emrank, on Flickr"><img src="http://farm4.staticflickr.com/3196/3291247985_e1206ab814_m.jpg" width="180" height="240" alt="Sharing is caring - Oasis 21"></a>

How to setup file sharing between two unix users.

<!-- more -->

```
    $ groupadd new_group

    # add both users to the new group  
    $ sudouseradd -G new_group user1
    $ sudouseradd -G new_group user2

    # update the folder's group to be the new_group and make it sticky
    $ chgrp -R new_group folder_to_share
    $ chmod g+w folder_to_share
    $ chmod g+s folder_to_share

    # verify the umask setting for the user ensures group files are readable (this is normally the default)
```
