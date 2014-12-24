---
layout: post
title: "Saving a Snapshot"
description:
comments: false 
tags: [06 SAVING SESSIONS]
image:
  feature: Ardour3_Empty_Session_Transparent.png
  credit:  
  creditlink:  
---

Saving a **Snapshot** in Ardour is similar to saving your Session to a
new file, however using a Snapshot avoids overwriting the original
Session file. A Snapshot contains the current state of your work, while
sharing all the audio and data files of the Session.

## Saving a Snapshot

You can save a Snapshot via the menu: *Session > Snapshot* (shortcut "*Control*" + "*Shift*" + "*S*").

![snapshots]({{ site.url }}/images/Ardour3_Snapshots1.png)

By default the program will name the new Snapshot according to the
current date and timestamp of your system. If you wish, you can change
the name to one that more meaningfully corresponds to the Session you
are working on.

## Recalling Snapshots

You can recall a saved Snapshot via the '*Snapshots*' tab in the area on
the right:

![snapshot2]({{ site.url }}/images/Ardour3_Snapshot2.png)

There you see a few Snapshots that we created, and the '*my_session*' entry
represents the original state of our session.

Double-click on any Snapshot from the list to reload it.

## Continuing

Sometimes it is helpful to have a default starting point for new
Sessions, for example for a set-up that you use all the time when starting a new project. To learn how
to do this, please continue to the next session called **Saving a Template**. 

Next: [SAVING A TEMPLATE](../saving-a-template)

