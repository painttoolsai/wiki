=============================
SAI Ver.1 Critical Bug Fix
=============================

.. meta::
   :description: Critical bug fix for Paint Tool SAI Ver.1.2.5 and earlier. Prevent data loss during file saving operations.
   :keywords: paint tool sai, bug fix, ver 1.2.5, ver 1.2.6, data loss, critical update

.. danger::
   **CRITICAL UPDATE REQUIRED:** Users running SAI Ver.1.2.5 or earlier versions must update immediately to prevent potential data loss.

Overview
========

A critical bug was discovered in Paint Tool SAI Version 1.2.5 and earlier that could cause **data loss during file saving operations** in rare circumstances. This issue has been addressed in **Ver.1.2.6-Beta.3**.

Affected Versions
=================

The following versions are affected:

* SAI Ver.1.2.5
* SAI Ver.1.2.4
* SAI Ver.1.2.3
* All earlier versions

.. important::
   If you are using any of the above versions, please update to Ver.1.2.6-Beta.3 immediately.

What Is the Bug?
================

The bug can occur during the file saving process when:

* Saving to a network drive with unstable connection
* Saving very large files (100+ layers)
* System resources are constrained during save operation

In these rare cases, the save operation could fail silently or produce a corrupted file without proper error notification.

Symptoms
--------

* Files appear to save successfully but are corrupted when reopened
* Unexpected file size (significantly smaller than expected)
* Error messages when opening previously saved files
* Loss of layer data or canvas content

How to Update
=============

Step 1: Backup Your Work
------------------------

Before updating, backup all your current projects:

1. Locate your SAI installation folder
2. Copy all ``.sai`` and ``.psd`` files to a safe location
3. Export important brushes and materials

Step 2: Download the Update
---------------------------

1. Visit the `official SYSTEMAX website <https://www.systemax.jp/en/sai/>`_
2. Download **Ver.1.2.6-Beta.3**
3. Save the file to an accessible location

Step 3: Install the Update
--------------------------

1. Close Paint Tool SAI completely
2. Extract the new version to a new folder (do not overwrite the old version initially)
3. Copy your custom brushes and settings from the old installation
4. Test the new version with your backed-up files
5. Once verified working, you may remove the old installation

Verification
============

To verify your version after updating:

1. Launch Paint Tool SAI
2. Go to **Help** → **About**
3. Confirm the version shows **Ver.1.2.6-Beta.3** or later

.. tip::
   Always keep a backup copy of your brush textures and custom settings before any update.

Prevention Tips
===============

To minimize data loss risks:

* **Save frequently** - Enable autosave if available
* **Save locally first** - Avoid saving directly to network drives
* **Keep backups** - Maintain multiple backup copies of important work
* **Monitor disk space** - Ensure adequate free space on your save drive

Related Information
===================

* :doc:`paint-tool-sai-2-technical-preview`
* :doc:`installation-guide-no-installer`
* :doc:`../tech/system-requirements`
