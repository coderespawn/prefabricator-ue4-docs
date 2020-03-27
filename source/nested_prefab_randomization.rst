Nested Prefab Randomization
===========================

When a prefab actor is randomized, it would randomize the seed of every nested child prefab down to the lowest level

This allows you to have interesting randomization with more complex nested prefabs built from simpler prefab collections

In this example, we'll assemble the following building:


.. image:: /images/build_events/before.gif



----

Sample Nested Prefab Preparation
--------------------------------

We will build the building prefab using the following smaller prefabs
* Ground Floor Prefab - Represents the ground floor / entrance of the building
* Floor Prefab - Represents a single floor
* Roof Prefab - Roof of the building
* Facade Decoration - The decoration added to the facade of the building (fire exit)

Since we have multiple variations for each of these prefabs, we'll use prefab collections for the above 4


Ground Floor Prefab Collection
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
We have assembled 2 ground floor prefab variations.  Add them into a *GroundFloor* prefab collection

.. image:: /images/nested_rand/01.png



Floor Prefab Collection
^^^^^^^^^^^^^^^^^^^^^^^

We have assembled 3 floor prefab variations.  Add them into a *Floor* prefab collection

.. image:: /images/nested_rand/02.png



Roof Prefab Collection
^^^^^^^^^^^^^^^^^^^^^^

We have assembled 2 roof prefab variations.  Add them into a *Roof* prefab collection

.. image:: /images/nested_rand/03.png



Facade Decoration Collection
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

We want to decroate the facade of the buildings and prepared 5 different prefabs for it

.. image:: /images/nested_rand/04.png


An empty prefab was included in the list so we don't have any decorations sometimes


.. note::
   Make sure all the prefabs in your collections have consistent pivots so all the items in the collection spawn consistently in the right place

----

Sample Nested Prefab Assembly
-----------------------------

Now that we have the pieces in place, assemble our master building prefab

* Drop in the ground floor prefab collection on to the scene
* Drop as many floor prefab collections as necessary
* Drop in the roof prefab collection
* Drop in the facade decoration prefab collection

.. image:: /images/nested_rand/prefab_rand_assembly.gif



Select the prefabs you just dropped by holding the *Control* key and clicking on them

.. image:: /images/nested_rand/select_building_items.jpg



Create a prefab with the current selection

.. figure:: /images/getting_started/A_create_prefab_menu.png

  Create prefab menu


----

Sample Nested Prefab Randomization
----------------------------------

Select your newly created prefab and click Randomize.  It would randomize everything inside it 
(the floors, ground floor, roofs, facade decorations)


.. image:: /images/nested_rand/randomize_nested_detail.png


.. image:: /images/build_events/before.gif


----

Nested Child Prefab Randomization
---------------------------------

You can select child prefabs and randomize them individually for more fine tuned control

.. image:: /images/nested_rand/prefab_rand_child.gif
