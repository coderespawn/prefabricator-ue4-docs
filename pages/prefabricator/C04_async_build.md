---
title: Asynchronous Building
keywords: prefab
sidebar: prefabricator_sidebar
permalink: async_build.html
folder: prefabricator
---

## Asynchronous Building

Levels that are randomized using the [Prefab Randomizer][level_randomization] actor can be run asynchronously

Select the *Prefab Randomizer* actor and inspect the details panel


{% include inline_image.html file="async_build/01.png" %}

{% include inline_image.html file="async_build/02.png" %}


The *Max Build Time Per Frame* determines how much time (in seconds) should be alloted per frame for building the prefabs

Settings this to 0.0 disables asynchronous builds and everything is built on the same frame synchronously

A value of 0.02 means 20ms are alloted per frame for building the prefabs

This helps in maintaining a smooth framerate on level rebuilds

---

{% include links.html %}

Explore the next section from the side bar



