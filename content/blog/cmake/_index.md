---
title: 💻 CMake
summary: ''
date: 2024-10-15
weight: 1

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: ''

authors:
  - admin

tags:
  - CMake
---

> [CMake is the de-facto standard for building C++ code [...]. It’s a powerful, comprehensive solution for managing the software build process.](https://cmake.org/)

The [State of Developer Ecosystem](https://www.jetbrains.com/lp/devecosystem-2023/cpp/) reports from 2018 to 2023 demonstrate [CMake](https://cmake.org/)'s ongoing dominance as the most popular build system for [C++](https://en.cppreference.com/w/) projects. The data also reveals that [Python](https://www.python.org/) is the programming language most likely to be paired with C++.

Although CMake has existed long before its current success and has gone through many significant changes since its inception, it still aims to maintain backwards compatibility. As such, bad CMake practices remain prevalent in many open-source codebases, especially in the research community.

Many resources on "effective" and "modern" CMake already exist online, and I don't wish to repeat the same information all over again. Unfortunately, some of those resources may conflict with others on what exactly are CMake's best practices and how to use it effectively. 

Thus, I would highly encourage readers interested in developing open-source C++ projects to read [Craig Scott](https://crascit.com/)'s [Professional CMake](https://crascit.com/professional-cmake/), as the author is one of the co-maintainers of CMake itself and has extensive relevant experience on the topic. His [CppCon talk](https://crascit.com/2019/10/16/cppcon-2019-deep-cmake-for-library-authors/) and book were very well received by the C++ community, and I myself find his book to be the best CMake learning resource that I have read out of many others.

This series of blog posts will go over how I created and maintain an open-source cross-platform C++ project, which is managed by CMake. I will aim to write hands-on flavored articles that focus on typical research use cases, with code snippets that the reader can easily copy, paste and replace in their own project. Going over these use cases entails that we will cover topics such as 
- static/shared libraries
- dependency management
- compiling CUDA code
- automated testing
- installation
- Python bindings. 

The hope is that it will not be too hard to capture the fundamental principles that have guided the decisions that went into my own codebase, and generalize them to the reader's particular situation.