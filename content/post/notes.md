---
title: "My first post"
author: "TC"
date: '2017-04-27'
slug: my-first-post
tags:
  - trivial
categories:
  - trivial
draft: true
---


## A good cmake tutorial:

https://medium.com/@onur.dundar1/cmake-tutorial-585dd180109b

## regex

replace _ to - in all files

```
sed -i -E "s+(^slug.*)_(.*)_(.*$)+\1-\2-\3+" *md
```
explanation:
-i: inplace edit
-E: extended regex



