
********************
Material Color Nodes
********************

MixRGB
======

.. figure:: /images/26-Manual-Material-Color-Node-Mix.jpg

   MixRGB node


This node mixes a base color or image (threaded to the top socket)
together with a second color or image (bottom socket)
by working on the individual and corresponding pixels in the two images or surfaces.
The way the output image is produced is selected in the drop-down menu. The size
(output resolution) of the image produced by the mix node is the size of the base image.
The alpha and Z channels (for compositing nodes) are mixed as well.


Not one, not two, but count 'em, sixteen mixing choices include:

.. seealso::

   :term:`Color Blend Modes` for details on each blending mode.


Inputs
------

Fac
   The amount of mixing of the bottom socket is selected by the Factor input field (Fac:).
   A factor of zero does not use the bottom socket, whereas a value of ``1.0`` makes full use.
   In Mix mode, 50:50 (0.50) is an even mix between the two,
   but in Add mode, ``0.5`` means that only half of the second socket's influence will be applied.
Color 1
   Input color value.  The value can be provided by another node or set manually.
   Includes a color swatch, allowing you to select the color directly on the node.
Color 2
   Input color value.  The value can be provided by another node or set manually.
   Includes a color swatch, allowing you to select the color directly on the node.


Outputs
-------

Color
   Value of the color, combined by the node.


Controls
--------

Clamp
   Clamp result of the node to 0...1 range.


RGB Curves
==========

.. figure:: /images/26-Manual-Material-Color-Node-Curves.jpg

   RGB Curves node


For each color component channel (RGB) or the composite (C),
this node allows you to define a bezier curve that varies the input (across the bottom,
or x-axis) to produce an output value (the y-axis). By default,
it is a straight line with a constant slope, so that .5 along the x-axis results in a .
5 y-axis output.
Click and drag along the curve to create a control point and to change the curve's shape.
Use the *X* to delete the selected (white) point.

Clicking on each *C R G B* component displays the curve for that channel.
For example, making the composite curve flatter
(by clicking and dragging the left-hand point of the curve up)
means that a little amount of color will result in a lot more color (a higher Y value).
Effectively, this bolsters the faint details while reducing overall contrast.
You can also set a curve just for the red, and for example,
set the curve so that a little red does not show at all, but a lot of red does.


Inputs
------

Fac:
   Factor. The degree of node's influence in node tree.
   The value can be provided by another node or set manually.
   Value range - from «-1» (inverted effect) to «1».
Color
   Input color value. The value can be provided by another node or set manually.
   Includes a color swatch, allowing you to select the color directly on the node.


Outputs
-------

Color
   Value of the color, combined by the node.


Controls
--------

.. figure:: /images/26-Manual-Material-Color-Node-Curves-Channels.jpg

   Curve channel selector


Channel selector
   Allows to select appropriate curve channel.

   C
      Composite curve.
   R, G, B
      Red/Green/Blue channel curve.


.. figure:: /images/26-Manual-Material-Color-Node-Curves-Controls.jpg

   Node curve controls


.. figure:: /images/26-Material-Color-Node-Curves-Zoomin-Buticon.jpg

   Zoom in curve.


.. figure:: /images/26-Material-Color-Node-Curves-Zoomout-Buticon.jpg

   Zoom out curve.


.. figure:: /images/26-Material-Color-Node-Curves-Tools.jpg

   Advanced tools for curve


Reset View
   Resets view of the cuve.
Vector Handle
   Vector type of curve point's handle.
Auto Handle
   Automatic type of curve point's handle.
Extend Horizontal
   Extends the curve horizontal.
Extend Extrapolated
   Extends the curve extrapolated.
Reset Curve
   Resets the curve in default (removes all added curve's points).


.. figure:: /images/26-Material-Color-Node-Curves-Clipping-Buticon.jpg

   Clipping options display of the curve.


.. figure:: /images/26-Material-Color-Node-Curves-Delpoints-Buticon.jpg

   Deletes points of the curve.


Here are some common curves you can use to achieve desired effects:


.. figure:: /images/26-Manual-Material-Color-Node-Curves-Uses.jpg
   :width: 900px
   :figwidth: 900px

   See:

   A) Lighten
   B) Negative
   C) Decrease Contrast
   D) Posterize


Invert
======

.. figure:: /images/26-Manual-Material-Color-Node-Invert.jpg

   Invert node


This node simply inverts the input values and colors.


Inputs
------

Fac:
   Factor. The degree of node's influence in node tree. The value can be provided by another node or set manually.
Color
   Input color value. The value can be provided by another node or set manually.
   Includes a color swatch, allowing you to select the color directly on the node.


Outputs
-------

Color
   Value of the color, combined by the node.


Hue Saturation Value
====================

.. figure:: /images/26-Manual-Material-Color-Node-HSV.jpg

   Hue Saturation Value node


Use this node to adjust the Hue, Saturation, and Value of an input.


Inputs
------

Fac
   Factor. The degree of node's influence in node tree. The value can be provided by another node or set manually.
Hue
   Input hue value of color. The value can be provided by another node or set manually.
Saturation
   Input saturation value of color . The value can be provided by another node or set manually.
Value
   Input HSV-Value of color. The value can be provided by another node or set manually.
Fac
   Factor. The degree of node's influence in node tree. The value can be provided by another node or set manually.
Color
   Input color value. The value can be provided by another node or set manually.
   Includes a color swatch, allowing you to select the color directly on the node.


Outputs
-------

Color
   Value of the color, combined by the node.

