---
title: import rules
author: tc
date: '2018-05-23'
slug: import-rules
categories:
  - blogdown
tags:
  - blogdown
  - css
---

I've used xaringan to do slides for a few months, and one thing bugs me is that all those google fonts imported are missing.  

Then I found out that netlify likes to bundle and minify css files for you.
But [@import rules must be at the top of a css](https://www.w3schools.com/cssref/pr_import_rule.asp)  

Turns out scrashing your css files into one is a bad idea.  
