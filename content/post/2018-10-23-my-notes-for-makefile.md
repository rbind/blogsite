---
title: My Notes for Makefile
author: TC
date: '2018-10-23'
slug: my-notes-for-makefile
categories:
  - programming
tags:
  - trivial
---

Although `make` is part of the gnu toolset, its use is not restricted to compile a c++ program. make can be used to do various kinds of work.

Here is my notes on makefile for my future self. I find it of great help to keep these notes handy. For example, I often come back for [this one](/post/2018/03/27/bash-build-in-variables/)


### Macro

- Define macro(variable, but it's called macro in makefile) with equal sign, multiple values can be assigned to one macro. use macro in the form of `$(A)`

```
A = a b c
$(A)
```

### Rules

- The structure of a rule

```
%.o: $(DEPS)
	$(CC) -c -o $@ $< $(CFLAGS)
```

- %.o: target file
- $(DEPS): file dependency (to generate target)
- \tab+command: usual linux commands

My notes:

- Type `make` will run the first rule in a Makefile.
    
- Special rule: `.PHONY: clean` tells make that clean is not a file. Always execute commands under the `clean` rule, even if there's a clean file in the working directory.

- Automatic variables
    - `$@` target of the rule
    - `$<` first prerequisite
    - `$^` all prerequisite

- Sublime will transform tab to 4 spaces, turn that off for makefile

- `@` before a command will prevent printing the command before executing.

- `%` for quoting.

## Resources


[gnu make manual](https://www.gnu.org/software/make/manual/make.html)

[A Simple Makefile Tutorial](http://www.cs.colby.edu/maxwell/courses/tutorials/maketutor/)

[An interesting SO question of makefile use case](https://stackoverflow.com/questions/52939722/r-markdown-importing-r-script-objects/52939860#52939860)


