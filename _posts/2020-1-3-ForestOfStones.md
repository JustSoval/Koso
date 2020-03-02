---
layout: post
title:  "Forest of stones"
image:  /img/ForestOfStonesCoverArt.png
tags: ["projects", "software"]
---

# Forest of stones

<p>&nbsp;</p>
<img src="/img/ForestOfStonesCoverArt.png" alt="Cover art" style="width:100%;"/>
<p>&nbsp;</p>

Forest of stones is a 2d mobile game built with unity. This was a major stepping stone in my design and software development journey. This project taught me to use c#, json files, character animation, particle effects, and unity to produce what I feel is a sucessful project.

<p>&nbsp;</p>

#### The game breaking bug.

Close to the completion of my project, I found a bug which caused the play.c# script not to run on the first time running the game. This bug was caused by a failure to create the player save data json file on the first execution of the game. Once found, this bug was very easy to fix by checking for a json file, and creating one if none is found. However, it was very difficult to diagnose for a variety of reasons.

<p>&nbsp;</p>

##### Ambiguous error codes.
The only eror code thrown by this bug was

> NullReferenceException: Object reference not set to an instance of an object

This was caused by references to the player script not working, but it took me a while to realise this, and even then, the error provided no information about why the playerscript was not running.
