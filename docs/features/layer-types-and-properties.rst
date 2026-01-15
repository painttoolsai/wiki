===========================
Layer Types and Properties
===========================

.. meta::
   :description: Guide to layer types in Paint Tool SAI 2 - raster, vector, text, shape, and linework layers.
   :keywords: paint tool sai, layers, blending modes, clipping, text layer, linework

Layer Types Overview
====================

+------------------+-------+-------+---------------------------+
| Layer Type       | Ver.1 | Ver.2 | Description               |
+==================+=======+=======+===========================+
| Normal Layer     | ✅    | ✅    | Standard raster painting  |
+------------------+-------+-------+---------------------------+
| Linework Layer   | ✅    | ✅    | Vector lines with pressure|
+------------------+-------+-------+---------------------------+
| Layer Set        | ✅    | ✅    | Folder for layers         |
+------------------+-------+-------+---------------------------+
| Text Layer       | ❌    | ✅    | Editable text             |
+------------------+-------+-------+---------------------------+
| Shape Layer      | ❌    | ✅    | Vector shapes             |
+------------------+-------+-------+---------------------------+

Normal Layer
============

Standard raster layer for painting. Create with Ctrl+Shift+N.

Properties:
* **Opacity:** 0-100%
* **Blending Mode:** Multiply, Screen, Overlay, etc.
* **Preserve Opacity:** Paint only on existing pixels
* **Clipping Group:** Clip to layer below

Linework Layer
==============

Vector-based layer for clean line art.

* Pressure sensitivity preserved after drawing
* Editable control points
* Convert to raster with right-click → Rasterize

Text Layer (Ver.2)
==================

Native text with full editing. Properties include font, size, color, and alignment.

Shape Layer (Ver.2)
===================

Vector shapes: Rectangle, Ellipse, Polygon with fill and stroke options.

Blending Modes
==============

* **Normal** - Standard layering
* **Multiply** - Darkens (shadows)
* **Screen** - Lightens (highlights)
* **Overlay** - Combines multiply and screen
* **Add** - Additive blending (glow)

See Also
========

* :doc:`linework-tools`
* :doc:`canvas-and-file-formats`
