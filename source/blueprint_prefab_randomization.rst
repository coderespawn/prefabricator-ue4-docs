Blueprint Prefab Randomization
==============================

Existing prefabs in the scene can be randomized and rebuilt

.. image:: /images/rand_prefab/rand_prefab_bp.png



----

Randomize Seed Node
-------------------

Randomizes the seed of the prefab, and optionally the child prefabs as well.  This node does not build the prefab, only modifies the seed value

* Target: The prefab actor in the scene that you'd like to randomize
* Random: Assign an existing random stream or create a new one
* Recursive: If checked, will randomize all the children down to the lowest level


----

Load Prefab
-----------

This node reloads the prefab, recreating the actors as necessary

* Target: The prefab actor in the scene that you'd like to randomize
