---
title: Segmentation fault (core dumped)
author: TC
date: '2018-06-15'
slug: segmentation-fault-core-dumped
categories:
  - c++
tags:
  - rant
  - cpp
  - useless things
---

`Segmentation fault (core dumped)` is the most unhelpful, brutal, ruthless & savage error message thrown at my face.

Another reason why working with c++ is not fun.

Ouch.

> update

After 2 hours of search/ debugging, it seems I've get my first **stack overflow** !
The lesson here is that I should not assign a large array on a stack.
code :

```
#include <iostream>

using namespace std;
int main(int argc, char const *argv[])
{

    double dfire_dipo_pn[85][85][6][30];

   	return 0;
}

```

It compiles fine, and throws segmentation fault while I attempted to run it, memory used should be under 10mb.




[Related SO question](https://stackoverflow.com/questions/1847789/segmentation-fault-on-large-array-sizes)

[what-and-where-are-the-stack-and-heap](https://stackoverflow.com/questions/79923/what-and-where-are-the-stack-and-heap)

---

It feels really bad because such gimmicks in C++ always distract me away from "really doing the job". 


