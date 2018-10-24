---
title: error messages
author: tc
date: '2018-10-22'
slug: error-messages
categories:
  - c++
tags:
  - rant
  - trivial
---

C++ error messages are notorious for being unhelpful at all:

- segmentation fault

- stack overflow

Besides the obnoxious two, I have this today:

- `train: /usr/local/boost_1_67_0/boost/multi_array/base.hpp:135: Reference boost::detail::multi_array::value_accessor_n<T, NumDims>::access(boost::type<Reference>, boost::detail::multi_array::value_accessor_n<T, NumDims>::index, TPtr, const size_type*, const index*, const index*) const [with Reference = boost::detail::multi_array::sub_array<int, 1>; TPtr = int*; T = int; long unsigned int NumDims = 2; boost::detail::multi_array::value_accessor_n<T, NumDims>::index = long int; boost::detail::multi_array::multi_array_base::size_type = long unsigned int]: Assertion idx - index_bases[0] >= 0 failed.`

Basically it is an error from the boost multi_array library. It tells me that I have an `index out of range` error.

But it doesn't help me to locate where the error occurs (who even does that).

I have to compile the file with `-g` debug flag, fire up gdb, load the binary, set a couple of breakpoints and manually check the code line by line to finally "locate the error".

Only after that whole process can I finally fix the problem.

I have been learning programming in C++ for more than half a year, I have lived through all the hussles such as pointers, class inheritance, virtual functions, templates, g++ flags, makefile, cmake, out-of-source-compile, boost library, and what not.

But I do not enjoy coding in c++ at all.

Nah, not even once.

