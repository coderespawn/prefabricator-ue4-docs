Blueprint Level Randomization
=============================

Randomize a level at runtime by invoking it from blueprints

----

Place a ``Prefab Randomizer`` actor on the scene if not placed already

Get a reference of this actor into your blueprint.  In this example, a level blueprint is used.

To get a reference in the level blueprint, select the actor in the viewport and right click on the level blueprint

.. image:: /images/level_rand_bp/01.png


----

Call the Randomize function.  In the following example this gets called with the X key is pressed

.. image:: /images/level_rand_bp/02.png



----

.. image:: /images/level_rand/level_rand.gif

