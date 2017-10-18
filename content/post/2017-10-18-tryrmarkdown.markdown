---
title: tryrmarkdown
author: tc
date: '2017-10-18'
slug: tryrmarkdown
categories:
  - r
tags:
  - blogdown
  - r-markdown
draft: true
---

## aaa






```r
strip_head <- function(filepath){
  lines <- readLines(filepath)
  message(lines[1])
  tmp <- which(lines %>% grepl("---",.))[1:2]
  start <- tmp[1] + 1
  end <- tmp[2] - 1
  message(start)
  message(end)
  headerlines <-lines[start:end]
  return(yaml::yaml.load(paste0(headerlines,collapse = "\n")))
}
```


```r
gettitle <- function(lines){
  title <- grep("title:(.*)$",tmp2,value = TRUE)[1] %>% gsub("title:","",.) %>% stringr::str_trim()
}
```



