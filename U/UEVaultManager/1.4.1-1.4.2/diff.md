# Comparing `tmp/UEVaultManager-1.4.1.tar.gz` & `tmp/UEVaultManager-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UEVaultManager-1.4.1.tar", last modified: Tue May 23 09:48:51 2023, max compression
+gzip compressed data, was "UEVaultManager-1.4.2.tar", last modified: Tue May 23 13:47:27 2023, max compression
```

## Comparing `UEVaultManager-1.4.1.tar` & `UEVaultManager-1.4.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 09:48:51.896564 UEVaultManager-1.4.1/
--rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.4.1/LICENSE
--rw-rw-rw-   0        0        0     5779 2023-05-23 09:48:51.895563 UEVaultManager-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     4948 2023-05-15 08:41:23.000000 UEVaultManager-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 09:48:51.694486 UEVaultManager-1.4.1/UEVaultManager/
--rw-rw-rw-   0        0        0      780 2023-05-23 08:04:27.000000 UEVaultManager-1.4.1/UEVaultManager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:48:51.732999 UEVaultManager-1.4.1/UEVaultManager/api/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.1/UEVaultManager/api/__init__.py
--rw-rw-rw-   0        0        0    25469 2023-05-18 09:30:29.000000 UEVaultManager-1.4.1/UEVaultManager/api/egs.py
--rw-rw-rw-   0        0        0     3142 2023-05-17 13:34:09.000000 UEVaultManager-1.4.1/UEVaultManager/api/uevm.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:48:51.744000 UEVaultManager-1.4.1/UEVaultManager/assets/
--rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.4.1/UEVaultManager/assets/UEVM_200x200.png
--rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.4.1/UEVaultManager/assets/checked_16.png
--rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.4.1/UEVaultManager/assets/main.ico
--rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.4.1/UEVaultManager/assets/unchecked_16.png
--rw-rw-rw-   0        0        0    71745 2023-05-22 10:32:14.000000 UEVaultManager-1.4.1/UEVaultManager/cli.py
--rw-rw-rw-   0        0        0    47574 2023-05-22 13:00:35.000000 UEVaultManager-1.4.1/UEVaultManager/core.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:48:51.758351 UEVaultManager-1.4.1/UEVaultManager/downloader/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.1/UEVaultManager/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:48:51.778368 UEVaultManager-1.4.1/UEVaultManager/downloader/mp/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.1/UEVaultManager/downloader/mp/__init__.py
--rw-rw-rw-   0        0        0    38030 2023-05-15 06:30:52.000000 UEVaultManager-1.4.1/UEVaultManager/downloader/mp/manager.py
--rw-rw-rw-   0        0        0    12365 2023-05-17 13:38:36.000000 UEVaultManager-1.4.1/UEVaultManager/downloader/mp/workers.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:48:51.797370 UEVaultManager-1.4.1/UEVaultManager/lfs/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.1/UEVaultManager/lfs/__init__.py
--rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.4.1/UEVaultManager/lfs/egl.py
--rw-rw-rw-   0        0        0     6428 2023-05-15 06:51:22.000000 UEVaultManager-1.4.1/UEVaultManager/lfs/eos.py
--rw-rw-rw-   0        0        0    23209 2023-05-21 07:37:16.000000 UEVaultManager-1.4.1/UEVaultManager/lfs/uevmlfs.py
--rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.4.1/UEVaultManager/lfs/utils.py
--rw-rw-rw-   0        0        0     3122 2023-05-15 06:51:32.000000 UEVaultManager-1.4.1/UEVaultManager/lfs/windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:48:51.828478 UEVaultManager-1.4.1/UEVaultManager/models/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.1/UEVaultManager/models/__init__.py
--rw-rw-rw-   0        0        0     4269 2023-05-17 13:38:36.000000 UEVaultManager-1.4.1/UEVaultManager/models/app.py
--rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.4.1/UEVaultManager/models/chunk.py
--rw-rw-rw-   0        0        0     2703 2023-05-20 09:18:48.000000 UEVaultManager-1.4.1/UEVaultManager/models/config.py
--rw-rw-rw-   0        0        0     2131 2023-05-22 12:33:51.000000 UEVaultManager-1.4.1/UEVaultManager/models/csv.py
--rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.4.1/UEVaultManager/models/downloading.py
--rw-rw-rw-   0        0        0     5094 2023-05-15 06:33:02.000000 UEVaultManager-1.4.1/UEVaultManager/models/egl.py
--rw-rw-rw-   0        0        0      256 2023-05-20 09:20:19.000000 UEVaultManager-1.4.1/UEVaultManager/models/exceptions.py
--rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.4.1/UEVaultManager/models/json_manifest.py
--rw-rw-rw-   0        0        0    30505 2023-05-17 13:38:36.000000 UEVaultManager-1.4.1/UEVaultManager/models/manifest.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:48:51.838900 UEVaultManager-1.4.1/UEVaultManager/tkgui/
--rw-rw-rw-   0        0        0       16 2023-05-14 16:45:45.000000 UEVaultManager-1.4.1/UEVaultManager/tkgui/__init__.py
--rw-rw-rw-   0        0        0     1123 2023-05-20 07:12:03.000000 UEVaultManager-1.4.1/UEVaultManager/tkgui/main.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:48:51.872552 UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/
--rw-rw-rw-   0        0        0     6948 2023-05-22 15:49:22.000000 UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
--rw-rw-rw-   0        0        0     4843 2023-05-22 17:13:42.000000 UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/EditCellWindowClass.py
--rw-rw-rw-   0        0        0     6832 2023-05-17 14:47:22.000000 UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/EditRowWindowClass.py
--rw-rw-rw-   0        0        0    32447 2023-05-22 17:07:09.000000 UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/EditableTableClass.py
--rw-rw-rw-   0        0        0    14038 2023-05-22 16:36:16.000000 UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
--rw-rw-rw-   0        0        0     2562 2023-05-22 14:44:53.000000 UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/GUISettingsClass.py
--rw-rw-rw-   0        0        0    14228 2023-05-22 12:42:07.000000 UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
--rw-rw-rw-   0        0        0     2251 2023-05-18 09:28:54.000000 UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/SaferDictClass.py
--rw-rw-rw-   0        0        0     6168 2023-05-23 07:32:20.000000 UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
--rw-rw-rw-   0        0        0    42992 2023-05-22 16:55:28.000000 UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/UEVMGuiClass.py
--rw-rw-rw-   0        0        0      543 2023-05-16 16:57:06.000000 UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
--rw-rw-rw-   0        0        0     2230 2023-05-15 10:13:54.000000 UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/WebImageClass.py
--rw-rw-rw-   0        0        0       16 2023-05-14 16:44:57.000000 UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/__init__.py
--rw-rw-rw-   0        0        0    12815 2023-05-20 14:28:39.000000 UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/functions.py
--rw-rw-rw-   0        0        0     2633 2023-05-20 10:13:14.000000 UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/globals.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:48:51.893562 UEVaultManager-1.4.1/UEVaultManager/utils/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.1/UEVaultManager/utils/__init__.py
--rw-rw-rw-   0        0        0     3478 2023-05-17 13:38:36.000000 UEVaultManager-1.4.1/UEVaultManager/utils/aliasing.py
--rw-rw-rw-   0        0        0     5897 2023-05-18 09:32:02.000000 UEVaultManager-1.4.1/UEVaultManager/utils/cli.py
--rw-rw-rw-   0        0        0     1342 2023-05-15 06:55:20.000000 UEVaultManager-1.4.1/UEVaultManager/utils/custom_parser.py
--rw-rw-rw-   0        0        0    10286 2023-05-15 06:33:02.000000 UEVaultManager-1.4.1/UEVaultManager/utils/egl_crypt.py
--rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.4.1/UEVaultManager/utils/env.py
--rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.4.1/UEVaultManager/utils/rolling_hash.py
--rw-rw-rw-   0        0        0     7260 2023-05-17 13:34:09.000000 UEVaultManager-1.4.1/UEVaultManager/utils/webview_login.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:48:51.717986 UEVaultManager-1.4.1/UEVaultManager.egg-info/
--rw-rw-rw-   0        0        0     5779 2023-05-23 09:48:51.000000 UEVaultManager-1.4.1/UEVaultManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2295 2023-05-23 09:48:51.000000 UEVaultManager-1.4.1/UEVaultManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 09:48:51.000000 UEVaultManager-1.4.1/UEVaultManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-23 09:48:51.000000 UEVaultManager-1.4.1/UEVaultManager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      286 2023-05-23 09:48:51.000000 UEVaultManager-1.4.1/UEVaultManager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-23 09:48:51.000000 UEVaultManager-1.4.1/UEVaultManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 09:48:51.896564 UEVaultManager-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     2951 2023-05-23 08:03:04.000000 UEVaultManager-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.929815 UEVaultManager-1.4.2/
+-rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.4.2/LICENSE
+-rw-rw-rw-   0        0        0     6130 2023-05-23 13:47:27.928817 UEVaultManager-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5286 2023-05-23 12:39:00.000000 UEVaultManager-1.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.768892 UEVaultManager-1.4.2/UEVaultManager/
+-rw-rw-rw-   0        0        0      780 2023-05-23 13:45:32.000000 UEVaultManager-1.4.2/UEVaultManager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.803807 UEVaultManager-1.4.2/UEVaultManager/api/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.2/UEVaultManager/api/__init__.py
+-rw-rw-rw-   0        0        0    25469 2023-05-18 09:30:29.000000 UEVaultManager-1.4.2/UEVaultManager/api/egs.py
+-rw-rw-rw-   0        0        0     3142 2023-05-17 13:34:09.000000 UEVaultManager-1.4.2/UEVaultManager/api/uevm.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.813412 UEVaultManager-1.4.2/UEVaultManager/assets/
+-rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.4.2/UEVaultManager/assets/UEVM_200x200.png
+-rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.4.2/UEVaultManager/assets/checked_16.png
+-rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.4.2/UEVaultManager/assets/main.ico
+-rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.4.2/UEVaultManager/assets/unchecked_16.png
+-rw-rw-rw-   0        0        0    71745 2023-05-22 10:32:14.000000 UEVaultManager-1.4.2/UEVaultManager/cli.py
+-rw-rw-rw-   0        0        0    47574 2023-05-22 13:00:35.000000 UEVaultManager-1.4.2/UEVaultManager/core.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.820414 UEVaultManager-1.4.2/UEVaultManager/downloader/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.2/UEVaultManager/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.833412 UEVaultManager-1.4.2/UEVaultManager/downloader/mp/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.2/UEVaultManager/downloader/mp/__init__.py
+-rw-rw-rw-   0        0        0    38030 2023-05-15 06:30:52.000000 UEVaultManager-1.4.2/UEVaultManager/downloader/mp/manager.py
+-rw-rw-rw-   0        0        0    12365 2023-05-17 13:38:36.000000 UEVaultManager-1.4.2/UEVaultManager/downloader/mp/workers.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.850622 UEVaultManager-1.4.2/UEVaultManager/lfs/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.2/UEVaultManager/lfs/__init__.py
+-rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.4.2/UEVaultManager/lfs/egl.py
+-rw-rw-rw-   0        0        0     6428 2023-05-15 06:51:22.000000 UEVaultManager-1.4.2/UEVaultManager/lfs/eos.py
+-rw-rw-rw-   0        0        0    23209 2023-05-21 07:37:16.000000 UEVaultManager-1.4.2/UEVaultManager/lfs/uevmlfs.py
+-rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.4.2/UEVaultManager/lfs/utils.py
+-rw-rw-rw-   0        0        0     3122 2023-05-15 06:51:32.000000 UEVaultManager-1.4.2/UEVaultManager/lfs/windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.872621 UEVaultManager-1.4.2/UEVaultManager/models/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.2/UEVaultManager/models/__init__.py
+-rw-rw-rw-   0        0        0     4269 2023-05-17 13:38:36.000000 UEVaultManager-1.4.2/UEVaultManager/models/app.py
+-rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.4.2/UEVaultManager/models/chunk.py
+-rw-rw-rw-   0        0        0     2703 2023-05-20 09:18:48.000000 UEVaultManager-1.4.2/UEVaultManager/models/config.py
+-rw-rw-rw-   0        0        0     2131 2023-05-22 12:33:51.000000 UEVaultManager-1.4.2/UEVaultManager/models/csv.py
+-rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.4.2/UEVaultManager/models/downloading.py
+-rw-rw-rw-   0        0        0     5094 2023-05-15 06:33:02.000000 UEVaultManager-1.4.2/UEVaultManager/models/egl.py
+-rw-rw-rw-   0        0        0      256 2023-05-20 09:20:19.000000 UEVaultManager-1.4.2/UEVaultManager/models/exceptions.py
+-rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.4.2/UEVaultManager/models/json_manifest.py
+-rw-rw-rw-   0        0        0    30505 2023-05-17 13:38:36.000000 UEVaultManager-1.4.2/UEVaultManager/models/manifest.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.880280 UEVaultManager-1.4.2/UEVaultManager/tkgui/
+-rw-rw-rw-   0        0        0       16 2023-05-14 16:45:45.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/__init__.py
+-rw-rw-rw-   0        0        0     1123 2023-05-20 07:12:03.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/main.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.908470 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/
+-rw-rw-rw-   0        0        0     6667 2023-05-23 13:36:34.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
+-rw-rw-rw-   0        0        0     4562 2023-05-23 13:37:02.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/EditCellWindowClass.py
+-rw-rw-rw-   0        0        0     6553 2023-05-23 13:36:54.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/EditRowWindowClass.py
+-rw-rw-rw-   0        0        0    32447 2023-05-22 17:07:09.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/EditableTableClass.py
+-rw-rw-rw-   0        0        0    14038 2023-05-22 16:36:16.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
+-rw-rw-rw-   0        0        0     2562 2023-05-22 14:44:53.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/GUISettingsClass.py
+-rw-rw-rw-   0        0        0    13947 2023-05-23 13:37:12.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
+-rw-rw-rw-   0        0        0     2251 2023-05-18 09:28:54.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/SaferDictClass.py
+-rw-rw-rw-   0        0        0     6168 2023-05-23 07:32:20.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
+-rw-rw-rw-   0        0        0    42713 2023-05-23 13:39:57.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/UEVMGuiClass.py
+-rw-rw-rw-   0        0        0      543 2023-05-16 16:57:06.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
+-rw-rw-rw-   0        0        0     2230 2023-05-15 10:13:54.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/WebImageClass.py
+-rw-rw-rw-   0        0        0       16 2023-05-14 16:44:57.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/__init__.py
+-rw-rw-rw-   0        0        0    14641 2023-05-23 13:35:44.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/functions.py
+-rw-rw-rw-   0        0        0     2631 2023-05-23 13:39:29.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/globals.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.927815 UEVaultManager-1.4.2/UEVaultManager/utils/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.2/UEVaultManager/utils/__init__.py
+-rw-rw-rw-   0        0        0     3478 2023-05-17 13:38:36.000000 UEVaultManager-1.4.2/UEVaultManager/utils/aliasing.py
+-rw-rw-rw-   0        0        0     5897 2023-05-18 09:32:02.000000 UEVaultManager-1.4.2/UEVaultManager/utils/cli.py
+-rw-rw-rw-   0        0        0     1342 2023-05-15 06:55:20.000000 UEVaultManager-1.4.2/UEVaultManager/utils/custom_parser.py
+-rw-rw-rw-   0        0        0    10286 2023-05-15 06:33:02.000000 UEVaultManager-1.4.2/UEVaultManager/utils/egl_crypt.py
+-rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.4.2/UEVaultManager/utils/env.py
+-rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.4.2/UEVaultManager/utils/rolling_hash.py
+-rw-rw-rw-   0        0        0     7260 2023-05-17 13:34:09.000000 UEVaultManager-1.4.2/UEVaultManager/utils/webview_login.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.791031 UEVaultManager-1.4.2/UEVaultManager.egg-info/
+-rw-rw-rw-   0        0        0     6130 2023-05-23 13:47:27.000000 UEVaultManager-1.4.2/UEVaultManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2295 2023-05-23 13:47:27.000000 UEVaultManager-1.4.2/UEVaultManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 13:47:27.000000 UEVaultManager-1.4.2/UEVaultManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-23 13:47:27.000000 UEVaultManager-1.4.2/UEVaultManager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      286 2023-05-23 13:47:27.000000 UEVaultManager-1.4.2/UEVaultManager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-23 13:47:27.000000 UEVaultManager-1.4.2/UEVaultManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 13:47:27.929815 UEVaultManager-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     3008 2023-05-23 12:39:50.000000 UEVaultManager-1.4.2/setup.py
```

### Comparing `UEVaultManager-1.4.1/LICENSE` & `UEVaultManager-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/PKG-INFO` & `UEVaultManager-1.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.4.1
+Version: 1.4.2
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: webview
 Provides-Extra: webview_gtk
 License-File: LICENSE
 
 Welcome to UEVaultManager
@@ -30,21 +30,26 @@
 their data from the Epic Games Marketplace. It is developed in Python, so
 it can run on any platform that support this language.
 
 Its main purpose is to list the assets (with or without user login),
 filter (optional) and save the list into a file that can be reused later
 as a data source (in an Excel sheet for instance).
 
-**This project is under active development**
+| Hot news                                                                                                                                                                                         |                                                                                                           |
+|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------|
+| The new version is out : Now with a GUI !<br/>Edit the data in the GUI and save it back to the file<br/>Use colors to visualize your asset status<br/>Use filters and search to find them easily | [![preview](https://i.imgur.com/dXS62o4.png)](https://uevaultmanager.readthedocs.io/en/latest/tkgui.html) |
+
+**This project is still under active development**                                                                    |
 
 To go further, dive into [the documentation](https://uevaultmanager.readthedocs.io/en/latest/index.html) or just go
 for [a quickstart](https://uevaultmanager.readthedocs.io/en/latest/quickstart.html)
 
 Contents:
 
+* [Hot new feature !](https://uevaultmanager.readthedocs.io/en/latest/tkgui.html)
 * [UEVaultManager](https://uevaultmanager.readthedocs.io/en/latest/intro.html)
   * [A free and open-source Epic Games Assets Manager for Unreal Engine](https://uevaultmanager.readthedocs.io/en/latest/intro.html#a-free-and-open-source-epic-games-assets-manager-for-unreal-engine)
   * [Known bugs and limitations](https://uevaultmanager.readthedocs.io/en/latest/intro.html#known-bugs-and-limitations)
 * [Quickstart](https://uevaultmanager.readthedocs.io/en/latest/quickstart.html)
   * [Installation](https://uevaultmanager.readthedocs.io/en/latest/quickstart.html#installation)
   * [log in](https://uevaultmanager.readthedocs.io/en/latest/quickstart.html#log-in)
   * [Listing your asset](https://uevaultmanager.readthedocs.io/en/latest/quickstart.html#listing-your-asset)
@@ -54,18 +59,12 @@
   * [Prerequisites](https://uevaultmanager.readthedocs.io/en/latest/setup.html#prerequisites)
   * [Directly from the repo](https://uevaultmanager.readthedocs.io/en/latest/setup.html#directly-from-the-repo)
   * [Direct installation (any)](https://uevaultmanager.readthedocs.io/en/latest/setup.html#direct-installation-any)
 * [Usage](https://uevaultmanager.readthedocs.io/en/latest/usage.html)
 * [Configuration](https://uevaultmanager.readthedocs.io/en/latest/configuration.html)
   * [Config folder](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-folder)
   * [Config file](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-file)
-* [Output Format and file](https://uevaultmanager.readthedocs.io/en/latest/output.html)
-  * [Log files and debug](https://uevaultmanager.readthedocs.io/en/latest/output.html#log-files-and-debug)
-  * [The output file](https://uevaultmanager.readthedocs.io/en/latest/output.html#the-output-file)
-  * [The individual json files](https://uevaultmanager.readthedocs.io/en/latest/output.html#the-individual-json-files)
-  * [how to fix invalid search result during the grabbing process](https://uevaultmanager.readthedocs.io/en/latest/output.html#how-to-fix-invalid-search-result-during-the-grabbing-process)
-  * [possible values in the error Field](https://uevaultmanager.readthedocs.io/en/latest/output.html#possible-values-in-the-error-field)
 
-[Next](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
+[More info](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
 
 
- UEVaultManager ## version:1.4.1 ## codename: Phoenix+1
+ UEVaultManager ## version:1.4.2 ## codename: Phoenix+2
```

### Comparing `UEVaultManager-1.4.1/README.md` & `UEVaultManager-1.4.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -10,21 +10,26 @@
 their data from the Epic Games Marketplace. It is developed in Python, so
 it can run on any platform that support this language.
 
 Its main purpose is to list the assets (with or without user login),
 filter (optional) and save the list into a file that can be reused later
 as a data source (in an Excel sheet for instance).
 
-**This project is under active development**
+| Hot news                                                                                                                                                                                         |                                                                                                           |
+|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------|
+| The new version is out : Now with a GUI !<br/>Edit the data in the GUI and save it back to the file<br/>Use colors to visualize your asset status<br/>Use filters and search to find them easily | [![preview](https://i.imgur.com/dXS62o4.png)](https://uevaultmanager.readthedocs.io/en/latest/tkgui.html) |
+
+**This project is still under active development**                                                                    |
 
 To go further, dive into [the documentation](https://uevaultmanager.readthedocs.io/en/latest/index.html) or just go
 for [a quickstart](https://uevaultmanager.readthedocs.io/en/latest/quickstart.html)
 
 Contents:
 
+* [Hot new feature !](https://uevaultmanager.readthedocs.io/en/latest/tkgui.html)
 * [UEVaultManager](https://uevaultmanager.readthedocs.io/en/latest/intro.html)
   * [A free and open-source Epic Games Assets Manager for Unreal Engine](https://uevaultmanager.readthedocs.io/en/latest/intro.html#a-free-and-open-source-epic-games-assets-manager-for-unreal-engine)
   * [Known bugs and limitations](https://uevaultmanager.readthedocs.io/en/latest/intro.html#known-bugs-and-limitations)
 * [Quickstart](https://uevaultmanager.readthedocs.io/en/latest/quickstart.html)
   * [Installation](https://uevaultmanager.readthedocs.io/en/latest/quickstart.html#installation)
   * [log in](https://uevaultmanager.readthedocs.io/en/latest/quickstart.html#log-in)
   * [Listing your asset](https://uevaultmanager.readthedocs.io/en/latest/quickstart.html#listing-your-asset)
@@ -34,15 +39,9 @@
   * [Prerequisites](https://uevaultmanager.readthedocs.io/en/latest/setup.html#prerequisites)
   * [Directly from the repo](https://uevaultmanager.readthedocs.io/en/latest/setup.html#directly-from-the-repo)
   * [Direct installation (any)](https://uevaultmanager.readthedocs.io/en/latest/setup.html#direct-installation-any)
 * [Usage](https://uevaultmanager.readthedocs.io/en/latest/usage.html)
 * [Configuration](https://uevaultmanager.readthedocs.io/en/latest/configuration.html)
   * [Config folder](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-folder)
   * [Config file](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-file)
-* [Output Format and file](https://uevaultmanager.readthedocs.io/en/latest/output.html)
-  * [Log files and debug](https://uevaultmanager.readthedocs.io/en/latest/output.html#log-files-and-debug)
-  * [The output file](https://uevaultmanager.readthedocs.io/en/latest/output.html#the-output-file)
-  * [The individual json files](https://uevaultmanager.readthedocs.io/en/latest/output.html#the-individual-json-files)
-  * [how to fix invalid search result during the grabbing process](https://uevaultmanager.readthedocs.io/en/latest/output.html#how-to-fix-invalid-search-result-during-the-grabbing-process)
-  * [possible values in the error Field](https://uevaultmanager.readthedocs.io/en/latest/output.html#possible-values-in-the-error-field)
 
-[Next](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
+[More info](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
```

### Comparing `UEVaultManager-1.4.1/UEVaultManager/__init__.py` & `UEVaultManager-1.4.2/UEVaultManager/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 UEVaultManager setup file.
 """
 import datetime
 
 year = datetime.date.today().year
 
 __name__ = 'UEVaultManager'
-__version__ = '1.4.1'
+__version__ = '1.4.2'
 # 0 Pegasus Seiya
 # 1 Dragon Shiryu
 # 2 Cygnus Hyoga
 # 3 Andromeda Shun
 # 4 Phoenix Ikki
-__codename__ = 'Phoenix+1'
+__codename__ = 'Phoenix+2'
 # 5 Leo Aiolia
 # 5 Virgo Shaka
 # 6 Libra Dohko
 # 7 Scorpio Milo
 # 8 Sagittarius Aiolos
 # 9 Capricorn Shura
 # 10 Aquarius Camus
```

### Comparing `UEVaultManager-1.4.1/UEVaultManager/api/egs.py` & `UEVaultManager-1.4.2/UEVaultManager/api/egs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/api/uevm.py` & `UEVaultManager-1.4.2/UEVaultManager/api/uevm.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/assets/UEVM_200x200.png` & `UEVaultManager-1.4.2/UEVaultManager/assets/UEVM_200x200.png`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/assets/main.ico` & `UEVaultManager-1.4.2/UEVaultManager/assets/main.ico`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/cli.py` & `UEVaultManager-1.4.2/UEVaultManager/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/core.py` & `UEVaultManager-1.4.2/UEVaultManager/core.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/downloader/mp/manager.py` & `UEVaultManager-1.4.2/UEVaultManager/downloader/mp/manager.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/downloader/mp/workers.py` & `UEVaultManager-1.4.2/UEVaultManager/downloader/mp/workers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/lfs/egl.py` & `UEVaultManager-1.4.2/UEVaultManager/lfs/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/lfs/eos.py` & `UEVaultManager-1.4.2/UEVaultManager/lfs/eos.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/lfs/uevmlfs.py` & `UEVaultManager-1.4.2/UEVaultManager/lfs/uevmlfs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/lfs/utils.py` & `UEVaultManager-1.4.2/UEVaultManager/lfs/utils.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/lfs/windows_helpers.py` & `UEVaultManager-1.4.2/UEVaultManager/lfs/windows_helpers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/models/app.py` & `UEVaultManager-1.4.2/UEVaultManager/models/app.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/models/chunk.py` & `UEVaultManager-1.4.2/UEVaultManager/models/chunk.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/models/config.py` & `UEVaultManager-1.4.2/UEVaultManager/models/config.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/models/csv.py` & `UEVaultManager-1.4.2/UEVaultManager/models/csv.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/models/downloading.py` & `UEVaultManager-1.4.2/UEVaultManager/models/downloading.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/models/egl.py` & `UEVaultManager-1.4.2/UEVaultManager/models/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/models/json_manifest.py` & `UEVaultManager-1.4.2/UEVaultManager/models/json_manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/models/manifest.py` & `UEVaultManager-1.4.2/UEVaultManager/models/manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/tkgui/main.py` & `UEVaultManager-1.4.2/UEVaultManager/tkgui/main.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py` & `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,22 +40,15 @@
         #     style = ttk.Style(tk._default_root)
         #     print(f"style ROOT = {style.theme_use()}")
         #
         # self.style = style
 
         geometry = gui_f.center_window_on_screen(screen_index, height, width)
         self.geometry(geometry)
-
-        if icon is None:
-            self.attributes('-toolwindow', True)
-        else:
-            # windows only (remove the minimize/maximize buttons and the icon)
-            icon = gui_f.path_from_relative_to_absolute(icon)
-            if icon != '' and os.path.isfile(icon):
-                self.iconbitmap(icon)
+        gui_f.set_icon_and_minmax(self, icon)
         self.resizable(True, False)
         self.quit_on_close = quit_on_close
         self.keep_existing = False  # whether to keep the existing content when adding a new one
         self.content_frame = self.ContentFrame(self)
         self.control_frame = self.ControlFrame(self)
 
         self.content_frame.pack(ipadx=5, ipady=5, padx=5, pady=5, fill=tk.X)
```

### Comparing `UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/EditCellWindowClass.py` & `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/EditCellWindowClass.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,22 +28,15 @@
     def __init__(self, parent, title: str, width: int = 600, height: int = 400, icon=None, screen_index=0, editable_table=None):
         super().__init__(parent)
         self.title(title)
         style = gui_f.set_custom_style(gui_g.s.theme_name, gui_g.s.theme_font)
         self.style = style
         geometry = gui_f.center_window_on_screen(screen_index, height, width)
         self.geometry(geometry)
-
-        if icon is None:
-            self.attributes('-toolwindow', True)
-        else:
-            # windows only (remove the minimize/maximize buttons and the icon)
-            icon = gui_f.path_from_relative_to_absolute(icon)
-            if icon != '' and os.path.isfile(icon):
-                self.iconbitmap(icon)
+        gui_f.set_icon_and_minmax(self, icon)
         self.resizable(True, False)
 
         self.editable_table = editable_table
         self.must_save = False
         self.initial_values = []
 
         self.content_frame = self.ContentFrame(self)
```

### Comparing `UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/EditRowWindowClass.py` & `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/EditRowWindowClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,21 +28,15 @@
     def __init__(self, parent, title: str, width: int = 600, height: int = 800, icon=None, screen_index: int = 0, editable_table=None):
         super().__init__(parent)
         self.title(title)
         style = gui_f.set_custom_style(gui_g.s.theme_name, gui_g.s.theme_font)
         self.style = style
         geometry = gui_f.center_window_on_screen(screen_index, height, width)
         self.geometry(geometry)
-        if icon is None:
-            self.attributes('-toolwindow', True)
-        else:
-            # windows only (remove the minimize/maximize buttons and the icon)
-            icon = gui_f.path_from_relative_to_absolute(icon)
-            if icon != '' and os.path.isfile(icon):
-                self.iconbitmap(icon)
+        gui_f.set_icon_and_minmax(self, icon)
         self.resizable(True, False)
 
         self.editable_table = editable_table
         self.must_save = False
         self.initial_values = []
         self.width = width
         # the photoimage is stored is the variable to avoid garbage collection
```

### Comparing `UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/EditableTableClass.py` & `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/EditableTableClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py` & `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/GUISettingsClass.py` & `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/GUISettingsClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/ProgressWindowsClass.py` & `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/ProgressWindowsClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,22 +46,15 @@
         function_parameters: dict = None,
         quit_on_close=False
     ):
         super().__init__()
         self.title(title)
         geometry = gui_f.center_window_on_screen(screen_index, height, width)
         self.geometry(geometry)
-
-        if icon is None:
-            self.attributes('-toolwindow', True)
-        else:
-            # windows only (remove the minimize/maximize buttons and the icon)
-            icon = gui_f.path_from_relative_to_absolute(icon)
-            if icon != '' and os.path.isfile(icon):
-                self.iconbitmap(icon)
+        gui_f.set_icon_and_minmax(self, icon)
         self._thread_check_delay = 100
         self.must_end = False
         self.quit_on_close = quit_on_close
         self.max_value = max_value
         self.continue_execution = True
         self.function = function
         self.function_params = function_parameters
```

### Comparing `UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/SaferDictClass.py` & `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/SaferDictClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py` & `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/UEVMGuiClass.py` & `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/UEVMGuiClass.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,21 +32,15 @@
     def __init__(self, title: str, width=1200, height=800, icon='', screen_index=0, file='', show_open_file_dialog=False, rebuild_data=False):
         super().__init__()
         self.title(title)
         style = set_custom_style(gui_g.s.theme_name, gui_g.s.theme_font)
         self.style = style
         geometry = gui_f.center_window_on_screen(screen_index, height, width)
         self.geometry(geometry)
-        if icon is None:
-            self.attributes('-toolwindow', True)
-        else:
-            # windows only (remove the minimize/maximize buttons and the icon)
-            icon = gui_f.path_from_relative_to_absolute(icon)
-            if icon != '' and os.path.isfile(icon):
-                self.iconbitmap(icon)
+        gui_f.set_icon_and_minmax(self, icon)
         self.resizable(True, False)
         self.editable_table = None
         self.do_not_launch_search = False
         pack_def_options = {'ipadx': 5, 'ipady': 5, 'padx': 3, 'pady': 3}
 
         table_frame = self.TableFrame(self)
```

### Comparing `UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py` & `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/WebImageClass.py` & `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/WebImageClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/functions.py` & `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import datetime
 import os
 import time
 import tkinter as tk
 from io import BytesIO
 from tkinter import messagebox
 
+import ctypes as ct
 import requests
 import ttkbootstrap as ttk
 from PIL import ImageTk, Image
 from screeninfo import get_monitors
 from termcolor import colored
 
 from UEVaultManager.tkgui.modules import globals as gui_g
@@ -292,18 +293,61 @@
     # Horizontal.TScrollbar or Vertical.TScrollbar (depending on the orient option)
     style.configure('TLabel', font=font, spacing=1, padding=2)
     style.configure('TButton', font=font, spacing=1, padding=2)
     style.configure('TEntry', font=font, spacing=1, padding=2)
     style.configure('TFrame', font=font, spacing=1, padding=1)
     style.configure('TCombobox', font=font, spacing=1, padding=1)
     style.configure('TLabelFrame', font=font, spacing=1, padding=1)
-
     return style
 
 
+def set_toolbar_style(tk_window) -> None:
+    """
+    Remove the minimize and maximize buttons from a tkinter window.
+    This version is compatible with Windows AND Non-windows OS
+    # see https://stackoverflow.com/questions/2969870/removing-minimize-maximize-buttons-in-tkinter
+    :param tk_window: the tkinter window
+    """
+    set_window_pos = ct.windll.user32.SetWindowPos
+    set_window_long = ct.windll.user32.SetWindowLongPtrW
+    get_window_long = ct.windll.user32.GetWindowLongPtrW
+    get_parent = ct.windll.user32.GetParent
+    # Identifiers
+    gwl_style = -16
+    ws_minimizebox = 131072
+    ws_maximizebox = 65536
+    swp_nozorder = 4
+    swp_nomove = 2
+    swp_nosize = 1
+    swp_framechanged = 32
+    hwnd = get_parent(tk_window.winfo_id())
+    old_style = get_window_long(hwnd, gwl_style)  # Get the style
+    new_style = old_style & ~ws_maximizebox & ~ws_minimizebox  # New style, without max/min buttons
+    set_window_long(hwnd, gwl_style, new_style)  # Apply the new style
+    set_window_pos(hwnd, 0, 0, 0, 0, 0, swp_nomove | swp_nosize | swp_nozorder | swp_framechanged)  # Updates
+
+
+def set_icon_and_minmax(tk_window, icon=None) -> None:
+    """
+    Set the icon and remove the min/max buttons of the window if no icon is provided
+    :param tk_window:
+    :param icon:
+    """
+    if icon is None:
+        # remove the min/max buttons of the window
+        # this code works on Window only
+        # tk_window.attributes('-toolwindow', True)
+        tk_window.after(300, lambda: set_toolbar_style(tk_window))
+    else:
+        # windows only (remove the minimize/maximize buttons and the icon)
+        icon = path_from_relative_to_absolute(icon)
+        if icon != '' and os.path.isfile(icon):
+            tk_window.iconbitmap(icon)
+
+
 def json_print_key_val(json_obj, indent=4, print_result=True, output_on_gui=False) -> None:
     """
     Pretty prints a JSON object in a simple 'key: value' format.
     :param json_obj:  The JSON object to print.
     :param indent: The number of spaces to indent each level.
     :param print_result: Determines whether to print the result.
     :param output_on_gui: Determines whether to print the result on the GUI.
```

### Comparing `UEVaultManager-1.4.1/UEVaultManager/tkgui/modules/globals.py` & `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 #  If empty, log will be message printed in the console
 UEVM_log_ref = None
 #  reference to the default command line parser (used for help button in gui).
 UEVM_parser_ref = None
 
 # global variables
 # noinspection PyTypeChecker
-UEVM_cli_args: SaferDict = None
+UEVM_cli_args: SaferDict = {}
 UEVM_filter_category = ''
 
 s = GUISettings()  # using the shortest variable name for GUISettings for convenience
 
 
 # options that can be changed in the GUI
 def set_args_force_refresh(value: bool) -> None:
```

### Comparing `UEVaultManager-1.4.1/UEVaultManager/utils/aliasing.py` & `UEVaultManager-1.4.2/UEVaultManager/utils/aliasing.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/utils/cli.py` & `UEVaultManager-1.4.2/UEVaultManager/utils/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/utils/custom_parser.py` & `UEVaultManager-1.4.2/UEVaultManager/utils/custom_parser.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/utils/egl_crypt.py` & `UEVaultManager-1.4.2/UEVaultManager/utils/egl_crypt.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/utils/rolling_hash.py` & `UEVaultManager-1.4.2/UEVaultManager/utils/rolling_hash.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager/utils/webview_login.py` & `UEVaultManager-1.4.2/UEVaultManager/utils/webview_login.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/UEVaultManager.egg-info/PKG-INFO` & `UEVaultManager-1.4.2/UEVaultManager.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.4.1
+Version: 1.4.2
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: webview
 Provides-Extra: webview_gtk
 License-File: LICENSE
 
 Welcome to UEVaultManager
@@ -30,21 +30,26 @@
 their data from the Epic Games Marketplace. It is developed in Python, so
 it can run on any platform that support this language.
 
 Its main purpose is to list the assets (with or without user login),
 filter (optional) and save the list into a file that can be reused later
 as a data source (in an Excel sheet for instance).
 
-**This project is under active development**
+| Hot news                                                                                                                                                                                         |                                                                                                           |
+|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------|
+| The new version is out : Now with a GUI !<br/>Edit the data in the GUI and save it back to the file<br/>Use colors to visualize your asset status<br/>Use filters and search to find them easily | [![preview](https://i.imgur.com/dXS62o4.png)](https://uevaultmanager.readthedocs.io/en/latest/tkgui.html) |
+
+**This project is still under active development**                                                                    |
 
 To go further, dive into [the documentation](https://uevaultmanager.readthedocs.io/en/latest/index.html) or just go
 for [a quickstart](https://uevaultmanager.readthedocs.io/en/latest/quickstart.html)
 
 Contents:
 
+* [Hot new feature !](https://uevaultmanager.readthedocs.io/en/latest/tkgui.html)
 * [UEVaultManager](https://uevaultmanager.readthedocs.io/en/latest/intro.html)
   * [A free and open-source Epic Games Assets Manager for Unreal Engine](https://uevaultmanager.readthedocs.io/en/latest/intro.html#a-free-and-open-source-epic-games-assets-manager-for-unreal-engine)
   * [Known bugs and limitations](https://uevaultmanager.readthedocs.io/en/latest/intro.html#known-bugs-and-limitations)
 * [Quickstart](https://uevaultmanager.readthedocs.io/en/latest/quickstart.html)
   * [Installation](https://uevaultmanager.readthedocs.io/en/latest/quickstart.html#installation)
   * [log in](https://uevaultmanager.readthedocs.io/en/latest/quickstart.html#log-in)
   * [Listing your asset](https://uevaultmanager.readthedocs.io/en/latest/quickstart.html#listing-your-asset)
@@ -54,18 +59,12 @@
   * [Prerequisites](https://uevaultmanager.readthedocs.io/en/latest/setup.html#prerequisites)
   * [Directly from the repo](https://uevaultmanager.readthedocs.io/en/latest/setup.html#directly-from-the-repo)
   * [Direct installation (any)](https://uevaultmanager.readthedocs.io/en/latest/setup.html#direct-installation-any)
 * [Usage](https://uevaultmanager.readthedocs.io/en/latest/usage.html)
 * [Configuration](https://uevaultmanager.readthedocs.io/en/latest/configuration.html)
   * [Config folder](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-folder)
   * [Config file](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-file)
-* [Output Format and file](https://uevaultmanager.readthedocs.io/en/latest/output.html)
-  * [Log files and debug](https://uevaultmanager.readthedocs.io/en/latest/output.html#log-files-and-debug)
-  * [The output file](https://uevaultmanager.readthedocs.io/en/latest/output.html#the-output-file)
-  * [The individual json files](https://uevaultmanager.readthedocs.io/en/latest/output.html#the-individual-json-files)
-  * [how to fix invalid search result during the grabbing process](https://uevaultmanager.readthedocs.io/en/latest/output.html#how-to-fix-invalid-search-result-during-the-grabbing-process)
-  * [possible values in the error Field](https://uevaultmanager.readthedocs.io/en/latest/output.html#possible-values-in-the-error-field)
 
-[Next](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
+[More info](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
 
 
- UEVaultManager ## version:1.4.1 ## codename: Phoenix+1
+ UEVaultManager ## version:1.4.2 ## codename: Phoenix+2
```

### Comparing `UEVaultManager-1.4.1/UEVaultManager.egg-info/SOURCES.txt` & `UEVaultManager-1.4.2/UEVaultManager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.1/setup.py` & `UEVaultManager-1.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,13 +63,14 @@
     ]),
     python_requires='>=3.9',
     classifiers=[
         'License :: OSI Approved :: BSD License',  #
         'Programming Language :: Python :: 3.9',  #
         'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11',  #
         'Operating System :: OS Independent',  #
-        'Development Status :: 4 - Beta'
+        'Development Status :: 5 - Production/Stable'
+        # 'Development Status :: 4 - Beta'
     ]
 )
 
 if __name__ == '__main__':
     setup()
```

