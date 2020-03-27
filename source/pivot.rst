Pivot
=====

Just like meshes, Prefabs also have pivots that affect how the rotation and scaling is done.   

You can modify the pivot after the prefab has been created

By default, the pivot will be created at the lowest center of the bounding box.  

{% include note.html content="The default pivot will be snapped to the editor's current grid settings to avoid alignment issues" %}

We've assembled a simple pitshop setup.   Select these and create a prefab

.. image:: /images/pivot/pivot_01.jpg


.. image:: /images/pivot/pivot_02.jpg



The Pivot for this was created at the lower center of the prefab bounding box

.. image:: /images/pivot/pivot_03.png



----

To change the pivot, select all the items inside the prefab.  Use the World Outliner to do this:

{% include note.html content="Make sure you do not select the prefab you are trying to modify but only the items inside of it" %}

.. image:: /images/pivot/pivot_04.png


.. image:: /images/pivot/pivot_05.jpg


Move these items so your pivot is in the desired place

.. image:: /images/pivot/pivot_06.jpg


----

Select the prefab by clicking on any of the meshes and notice the pivot has changed

.. image:: /images/pivot/pivot_07.jpg


You'll need to save these changes back to the prefab asset

.. image:: /images/pivot/pivot_08.png


