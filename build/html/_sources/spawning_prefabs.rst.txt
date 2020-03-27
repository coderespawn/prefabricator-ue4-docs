Spawning Prefabs
================

Use blueprints to spawn prefabs at runtime

.. image:: /images/spawn_prefab/01.png


.. image:: /images/spawn_prefab/02.png



The *Spawn Prefab* function takes in the following parameters:
* World Context Object: Pass a reference to any actor in the scene. This is needed by the library to grab a reference of the world to create the prefab in
* Prefab: The prefab asset that should be spawned on the scene
* Transform: The world transform of the spawned prefab actor
* Seed: Used for randomization.   Randomize it with your game's seed or pass in a random number

