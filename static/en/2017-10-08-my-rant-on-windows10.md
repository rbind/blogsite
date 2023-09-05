---
title: my rant on windows10
author: TC
date: '2017-10-08'
slug: my-rant-on-windows10
categories:
  - trivial
tags:
  - OS
  - windows
  - rant
---

## windows10 is horrific to use

I use Ubuntu 16.04 on my laptop for my daily work. Windows 10 sits in my other laptop to run entertainment-related stuff, like steam games.

But my experience with windows 10 is so terrible that I've decided to dedicate this post to it.

## Confusing and hard-to-use configurations

Today, I need to set the shortcut for toggling between input methods. In Ubuntu, I set F12 for this function, because there's no chance that I hit it by accident.

- I started by looking around in windows settings
- randomly clicked millions of links, options, nothing near what I expected. I spent 5 minutes roaming around without any clue where I should be looking at.
- Shit I have to Google it in the end.
- *Googling*
- And it turned out to be in the CONTROL PANEL BURRIED DEEP DOWN IN SOME KIND OF ADVANCED SETTINGS IN THE SECOND PAGE, GOTCHA YOU LITTLE SHIT!
- And you have to choose between `ctrl+ alt`, `alt+ shift` and "`", nothing more?!! Why can't I set F12 for toggling? Is it too difficult to implement? Why can the Ubuntu guys do it??

In summary, configurations is a nightmare in windows, even though I have used windows for more than 13 years, these nasty settings are always difficult to find without googling ~~the shit out of SO~~

And when you finally find it ~~with a great amount of luck~~, you will probably be provided with limited options that reads at you:

> "NO YOU CAN'T DO THIS BECAUSE I SAY SO."
> - MS [in sunglasses]

![](http://www.buffalo.edu/~skim25/lis506-2/meme/meme08.jpg)

## Personal preferences are randomly changed during updates

Really? MS? Really? 

I have 3 input methods installed for English, Chinese and Japanese. The shortcut for switching between them was, and had always been, `WIN+SPACE`. I've been using this for more than a year and were get used to it.

ALL OF A SUDDEN WINDOWS SOMEHOW CHANGED IT TO `ALT+SHIFT`. REALLY? MS? REALLY?

I smashed my old shortcut and nothing happened as expected in the past WHOLE YEAR!
I had to googled how to set these switch shortcut

![](https://media.giphy.com/media/12XMGIWtrHBl5e/giphy.gif)

WHY?
WHAT DID I DO?
WHAT HAPPENED?

## Do we need superfetch that takes up 99% of your ram all the time?

Another day I noticed that in my task manager,  my memory usage and disk usage stay at 99% while I was not running any resource-hungry programs.

I googled and found that superfetch caused this. Basically, superfetch preload "frequently used" data into the memory so that users can get the data immediately when requested. But as SSD gets popular, this mechanism seems obsolete, improved little.

I disabled it and memory usage went back to normal.^[By the way, the disk usage is because of Geforce experience that "WOULD LIKE TO SCAN EVERY SINGLE FILE UNDER MY STEAM DIRECTORY EVERY TIME I REBOOT", which is also stupid.]

ALSO, I hate it when MS decided to use my computer resources to do some preloading work for what they "predicted" me doing.

STOP ASSUMING YOU KNOW WHAT I WOULD LIKE TO DO WITH MY COMPUTER! MICROSOFT YOU LITTLE SHIT!

![](https://i.imgur.com/sgTanck.gif)

## STUPID shortcuts

---

(update 2017-10-11 21:44)STUPID shortcuts



In r studio, `ctrl+alt+i` inserts an R code chunk in the rmarkdown file.

Guess what I got in windows 10?

A FUCKING "í"

![](https://i.imgur.com/jeWT0ta.gif)

--- 

(update 2017-10-13 15:42)

Actually I found out that my keyboard ended up being USA international, which explains why these strange shortcuts for accented letters. switching to US keyboard fixed it.


## terrible terminals

So there are two types of ecosystems for operating system: windows, and the others^[mac and Linux are somewhat similar].

They differ in various ways, but missing a handy terminal really makes windows unbearable.

Especially when you've tasted the pleasure and convenience of terminals in Ubuntu.

- You can `find -name *md |xargs egrep "TP53"` to find related documents related with a keyword.

- You can `sudo apt-get install git` to install a software without googling online, downloading the installer bundled with millions of malwares. and always keep the software up-to-date.

- You can call `subl .` to call up sublime3 and open up current fold. 
- You can `rsync` 

- If there are more than 3 files you need to repeat operations on, such as rename, move, search text keywords and stuff, I would rather die than manually doing them by clicking my mouses all around a file folder. GIVE ME A FUCKING SH TERMINAL

- OK windows has a command prompt, or power shell, or GIT GUI if you installed that shit. but they are really difficult to use because you are basically stopped by the tedious unbearable procedures for setting up environment variables: PATH, LIB_PATH, R_LIB and stuff. 

- AAAAAND, you can't even doing them in the terminal? SO WHAT'S THE POINT OF USING A TERMINAL IN WINDOWS IF YOU CAN'T FINISH JOBS AS SIMPLE AS SETTING THE PATH?



