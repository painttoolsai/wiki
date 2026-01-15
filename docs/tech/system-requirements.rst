===================
System Requirements
===================

.. meta::
   :description: System requirements for Paint Tool SAI 1 and 2. Minimum and recommended specifications for optimal performance.
   :keywords: paint tool sai, system requirements, specifications, windows, hardware

This page details the minimum and recommended system requirements for running Paint Tool SAI Ver.1 and Ver.2 effectively.

.. note::
   Requirements vary based on canvas size and complexity. Larger canvases require more RAM and processing power.

Quick Reference
===============

+------------------+------------------------+---------------------------+
| Component        | Minimum                | Recommended               |
+==================+========================+===========================+
| Operating System | Windows XP             | Windows 10/11             |
+------------------+------------------------+---------------------------+
| CPU              | Core 2 Duo 1.6GHz      | Intel Core i5 or better   |
+------------------+------------------------+---------------------------+
| RAM              | 1GB                    | 8GB+                      |
+------------------+------------------------+---------------------------+
| Storage          | 100MB (install)        | SSD with 20GB+ free       |
+------------------+------------------------+---------------------------+
| Graphics         | Any DirectX 9 capable  | Dedicated GPU             |
+------------------+------------------------+---------------------------+
| Input Device     | Mouse                  | Pen Tablet                |
+------------------+------------------------+---------------------------+

Operating System
================

Supported Windows Versions
--------------------------

* Windows XP (Service Pack 3)
* Windows Vista
* Windows 7
* Windows 8 / 8.1
* Windows 10
* Windows 11

.. warning::
   Paint Tool SAI is **Windows only**. There is no official macOS or Linux version.

32-bit vs 64-bit Windows
------------------------

* **32-bit Windows:** Can only run SAI 32-bit version
* **64-bit Windows:** Can run both versions (64-bit recommended)

Processor (CPU)
===============

Minimum Requirements
--------------------

* **Intel:** Core 2 Duo 1.6GHz or better
* **AMD:** Equivalent Athlon X2 or better

Recommended for Large Canvases
------------------------------

* **Intel:** Core i5 6th generation or newer
* **AMD:** Ryzen 5 or better
* Higher clock speeds benefit brush response

.. tip::
   SAI is optimized for single-thread performance. Higher single-core clock speeds provide better brush responsiveness.

Memory (RAM)
============

For Different Canvas Sizes
--------------------------

+------------------+-------------+------------------+
| Canvas Size      | Minimum RAM | Recommended      |
+==================+=============+==================+
| Up to 2000px     | 1GB         | 4GB              |
+------------------+-------------+------------------+
| Up to 5000px     | 2GB         | 8GB              |
+------------------+-------------+------------------+
| Up to 10000px    | 4GB         | 16GB             |
+------------------+-------------+------------------+
| 10000px+ (64-bit)| 8GB         | 32GB             |
+------------------+-------------+------------------+

.. important::
   The 32-bit version is limited to approximately 3GB RAM regardless of installed memory This is a Windows limitation for 32-bit applications.

Storage
=======

Installation Space
------------------

* **SAI Ver.1:** ~50MB
* **SAI Ver.2:** ~100MB
* **Brushes & Textures:** Variable (50MB - 500MB typical)

Scratch Disk Space
------------------

SAI uses temporary files during editing:

* **Minimum:** 5GB free space
* **Recommended:** 20GB+ on SSD

.. tip::
   Using an SSD for scratch disk significantly improves performance when working with large files.

Graphics
========

General Requirements
--------------------

* DirectX 9.0c compatible graphics
* Any modern integrated or dedicated GPU
* Display resolution: 1024x768 minimum

.. note::
   SAI primarily uses CPU for brush calculations. GPU is mainly for display.

Display Recommendations
-----------------------

* **Resolution:** 1920x1080 or higher
* **Color Accuracy:** IPS panel for color-sensitive work
* **Calibration:** Use color management for professional work

Input Devices
=============

Supported Tablet APIs
---------------------

Paint Tool SAI supports two tablet APIs:

1. **WinTab** - Traditional tablet API
   
   * Supported by most professional tablets
   * Wacom, XP-Pen, Huion, etc.

2. **TabletPC** - Windows Ink compatible
   
   * Built into Windows
   * Supports touch and pen

Recommended Tablets
-------------------

Any graphics tablet with pressure sensitivity:

* **Wacom:** Intuos, Cintiq series
* **XP-Pen:** Deco, Artist series
* **Huion:** Inspiroy, Kamvas series
* **Others:** Any WinTab or TabletPC compatible

.. warning::
   Mouse can be used but lacks pressure sensitivity essential for digital painting.

Performance Optimization
========================

For Best Performance
--------------------

1. **Use 64-bit version** on 64-bit Windows
2. **Close background applications** while painting
3. **Use SSD** for scratch disk
4. **Keep 30%+ disk space free** on scratch drive
5. **Update tablet drivers** regularly

For Large Canvases
------------------

* Increase RAM allocation if possible
* Use fewer layers when feasible
* Flatten completed sections
* Save frequently to prevent data loss

Compatibility Notes
===================

Virtualization
--------------

SAI may have issues running in:

* Virtual machines (VMware, VirtualBox)
* Windows compatibility modes
* Wine (Linux/macOS)

Antivirus Software
------------------

Some antivirus programs may flag SAI incorrectly:

* Add SAI folder to antivirus exclusions
* Exclude ``sai2.exe`` from real-time scanning

See Also
========

* :doc:`32bit-vs-64bit-canvas-limits`
* :doc:`../getting-started/installation-guide-no-installer`
* :doc:`../getting-started/paint-tool-sai-2-technical-preview`
