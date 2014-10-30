
Snapping
********

There are two types of snap operations that you can use in Blender. The first type snaps your
selection or cursor to a given point while the second type is used during transformations
(translate, rotate, scale) and snaps your selection to elements within the scene.


Snap

----


.. admonition:: Reference
   :class: refbox

   | Mode:     :guilabel:`Object` and :guilabel:`Edit` modes
   | Hotkey:   :kbd:`shift-S`


The :guilabel:`Snap` menu
(also available from the 3D header in both :guilabel:`Object` and :guilabel:`Edit` mode
(:menuselection:`Object --> Snap` and :menuselection:`Mesh --> Snap`).
This menu provides a number of options to move the cursor or your selection to a defined point
(the cursor, selection or the grid).


.. figure:: /images/3D-interaction_Transform-Control_Snap-snap-menu.jpg

   Snap menu


Selection to Grid
   Snaps the currently selected object(s) to the nearest grid point.

Selection to Cursor
   Snaps the currently selected object(s) to the cursor location.

Cursor to Selected
   Moves the cursor to the center of the selected object(s).

Cursor to Center
   Moves the cursor to the center of the grid.

Cursor to Grid
   Moves the cursor to the nearest grid point.

Cursor to Active
   Moves the cursor to the center of the active object.


Transform Snapping
==================

The ability to snap Objects and Mesh element to various types of scene elements during a
transformation is available by toggling the magnet icon (which will turn red)
in the 3D view's header buttons.


.. figure:: /images/3D-interaction_Transform-Control_Snap-magnet-header.jpg

   Magnet icon in the 3D view header (red when enabled).


Snapping Modes
**************

Snap Element
============

.. figure:: /images/3D-interaction_Transform-Control_Snap-snap-element.jpg

   Snap Element menu


Volume
   Snaps to regions within the volume of the first Object found below the mouse cursor. Unlike the other options, this one controls the depth (i.e. Z-coordinates in current view space) of the transformed element. By toggling the button that appears to the right of the snap target menu (see below), target objects will be considered as a whole when determining the volume center.
Face
   Snap to the surfaces of faces in mesh objects. Useful for retopologizing.
Edge
   Snap to edges of mesh objects.
Vertex
   Snap to vertices of mesh objects.
Increment
   Snap to grid points. When in Orthographic view, the snapping increment changes depending on zoom level.


Snap Target
===========

.. figure:: /images/3D-interaction_Transform-Control_Snap-snap-target.jpg

   Snap Target menu.


Snap target options become active when either :guilabel:`Vertex`, :guilabel:`Edge`,
:guilabel:`Face`, or :guilabel:`Volume` is selected as the snap element.
These determine what part of the selection snaps to the target objects.

Active
   move the active element (vertex in Edit mode, object in Object mode) to the target.
Median
   move the median of the selection to the target.
Center
   move the current transformation center to the target. Can be used with 3D cursor to snap with an offset.
Closest
   move the closest point of the selection to the target.


+--------------------------------------------------------------------------+-------------------------------------------------------------------------+-------------------------------------------------------------------------+
+.. figure:: /images/3D-interaction_Transform-Control_Snap-snap-closest.jpg|.. figure:: /images/3D-interaction_Transform-Control_Snap-snap-active.jpg|.. figure:: /images/3D-interaction_Transform-Control_Snap-snap-median.jpg+
+                                                                          |                                                                         |                                                                         +
+   Closest                                                                |   Active                                                                |   Median                                                                +
+--------------------------------------------------------------------------+-------------------------------------------------------------------------+-------------------------------------------------------------------------+


Additional snap options
-----------------------

+--------------------------------------------------------------------------------------+------------------------------------------------------------------------------------+
+.. figure:: /images/3D-interaction_Transform-Control_Snap-snap-options-object-mode.jpg|.. figure:: /images/3D-interaction_Transform-Control_Snap-snap-options-edit-mode.jpg+
+                                                                                      |                                                                                    +
+   Object mode                                                                        |   Edit mode                                                                        +
+--------------------------------------------------------------------------------------+------------------------------------------------------------------------------------+


As seen by the red highlighted areas in the image above,
additional controls are available to alter snap behaviour. These options vary between mode
(Object and Edit) as well as Snap Element. The four options available are:


- .. figure:: /images/3D-interaction_Transform-Control_Snap-snap-options-align-rotation.jpg

   Align rotation with the snapping target.

- .. figure:: /images/3D-interaction_Transform-Control_Snap-snap-options-project-elements.jpg

   Project individual elements on the surface of other objects.

- .. figure:: /images/3D-interaction_Transform-Control_Snap-snap-options-snap-itself.jpg

   Snaps elements to its own mesh.

- .. figure:: /images/3D-interaction_Transform-Control_Snap-snap-options-objects-whole.jpg

   Consider Objects as whole when finding volume center.


Multiple Snap Targets
---------------------

.. figure:: /images/3D-interaction_Transform-Control_Snap_Multiple_Snap_Target.jpg

   Multiple snapping targets.


Once transforming a selection with Snapping on (not just with the Ctrl key held),
you can press A to mark the current snapping point, then proceed to mark as many other
snapping points as you wish and the selection will be snapped to the average location of all
the marked points.

Marking a point more than once will give it more weight in the averaged location.
