---
title: Build Event Listener
keywords: prefab
sidebar: prefabricator_sidebar
permalink: build_event_listener.html
folder: prefabricator
---

## Build Event Listeners

These are blueprints that you can attach to a prefab asset.    It allows you to
hook into the various build stages of the prefab when it is spawned into the world and modify the 
spawned actors through your blueprint logic

These are great for applying random materials, changing light colors or your custom game logic etc

---

In this example, we'll use the following nested building prefab.

{% include inline_image.html file="build_events/prefab_asset.png" %}

The prefab is built using smaller prefabs: ground floor prefab, 3 floor prefabs, a roof prefab and facade decorations prefab


{% include inline_image.html file="build_events/before.gif" %}


The art asset comes with various materials that when applied, changes the look of the building.   Instead of recreating 
the prefab each with a different material,  we'll use blueprints to randomly assign one of the materials so it looks like this

{% include inline_image.html file="build_events/after.gif" %}

---

Create a *Prefabricator Event Listener* blueprint

{% include inline_image.html file="build_events/bp_01.png" %}

{% include inline_image.html file="build_events/bp_02.png" %}

{% include inline_image.html file="build_events/bp_03.png" %}

---

Override the Post Spawn function and add your logic here

{% include inline_image.html file="build_events/bp_04.png" %}

---

There's a helper function that lets you grab all the child actors (included the nested ones). This can be used to assign the material

{% include inline_image.html file="build_events/bp_05.png" %}

---

Assign this blueprint to all the relavant prefab assets.

Double click the prefab asset to open the properties

{% include inline_image.html file="build_events/prefab_asset.png" %}

{% include inline_image.html file="build_events/bp_06.png" %}


Spawning the prefab or randomizing it would now execute your script and pick up the new materials

---


## Sample Blueprint

Here are the screenshots of the blueprint used above

### Post Spawn

{% include inline_image.html file="build_events/bp/01.png" %}

Variables:
* **Materials** : Material Interface (Array)
* {% include inline_image.html file="build_events/bp/01_vars.png" %}

Populate your materials in this MaterialInterface array

---

### Apply Random Material

{% include inline_image.html file="build_events/bp/02.png" %}

Variables:
* **Material** : Material Interface
* {% include inline_image.html file="build_events/bp/02_vars.png" %}


---

### Get Random Material

{% include inline_image.html file="build_events/bp/03.png" %}

---

{% include links.html %}

Explore the next section from the side bar



