---
title: learning python
author: tc
date: '2017-10-28'
slug: learning-python
categories:
  - notes
tags:
  - python
  - R
---

# Python looks fun

Recently I'm planning to learn python. Because I have came across a few incredible [packages](https://github.com/agermanidis/autosub/) or [scripts](https://github.com/Vespa314/bilibili-api) written in python. They look amazing and I think I'll definitively enjoy writing in python.

In addition, I've used bash, c, java before, and I'm becoming fluent in R in the last year. According to my previous experience, when you have learned one programming language, picking up another programming language should not be that hard. After all, the most part of them are the same core concepts implemented in a slightly different ways.

# My impression of other languages.

- c: As a intro course of my college, I didn't use c a lot besides finishing the course projects. What I remember of c is that **pointers** is really confusing to use. 
Recently I've heard from my supervisor (and others) that he use bash or python to manage the project, and use c to get jobs done fast.

- java: I used java for around 3 to 4 years during my master project back in labliu. The reason of using java is that the project was written in java when firstly launched. And this tradition was then carried on by the project's successors.
From java I learned how objective oriented programming works. 

- bash: bash scripts is a natural choice while I shifted from windows to ubuntu two years ago^[goodbye windows I won't miss you]. The thing I love bash a lot is that I can automatize my daily routines, put it in crontab and let my jobs done in the background. 

- R: R has becoming my daily driver for everything in the last one and a half year. The more I learn about R, the more I fond it.
Some might argue that R is "statistics oriented" language that specifically used in analyzing data. But I don't think so. There is literally "nothing" you can't do using R: Thanks to rstudio, knitr and r markdown that made the following jobs done in an elegant way:  
    - Professional academic reports
        - references  
        - cross-reference of figures& tables;
        - numbering of figures and tabs; 
        - auto-numbering chapter & sections;
        - code blocks; 
        - integration of R's outputs;
    - Reproducible notebook:
        - coding in R code chunks in an r markdown, record both results, analysis, description and outputs, and you can reproduce the results after 6 months.
    - Fancy [html5 slides](https://github.com/yihui/xaringan)
    - [Write books](https://bookdown.org/yihui/blogdown/)
    - Host your [personal blog](https://bookdown.org/yihui/blogdown/)
    - cran, bioconductor and github get your back!

And for Rstudio, I can't express how much I love this IDE: github integration, object viewer, package manager, wonderful editor, shortcuts, package management. Part of the reason I didn't go into python is that there's nothing like rstudio for python.

# Setup
My basic python environment setup is sublime text3 + bash terminal under ubuntu 16.04

I like to use sublime, so I tried [anaconda for sublime](http://damnwidget.github.io/anaconda/) which provides several handy utilities:

- view the docstring(like help in R) with Ctrl+alt+D

- jump to definition (really handy!) by putting cursor on the function name

- auto completion

Well that's already good enough for me.

some useful shortcuts:

- ctrl+alt+g goto definition
- ctrl+alt+d docstring
-


# Notes of an useR during learning python:

- Start by reading[A byte of python](https://python.swaroopch.com/control_flow.html), it's simple and well explained and has a lot of useful notes for c/c++ users.

- put an empty  `__init__.py` in a folder to make it a package.

- everything is an object, including function.

- flow control:
    - if looks something like this
    
        ```python
        if a or b:
            print "hello"
        else:
            print "hello again"
        ```
        
    - `for i in range(1:5)` doesn't include 5
    
    - `continue` to break loop, in R, it's `next`
    

