---
title: tabletest
author: tc
date: '2019-03-28'
slug: tabletest
categories:
  - markdown
tags:
  - r-markdown
---




```r
library(ggplot2)

ggplot(mtcars,aes(x = mpg , y =cyl)) + 
  geom_point()+
  facet_grid(gear ~ . )+
  # ggtitle("test")+
  labs(title="test")+theme(plot.title = element_text())
```

<img src="/post/2019-03-28-tabletest_files/figure-html/unnamed-chunk-1-1.png" width="672" />


