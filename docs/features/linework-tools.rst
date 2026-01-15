==============
Linework Tools
==============

.. meta::
   :description: Complete guide to linework tools in Paint Tool SAI. Vector drawing, curve editing, and stroke controls.
   :keywords: paint tool sai, linework, vector, pen tool, curve, stroke editing

Linework layers provide vector-based line art with full pressure sensitivity and editability.

Creating Linework Layers
========================

1. Click **New Linework Layer** in the Layers panel
2. Or: **Layer** → **New Layer** → **Linework Layer**

Linework Tools
==============

Pen Tool
--------
Draw freehand strokes with pressure sensitivity. Strokes become editable paths.

Curve Tool
----------
Create Bezier curves by clicking to place points. Drag handles to adjust curve shape.

Line Tool
---------
Draw straight lines between two points.

Edit Tool
---------
Modify existing strokes:

* Select and move control points
* Adjust curve handles
* Delete points

Pressure Tool
-------------
Edit stroke pressure after drawing. Click and drag along a stroke to adjust thickness.

Weight Tool
-----------
Uniformly change stroke thickness.

Stroke Properties
=================

* **Min Width** - Thinnest point of stroke
* **Max Width** - Thickest point of stroke
* **Size** - Base stroke size
* **Density** - Stroke opacity

Editing Tips
============

* Double-click stroke to select all points
* Ctrl+click to add control points
* Delete key removes selected points
* Hold Shift for straight lines

Converting to Raster
====================

Right-click layer → **Rasterize Linework Layer**

.. warning::
   Rasterization is permanent. Duplicate the layer first if you may need to edit later.

See Also
========

* :doc:`layer-types-and-properties`
* :doc:`perspective-rulers-guide`
