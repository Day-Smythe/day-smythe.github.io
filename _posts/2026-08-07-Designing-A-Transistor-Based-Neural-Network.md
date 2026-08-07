---
title: Transistor Based Neural Network
description: >-
  Designing a transistor based neural network that is built to be as modular as possible.
author: Day-Smythe
date: 2026-08-07 14:44:00 +0200
categories: [Neural-Networks, Explanation]
tags: [getting started]
pin: true
---

## Setting Up Realistic Goals

To be fully clear on what this project is, We should set out a few things that this will be and a few things that it wont be.

For starters, even with a minuscule power draw, this system will not be power efficient, using individual components means that we would need to route signals and electricity from one component to another over thin copper tape at distances well over a few centimeters, this also means that there will be a lot of resistance, which would decrease the power efficiency dramatically.

Another good thing to conform is that this system would be fairly slow, we would be using standard hobby transistors which have about a 10 nanosecond all the way up to a 120 nanosecond delay in terms of switching speed, when compared to a modern cpu's transistors which can be over 300 000 times fater at less than 0,1 picoseconds 

## Self Imposed Limitations
