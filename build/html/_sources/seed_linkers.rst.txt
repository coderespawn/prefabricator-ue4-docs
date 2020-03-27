Seed Linkers
============

Use Seed Linkers to enforce same random selection across multiple prefab instance
(e.g. have all the fence prefabs in the scene select the same random fence from the collection)

----

Somtimes, you'd want certain prefab actors in the scene to share the same random selection. 

Consider the following example with a prefab collection with Pillar prefabs.   


.. image:: /images/seed_linker/seed_linkers.gif



----

Drop in a Seed Linker actor on the scene and rename it to something user-friendly (you will be referencing this later)

.. image:: /images/seed_linker/sl_drop_actor.png


.. image:: /images/seed_linker/seed_linker_rename.png



----

Inspect the seed linker actor in the details panel

.. image:: /images/seed_linker/01.png


This specifies the list of prefabs that should have their seeds linked (i.e. share the same random result)

You can manually add the prefab actor references here. However there's an easier way

----

Select all the actors that should have their seeds linked. Hold down *Control* key and select the Pillar Prefab Actors

.. image:: /images/seed_linker/02.jpg


On the editor's main toolbar, click the Prefabricator Tool button > Link Selected Prefab Collection Seeds > [SeedLinkerName]

.. image:: /images/seed_linker/03.jpg


----

Select the seed linker and you should be able to see red lines to the prefabs that the seed linker is referencing

.. image:: /images/seed_linker/04.jpg



----

Randomizing the level will now enforce same random selection for these prefabs

