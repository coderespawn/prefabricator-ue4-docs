---
title: Blueprint Level Randomization
keywords: prefab
sidebar: prefabricator_sidebar
permalink: blueprint_level_randomization.html
folder: prefabricator
---

## Blueprint Level Randomization

Randomize a level at runtime by invoking it from blueprints

---

Place a [Prefab Randomizer][level_randomization] actor on the scene if not placed already

Get a reference of this actor into your blueprint.  In this example, a level blueprint is used.

To get a reference in the level blueprint, select the actor in the viewport and right click on the level blueprint

{% include inline_image.html file="level_rand_bp/01.png" %}

---

Call the Randomize function.  In the following example this gets called with the X key is pressed

{% include inline_image.html file="level_rand_bp/02.png" %}


---

{% include inline_image.html file="level_rand/level_rand.gif" %}

---

{% include links.html %}

Explore the next section from the side bar



