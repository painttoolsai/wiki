=========================
Canvas and File Formats
=========================

.. meta::
   :description: Complete guide to canvas options and file formats in Paint Tool SAI. Support for SAI, PSD, BMP, PNG, and more.
   :keywords: paint tool sai, file format, sai format, psd, canvas, export, save

Paint Tool SAI supports various file formats for different purposes. This guide covers canvas setup and all supported file formats for saving and exporting your artwork.

Canvas Setup
============

Creating a New Canvas
---------------------

1. **File** → **New** (or Ctrl+N)
2. Configure canvas options:
   
   * **Width/Height:** In pixels
   * **Resolution:** DPI for print (typically 300)
   * **Background:** White, transparent, or custom color

Preset Sizes
------------

Common canvas presets:

+-------------------+----------------+------------------+
| Preset            | Dimensions     | Best For         |
+===================+================+==================+
| A4 (300 DPI)      | 2480 x 3508    | Print documents  |
+-------------------+----------------+------------------+
| Letter (300 DPI)  | 2550 x 3300    | US print         |
+-------------------+----------------+------------------+
| HD 1080p          | 1920 x 1080    | Digital display  |
+-------------------+----------------+------------------+
| 4K UHD            | 3840 x 2160    | High-res display |
+-------------------+----------------+------------------+
| Square Social     | 1080 x 1080    | Instagram        |
+-------------------+----------------+------------------+

Canvas Size Limits
------------------

See :doc:`../tech/32bit-vs-64bit-canvas-limits` for detailed information on maximum canvas sizes.

Native SAI Format (.sai / .sai2)
================================

Overview
--------

SAI's native format preserves all features:

* **All layer types** - Including special layers
* **Layer properties** - Opacity, blending modes, clipping
* **Selection data** - Saved selections
* **Tool settings** - Brush configurations used

SAI Ver.1 Format (.sai)
-----------------------

* Used by Paint Tool SAI Ver.1
* Compatible with Ver.2 (can open in both)
* Maximum file size: 2GB

SAI Ver.2 Format (.sai2)
------------------------

* Native format for SAI Ver.2
* Supports Ver.2 exclusive features:
  
  * Text layers
  * Shape layers  
  * Linework layers
  * Perspective rulers

* Not compatible with Ver.1

.. tip::
   Save in .sai format if you need to open files in both Ver.1 and Ver.2.

Adobe Photoshop Format (.psd)
=============================

SAI provides excellent PSD compatibility:

Export Features
---------------

When exporting to PSD:

* ✅ Raster layers
* ✅ Layer groups (folders)
* ✅ Opacity and blending modes
* ✅ Layer masks (clipping groups)
* ⚠️ Text layers (rasterized)
* ⚠️ Shape layers (rasterized)
* ⚠️ Linework layers (rasterized)

Import Features
---------------

When importing from PSD:

* ✅ Standard layers
* ✅ Layer groups
* ✅ Common blending modes
* ⚠️ Adjustment layers (ignored)
* ⚠️ Smart objects (rasterized)
* ⚠️ Layer styles (may be flattened)

.. note::
   SAI will rasterize vector content from PSD files. Keep original PSDs if you need to edit vector elements.

Image Formats
=============

BMP (Bitmap)
------------

* **Extension:** .bmp
* **Layers:** Flattened only
* **Color Depth:** 24-bit RGB
* **Transparency:** Not supported
* **Best For:** Maximum compatibility, no compression

PNG (Portable Network Graphics)
-------------------------------

* **Extension:** .png
* **Layers:** Flattened only
* **Color Depth:** 8-bit or 24-bit + alpha
* **Transparency:** Full alpha channel support
* **Compression:** Lossless
* **Best For:** Web graphics, transparent images

JPEG (Joint Photographic Experts Group)
---------------------------------------

* **Extension:** .jpg / .jpeg
* **Layers:** Flattened only
* **Color Depth:** 24-bit RGB
* **Transparency:** Not supported
* **Compression:** Lossy (quality adjustable)
* **Best For:** Photos, web sharing

.. warning::
   JPEG compression causes quality loss. Avoid repeatedly saving as JPEG.

TGA (Targa)
-----------

* **Extension:** .tga
* **Layers:** Flattened only
* **Color Depth:** 24-bit or 32-bit
* **Transparency:** Alpha channel optional
* **Best For:** Game development, 3D textures

Export Settings
===============

Best Practices by Use Case
--------------------------

**For continued editing:**
   Save as .sai2 (or .sai for Ver.1 compatibility)

**For Photoshop workflow:**
   Export as .psd

**For web publishing:**
   Export as .png (transparent) or .jpg (opaque)

**For printing:**
   Export as .png at full resolution, or .psd for print shop workflow

**For archiving:**
   Keep .sai2 original + .png backup

Quality Settings for JPEG
-------------------------

When exporting JPEG, consider:

+----------+-------------------+----------------+
| Quality  | File Size         | Best For       |
+==========+===================+================+
| 100%     | Largest           | Print, archive |
+----------+-------------------+----------------+
| 85-95%   | Moderate          | High-quality web|
+----------+-------------------+----------------+
| 70-85%   | Smaller           | General web    |
+----------+-------------------+----------------+
| 50-70%   | Small             | Thumbnails     |
+----------+-------------------+----------------+

Working with Multiple Formats
=============================

Recommended Workflow
--------------------

1. **Work in native format** - Save as .sai2 while working
2. **Save frequently** - Use Ctrl+S often
3. **Export when needed** - Create PNG/PSD copies for sharing
4. **Keep originals** - Never overwrite .sai2 with flattened exports

File Organization
-----------------

Suggested folder structure::

   Project/
   ├── Working/          # .sai2 files
   ├── PSD/              # Photoshop exports
   ├── Final/            # Finished PNG/JPG
   └── Reference/        # Reference images

Troubleshooting
===============

Can't open .sai2 in Ver.1
-------------------------

.sai2 format is Ver.2 only. Open in Ver.2 and save as .sai or export to PSD.

PSD layers don't match
----------------------

Some Photoshop features don't translate. Check for:

* Adjustment layers
* Smart objects
* Layer styles
* Blend mode compatibility

File too large
--------------

* Reduce canvas size if possible
* Merge unnecessary layers
* For PSD, consider "Maximize Compatibility" being disabled

See Also
========

* :doc:`layer-types-and-properties`
* :doc:`../tech/32bit-vs-64bit-canvas-limits`
* :doc:`../getting-started/installation-guide-no-installer`
