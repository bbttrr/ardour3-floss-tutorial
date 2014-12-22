---
layout: post
title: "Saving a Session"
description:
comments: false 
tags: [06 SAVING SESSIONS]
image:
  feature: Ardour3_Empty_Session_Transparent.png
  credit:  
  creditlink:  
---

There are a number of ways to save Sessions in Ardour, so that each
Session can be use later on. The simplest way is to save the entire
Session just like you would save other documents: hitting "Control" + "S".

A new Session is first saved at the moment you create it. While you are working on it, you should save it
frequently. Get into the habit of hitting *"Control"* + *"S"* (or *"Command"* + *"S"* on a Mac) every few minutes.

> TIP: Avoid using any characters other than letters and numbers when naming your session. Avoid white spaces, accented letters, !@#$%*()+, periods, commas, etc. Use dashes or underscores if you like. For example, instead of "My Great Session!", prefer "My_Great_Session", or "MyGreatSession", or "my-great-session". Instead of "Açaí", write "Acai" (without accented letters), etc. Once you have created your Ardour session, do **not** manually rename any folders or files that belong to the Session.

## Ardour File and Folder Format

The contents of a typical Session's folder on your hard drive might look something like
this:

![Ardour Folder](../images/Ardour3_Session_Folder_Structure.png)

A bit of information about some of the components inside that folder:

* The name of this Session is "*my_session*".
* The main session file is called "*my_session.ardour*". The Session file is periodically backed up by Ardour with a *.bak* extension.
* The *.history* file keeps a record of changes you have made during your Session, and is also periodically backed up.
* The *interchange* folder contains the actual audio data of all the Regions used in your Session.
* The *export* folder is where exported files are saved by default.

> TIP: If double-clicking on the session file does not launch Ardour, use the standard method of first opening the application itself, then choosing a session from the Session Setup dialog.

![Ardour Opening](../images/Ardour3_Session_Setup_Dialog.png)

## Continuing

Saving an entire Session allows you to open it again at a later time.
However, if you would like to preserve a certain state that your Session
is in, to be able to return to that state later on after you have made
changes, then please continue to the next session called **Saving 
a Snapshot**. 

Next: [SAVING A SNAPSHOT](../saving-a-snapshot)
