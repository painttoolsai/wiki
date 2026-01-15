=======================
Bristle Bitmap Corrector
=======================

.. meta::
   :description: How to fix invalid brush textures in Paint Tool SAI 2 after the February 2024 security update. Bristle loader corrector tool guide.
   :keywords: paint tool sai, bristle, brush texture, corrector, bitmap, security update, fix

Starting with the February 2024 update, Paint Tool SAI 2 implemented new security measures for brush textures. Some older brush files may be rejected and require correction using the Bristle Bitmap Corrector tool.

.. important::
   If your custom brushes stopped working after updating SAI 2, this guide will help you fix them.

Background
==========

What Changed
------------

In February 2024, SYSTEMAX implemented stricter validation for brush texture files to:

* Prevent potential security vulnerabilities
* Ensure consistent brush behavior
* Improve application stability

Affected Files
--------------

The following brush components may be affected:

* **Blotmap files** - Brush shape textures
* **Brushtex files** - Brush pattern textures
* **Elemap files** - Element maps for special brushes
* **Scatter files** - Particle scatter data

Symptoms of Invalid Textures
============================

You may experience the following issues:

* Brushes display as solid circles instead of textured
* Error messages about invalid bitmap format
* Brushes disappear from the brush list
* Warning dialogs on startup about rejected files

Identifying Problem Files
=========================

Check the Log
-------------

1. Launch SAI 2
2. Look for warning messages on startup
3. Check the application log (if available)

Manual Inspection
-----------------

Invalid files often have:

* Incorrect color depth (not 8-bit grayscale)
* Wrong file dimensions
* Corrupted file headers
* Unsupported compression

Using the Bristle Bitmap Corrector
==================================

SAI 2 includes a built-in tool to correct invalid textures:

Step 1: Locate the Tool
-----------------------

The corrector tool is included in your SAI 2 installation:

1. Navigate to your SAI 2 folder
2. Look for ``saicorrt.exe`` or similar utility
3. If not present, download from the SYSTEMAX website

Step 2: Backup Your Brushes
---------------------------

.. warning::
   Always backup before making changes!

1. Copy the following folders to a safe location:
   
   * ``blotmap/``
   * ``brushtex/``
   * ``elemap/``
   * ``scatter/``

Step 3: Run the Corrector
-------------------------

1. Close SAI 2 completely
2. Run the corrector tool
3. Point it to your SAI 2 installation folder
4. The tool will scan and identify invalid files

Step 4: Apply Corrections
-------------------------

The corrector tool will:

* Convert invalid color depths to proper 8-bit grayscale
* Fix file headers
* Re-encode compressed files
* Report unfixable files

Step 5: Verify
--------------

1. Launch SAI 2
2. Check that previously broken brushes now work
3. Test brush functionality

Manual Correction Methods
=========================

If the automatic corrector doesn't work, you can manually fix textures:

Using Image Editors
-------------------

1. Open the texture file in an image editor (Photoshop, GIMP, etc.)
2. Convert to **8-bit Grayscale** mode
3. Save as BMP with no compression
4. Replace the original file

Requirements for Valid Textures
-------------------------------

* **Color Mode:** 8-bit Grayscale
* **Format:** Uncompressed BMP
* **Dimensions:** Power of 2 recommended (256x256, 512x512, etc.)
* **Bit Depth:** 8 bits per pixel

Using GIMP (Free)
-----------------

1. Open texture file in GIMP
2. **Image** → **Mode** → **Grayscale**
3. **Image** → **Mode** → **8 bpc**
4. **File** → **Export As** → BMP
5. In export options: Select no compression, 8-bit

Creating Compatible Brush Textures
==================================

If you're creating new brush textures:

Specifications
--------------

* **Size:** 64x64 to 1024x1024 pixels (power of 2)
* **Color:** Grayscale only
* **Depth:** 8-bit
* **Format:** BMP (uncompressed)

Design Tips
-----------

* White = full opacity/effect
* Black = no opacity/effect
* Grays = partial effect
* Consider tiling for pattern brushes

Common Issues and Solutions
===========================

"Bitmap format not supported"
-----------------------------

**Cause:** Wrong color depth or compression

**Fix:** Re-save as 8-bit grayscale uncompressed BMP

"Texture dimensions invalid"
----------------------------

**Cause:** Non-standard dimensions

**Fix:** Resize to power of 2 (256, 512, 1024, etc.)

"File corrupted"
----------------

**Cause:** Damaged file or incomplete download

**Fix:** Re-download or restore from backup

Brushes still not working after correction
------------------------------------------

**Try:**

1. Clear SAI 2 cache (delete temp files)
2. Restart the application
3. Reinstall the brush pack
4. Check for updates to SAI 2

Prevention
==========

To avoid issues in the future:

1. **Keep backups** of working brush configurations
2. **Update SAI 2** regularly
3. **Download brushes** from trusted sources
4. **Verify brush packs** before installing

Trusted Brush Sources
---------------------

* Official SYSTEMAX brushes
* Well-known artist brush packs
* Brushes tested with current SAI versions

See Also
========

* :doc:`system-requirements`
* :doc:`../getting-started/paint-tool-sai-2-technical-preview`
* :doc:`../features/linework-tools`
