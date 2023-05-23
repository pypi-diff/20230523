# Comparing `tmp/UEVaultManager-1.4.2.tar.gz` & `tmp/UEVaultManager-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UEVaultManager-1.4.2.tar", last modified: Tue May 23 13:47:27 2023, max compression
+gzip compressed data, was "UEVaultManager-1.4.3.tar", last modified: Tue May 23 13:51:01 2023, max compression
```

## Comparing `UEVaultManager-1.4.2.tar` & `UEVaultManager-1.4.3.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.929815 UEVaultManager-1.4.2/
--rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.4.2/LICENSE
--rw-rw-rw-   0        0        0     6130 2023-05-23 13:47:27.928817 UEVaultManager-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     5286 2023-05-23 12:39:00.000000 UEVaultManager-1.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.768892 UEVaultManager-1.4.2/UEVaultManager/
--rw-rw-rw-   0        0        0      780 2023-05-23 13:45:32.000000 UEVaultManager-1.4.2/UEVaultManager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.803807 UEVaultManager-1.4.2/UEVaultManager/api/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.2/UEVaultManager/api/__init__.py
--rw-rw-rw-   0        0        0    25469 2023-05-18 09:30:29.000000 UEVaultManager-1.4.2/UEVaultManager/api/egs.py
--rw-rw-rw-   0        0        0     3142 2023-05-17 13:34:09.000000 UEVaultManager-1.4.2/UEVaultManager/api/uevm.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.813412 UEVaultManager-1.4.2/UEVaultManager/assets/
--rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.4.2/UEVaultManager/assets/UEVM_200x200.png
--rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.4.2/UEVaultManager/assets/checked_16.png
--rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.4.2/UEVaultManager/assets/main.ico
--rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.4.2/UEVaultManager/assets/unchecked_16.png
--rw-rw-rw-   0        0        0    71745 2023-05-22 10:32:14.000000 UEVaultManager-1.4.2/UEVaultManager/cli.py
--rw-rw-rw-   0        0        0    47574 2023-05-22 13:00:35.000000 UEVaultManager-1.4.2/UEVaultManager/core.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.820414 UEVaultManager-1.4.2/UEVaultManager/downloader/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.2/UEVaultManager/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.833412 UEVaultManager-1.4.2/UEVaultManager/downloader/mp/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.2/UEVaultManager/downloader/mp/__init__.py
--rw-rw-rw-   0        0        0    38030 2023-05-15 06:30:52.000000 UEVaultManager-1.4.2/UEVaultManager/downloader/mp/manager.py
--rw-rw-rw-   0        0        0    12365 2023-05-17 13:38:36.000000 UEVaultManager-1.4.2/UEVaultManager/downloader/mp/workers.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.850622 UEVaultManager-1.4.2/UEVaultManager/lfs/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.2/UEVaultManager/lfs/__init__.py
--rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.4.2/UEVaultManager/lfs/egl.py
--rw-rw-rw-   0        0        0     6428 2023-05-15 06:51:22.000000 UEVaultManager-1.4.2/UEVaultManager/lfs/eos.py
--rw-rw-rw-   0        0        0    23209 2023-05-21 07:37:16.000000 UEVaultManager-1.4.2/UEVaultManager/lfs/uevmlfs.py
--rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.4.2/UEVaultManager/lfs/utils.py
--rw-rw-rw-   0        0        0     3122 2023-05-15 06:51:32.000000 UEVaultManager-1.4.2/UEVaultManager/lfs/windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.872621 UEVaultManager-1.4.2/UEVaultManager/models/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.2/UEVaultManager/models/__init__.py
--rw-rw-rw-   0        0        0     4269 2023-05-17 13:38:36.000000 UEVaultManager-1.4.2/UEVaultManager/models/app.py
--rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.4.2/UEVaultManager/models/chunk.py
--rw-rw-rw-   0        0        0     2703 2023-05-20 09:18:48.000000 UEVaultManager-1.4.2/UEVaultManager/models/config.py
--rw-rw-rw-   0        0        0     2131 2023-05-22 12:33:51.000000 UEVaultManager-1.4.2/UEVaultManager/models/csv.py
--rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.4.2/UEVaultManager/models/downloading.py
--rw-rw-rw-   0        0        0     5094 2023-05-15 06:33:02.000000 UEVaultManager-1.4.2/UEVaultManager/models/egl.py
--rw-rw-rw-   0        0        0      256 2023-05-20 09:20:19.000000 UEVaultManager-1.4.2/UEVaultManager/models/exceptions.py
--rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.4.2/UEVaultManager/models/json_manifest.py
--rw-rw-rw-   0        0        0    30505 2023-05-17 13:38:36.000000 UEVaultManager-1.4.2/UEVaultManager/models/manifest.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.880280 UEVaultManager-1.4.2/UEVaultManager/tkgui/
--rw-rw-rw-   0        0        0       16 2023-05-14 16:45:45.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/__init__.py
--rw-rw-rw-   0        0        0     1123 2023-05-20 07:12:03.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/main.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.908470 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/
--rw-rw-rw-   0        0        0     6667 2023-05-23 13:36:34.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
--rw-rw-rw-   0        0        0     4562 2023-05-23 13:37:02.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/EditCellWindowClass.py
--rw-rw-rw-   0        0        0     6553 2023-05-23 13:36:54.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/EditRowWindowClass.py
--rw-rw-rw-   0        0        0    32447 2023-05-22 17:07:09.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/EditableTableClass.py
--rw-rw-rw-   0        0        0    14038 2023-05-22 16:36:16.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
--rw-rw-rw-   0        0        0     2562 2023-05-22 14:44:53.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/GUISettingsClass.py
--rw-rw-rw-   0        0        0    13947 2023-05-23 13:37:12.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
--rw-rw-rw-   0        0        0     2251 2023-05-18 09:28:54.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/SaferDictClass.py
--rw-rw-rw-   0        0        0     6168 2023-05-23 07:32:20.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
--rw-rw-rw-   0        0        0    42713 2023-05-23 13:39:57.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/UEVMGuiClass.py
--rw-rw-rw-   0        0        0      543 2023-05-16 16:57:06.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
--rw-rw-rw-   0        0        0     2230 2023-05-15 10:13:54.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/WebImageClass.py
--rw-rw-rw-   0        0        0       16 2023-05-14 16:44:57.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/__init__.py
--rw-rw-rw-   0        0        0    14641 2023-05-23 13:35:44.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/functions.py
--rw-rw-rw-   0        0        0     2631 2023-05-23 13:39:29.000000 UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/globals.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.927815 UEVaultManager-1.4.2/UEVaultManager/utils/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.2/UEVaultManager/utils/__init__.py
--rw-rw-rw-   0        0        0     3478 2023-05-17 13:38:36.000000 UEVaultManager-1.4.2/UEVaultManager/utils/aliasing.py
--rw-rw-rw-   0        0        0     5897 2023-05-18 09:32:02.000000 UEVaultManager-1.4.2/UEVaultManager/utils/cli.py
--rw-rw-rw-   0        0        0     1342 2023-05-15 06:55:20.000000 UEVaultManager-1.4.2/UEVaultManager/utils/custom_parser.py
--rw-rw-rw-   0        0        0    10286 2023-05-15 06:33:02.000000 UEVaultManager-1.4.2/UEVaultManager/utils/egl_crypt.py
--rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.4.2/UEVaultManager/utils/env.py
--rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.4.2/UEVaultManager/utils/rolling_hash.py
--rw-rw-rw-   0        0        0     7260 2023-05-17 13:34:09.000000 UEVaultManager-1.4.2/UEVaultManager/utils/webview_login.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:47:27.791031 UEVaultManager-1.4.2/UEVaultManager.egg-info/
--rw-rw-rw-   0        0        0     6130 2023-05-23 13:47:27.000000 UEVaultManager-1.4.2/UEVaultManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2295 2023-05-23 13:47:27.000000 UEVaultManager-1.4.2/UEVaultManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 13:47:27.000000 UEVaultManager-1.4.2/UEVaultManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-23 13:47:27.000000 UEVaultManager-1.4.2/UEVaultManager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      286 2023-05-23 13:47:27.000000 UEVaultManager-1.4.2/UEVaultManager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-23 13:47:27.000000 UEVaultManager-1.4.2/UEVaultManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 13:47:27.929815 UEVaultManager-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0     3008 2023-05-23 12:39:50.000000 UEVaultManager-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:51:01.048076 UEVaultManager-1.4.3/
+-rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.4.3/LICENSE
+-rw-rw-rw-   0        0        0     6129 2023-05-23 13:51:01.047077 UEVaultManager-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5285 2023-05-23 13:48:41.000000 UEVaultManager-1.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 13:51:00.878845 UEVaultManager-1.4.3/UEVaultManager/
+-rw-rw-rw-   0        0        0      780 2023-05-23 13:49:41.000000 UEVaultManager-1.4.3/UEVaultManager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:51:00.916412 UEVaultManager-1.4.3/UEVaultManager/api/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.3/UEVaultManager/api/__init__.py
+-rw-rw-rw-   0        0        0    25469 2023-05-18 09:30:29.000000 UEVaultManager-1.4.3/UEVaultManager/api/egs.py
+-rw-rw-rw-   0        0        0     3142 2023-05-17 13:34:09.000000 UEVaultManager-1.4.3/UEVaultManager/api/uevm.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:51:00.925891 UEVaultManager-1.4.3/UEVaultManager/assets/
+-rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.4.3/UEVaultManager/assets/UEVM_200x200.png
+-rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.4.3/UEVaultManager/assets/checked_16.png
+-rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.4.3/UEVaultManager/assets/main.ico
+-rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.4.3/UEVaultManager/assets/unchecked_16.png
+-rw-rw-rw-   0        0        0    71745 2023-05-22 10:32:14.000000 UEVaultManager-1.4.3/UEVaultManager/cli.py
+-rw-rw-rw-   0        0        0    47574 2023-05-22 13:00:35.000000 UEVaultManager-1.4.3/UEVaultManager/core.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:51:00.931891 UEVaultManager-1.4.3/UEVaultManager/downloader/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.3/UEVaultManager/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:51:00.945175 UEVaultManager-1.4.3/UEVaultManager/downloader/mp/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.3/UEVaultManager/downloader/mp/__init__.py
+-rw-rw-rw-   0        0        0    38030 2023-05-15 06:30:52.000000 UEVaultManager-1.4.3/UEVaultManager/downloader/mp/manager.py
+-rw-rw-rw-   0        0        0    12365 2023-05-17 13:38:36.000000 UEVaultManager-1.4.3/UEVaultManager/downloader/mp/workers.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:51:00.963524 UEVaultManager-1.4.3/UEVaultManager/lfs/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.3/UEVaultManager/lfs/__init__.py
+-rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.4.3/UEVaultManager/lfs/egl.py
+-rw-rw-rw-   0        0        0     6428 2023-05-15 06:51:22.000000 UEVaultManager-1.4.3/UEVaultManager/lfs/eos.py
+-rw-rw-rw-   0        0        0    23209 2023-05-21 07:37:16.000000 UEVaultManager-1.4.3/UEVaultManager/lfs/uevmlfs.py
+-rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.4.3/UEVaultManager/lfs/utils.py
+-rw-rw-rw-   0        0        0     3122 2023-05-15 06:51:32.000000 UEVaultManager-1.4.3/UEVaultManager/lfs/windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:51:00.986530 UEVaultManager-1.4.3/UEVaultManager/models/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.3/UEVaultManager/models/__init__.py
+-rw-rw-rw-   0        0        0     4269 2023-05-17 13:38:36.000000 UEVaultManager-1.4.3/UEVaultManager/models/app.py
+-rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.4.3/UEVaultManager/models/chunk.py
+-rw-rw-rw-   0        0        0     2703 2023-05-20 09:18:48.000000 UEVaultManager-1.4.3/UEVaultManager/models/config.py
+-rw-rw-rw-   0        0        0     2131 2023-05-22 12:33:51.000000 UEVaultManager-1.4.3/UEVaultManager/models/csv.py
+-rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.4.3/UEVaultManager/models/downloading.py
+-rw-rw-rw-   0        0        0     5094 2023-05-15 06:33:02.000000 UEVaultManager-1.4.3/UEVaultManager/models/egl.py
+-rw-rw-rw-   0        0        0      256 2023-05-20 09:20:19.000000 UEVaultManager-1.4.3/UEVaultManager/models/exceptions.py
+-rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.4.3/UEVaultManager/models/json_manifest.py
+-rw-rw-rw-   0        0        0    30505 2023-05-17 13:38:36.000000 UEVaultManager-1.4.3/UEVaultManager/models/manifest.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:51:00.993488 UEVaultManager-1.4.3/UEVaultManager/tkgui/
+-rw-rw-rw-   0        0        0       16 2023-05-14 16:45:45.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/__init__.py
+-rw-rw-rw-   0        0        0     1123 2023-05-20 07:12:03.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/main.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:51:01.025077 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/
+-rw-rw-rw-   0        0        0     6667 2023-05-23 13:36:34.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
+-rw-rw-rw-   0        0        0     4562 2023-05-23 13:37:02.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/EditCellWindowClass.py
+-rw-rw-rw-   0        0        0     6553 2023-05-23 13:36:54.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/EditRowWindowClass.py
+-rw-rw-rw-   0        0        0    32447 2023-05-22 17:07:09.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/EditableTableClass.py
+-rw-rw-rw-   0        0        0    14038 2023-05-22 16:36:16.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
+-rw-rw-rw-   0        0        0     2562 2023-05-22 14:44:53.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/GUISettingsClass.py
+-rw-rw-rw-   0        0        0    13947 2023-05-23 13:37:12.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
+-rw-rw-rw-   0        0        0     2251 2023-05-18 09:28:54.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/SaferDictClass.py
+-rw-rw-rw-   0        0        0     6168 2023-05-23 07:32:20.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
+-rw-rw-rw-   0        0        0    42713 2023-05-23 13:39:57.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/UEVMGuiClass.py
+-rw-rw-rw-   0        0        0      543 2023-05-16 16:57:06.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
+-rw-rw-rw-   0        0        0     2230 2023-05-15 10:13:54.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/WebImageClass.py
+-rw-rw-rw-   0        0        0       16 2023-05-14 16:44:57.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/__init__.py
+-rw-rw-rw-   0        0        0    14641 2023-05-23 13:35:44.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/functions.py
+-rw-rw-rw-   0        0        0     2631 2023-05-23 13:39:29.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/globals.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:51:01.046076 UEVaultManager-1.4.3/UEVaultManager/utils/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.3/UEVaultManager/utils/__init__.py
+-rw-rw-rw-   0        0        0     3478 2023-05-17 13:38:36.000000 UEVaultManager-1.4.3/UEVaultManager/utils/aliasing.py
+-rw-rw-rw-   0        0        0     5897 2023-05-18 09:32:02.000000 UEVaultManager-1.4.3/UEVaultManager/utils/cli.py
+-rw-rw-rw-   0        0        0     1342 2023-05-15 06:55:20.000000 UEVaultManager-1.4.3/UEVaultManager/utils/custom_parser.py
+-rw-rw-rw-   0        0        0    10286 2023-05-15 06:33:02.000000 UEVaultManager-1.4.3/UEVaultManager/utils/egl_crypt.py
+-rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.4.3/UEVaultManager/utils/env.py
+-rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.4.3/UEVaultManager/utils/rolling_hash.py
+-rw-rw-rw-   0        0        0     7260 2023-05-17 13:34:09.000000 UEVaultManager-1.4.3/UEVaultManager/utils/webview_login.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:51:00.901492 UEVaultManager-1.4.3/UEVaultManager.egg-info/
+-rw-rw-rw-   0        0        0     6129 2023-05-23 13:51:00.000000 UEVaultManager-1.4.3/UEVaultManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2295 2023-05-23 13:51:00.000000 UEVaultManager-1.4.3/UEVaultManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 13:51:00.000000 UEVaultManager-1.4.3/UEVaultManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-23 13:51:00.000000 UEVaultManager-1.4.3/UEVaultManager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      286 2023-05-23 13:51:00.000000 UEVaultManager-1.4.3/UEVaultManager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-23 13:51:00.000000 UEVaultManager-1.4.3/UEVaultManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 13:51:01.048076 UEVaultManager-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     3008 2023-05-23 12:39:50.000000 UEVaultManager-1.4.3/setup.py
```

### Comparing `UEVaultManager-1.4.2/LICENSE` & `UEVaultManager-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/PKG-INFO` & `UEVaultManager-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.4.2
+Version: 1.4.3
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: webview
 Provides-Extra: webview_gtk
 License-File: LICENSE
 
 Welcome to UEVaultManager
 ==========================================
-[![Logo](https://laurentongaro.github.io/UEVaultManager/statics/UEVM_200x200.png)
+![Logo](https://laurentongaro.github.io/UEVaultManager/statics/UEVM_200x200.png)
 
 | pypi                                                                                                                 | py_versions                                                                                                          | github                                                                                                                         | docs                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|
 | [![Current PyPi Version](https://img.shields.io/pypi/v/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![py_versions](https://img.shields.io/pypi/pyversions/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![github](https://img.shields.io/github/v/tag/LaurentOngaro/uevaultmanager)](https://github.com/LaurentOngaro/UEVaultManager) | [![docs](https://img.shields.io/readthedocs/uevaultmanager/latest)](https://uevaultmanager.readthedocs.io/en/latest/?badge=latest) |
 
 **UEVaultManager** is an open-source assets manager that can list assets and
 their data from the Epic Games Marketplace. It is developed in Python, so
@@ -63,8 +63,8 @@
 * [Configuration](https://uevaultmanager.readthedocs.io/en/latest/configuration.html)
   * [Config folder](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-folder)
   * [Config file](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-file)
 
 [More info](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
 
 
- UEVaultManager ## version:1.4.2 ## codename: Phoenix+2
+ UEVaultManager ## version:1.4.3 ## codename: Phoenix+3
```

### Comparing `UEVaultManager-1.4.2/README.md` & `UEVaultManager-1.4.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Welcome to UEVaultManager
 ==========================================
-[![Logo](https://laurentongaro.github.io/UEVaultManager/statics/UEVM_200x200.png)
+![Logo](https://laurentongaro.github.io/UEVaultManager/statics/UEVM_200x200.png)
 
 | pypi                                                                                                                 | py_versions                                                                                                          | github                                                                                                                         | docs                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|
 | [![Current PyPi Version](https://img.shields.io/pypi/v/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![py_versions](https://img.shields.io/pypi/pyversions/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![github](https://img.shields.io/github/v/tag/LaurentOngaro/uevaultmanager)](https://github.com/LaurentOngaro/UEVaultManager) | [![docs](https://img.shields.io/readthedocs/uevaultmanager/latest)](https://uevaultmanager.readthedocs.io/en/latest/?badge=latest) |
 
 **UEVaultManager** is an open-source assets manager that can list assets and
 their data from the Epic Games Marketplace. It is developed in Python, so
```

### Comparing `UEVaultManager-1.4.2/UEVaultManager/__init__.py` & `UEVaultManager-1.4.3/UEVaultManager/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 UEVaultManager setup file.
 """
 import datetime
 
 year = datetime.date.today().year
 
 __name__ = 'UEVaultManager'
-__version__ = '1.4.2'
+__version__ = '1.4.3'
 # 0 Pegasus Seiya
 # 1 Dragon Shiryu
 # 2 Cygnus Hyoga
 # 3 Andromeda Shun
 # 4 Phoenix Ikki
-__codename__ = 'Phoenix+2'
+__codename__ = 'Phoenix+3'
 # 5 Leo Aiolia
 # 5 Virgo Shaka
 # 6 Libra Dohko
 # 7 Scorpio Milo
 # 8 Sagittarius Aiolos
 # 9 Capricorn Shura
 # 10 Aquarius Camus
```

### Comparing `UEVaultManager-1.4.2/UEVaultManager/api/egs.py` & `UEVaultManager-1.4.3/UEVaultManager/api/egs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/api/uevm.py` & `UEVaultManager-1.4.3/UEVaultManager/api/uevm.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/assets/UEVM_200x200.png` & `UEVaultManager-1.4.3/UEVaultManager/assets/UEVM_200x200.png`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/assets/main.ico` & `UEVaultManager-1.4.3/UEVaultManager/assets/main.ico`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/cli.py` & `UEVaultManager-1.4.3/UEVaultManager/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/core.py` & `UEVaultManager-1.4.3/UEVaultManager/core.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/downloader/mp/manager.py` & `UEVaultManager-1.4.3/UEVaultManager/downloader/mp/manager.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/downloader/mp/workers.py` & `UEVaultManager-1.4.3/UEVaultManager/downloader/mp/workers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/lfs/egl.py` & `UEVaultManager-1.4.3/UEVaultManager/lfs/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/lfs/eos.py` & `UEVaultManager-1.4.3/UEVaultManager/lfs/eos.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/lfs/uevmlfs.py` & `UEVaultManager-1.4.3/UEVaultManager/lfs/uevmlfs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/lfs/utils.py` & `UEVaultManager-1.4.3/UEVaultManager/lfs/utils.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/lfs/windows_helpers.py` & `UEVaultManager-1.4.3/UEVaultManager/lfs/windows_helpers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/models/app.py` & `UEVaultManager-1.4.3/UEVaultManager/models/app.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/models/chunk.py` & `UEVaultManager-1.4.3/UEVaultManager/models/chunk.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/models/config.py` & `UEVaultManager-1.4.3/UEVaultManager/models/config.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/models/csv.py` & `UEVaultManager-1.4.3/UEVaultManager/models/csv.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/models/downloading.py` & `UEVaultManager-1.4.3/UEVaultManager/models/downloading.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/models/egl.py` & `UEVaultManager-1.4.3/UEVaultManager/models/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/models/json_manifest.py` & `UEVaultManager-1.4.3/UEVaultManager/models/json_manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/models/manifest.py` & `UEVaultManager-1.4.3/UEVaultManager/models/manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/tkgui/main.py` & `UEVaultManager-1.4.3/UEVaultManager/tkgui/main.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py` & `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/EditCellWindowClass.py` & `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/EditCellWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/EditRowWindowClass.py` & `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/EditRowWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/EditableTableClass.py` & `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/EditableTableClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py` & `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/GUISettingsClass.py` & `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/GUISettingsClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/ProgressWindowsClass.py` & `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/ProgressWindowsClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/SaferDictClass.py` & `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/SaferDictClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py` & `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/UEVMGuiClass.py` & `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/UEVMGuiClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py` & `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/WebImageClass.py` & `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/WebImageClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/functions.py` & `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/functions.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/tkgui/modules/globals.py` & `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/globals.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/utils/aliasing.py` & `UEVaultManager-1.4.3/UEVaultManager/utils/aliasing.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/utils/cli.py` & `UEVaultManager-1.4.3/UEVaultManager/utils/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/utils/custom_parser.py` & `UEVaultManager-1.4.3/UEVaultManager/utils/custom_parser.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/utils/egl_crypt.py` & `UEVaultManager-1.4.3/UEVaultManager/utils/egl_crypt.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/utils/rolling_hash.py` & `UEVaultManager-1.4.3/UEVaultManager/utils/rolling_hash.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager/utils/webview_login.py` & `UEVaultManager-1.4.3/UEVaultManager/utils/webview_login.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/UEVaultManager.egg-info/PKG-INFO` & `UEVaultManager-1.4.3/UEVaultManager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.4.2
+Version: 1.4.3
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: webview
 Provides-Extra: webview_gtk
 License-File: LICENSE
 
 Welcome to UEVaultManager
 ==========================================
-[![Logo](https://laurentongaro.github.io/UEVaultManager/statics/UEVM_200x200.png)
+![Logo](https://laurentongaro.github.io/UEVaultManager/statics/UEVM_200x200.png)
 
 | pypi                                                                                                                 | py_versions                                                                                                          | github                                                                                                                         | docs                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|
 | [![Current PyPi Version](https://img.shields.io/pypi/v/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![py_versions](https://img.shields.io/pypi/pyversions/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![github](https://img.shields.io/github/v/tag/LaurentOngaro/uevaultmanager)](https://github.com/LaurentOngaro/UEVaultManager) | [![docs](https://img.shields.io/readthedocs/uevaultmanager/latest)](https://uevaultmanager.readthedocs.io/en/latest/?badge=latest) |
 
 **UEVaultManager** is an open-source assets manager that can list assets and
 their data from the Epic Games Marketplace. It is developed in Python, so
@@ -63,8 +63,8 @@
 * [Configuration](https://uevaultmanager.readthedocs.io/en/latest/configuration.html)
   * [Config folder](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-folder)
   * [Config file](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-file)
 
 [More info](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
 
 
- UEVaultManager ## version:1.4.2 ## codename: Phoenix+2
+ UEVaultManager ## version:1.4.3 ## codename: Phoenix+3
```

### Comparing `UEVaultManager-1.4.2/UEVaultManager.egg-info/SOURCES.txt` & `UEVaultManager-1.4.3/UEVaultManager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.2/setup.py` & `UEVaultManager-1.4.3/setup.py`

 * *Files identical despite different names*

