=====================================
Installation Guide (No Installer)
=====================================

.. meta::
   :description: How to install Paint Tool SAI 2 without a traditional installer. Extract and run guide for SAI 2.
   :keywords: paint tool sai 2, installation, no installer, extract, setup guide

Paint Tool SAI 2 uses a **portable installation method** rather than a traditional installer. This means you simply extract the downloaded archive and run the executable directly.

.. note::
   This portable approach allows you to run SAI 2 from any location, including USB drives.

Before You Begin
================

Ensure you have:

* Downloaded the latest SAI 2 Technical Preview from the official website
* A file extraction tool (Windows 10/11 has built-in ZIP support)
* Administrator access (recommended for first-time setup)
* Sufficient disk space (100MB minimum, plus scratch disk space)

Step-by-Step Installation
=========================

Step 1: Download
----------------

1. Visit the `SYSTEMAX official website <https://www.systemax.jp/en/sai/>`_
2. Navigate to the SAI 2 download section
3. Choose your version:
   
   * **64-bit** - Recommended for modern systems
   * **32-bit** - For older Windows installations

4. Download the ZIP archive

Step 2: Extract Files
---------------------

1. Locate the downloaded ZIP file (usually in your Downloads folder)
2. Right-click the ZIP file
3. Select **Extract All...** or use your preferred extraction tool
4. Choose a destination folder, for example:

   * ``C:\Program Files\SAI2\`` (requires admin rights)
   * ``C:\Users\YourName\SAI2\`` (no admin required)
   * ``D:\Art Software\SAI2\``

5. Click **Extract**

.. warning::
   Avoid extracting to folders with special characters or very long paths.

Step 3: First Launch
--------------------

1. Open the extracted folder
2. Locate ``sai2.exe``
3. Double-click to launch

   .. tip::
      Right-click ``sai2.exe`` and select **Run as administrator** for the first launch.

4. SAI 2 will create necessary configuration files on first run

Step 4: Create a Shortcut (Optional)
------------------------------------

1. Right-click ``sai2.exe``
2. Select **Create shortcut**
3. Move the shortcut to your Desktop or Start Menu

Folder Structure
================

After extraction, your SAI 2 folder should contain:

::

   SAI2/
   ├── sai2.exe          # Main application
   ├── sai2_x86.exe      # 32-bit version (if included)
   ├── blotmap/          # Brush textures
   ├── brushtex/         # Additional brush textures
   ├── elemap/           # Element maps
   ├── papertex/         # Paper textures
   ├── scatter/          # Scatter brush data
   └── toolink/          # Tool settings

Configuration Files
===================

SAI 2 stores configuration in the following locations:

* **User settings:** Within the SAI2 installation folder
* **License certificate:** In the installation folder
* **Scratch disk (temp files):** Configurable in SAI settings

Updating SAI 2
==============

To update to a newer version:

1. **Backup custom content:**
   
   * Copy your custom brushes
   * Export tool presets
   * Save any custom textures

2. **Download new version**

3. **Extract to a new folder** (don't overwrite immediately)

4. **Copy custom content** to the new installation

5. **Test the new version**

6. **Keep the old version** as backup until verified

Troubleshooting
===============

Application Won't Start
-----------------------

**Solution:** Install the latest Visual C++ Redistributable:

1. Download from Microsoft's website
2. Install both x86 and x64 versions
3. Restart your computer
4. Try launching SAI 2 again

Missing DLL Errors
------------------

**Common DLLs and solutions:**

* ``MSVCP140.dll`` - Install Visual C++ 2015-2022 Redistributable
* ``VCRUNTIME140.dll`` - Same as above
* ``api-ms-win-*.dll`` - Update Windows or install Windows Updates

Tablet Not Detected
-------------------

1. Ensure tablet drivers are installed
2. Check that WinTab or TabletPC API is enabled in tablet settings
3. Restart SAI 2 after connecting the tablet
4. Try running SAI 2 as administrator

Slow Performance
----------------

1. Check :doc:`../tech/system-requirements`
2. Close other applications
3. Increase scratch disk space in SAI settings
4. Consider using the 64-bit version for large canvases

Uninstallation
==============

To completely remove SAI 2:

1. Close SAI 2 if running
2. Delete the SAI2 folder
3. Remove any created shortcuts
4. (Optional) Clean scratch disk location

.. note::
   Since there's no installer, there are no registry entries to clean up.

See Also
========

* :doc:`paint-tool-sai-2-technical-preview`
* :doc:`license-activation-transfer`
* :doc:`../tech/system-requirements`
