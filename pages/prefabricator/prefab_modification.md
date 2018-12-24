---
title: Prefab Modifications
keywords: prefab
sidebar: prefabricator_sidebar
permalink: prefab_modification.html
folder: prefabricator
---

## Modifying Prefabs

A prefab can be modified after it has been created.   You do this by 
selecting and modifying the items inside the prefab as necessary

In the following example, the barrel prefab is made up of 3 cylinders.  

--- 

Select the barrel prefab by clicking on it

{% include inline_image.html file="modification/s1.jpg" %}

--- 

Click on it again to select the item inside the prefab (the center cylinder)

{% include inline_image.html file="modification/s2.jpg" %}

--- 

Modify the position or any other property of this actor. In this case, we'll chage 
the material

{% include inline_image.html file="modification/s6.png" %}

{% include inline_image.html file="modification/s4.jpg" %}


## Saving Prefabs

Click on the mesh again to select the prefab actor

{% include inline_image.html file="modification/s5.jpg" %}

--- 

The prefab actor has an option to save the changes to the prefab asset

{% include inline_image.html file="modification/s_details.png" %}

Click *Save Prefab to Asset*

{% include inline_image.html file="modification/s_details2.png" %}

Once saved, these changes would automatically be propagated to all the 
instances in the level.  This also works across different maps

## Restoring Prefabs

If you have unsaved changes on a prefab actor and would like to discard those changes 
and reload them from the asset file, click *Load Prefab from Asset*

{% include inline_image.html file="modification/load_from_asset.png" %}



{% include links.html %}
