Level Randomization
===================

Randomize all the prefabs in a level asynchronously over multiple frames

Prefab Randomizer Actor
-----------------------

This utility actor helps with randomizing all the prefabs in the level 

Drop in a Prefab Randomizer actor on the level 

.. image:: /images/level_rand/01.png


Select the actor and inspect the details panel.  

.. image:: /images/level_rand/02.png


Click Randomizer

----

.. image:: /images/level_rand/level_rand.gif



You can also randomize this at runtime using [Blueprints][blueprint_level_randomization]


Randomize on Begin Play
-----------------------
Select this option if you want your level to be randomized when the game starts

.. image:: /images/level_rand/rand_prop.png


Randomize Selected Prefabs
--------------------------

If you want to randomize only a certain set of prefabs actors (instead of the entire level), then assign those actors in the ``Actors To Randomize`` list.  If this list is left empty, every prefab actor in the level would be randomized

This can be useful if you want to the randomize heavy prefabs at runtime asychronously 

Here's a example of a helper function to randomize a prefab at runtime.  This function creates a prefab randomizer actor, sets the target prefab,  randomizes it asynchronously and when the randomization completes, it destroys the randomizer actor

.. image:: /images/level_rand/03.png
