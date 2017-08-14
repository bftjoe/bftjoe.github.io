---
layout: post
title: Waffling in University of Alberta Bot and Steamhammer
---

Steamhammer/UAB waffle back and forth in range of the enemy or static defense.

In Squad.cpp combat sim is only run when you are already in range of the enemy. Once the army is out of range, the sim is not run and the bot will attack. Once it gets into range, the combat sim will calculate a loss, and retreat.

The fix is simple, delete Lines 351 to 397 in [Squad.cpp](https://github.com/kant2002/steamhammer/blob/master/Steamhammer/Source/Squad.cpp#L351)



This is also why lings run up to zealots and die attempting to retreat, instead of keeping a safe distance. Due to the short range of zealots, it is especially bad.
