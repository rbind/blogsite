---
title: Create a gif screencast, a bash script
author: TC
date: '2017-10-20'
slug: create-a-gif-screencast-a-bash-script
categories:
  - useless
tags:
  - ffmpeg
  - slop
  - useless things
---

## CLI is COOL!

It all started with this great post:
[GIF screencasting; the UNIX way](https://unix.stackexchange.com/questions/113695/gif-screencasting-the-unix-way)

what the expected result is like this:

![](https://i.stack.imgur.com/VEeSx.gif)

like this:

![](https://i.stack.imgur.com/Qqmg6.gif)

And like this: 

![](https://github.com/lolilolicon/FFcast/wiki/i/trimcombo.gif)

## What's that?

Well, it's a bash script. What it does is simply amazing: select a region, and turn it into a high quality gif. 

In the back:

- it let's you select a region with your mouse, done by xrectsel
- it records the region into a video, done by ffmpeg
- turn it into a gif with convert from ImageMagick, optimized to save space.

However, xrectsel doesn't work well in my distro(Ubuntu 16.04LTS). 

So I made some modifications and replaced xrectsel with [slop](https://github.com/naelstrof/slop) ^[for ffmpeg, i use sudo apt-get; for slop, it seems for other distro to be possible to install with package manager, but in ubuntu 16.04, some dependencies needs to be installed manually https://github.com/naelstrof/slop/issues/52].

Sooo here's what I get:

![Imgur](/img/out.gif)

[Here is the little script](https://gist.github.com/tcgriffith/ae18d49dc97b7d29e2e3fcc22f1f5e09):

```bash
#!/bin/bash

read -r X Y W H G ID < <(slop -f "%x %y %w %h %g %i")
TMP_AVI=$(mktemp /tmp/outXXXXXXXXXX.avi)

ffmpeg -s "$W"x"$H" -y -f x11grab -i :0.0+$X,$Y -vcodec huffyuv -r 25 $TMP_AVI \
&& convert -set delay 5 -layers Optimize $TMP_AVI ./out.gif 
```


***

I find that imgur will transform uploaded gif into mp4 again...

here is what I got from them:

<video autoplay="" loop="" class="" style="max-width: 100%; min-height: 455px;"><source type="video/mp4" src="//i.imgur.com/UREOakJ.mp4"></video>

compared with the source file
1.avi 591.7MB 
1.gif 17.4MB
1.mp4 4.8MB

imgur surely did a great job on improving the network traffic!

