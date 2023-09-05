---
title: Differences of Rmd/Rmarkdown/md in blogdown
author: TC
date: '2019-02-21'
slug: differences-of-rmd-rmarkdown-md-in-blogdown
categories:
  - blogdown
  - hugo
tags:
  - blogdown
---

> Too many options is a curse.

Today there's a related [Github issue](https://github.com/rstudio/blogdown/issues/358) that spurs some interesting discussion regarding the different options in blogdown. In particular, the three different format(Rmd/Rmarkdown/md) when writing a blogdown post.

In fact, the differences I'm going to discuss reflect the differences between two markdown processors with different "extended" features. One processor is [pandoc](https://pandoc.org/), which works under the hood of most yihui's Rmarkdown packages. The other processor is
[blackfriday](https://github.com/russross/blackfriday) used by hugo.



