---
title: How To Use Web Fonts In blogdown
author: TC
date: '2018-02-15'
slug: how-to-use-web-fonts-in-blogdown
categories:
  - trivial
tags:
  - blogdown
  - hugo
---

<link href='https://fonts.googleapis.com/css?family=Sofia' rel='stylesheet'>

There are several ways to set font types in your blogdown site:

- Using web-safe fonts

- Using web fonts, you should provide the font file by yourself.

Font files for chinese are usually large so web font is not an option. But english fonts are fine.

In the rest of the post I'll demonstrate:

- how to embed a ttf font into a blogdown website.

- use google font.

## Results:

---

### I am in spin_cycle

#### ABCDEFGHIJKLMNOPQRSTUVWXYZ

---
## Web fonts

- Download the .ttf(or whatever it is) font file, put it under `static` directory
- In your css, add `@font-face` and set `font-family` in the class you wanna apply, done.

your css should look like:

```
@font-face {
  font-family: "spin_cycle";
  src: url("/spin_cycle.ttf");
}
body {
  font-family:  "spin_cycle"
}

```

Take a look at my repo for a example:
- [css](https://github.com/rbind/blogsite/blob/master/static/css/fonts.css)
- [font file](https://github.com/rbind/blogsite/tree/master/static)

## Google fonts

- use @import to include the google font in your css, note that @import should go first in the file.


your css should look like:

```
@import url(https://fonts.googleapis.com/css?family=Open+Sans);

body{
   font-family: 'Open Sans',serif;
}
``` 
