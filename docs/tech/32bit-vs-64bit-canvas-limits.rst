=============================
32-bit vs 64-bit Canvas Limits
=============================

.. meta::
   :description: Understanding canvas size limits in Paint Tool SAI 32-bit and 64-bit versions. Maximum resolutions and memory considerations.
   :keywords: paint tool sai, canvas size, 64-bit, 32-bit, resolution limits, large canvas

Paint Tool SAI offers both 32-bit and 64-bit versions, each with different canvas size capabilities. Understanding these limits helps you choose the right version for your workflow.

Quick Comparison
================

+-------------------+------------------+--------------------+
| Feature           | 32-bit Version   | 64-bit Version     |
+===================+==================+====================+
| Max Canvas        | 10,000 x 10,000px| 100,000 x 100,000px|
+-------------------+------------------+--------------------+
| Max RAM Usage     | ~3GB             | System RAM limit   |
+-------------------+------------------+--------------------+
| Recommended For   | Standard artwork | Large illustrations|
+-------------------+------------------+--------------------+
| Compatibility     | All Windows      | 64-bit Windows only|
+-------------------+------------------+--------------------+

.. important::
   For most digital artwork, the 32-bit limit of 10,000 x 10,000px is sufficient. Choose 64-bit only if you regularly work with very large canvases.

Understanding Canvas Limits
===========================

32-bit Version Limits
---------------------

* **Maximum Resolution:** 10,000 x 10,000 pixels
* **Memory Limit:** Approximately 3GB RAM
* **Layer Limit:** Depends on canvas size and available memory

The 32-bit version can only address about 3GB of RAM due to Windows architecture limitations. This restricts both canvas size and the number of layers you can use simultaneously.

64-bit Version Limits
---------------------

* **Maximum Resolution:** 100,000 x 100,000 pixels
* **Memory Limit:** Limited only by installed system RAM
* **Layer Limit:** Much higher practical limit

.. note::
   While the theoretical maximum is 100,000 x 100,000 pixels, practical limits depend on your available RAM and system performance.

Memory Requirements by Canvas Size
==================================

Approximate RAM usage per layer at different canvas sizes:

+------------------+-----------------+----------------+
| Canvas Size      | Per Layer (~)   | 10 Layers (~)  |
+==================+=================+================+
| 2,000 x 2,000    | 15MB            | 150MB          |
+------------------+-----------------+----------------+
| 4,000 x 4,000    | 60MB            | 600MB          |
+------------------+-----------------+----------------+
| 8,000 x 8,000    | 240MB           | 2.4GB          |
+------------------+-----------------+----------------+
| 10,000 x 10,000  | 380MB           | 3.8GB          |
+------------------+-----------------+----------------+
| 20,000 x 20,000  | 1.5GB           | 15GB           |
+------------------+-----------------+----------------+

.. warning::
   These are estimates. Actual usage varies based on layer content and application overhead.

Choosing the Right Version
==========================

Choose 32-bit if:
-----------------

* Your Windows is 32-bit
* You primarily work on canvases under 5,000 x 5,000 pixels
* Your system has 4GB RAM or less
* You need maximum compatibility

Choose 64-bit if:
-----------------

* Your Windows is 64-bit
* You create large illustrations or posters
* You work with many layers
* Your system has 8GB+ RAM
* You do print-resolution work

Workflow Recommendations
========================

For Print Work
--------------

**Resolution guidelines for print:**

* **Standard print (300 DPI):**
  
  * A4 (8.5" x 11"): 2550 x 3300 pixels
  * A3 (11" x 17"): 3300 x 5100 pixels
  * Poster (24" x 36"): 7200 x 10800 pixels

* **High-quality print (600 DPI):**
  
  * Requires 64-bit for anything larger than A4

For Web/Digital
---------------

**Common digital sizes:**

* Social media: 1200 x 1200 to 4000 x 4000
* Wallpapers: 1920 x 1080 to 3840 x 2160
* Web comics: 800 x 1200 to 2000 x 3000

These sizes work well with both 32-bit and 64-bit versions.

Working with Large Canvases
===========================

Tips for Large Files
--------------------

1. **Use 64-bit version** - Essential for canvases over 10,000 pixels
2. **Have sufficient RAM** - At least 16GB for very large files
3. **Use SSD scratch disk** - Faster temp file handling
4. **Save frequently** - Large files are more prone to issues
5. **Flatten when possible** - Merge completed layer groups

Managing Layers Efficiently
---------------------------

* Group and merge finished sections
* Use clipping layers instead of many overlay layers
* Delete unused layers
* Export layer groups separately for backup

Performance Considerations
==========================

Brush Performance
-----------------

Larger canvases mean slower brush strokes because:

* More pixels to calculate per stroke
* More memory to access
* More data to render

**Mitigation:**

* Use smaller brush sizes when possible
* Reduce brush density for sketching
* Work on smaller sections when detailing

Zoom and Pan
------------

* Zooming out on large canvases may be slow
* Consider working at 50-100% zoom for smooth navigation

Practical Limits
================

Even with 64-bit version and ample RAM, practical limits exist:

+-----------+------------------+---------------------------+
| RAM       | Comfortable Limit| Maximum Practical         |
+===========+==================+===========================+
| 8GB       | 15,000 x 15,000  | 20,000 x 20,000           |
+-----------+------------------+---------------------------+
| 16GB      | 25,000 x 25,000  | 35,000 x 35,000           |
+-----------+------------------+---------------------------+
| 32GB      | 40,000 x 40,000  | 60,000 x 60,000           |
+-----------+------------------+---------------------------+
| 64GB+     | 60,000 x 60,000  | 100,000 x 100,000         |
+-----------+------------------+---------------------------+

.. tip::
   These limits assume working with 10-20 layers. More layers require more memory.

Migration Between Versions
==========================

Files created in 32-bit can be opened in 64-bit and vice versa, with some considerations:

* **.sai files** - Fully compatible between versions
* **Settings** - May need to be reconfigured
* **Brushes** - Copy brush folders between installations

See Also
========

* :doc:`system-requirements`
* :doc:`../getting-started/installation-guide-no-installer`
* :doc:`../getting-started/paint-tool-sai-2-technical-preview`
