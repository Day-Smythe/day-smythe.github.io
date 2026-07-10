---
title: Measuring compile-time vs runtime tradeoffs.
date: 2026-07-10 14:39:55 +0200
categories: [Linux, Gentoo]
tags: [minimal-linux]     # TAG names should always be lowercase
description: No performance is free
---

Software performance is governed by a simple yet often overlooked principal, "computational complexity cannot be eliminated, only relocated". Every optimization strategy represents an active decision about where the cost of running computationally complex software will be paid. That cost may be brought up during compilation through architecture specific code generation, (such as aarch64 or x86_64), or even whole program optimization, or it may instead emerge when the program is being executed. In other words, the performance that may be gained is not free, it is simply pre paid by the time you spent compiling.

This concept forms the foundation of the Gentoo Linux philosophy. Unlike the more conventional binary distributions which must target a wide range of hardware and software configurations, Gentoo exposes almost all stages of the compilation pipeline to the end user. Through mechanisms such as the 'make.conf' file, which contains 'USE' flags as well as compiler flags, the operating system becomes configurable to the point where you can modify and observe and measure almost anything that will be built for your system.
