---
title: Pointer nightmar
author: tc
date: '2018-05-15'
slug: pointer-nightmar
categories:
  - programming
tags:
  - cpp
---

# Why pointers

Recently I'm messing around with historical code in my lab, written in c++. Dealing with pointers is inevitable. As I'm not a c++ native,pointers give me some trouble. 

Then I run into [this post](http://duramecho.com/ComputerInformation/WhyCPointers.html), which explains all those gimmicks behind the widely ~~abused~~ used pointers. Good read.

The basic idea behind `pointer` is simple: a variable that stores the address of another variable. 

But when pointers were used to implement features which c lack, pointers  quickly became a nightmare to haunt innocent young programmers ~~like me~~.

I've also noticed a trend in SO, regarding the same problem in different language, c/c++ programmers do like re-inventing the wheels:

> in C/C++: "how do I do dis"

- **20 lines code snippet, implementing the solution from scratch.

> in R/python/whatever: "How do I do dat"

- **recommend packages/other people's work that actually do the job.

======

Oh, and I also learned to use makefile.