---
title: bash build-in variables
author: tc
date: '2018-03-27'
slug: bash-build-in-variables
categories:
  - trivial
tags:
  - bash
---

There are some fancy build-in variables in bash that I picked up from others' scripts. They start with a dollar sign. Guess I'll take some notes. (mostly stole from SO)[https://stackoverflow.com/questions/5163144/what-are-the-special-dollar-sign-shell-variables]

- `$#` number of arguments

- `$@` and `$*` return all the parameters, but
[answer on SO](https://stackoverflow.com/questions/2761723/what-is-the-difference-between-and-in-shell-scripts)

> `$@` behaves like `$*` except that when quoted the arguments are broken up properly if there are spaces in them.

- `$?` was last command successful?

- `$0 $1 $2 ...` positional arguments, `$0` gives the 

- `$#` number of positional parameters ($0 excluded)

- `$-` current options set for the shell

- `$$` pid of the current shell

- `$_` most recent parameter (probably rarely used)

- `$IFS` field separator



