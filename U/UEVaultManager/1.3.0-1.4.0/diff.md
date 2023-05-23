# Comparing `tmp/UEVaultManager-1.3.0.tar.gz` & `tmp/UEVaultManager-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UEVaultManager-1.3.0.tar", last modified: Tue May 16 17:12:04 2023, max compression
+gzip compressed data, was "UEVaultManager-1.4.0.tar", last modified: Mon May 22 17:22:21 2023, max compression
```

## Comparing `UEVaultManager-1.3.0.tar` & `UEVaultManager-1.4.0.tar`

### file list

```diff
@@ -1,76 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.161909 UEVaultManager-1.3.0/
--rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     5779 2023-05-16 17:12:04.160909 UEVaultManager-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4948 2023-05-15 08:41:23.000000 UEVaultManager-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.002132 UEVaultManager-1.3.0/UEVaultManager/
--rw-rw-rw-   0        0        0      780 2023-05-16 17:05:23.000000 UEVaultManager-1.3.0/UEVaultManager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.038102 UEVaultManager-1.3.0/UEVaultManager/api/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.3.0/UEVaultManager/api/__init__.py
--rw-rw-rw-   0        0        0    25381 2023-05-16 09:42:26.000000 UEVaultManager-1.3.0/UEVaultManager/api/egs.py
--rw-rw-rw-   0        0        0     3095 2023-05-16 14:13:33.000000 UEVaultManager-1.3.0/UEVaultManager/api/uevm.py
-drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.040471 UEVaultManager-1.3.0/UEVaultManager/assets/
--rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.3.0/UEVaultManager/assets/UEVM_200x200.png
--rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.3.0/UEVaultManager/assets/main.ico
--rw-rw-rw-   0        0        0    65456 2023-05-16 16:56:25.000000 UEVaultManager-1.3.0/UEVaultManager/cli.py
--rw-rw-rw-   0        0        0    47084 2023-05-16 14:13:33.000000 UEVaultManager-1.3.0/UEVaultManager/core.py
-drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.041482 UEVaultManager-1.3.0/UEVaultManager/downloader/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.3.0/UEVaultManager/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.056504 UEVaultManager-1.3.0/UEVaultManager/downloader/mp/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.3.0/UEVaultManager/downloader/mp/__init__.py
--rw-rw-rw-   0        0        0    38030 2023-05-15 06:30:52.000000 UEVaultManager-1.3.0/UEVaultManager/downloader/mp/manager.py
--rw-rw-rw-   0        0        0    12365 2023-05-11 14:38:28.000000 UEVaultManager-1.3.0/UEVaultManager/downloader/mp/workers.py
-drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.075255 UEVaultManager-1.3.0/UEVaultManager/lfs/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.3.0/UEVaultManager/lfs/__init__.py
--rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.3.0/UEVaultManager/lfs/egl.py
--rw-rw-rw-   0        0        0     6428 2023-05-15 06:51:22.000000 UEVaultManager-1.3.0/UEVaultManager/lfs/eos.py
--rw-rw-rw-   0        0        0    23055 2023-05-16 09:53:50.000000 UEVaultManager-1.3.0/UEVaultManager/lfs/uevmlfs.py
--rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.3.0/UEVaultManager/lfs/utils.py
--rw-rw-rw-   0        0        0     3122 2023-05-15 06:51:32.000000 UEVaultManager-1.3.0/UEVaultManager/lfs/windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.099423 UEVaultManager-1.3.0/UEVaultManager/models/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.3.0/UEVaultManager/models/__init__.py
--rw-rw-rw-   0        0        0     4269 2023-05-11 14:38:28.000000 UEVaultManager-1.3.0/UEVaultManager/models/app.py
--rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.3.0/UEVaultManager/models/chunk.py
--rw-rw-rw-   0        0        0     1367 2023-05-15 06:33:02.000000 UEVaultManager-1.3.0/UEVaultManager/models/config.py
--rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.3.0/UEVaultManager/models/downloading.py
--rw-rw-rw-   0        0        0     5094 2023-05-15 06:33:02.000000 UEVaultManager-1.3.0/UEVaultManager/models/egl.py
--rw-rw-rw-   0        0        0       72 2023-05-11 14:38:28.000000 UEVaultManager-1.3.0/UEVaultManager/models/exceptions.py
--rw-rw-rw-   0        0        0     1350 2023-05-15 06:33:02.000000 UEVaultManager-1.3.0/UEVaultManager/models/gql.py
--rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.3.0/UEVaultManager/models/json_manifest.py
--rw-rw-rw-   0        0        0    30505 2023-05-15 06:30:52.000000 UEVaultManager-1.3.0/UEVaultManager/models/manifest.py
-drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.107422 UEVaultManager-1.3.0/UEVaultManager/tkgui/
--rw-rw-rw-   0        0        0       16 2023-05-14 16:45:45.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/__init__.py
--rw-rw-rw-   0        0        0      949 2023-05-14 16:45:45.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/main.py
-drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.138059 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/
--rw-rw-rw-   0        0        0     6042 2023-05-16 16:41:50.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
--rw-rw-rw-   0        0        0     4571 2023-05-15 10:13:54.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/EditCellWindowClass.py
--rw-rw-rw-   0        0        0     6834 2023-05-16 13:36:33.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/EditRowWindowClass.py
--rw-rw-rw-   0        0        0    24480 2023-05-16 16:57:32.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/EditableTableClass.py
--rw-rw-rw-   0        0        0    10159 2023-05-15 10:13:54.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
--rw-rw-rw-   0        0        0     1516 2023-05-15 10:14:37.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/GUISettingsClass.py
--rw-rw-rw-   0        0        0    14228 2023-05-15 10:17:32.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
--rw-rw-rw-   0        0        0     2253 2023-05-15 10:13:54.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/SaferDictClass.py
--rw-rw-rw-   0        0        0     5056 2023-05-15 10:19:15.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
--rw-rw-rw-   0        0        0    35352 2023-05-16 16:56:54.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/UEVMGuiClass.py
--rw-rw-rw-   0        0        0      543 2023-05-16 16:57:06.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
--rw-rw-rw-   0        0        0     2230 2023-05-15 10:13:54.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/WebImageClass.py
--rw-rw-rw-   0        0        0       16 2023-05-14 16:44:57.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/__init__.py
--rw-rw-rw-   0        0        0    12574 2023-05-16 15:35:58.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/functions.py
--rw-rw-rw-   0        0        0     1781 2023-05-16 14:18:21.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/globals.py
-drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.159910 UEVaultManager-1.3.0/UEVaultManager/utils/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.3.0/UEVaultManager/utils/__init__.py
--rw-rw-rw-   0        0        0     3478 2023-05-15 08:49:51.000000 UEVaultManager-1.3.0/UEVaultManager/utils/aliasing.py
--rw-rw-rw-   0        0        0     5628 2023-05-16 07:17:45.000000 UEVaultManager-1.3.0/UEVaultManager/utils/cli.py
--rw-rw-rw-   0        0        0     1342 2023-05-15 06:55:20.000000 UEVaultManager-1.3.0/UEVaultManager/utils/custom_parser.py
--rw-rw-rw-   0        0        0    10286 2023-05-15 06:33:02.000000 UEVaultManager-1.3.0/UEVaultManager/utils/egl_crypt.py
--rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.3.0/UEVaultManager/utils/env.py
--rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.3.0/UEVaultManager/utils/rolling_hash.py
--rw-rw-rw-   0        0        0     7214 2023-05-15 10:15:19.000000 UEVaultManager-1.3.0/UEVaultManager/utils/webview_login.py
-drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.024092 UEVaultManager-1.3.0/UEVaultManager.egg-info/
--rw-rw-rw-   0        0        0     5779 2023-05-16 17:12:03.000000 UEVaultManager-1.3.0/UEVaultManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2219 2023-05-16 17:12:03.000000 UEVaultManager-1.3.0/UEVaultManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 17:12:03.000000 UEVaultManager-1.3.0/UEVaultManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-16 17:12:03.000000 UEVaultManager-1.3.0/UEVaultManager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       96 2023-05-16 17:12:03.000000 UEVaultManager-1.3.0/UEVaultManager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-16 17:12:03.000000 UEVaultManager-1.3.0/UEVaultManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 17:12:04.161909 UEVaultManager-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2372 2023-05-16 08:14:34.000000 UEVaultManager-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:22:21.639226 UEVaultManager-1.4.0/
+-rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0     5777 2023-05-22 17:22:21.639226 UEVaultManager-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4948 2023-05-15 08:41:23.000000 UEVaultManager-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 17:22:21.468512 UEVaultManager-1.4.0/UEVaultManager/
+-rw-rw-rw-   0        0        0      778 2023-05-22 17:19:01.000000 UEVaultManager-1.4.0/UEVaultManager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:22:21.504355 UEVaultManager-1.4.0/UEVaultManager/api/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.0/UEVaultManager/api/__init__.py
+-rw-rw-rw-   0        0        0    25469 2023-05-18 09:30:29.000000 UEVaultManager-1.4.0/UEVaultManager/api/egs.py
+-rw-rw-rw-   0        0        0     3142 2023-05-17 13:34:09.000000 UEVaultManager-1.4.0/UEVaultManager/api/uevm.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:22:21.514916 UEVaultManager-1.4.0/UEVaultManager/assets/
+-rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.4.0/UEVaultManager/assets/UEVM_200x200.png
+-rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.4.0/UEVaultManager/assets/checked_16.png
+-rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.4.0/UEVaultManager/assets/main.ico
+-rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.4.0/UEVaultManager/assets/unchecked_16.png
+-rw-rw-rw-   0        0        0    71745 2023-05-22 10:32:14.000000 UEVaultManager-1.4.0/UEVaultManager/cli.py
+-rw-rw-rw-   0        0        0    47574 2023-05-22 13:00:35.000000 UEVaultManager-1.4.0/UEVaultManager/core.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:22:21.520918 UEVaultManager-1.4.0/UEVaultManager/downloader/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.0/UEVaultManager/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:22:21.534017 UEVaultManager-1.4.0/UEVaultManager/downloader/mp/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.0/UEVaultManager/downloader/mp/__init__.py
+-rw-rw-rw-   0        0        0    38030 2023-05-15 06:30:52.000000 UEVaultManager-1.4.0/UEVaultManager/downloader/mp/manager.py
+-rw-rw-rw-   0        0        0    12365 2023-05-17 13:38:36.000000 UEVaultManager-1.4.0/UEVaultManager/downloader/mp/workers.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:22:21.552843 UEVaultManager-1.4.0/UEVaultManager/lfs/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.0/UEVaultManager/lfs/__init__.py
+-rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.4.0/UEVaultManager/lfs/egl.py
+-rw-rw-rw-   0        0        0     6428 2023-05-15 06:51:22.000000 UEVaultManager-1.4.0/UEVaultManager/lfs/eos.py
+-rw-rw-rw-   0        0        0    23209 2023-05-21 07:37:16.000000 UEVaultManager-1.4.0/UEVaultManager/lfs/uevmlfs.py
+-rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.4.0/UEVaultManager/lfs/utils.py
+-rw-rw-rw-   0        0        0     3122 2023-05-15 06:51:32.000000 UEVaultManager-1.4.0/UEVaultManager/lfs/windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:22:21.577037 UEVaultManager-1.4.0/UEVaultManager/models/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.0/UEVaultManager/models/__init__.py
+-rw-rw-rw-   0        0        0     4269 2023-05-17 13:38:36.000000 UEVaultManager-1.4.0/UEVaultManager/models/app.py
+-rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.4.0/UEVaultManager/models/chunk.py
+-rw-rw-rw-   0        0        0     2703 2023-05-20 09:18:48.000000 UEVaultManager-1.4.0/UEVaultManager/models/config.py
+-rw-rw-rw-   0        0        0     2131 2023-05-22 12:33:51.000000 UEVaultManager-1.4.0/UEVaultManager/models/csv.py
+-rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.4.0/UEVaultManager/models/downloading.py
+-rw-rw-rw-   0        0        0     5094 2023-05-15 06:33:02.000000 UEVaultManager-1.4.0/UEVaultManager/models/egl.py
+-rw-rw-rw-   0        0        0      256 2023-05-20 09:20:19.000000 UEVaultManager-1.4.0/UEVaultManager/models/exceptions.py
+-rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.4.0/UEVaultManager/models/json_manifest.py
+-rw-rw-rw-   0        0        0    30505 2023-05-17 13:38:36.000000 UEVaultManager-1.4.0/UEVaultManager/models/manifest.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:22:21.584939 UEVaultManager-1.4.0/UEVaultManager/tkgui/
+-rw-rw-rw-   0        0        0       16 2023-05-14 16:45:45.000000 UEVaultManager-1.4.0/UEVaultManager/tkgui/__init__.py
+-rw-rw-rw-   0        0        0     1123 2023-05-20 07:12:03.000000 UEVaultManager-1.4.0/UEVaultManager/tkgui/main.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:22:21.615682 UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/
+-rw-rw-rw-   0        0        0     6948 2023-05-22 15:49:22.000000 UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
+-rw-rw-rw-   0        0        0     4843 2023-05-22 17:13:42.000000 UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/EditCellWindowClass.py
+-rw-rw-rw-   0        0        0     6832 2023-05-17 14:47:22.000000 UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/EditRowWindowClass.py
+-rw-rw-rw-   0        0        0    32447 2023-05-22 17:07:09.000000 UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/EditableTableClass.py
+-rw-rw-rw-   0        0        0    14038 2023-05-22 16:36:16.000000 UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
+-rw-rw-rw-   0        0        0     2562 2023-05-22 14:44:53.000000 UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/GUISettingsClass.py
+-rw-rw-rw-   0        0        0    14228 2023-05-22 12:42:07.000000 UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
+-rw-rw-rw-   0        0        0     2251 2023-05-18 09:28:54.000000 UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/SaferDictClass.py
+-rw-rw-rw-   0        0        0     6012 2023-05-22 16:36:16.000000 UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
+-rw-rw-rw-   0        0        0    42992 2023-05-22 16:55:28.000000 UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/UEVMGuiClass.py
+-rw-rw-rw-   0        0        0      543 2023-05-16 16:57:06.000000 UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
+-rw-rw-rw-   0        0        0     2230 2023-05-15 10:13:54.000000 UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/WebImageClass.py
+-rw-rw-rw-   0        0        0       16 2023-05-14 16:44:57.000000 UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/__init__.py
+-rw-rw-rw-   0        0        0    12815 2023-05-20 14:28:39.000000 UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/functions.py
+-rw-rw-rw-   0        0        0     2633 2023-05-20 10:13:14.000000 UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/globals.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:22:21.637230 UEVaultManager-1.4.0/UEVaultManager/utils/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.0/UEVaultManager/utils/__init__.py
+-rw-rw-rw-   0        0        0     3478 2023-05-17 13:38:36.000000 UEVaultManager-1.4.0/UEVaultManager/utils/aliasing.py
+-rw-rw-rw-   0        0        0     5897 2023-05-18 09:32:02.000000 UEVaultManager-1.4.0/UEVaultManager/utils/cli.py
+-rw-rw-rw-   0        0        0     1342 2023-05-15 06:55:20.000000 UEVaultManager-1.4.0/UEVaultManager/utils/custom_parser.py
+-rw-rw-rw-   0        0        0    10286 2023-05-15 06:33:02.000000 UEVaultManager-1.4.0/UEVaultManager/utils/egl_crypt.py
+-rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.4.0/UEVaultManager/utils/env.py
+-rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.4.0/UEVaultManager/utils/rolling_hash.py
+-rw-rw-rw-   0        0        0     7260 2023-05-17 13:34:09.000000 UEVaultManager-1.4.0/UEVaultManager/utils/webview_login.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:22:21.491100 UEVaultManager-1.4.0/UEVaultManager.egg-info/
+-rw-rw-rw-   0        0        0     5777 2023-05-22 17:22:21.000000 UEVaultManager-1.4.0/UEVaultManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2295 2023-05-22 17:22:21.000000 UEVaultManager-1.4.0/UEVaultManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 17:22:21.000000 UEVaultManager-1.4.0/UEVaultManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-22 17:22:21.000000 UEVaultManager-1.4.0/UEVaultManager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       96 2023-05-22 17:22:21.000000 UEVaultManager-1.4.0/UEVaultManager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-22 17:22:21.000000 UEVaultManager-1.4.0/UEVaultManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 17:22:21.639226 UEVaultManager-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2372 2023-05-16 08:14:34.000000 UEVaultManager-1.4.0/setup.py
```

### Comparing `UEVaultManager-1.3.0/LICENSE` & `UEVaultManager-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/PKG-INFO` & `UEVaultManager-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.3.0
+Version: 1.4.0
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -64,8 +64,8 @@
   * [The individual json files](https://uevaultmanager.readthedocs.io/en/latest/output.html#the-individual-json-files)
   * [how to fix invalid search result during the grabbing process](https://uevaultmanager.readthedocs.io/en/latest/output.html#how-to-fix-invalid-search-result-during-the-grabbing-process)
   * [possible values in the error Field](https://uevaultmanager.readthedocs.io/en/latest/output.html#possible-values-in-the-error-field)
 
 [Next](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
 
 
- UEVaultManager ## version:1.3.0 ## codename: Andromeda
+ UEVaultManager ## version:1.4.0 ## codename: Phoenix
```

### Comparing `UEVaultManager-1.3.0/README.md` & `UEVaultManager-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/__init__.py` & `UEVaultManager-1.4.0/UEVaultManager/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 UEVaultManager setup file.
 """
 import datetime
 
 year = datetime.date.today().year
 
 __name__ = 'UEVaultManager'
-__version__ = '1.3.0'
+__version__ = '1.4.0'
 # 0 Pegasus Seiya
 # 1 Dragon Shiryu
 # 2 Cygnus Hyoga
 # 3 Andromeda Shun
-__codename__ = 'Andromeda'
 # 4 Phoenix Ikki
+__codename__ = 'Phoenix'
 # 5 Leo Aiolia
 # 5 Virgo Shaka
 # 6 Libra Dohko
 # 7 Scorpio Milo
 # 8 Sagittarius Aiolos
 # 9 Capricorn Shura
 # 10 Aquarius Camus
```

### Comparing `UEVaultManager-1.3.0/UEVaultManager/api/egs.py` & `UEVaultManager-1.4.0/UEVaultManager/api/egs.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,15 @@
         """
         Starts a session.
         :param refresh_token: refresh token
         :param exchange_token: exchange token
         :param authorization_code: authorization code
         :param client_credentials: client credentials
         :return: The session.
+        :raise: ValueError,InvalidCredentialsError
         """
         if refresh_token:
             params = dict(grant_type='refresh_token', refresh_token=refresh_token, token_type='eg1')
         elif exchange_token:
             params = dict(grant_type='exchange_code', exchange_code=exchange_token, token_type='eg1')
         elif authorization_code:
             params = dict(grant_type='authorization_code', code=authorization_code, token_type='eg1')
@@ -298,31 +299,31 @@
             f'https://{self._entitlements_host}/entitlement/api/account/{user_id}/entitlements',
             params=dict(start=0, count=5000),
             timeout=self.request_timeout
         )
         r.raise_for_status()
         return r.json()
 
-    def get_item_info(self, namespace: str, catalog_item_id: str, timeout: float = None) -> dict:
+    def get_item_info(self, namespace: str, catalog_item_id: str, timeout: float = None) -> (dict, int):
         """
         Gets the item info.
         :param namespace: Namespace of the item
         :param catalog_item_id: Catalog item id of the item
         :param timeout: Timeout for the request
-        :return: The item info.
+        :return: (The item info, status code)
         """
         r = self.session.get(
             f'https://{self._catalog_host}/catalog/api/shared/namespace/{namespace}/bulk/items',
             params=dict(
                 id=catalog_item_id, includeDLCDetails=True, includeMainGameDetails=True, country=self.country_code, locale=self.language_code
             ),
             timeout=timeout or self.request_timeout
         )
         r.raise_for_status()
-        return r.json().get(catalog_item_id, None)
+        return r.json().get(catalog_item_id, None), r.status_code
 
     def get_artifact_service_ticket(self, sandbox_id: str, artifact_id: str, label='Live', platform='Windows') -> dict:
         """
         Gets the artifact service ticket.
         Unused but kept for the global API reference.
         :param sandbox_id: sandbox id
         :param artifact_id: artifact id
```

### Comparing `UEVaultManager-1.3.0/UEVaultManager/api/uevm.py` & `UEVaultManager-1.4.0/UEVaultManager/api/uevm.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 import re
 from enum import Enum
 from platform import system
 
 import requests
 from packaging import version
 
-from UEVaultManager import __version__
+# noinspection PyPep8Naming
+from UEVaultManager import __version__ as UEVM_version
 
 
 class UpdateSeverity(Enum):
     """
     Enum for update severity.
     """
     NONE = 0
@@ -62,15 +63,15 @@
 
 
 class UEVMAPI:
     """
     Class for interacting with the UEVaultManager API.
     """
     _package_name = 'UEVaultManager'
-    _user_agent = f'{_package_name}/{__version__} ({system()})'
+    _user_agent = f'{_package_name}/{UEVM_version} ({system()})'
 
     def __init__(self):
         self.session = requests.session()
         self.log = logging.getLogger('UEVMAPI')
         self.session.headers['User-Agent'] = self._user_agent
 
     def get_version_information(self) -> dict:
@@ -86,14 +87,14 @@
         pypi_codename = ''
         severity = UpdateSeverity.NONE
         release_url = ''
         summary = ''
         try:
             pypi_version = data['info']['version']
             pypi_codename = extract_codename(data['info']['description'])
-            severity = str(extract_severity(__version__, pypi_version).name)
+            severity = str(extract_severity(UEVM_version, pypi_version).name)
             release_url = data['info']['release_url']
             summary = data['info']['summary']
         except KeyError:
             self.log.warning('Failed to get version information from PyPI.')
 
         return dict(version=pypi_version, codename=pypi_codename, severity=severity, release_url=release_url, summary=summary)
```

### Comparing `UEVaultManager-1.3.0/UEVaultManager/assets/UEVM_200x200.png` & `UEVaultManager-1.4.0/UEVaultManager/assets/UEVM_200x200.png`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/assets/main.ico` & `UEVaultManager-1.4.0/UEVaultManager/assets/main.ico`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/cli.py` & `UEVaultManager-1.4.0/UEVaultManager/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,30 +18,108 @@
 from multiprocessing import freeze_support, Queue as MPQueue
 from platform import platform
 from sys import exit, stdout
 
 import UEVaultManager.tkgui.modules.functions as gui_f  # using the shortest variable name for globals for convenience
 import UEVaultManager.tkgui.modules.globals as gui_g  # using the shortest variable name for globals for convenience
 # noinspection PyPep8Naming
-from UEVaultManager import __version__, __codename__
+from UEVaultManager import __version__ as UEVM_version, __codename__ as UEVM_codename
 from UEVaultManager.api.egs import create_empty_assets_extras, GrabResult
 from UEVaultManager.api.uevm import UpdateSeverity
-from UEVaultManager.core import AppCore, CSV_headings
+from UEVaultManager.core import AppCore
+from UEVaultManager.models.csv import CSV_headings
 from UEVaultManager.models.exceptions import InvalidCredentialsError
-from UEVaultManager.tkgui.modules.DisplayContentWindowClass import DisplayContentWindow
+from UEVaultManager.tkgui.modules.functions import custom_print  # simplier way to use the custom_print function
 from UEVaultManager.tkgui.modules.functions import json_print_key_val
 from UEVaultManager.tkgui.modules.ProgressWindowsClass import ProgressWindow
 from UEVaultManager.tkgui.modules.UEVMGuiClass import UEVMGui
-from UEVaultManager.tkgui.modules.UEVMGuiHiddenRootClass import UEVMGuiHiddenRoot
-from UEVaultManager.utils.cli import str_to_bool, check_and_create_path, create_list_from_string
+from UEVaultManager.utils.cli import str_to_bool, check_and_create_path, create_list_from_string, str_is_bool
 from UEVaultManager.utils.custom_parser import HiddenAliasSubparsersAction
+from UEVaultManager.tkgui.modules.DisplayContentWindowClass import DisplayContentWindow
+from UEVaultManager.tkgui.modules.SaferDictClass import SaferDict
+from UEVaultManager.tkgui.modules.UEVMGuiHiddenRootClass import UEVMGuiHiddenRoot
 
 logging.basicConfig(format='[%(name)s] %(levelname)s: %(message)s', level=logging.INFO)
 
 
+def init_gui_args(args, additional_args=None) -> None:
+    """
+    Initialize the GUI arguments using the CLI arguments
+    :param args:
+    :param additional_args: dict of additional arguments to add
+    """
+
+    # args can not be used as it because it's an object that mainly run as a dict (but it's not)
+    # so we need to convert it to a dict first
+    temp_dict = vars(args)
+    temp_dict['csv'] = True  # force csv output
+    temp_dict['gui'] = True
+    if additional_args is not None:
+        temp_dict.update(additional_args)
+    # create a SaferDict object from the dict (it will avoid errors when trying to access non-existing keys)
+    gui_g.UEVM_cli_args = SaferDict({})
+    # copy the dict content to the SaferDict object
+    gui_g.UEVM_cli_args.copy_from(temp_dict)
+
+
+def init_progress_window(args, logger=None, callback=None) -> (bool, ProgressWindow):
+    """
+    Initialize the progress window
+    :param args: args of the command line
+    :param logger: logger to use
+    :param callback: callback function to call while progress updating
+    :return: (True if the UEVMGui window already existed | False, ProgressWindow)
+    """
+    gui_g.UEVM_log_ref = logger
+
+    # check if the GUI is already running
+    if gui_g.UEVM_gui_ref is None:
+        # create a fake root because ProgressWindow must always be a top level window
+        gui_g.UEVM_gui_ref = UEVMGuiHiddenRoot()
+        uewm_gui_exists = False
+    else:
+        uewm_gui_exists = True
+    force_refresh = True if args.force_refresh else False
+    window = ProgressWindow(
+        title="Updating Assets List",
+        quit_on_close=not uewm_gui_exists,
+        width=300,
+        height=150,
+        max_value=200,
+        show_start_button=False,
+        show_stop_button=True,
+        function=callback,
+        function_parameters={
+            'filter_category': gui_g.UEVM_filter_category,
+            'force_refresh': force_refresh,
+        }
+    )
+    return uewm_gui_exists, window
+
+
+def init_display_window(logger=None) -> (bool, DisplayContentWindow):
+    """
+    Initialize the display window
+    :param logger: logger to use
+    :return: (True if the UEVMGui window already existed | False, DisplayContentWindow)
+    """
+    gui_g.UEVM_log_ref = logger
+
+    # check if the GUI is already running
+    if gui_g.UEVM_gui_ref is None:
+        # create a fake root because DisplayContentWindow must always be a top level window
+        gui_g.UEVM_gui_ref = UEVMGuiHiddenRoot()
+        uewm_gui_exists = False
+    else:
+        uewm_gui_exists = True
+    if gui_g.display_content_window_ref is None:
+        gui_g.display_content_window_ref = DisplayContentWindow(title='UEVM: status command output', quit_on_close=not uewm_gui_exists)
+    return uewm_gui_exists, gui_g.display_content_window_ref
+
+
 class UEVaultManagerCLI:
     """
     Command line interface for UEVaultManager
     :param override_config: path to a config file to use instead of the default one
     :param api_timeout: timeout for API requests
     """
 
@@ -151,14 +229,15 @@
         review = no_int_data
         price = no_float_data
         purchased = bool_false_data
         discount_price = no_float_data
         supported_versions = no_text_data
         page_title = no_text_data
         grab_result = GrabResult.NO_ERROR.name
+        oigin = 'Marketplace'  # by default the asset are from the "MarketPlace"
         on_sale = bool_false_data
 
         try:
             asset_url = extras_data['asset_url']
             review = extras_data['review']
             price = extras_data['price']
             discount_price = extras_data['discount_price']
@@ -176,53 +255,53 @@
             supported_versions_list = supported_versions.lower().replace('UE_', '')
             supported_versions_list = create_list_from_string(supported_versions_list)
             obsolete = bool_true_data
             for _, version in enumerate(supported_versions_list):
                 if version == '':
                     continue
                 else:
-                    if float(self.core.engine_version_for_obsolete_assets) >= float(version):
+                    if float(self.core.engine_version_for_obsolete_assets) <= float(version):
                         obsolete = bool_false_data
                         break
         try:
             values = (
                 # dans les infos
                 asset_id  # 'asset_id'
                 , item.app_name  # 'App name'
                 , item.app_title  # 'App title'
                 , category  # 'Category'
-                , item.app_version('Windows')  # 'UE Version'
                 , review  # 'Review'
                 , metadata['developer']  # 'Developer'
                 , metadata['description']  # 'Description'
                 , metadata['status']  # 'status'
-                , discount_price  # 'Discount Price'
+                , discount_price  # 'Discount price'
                 , on_sale  # 'On Sale'
                 , purchased  # 'Purchased'
                 , obsolete  # 'obsolete'
                 , supported_versions  # 'supported versions'
-                , grab_result  # 'grab result'
+                , grab_result  # 'Grab result'
                 , price  # 'Price'
-                , no_float_data  # 'Old Price'
+                , no_float_data  # 'Old price'
                 # User Fields
                 , no_text_data  # 'Comment'
                 , no_float_data  # 'Stars'
-                , bool_false_data  # 'Must Buy'
+                , bool_false_data  # 'Must buy'
                 , no_text_data  # 'Test result
-                , no_text_data  # 'Installed Folder'
+                , no_text_data  # 'Installed folder'
                 , no_text_data  # 'Alternative'
-                , no_text_data  # 'Asset Folder'
+                , oigin  # 'Origin
                 # less important fields
                 , page_title  # 'page title'
                 , thumbnail_url  # 'Image' with 488 height
                 , asset_url  # 'Url'
                 , compatible_versions  # compatible_versions
-                , date_added  # 'Date Added'
-                , metadata['creationDate']  # 'Creation Date'
-                , metadata['lastModifiedDate']  # 'Update Date'
+                , date_added  # 'Date added'
+                , metadata['creationDate']  # 'Creation date'
+                , metadata['lastModifiedDate']  # 'Update date'
+                , item.app_version('Windows')  # 'UE version'
                 , uid  # 'Uid'
             )
             record = dict(zip(CSV_headings.keys(), values))
         except TypeError:
             self.logger.error(f'Could not create record for {item.app_name}')
 
         return asset_id, record
@@ -348,25 +427,36 @@
                             self.logger.error(
                                 f'In the existing file, asset {_asset_id} has no column named {key}. This asset is ignored and its values will be overwritten'
                             )
                             # print(f' CHECK for asset {_asset_id}')
                             return _csv_record
                         else:
                             if keep_value_in_file:
-                                _csv_record[index] = item_in_file[key]
+                                value = item_in_file[key]
+                                if str_is_bool(value):
+                                    value = str_to_bool(value)
+                                _csv_record[index] = value
                             # Get the old price in the previous file
                             if key == 'Price':
                                 price_index = index
                                 try:
                                     _price = float(_csv_record[price_index])
                                     old_price = float(
                                         item_in_file[key]
                                     )  # NOTE: the 'old price' is the 'price' saved in the file, not the 'old_price' in the file
                                 except Exception as _error:
-                                    self.logger.warning(f'Old Price value can not be converted for asset {_asset_id}\nError:{_error!r}')
+                                    self.logger.warning(f'Old price value can not be converted for asset {_asset_id}\nError:{_error!r}')
+                            if key == 'Origin':
+                                # all the folders when the asset came from are stored in a comma separated list
+                                folder_list = item_in_file[key].split(',')
+                                # add the new folder to the list without duplicates
+                                if _csv_record[index] not in folder_list:
+                                    folder_list.append(_csv_record[index])
+                                # update the list in the CSV record
+                                _csv_record[index] = ','.join(folder_list)
                         index += 1
 
                 _csv_record[price_index + 1] = old_price
             return _csv_record
 
         def update_and_merge_json_record_data(_asset, _items_in_file, _no_float_value: float, _no_bool_false_value: bool) -> dict:
             """
@@ -393,67 +483,48 @@
                 # Get the old price in the previous file
                 try:
                     _price = float(_json_record['Price'])
                     old_price = float(
                         _items_in_file[_asset_id]['Price']
                     )  # NOTE: the 'old price' is the 'price' saved in the file, not the 'old_price' in the file
                 except Exception as _error:
-                    self.logger.warning(f'Old Price values can not be converted for asset {_asset_id}\nError:{_error!r}')
-                _json_record['Old Price'] = old_price
+                    self.logger.warning(f'Old price values can not be converted for asset {_asset_id}\nError:{_error!r}')
+                _json_record['Old price'] = old_price
             return _json_record
 
+        output = stdout  # by default, we output to stdout
+
         self.logger.info('Logging in...')
         if not self.core.login():
             self.logger.error('Login failed, cannot continue!')
             self.core.clean_exit(1)
 
         if args.force_refresh:
-            self.logger.info('Refreshing asset list, this may take a while...')
+            self.logger.info(
+                'force_refresh option is active ...\nRefreshing asset list, this will take several minutes to acheived depending on the internet connection...'
+            )
         else:
             self.logger.info('Getting asset list... (this may take a while)')
 
         if args.filter_category and args.filter_category != gui_g.s.default_category_for_all:
             gui_g.UEVM_filter_category = args.filter_category
             self.logger.info(f'The String "{args.filter_category}" will be search in Assets category')
 
         gui_g.progress_window_ref = None
         progress_window = None
         if args.gui:
-            # check if the GUI is already running
-            if gui_g.UEVM_gui_ref is None:
-                # create a fake root because ProgressWindow must always be a top level window
-                gui_g.UEVM_gui_ref = UEVMGuiHiddenRoot()
-                uewm_gui_exists = False
-            else:
-                uewm_gui_exists = True
-            # create and use a progress window (as a top level window)
-            gui_g.UEVM_log_ref = self.logger
-            progress_window = ProgressWindow(
-                title="Updating Assets List",
-                quit_on_close=not uewm_gui_exists,
-                width=300,
-                height=150,
-                max_value=200,
-                show_start_button=False,
-                show_stop_button=True,
-                function=self.core.get_asset_list,
-                function_parameters={
-                    'filter_category': gui_g.UEVM_filter_category,
-                    'force_refresh': args.force_refresh
-                }
-            )
+            uewm_gui_exists, progress_window = init_progress_window(args=args, logger=self.logger, callback=self.core.get_asset_list)
             if uewm_gui_exists:
                 # if the main gui is running, we already have a tk.mainloop running
                 # we need to constantly update the progress bar
                 while not progress_window.must_end:
                     progress_window.update()
             else:
                 # if the main gui is not running, we need to start a tk.mainloop
                 progress_window.mainloop()
-
             items = progress_window.get_result()
 
         else:
             items = self.core.get_asset_list(platform='Windows', filter_category=args.filter_category, force_refresh=args.force_refresh)
 
         if args.include_non_asset:
             na_items = self.core.get_non_asset_library_items(skip_ue=False)
@@ -524,16 +595,14 @@
 
                 # write the content of the file to keep some data
                 if not check_and_create_path(file_src):
                     self.logger.critical(f'Could not create folder for {file_src}')
                     self.core.clean_exit(1)
                 # reopen file for writing
                 output = open(file_src, 'w', encoding='utf-8')
-            else:
-                output = stdout
             # end if args.output:
 
             try:
                 writer = csv.writer(output, dialect='excel-tab' if args.tsv else 'excel', lineterminator='\n')
                 writer.writerow(CSV_headings.keys())
                 cpt = 0
                 if gui_g.progress_window_ref is not None:
@@ -551,21 +620,14 @@
                             csv_record_merged = list(asset[1].values())
                         cpt += 1
                         writer.writerow(csv_record_merged)
                     except (OSError, UnicodeEncodeError, TypeError) as error:
                         self.logger.error(f'Could not write CSV record for {asset_id} into {args.output}\nError:{error!r}')
             except OSError:
                 self.logger.error(f'Could not write list result to {args.output}')
-            output.close()
-            self.logger.info(
-                f'\n======\n{cpt} assets have been printed or saved (without duplicates due to different UE versions)\nOperation Finished\n======\n'
-            )
-            if args.gui and progress_window is not None:
-                progress_window.close_window()
-            return
         # end if args.csv or args.tsv:
 
         if args.json:
             if args.output:
                 file_src = args.output
                 # If the output file exists, we read its content to keep some data
                 try:
@@ -577,16 +639,14 @@
 
                 # write the content of the file to keep some data
                 if not check_and_create_path(file_src):
                     self.logger.critical(f'Could not create folder for {file_src}')
                     self.core.clean_exit(1)
                 # reopen file for writing
                 output = open(file_src, 'w', encoding='utf-8')
-            else:
-                output = stdout
             # end if args.output:
 
             try:
                 cpt = 0
                 json_content = {}
                 if gui_g.progress_window_ref is not None:
                     gui_g.progress_window_ref.reset(
@@ -607,22 +667,36 @@
                         cpt += 1
                     except (OSError, UnicodeEncodeError, TypeError) as error:
                         self.logger.error(f'Could not write Json record for {asset_id} into {args.output}\nError:{error!r}')
 
                 json.dump(json_content, output, indent=2)
             except OSError:
                 self.logger.error(f'Could not write list result to {args.output}')
-            output.close()
+            # end if args.json:
+
+        if args.csv or args.tsv or args.json or args.input or args.gui:
+            # close the opened file
+            if output is not None:
+                output.close()
             self.logger.info(
                 f'\n======\n{cpt} assets have been printed or saved (without duplicates due to different UE versions)\nOperation Finished\n======\n'
             )
-            if args.gui and progress_window is not None:
+            if args.gui:
+                # During the editabletable initial rebuild_data process, the window will not close
+                # So we try to close it several times
+                max_tries = 3
+                progress_window.quit_on_close = True  # gentle quit
+                tries = 0
+                while progress_window is not None and progress_window.winfo_viewable() and tries < max_tries:
+                    progress_window.close_window()
+                    time.sleep(0.2)
+                    tries += 1
+                progress_window.quit_on_close = False  # force destroy the window
                 progress_window.close_window()
             return
-        # end if args.json:
 
         # here, no other output has been done before, so we print the asset in a quick format to the console
         print('\nAvailable UE Assets:')
         for asset in items:
             version = asset.app_version('Windows')
             print(f' * {asset.app_title.strip()} (App name: {asset.app_name} | Version: {version})')
         print(f'\nTotal: {len(items)}')
@@ -654,37 +728,47 @@
                 self.logger.critical(f'Could not fetch metadata for "{args.app_name}" (check spelling/account ownership)')
                 self.core.clean_exit(1)
             manifest_data, _ = self.core.get_cdn_manifest(item, platform='Windows')
 
         manifest = self.core.load_manifest(manifest_data)
         files = sorted(manifest.file_manifest_list.elements, key=lambda a: a.filename.lower())
 
+        content = ''
         if args.hashlist:
             for fm in files:
-                print(f'{fm.hash.hex()} *{fm.filename}')
+                content += f'{fm.hash.hex()} *{fm.filename}\n'
         elif args.csv or args.tsv:
             writer = csv.writer(stdout, dialect='excel-tab' if args.tsv else 'excel', lineterminator='\n')
             writer.writerow(['path', 'hash', 'size', 'install_tags'])
             writer.writerows((fm.filename, fm.hash.hex(), fm.file_size, '|'.join(fm.install_tags)) for fm in files)
         elif args.json:
             _files = [
                 dict(filename=fm.filename, sha_hash=fm.hash.hex(), install_tags=fm.install_tags, file_size=fm.file_size, flags=fm.flags)
                 for fm in files
             ]
+            print(content)
             return self._print_json(_files, args.pretty_json)
         else:
             install_tags = set()
             for fm in files:
-                print(fm.filename)
+                content += fm.filename + '\n'
                 for t in fm.install_tags:
                     install_tags.add(t)
             if install_tags:
                 # use the log output so this isn't included when piping file list into file
                 self.logger.info(f'Install tags: {", ".join(sorted(install_tags))}')
 
+        if args.gui:
+            uewm_gui_exists, _ = init_display_window(self.logger)
+            custom_print(content, keep_mode=False)  # as it, next print will not keep the content
+            if not uewm_gui_exists:
+                gui_g.UEVM_gui_ref.mainloop()
+        else:
+            print(content)
+
     def status(self, args) -> None:
         """
         Print the information about the vault and the available assets
         :param args: options passed to the command
         """
         if not args.offline:
             try:
@@ -714,57 +798,48 @@
 
         json_content = {
             'Epic account': user_name,  #
             'Last data update': last_update,
             'Last cache update': last_cache_update,
             'Config directory': self.core.uevmlfs.path,
             'Platform': f'{platform()} ({os.name})',
-            'Current version': f'{__version__} - {__codename__}',
+            'Current version': f'{UEVM_version} - {UEVM_codename}',
         }
         if not args.offline:
-            assets_available = len(self.core.get_asset_list(update_assets=not args.offline))
+            assets_available = len(self.core.get_asset_list(update_assets=args.force_refresh))
             json_content['Assets available'] = assets_available
             json_content['Update available'] = 'yes' if self.core.update_available else 'no'
 
             if self.core.update_available and update_information is not None:
-                json_content['Update info'] = '\n\n'
+                json_content['Update info'] = '\n'
                 json_content['New version'] = f'{update_information["version"]} - {update_information["codename"]}'
                 json_content['Release summary'] = update_information['summary']
                 json_content['Release Url'] = update_information['release_url']
                 json_content['Update recommendation'] = update_information['severity']
 
         if args.json:
             return self._print_json(json_content, args.pretty_json)
 
         if args.gui:
-            # check if the GUI is already running
-            if gui_g.UEVM_gui_ref is None:
-                # create a fake root because DisplayContentWindow must always be a top level window
-                gui_g.UEVM_gui_ref = UEVMGuiHiddenRoot()
-                uewm_gui_exists = False
-            else:
-                uewm_gui_exists = True
-            if gui_g.display_content_window_ref is None:
-                _ = DisplayContentWindow(title='UEVM: status command output', quit_on_close=not uewm_gui_exists)
-
+            uewm_gui_exists, _ = init_display_window(self.logger)
             json_print_key_val(json_content, output_on_gui=True)
             if not uewm_gui_exists:
                 gui_g.UEVM_gui_ref.mainloop()
         else:
             json_print_key_val(json_content)
 
         # prevent update message on close
         self.core.update_available = False
 
     def info(self, args) -> None:
         """
         Print information about a given app name or manifest url/path
         :param args: options passed to the command
         """
-        name_or_path = args.app_name_or_manifest
+        name_or_path = args.app_name_or_manifest or args.app_name
         app_name = manifest_uri = None
         if os.path.exists(name_or_path) or name_or_path.startswith('http'):
             manifest_uri = name_or_path
         else:
             app_name = self._resolve_aliases(name_or_path)
 
         if not args.offline and not manifest_uri:
@@ -800,15 +875,17 @@
             elif manifest_uri and os.path.exists(manifest_uri):
                 with open(manifest_uri, 'rb') as f:
                     manifest_data = f.read()
             else:
                 self.logger.info('Asset not installed and offline mode enabled, cannot load manifest.')
         elif item:
             # entitlements = self.core.egs.get_user_entitlements()
-            egl_meta = self.core.egs.get_item_info(item.namespace, item.catalog_item_id)
+            egl_meta, status_code = self.core.egs.get_item_info(item.namespace, item.catalog_item_id)
+            if status_code != 200:
+                self.logger.warning(f'Failed to fetch metadata for {item.app_name}: reponse code = {status_code}')
             item.metadata = egl_meta
             # Get manifest if asset exists for current platform
             if 'Windows' in item.asset_infos:
                 manifest_data, _ = self.core.get_cdn_manifest(item, 'Windows')
 
         if item:
             asset_infos = info_items['assets']
@@ -908,41 +985,49 @@
 
             def print_info_item(local_item: InfoItem) -> None:
                 """
                 Prints an info item to the console
                 :param local_item:  The info item to print
                 """
                 if local_item.value is None:
-                    print(f'- {local_item.name}: (None)')
+                    custom_print(f'- {local_item.name}: (None)')
                 elif isinstance(local_item.value, list):
-                    print(f'- {local_item.name}:')
+                    custom_print(f'- {local_item.name}:')
                     for list_item in local_item.value:
-                        print(' + ', list_item)
+                        custom_print(' + ', list_item)
                 elif isinstance(local_item.value, dict):
-                    print(f'- {local_item.name}:')
+                    custom_print(f'- {local_item.name}:')
                     for k, v in local_item.value.items():
-                        print(' + ', k, ':', v)
+                        custom_print(f' + {k} : {v}')
                 else:
-                    print(f'- {local_item.name}: {local_item.value}')
+                    custom_print(f'- {local_item.name}: {local_item.value}')
+
+            if args.gui:
+                uewm_gui_exists, _ = init_display_window(self.logger)
+            else:
+                uewm_gui_exists = False
 
             if info_items.get('asset'):
-                print('\nAsset Information:')
+                custom_print('\nAsset Information:')
                 for info_item in info_items['asset']:
                     print_info_item(info_item)
             if info_items.get('install'):
-                print('\nInstallation information:')
+                custom_print('\nInstallation information:')
                 for info_item in info_items['install']:
                     print_info_item(info_item)
             if info_items.get('manifest'):
-                print('\nManifest information:')
+                custom_print('\nManifest information:')
                 for info_item in info_items['manifest']:
                     print_info_item(info_item)
 
             if not any(info_items.values()):
-                print('No asset information available.')
+                custom_print('No asset information available.')
+            custom_print(keep_mode=False)  # as it, next print will not keep the content
+            if args.gui and not uewm_gui_exists:
+                gui_g.UEVM_gui_ref.mainloop()
         else:
             json_out = dict(asset=dict(), install=dict(), manifest=dict())
             if info_items.get('asset'):
                 for info_item in info_items['asset']:
                     json_out['asset'][info_item.json_name] = info_item.json_value
             if info_items.get('install'):
                 for info_item in info_items['install']:
@@ -1027,34 +1112,79 @@
             input_filename = gui_f.path_from_relative_to_absolute(args.input)
 
         app_icon_filename = gui_f.path_from_relative_to_absolute(gui_g.s.app_icon_filename)
         gui_g.UEVM_log_ref = self.logger
         gui_g.UEVM_cli_ref = self
 
         # set output file name from the input one. Used by the "rebuild file content" button (or rebuild_data method)
-        gui_f.init_gui_args(args, additional_args={'output': input_filename})
+        init_gui_args(args, additional_args={'output': input_filename})
+        rebuild = False
+        if not os.path.isfile(input_filename):
+            gui_f.create_empty_file(input_filename)
+            rebuild = True
 
         gui_g.UEVM_gui_ref = UEVMGui(
             title=gui_g.s.app_title,
             width=gui_g.s.app_width,
             height=gui_g.s.app_height,
             icon=app_icon_filename,
             screen_index=0,
             file=input_filename,
-            show_open_file_dialog=not os.path.isfile(input_filename),
+            rebuild_data=rebuild
         )
         gui_g.UEVM_gui_ref.mainloop()
         # gui_g.UEVM_gui_ref.quit()
 
+    @staticmethod
+    def print_help(args, parser=None) -> None:
+        """
+        Prints the help for the command
+        :param args:
+        :param parser: command line parser. If not provided, gui_g.UEVM_parser_ref will be used
+        """
+        if parser is None:
+            parser = gui_g.UEVM_parser_ref
+        if parser is None:
+            return
+        uewm_gui_exists = False
+
+        if args.full_help:
+            if args.gui:
+                uewm_gui_exists, _ = init_display_window()
+            custom_print(keep_mode=False, text=parser.format_help())
+
+            # Commands that should not be shown in full help/list of commands (e.g. aliases)
+            _hidden_commands = {'download', 'update', 'repair', 'get-token', 'verify-asset', 'list-assets'}
+            # Print the help for all the subparsers. Thanks stackoverflow!
+            custom_print(text='Individual command help:')
+            # noinspection PyProtectedMember,PyUnresolvedReferences
+            subparsers = next(a for a in parser._actions if isinstance(a, argparse._SubParsersAction))
+            # noinspection PyUnresolvedReferences
+            for choice, subparser in subparsers.choices.items():
+                if choice in _hidden_commands:
+                    continue
+                custom_print(text=f'\nCommand: {choice}')
+                custom_print(text=subparser.format_help())
+        elif os.name == 'nt':
+            from UEVaultManager.lfs.windows_helpers import double_clicked
+            if double_clicked():
+                custom_print(text='Please note that this is not the intended way to run UEVaultManager.')
+                custom_print(text='Follow https://github.com/LaurentOngaro/UEVaultManager#readme to set it up properly')
+                subprocess.Popen(['cmd', '/K', 'echo>nul'])
+        custom_print(keep_mode=False)  # as it, next print will not keep the content
+
+        if args.gui and not uewm_gui_exists:
+            gui_g.UEVM_gui_ref.mainloop()
+
 
 def main():
     """
     Main function
     """
-    parser = argparse.ArgumentParser(description=f'UEVaultManager v{__version__} - "{__codename__}"')
+    parser = argparse.ArgumentParser(description=f'UEVaultManager v{UEVM_version} - "{UEVM_codename}"')
     parser.register('action', 'parsers', HiddenAliasSubparsersAction)
 
     # general arguments
     parser.add_argument('-H', '--full-help', dest='full_help', action='store_true', help='Show full help (including individual command help)')
     parser.add_argument('-d', '--debug', dest='debug', action='store_true', help='Set loglevel to debug')
     parser.add_argument('-y', '--yes', dest='yes', action='store_true', help='Default to yes for all prompts')
     parser.add_argument('-V', '--version', dest='version', action='store_true', help='Print version and exit')
@@ -1068,14 +1198,22 @@
         dest='api_timeout',
         action='store',
         type=float,
         default=10,
         metavar='<seconds>',
         help='API HTTP request timeout (default: 10 seconds)'
     )
+    parser.add_argument(
+        '-g',
+        '--gui',
+        dest='gui',
+        action='store_true',
+        help='Display additional informations using gui elements like dialog boxes or progress window'
+    )
+    gui_g.UEVM_parser_ref = parser
 
     # all the commands
     subparsers = parser.add_subparsers(title='Commands', dest='subparser_name', metavar='<command>')
     auth_parser = subparsers.add_parser('auth', help='Authenticate with the Epic Games Store')
     clean_parser = subparsers.add_parser('cleanup', help='Remove old temporary, metadata, and manifest files')
     info_parser = subparsers.add_parser('info', help='Prints info about specified app name or manifest')
     list_parser = subparsers.add_parser('list', aliases=('list-assets',), hide_aliases=True, help='List available assets')
@@ -1116,102 +1254,113 @@
 
     list_parser.add_argument(
         '-T', '--third-party', dest='include_non_asset', action='store_true', default=False, help='Include assets that are not installable.'
     )
     list_parser.add_argument('--csv', dest='csv', action='store_true', help='Output in in CSV format')
     list_parser.add_argument('--tsv', dest='tsv', action='store_true', help='Output in in TSV format')
     list_parser.add_argument('--json', dest='json', action='store_true', help='Output in in JSON format')
-    list_parser.add_argument('-f', '--force-refresh', dest='force_refresh', action='store_true', help='Force a refresh of all assets metadata')
     list_parser.add_argument(
-        '-g',
-        '--gui',
-        dest='gui',
+        '-f',
+        '--force-refresh',
+        dest='force_refresh',
         action='store_true',
-        help='Display additional informations using gui elements like dialog boxes or progress window'
+        help='Force a refresh of all assets metadata. It could take some time ! If not forced, the cached data will be used'
     )
     list_parser.add_argument(
         '-fc',
         '--filter-category',
         dest='filter_category',
         action='store',
         help='Filter assets by category. Search against the asset category in the marketplace. Search is case insensitive and can be partial'
     )
     list_parser.add_argument(
         '-o', '--output', dest='output', metavar='<path/name>', action='store', help='The file name (with path) where the list should be written'
     )
+    list_parser.add_argument(
+        '-g',
+        '--gui',
+        dest='gui',
+        action='store_true',
+        help='Display additional informations using gui elements like dialog boxes or progress window'
+    )
 
     list_files_parser.add_argument(
         '--manifest', dest='override_manifest', action='store', metavar='<uri>', help='Manifest URL or path to use instead of the CDN one'
     )
     list_files_parser.add_argument('--csv', dest='csv', action='store_true', help='Output in CSV format')
     list_files_parser.add_argument('--tsv', dest='tsv', action='store_true', help='Output in TSV format')
     list_files_parser.add_argument('--json', dest='json', action='store_true', help='Output in JSON format')
     list_files_parser.add_argument(
         '--hashlist', dest='hashlist', action='store_true', help='Output file hash list in hashCheck/sha1sum -c compatible format'
     )
-    list_files_parser.add_argument('-f', '--force-refresh', dest='force_refresh', action='store_true', help='Force a refresh of all assets metadata')
+    list_files_parser.add_argument(
+        '-f',
+        '--force-refresh',
+        dest='force_refresh',
+        action='store_true',
+        help='Force a refresh of all assets metadata. It could take some time ! If not forced, the cached data will be used'
+    )
+    list_files_parser.add_argument(
+        '-g', '--gui', dest='gui', action='store_true', help='Display the output in a windows instead of using the console'
+    )
 
     status_parser.add_argument('--offline', dest='offline', action='store_true', help='Only print offline status information, do not login')
     status_parser.add_argument('--json', dest='json', action='store_true', help='Show status in JSON format')
+    status_parser.add_argument(
+        '-f',
+        '--force-refresh',
+        dest='force_refresh',
+        action='store_true',
+        help='Force a refresh of all assets metadata. It could take some time ! If not forced, the cached data will be used'
+    )
     status_parser.add_argument('-g', '--gui', dest='gui', action='store_true', help='Display the output in a windows instead of using the console')
+
     clean_parser.add_argument(
         '-m,'
         '--delete-metadata', dest='delete_metadata', action='store_true', help='Also delete metadata files. They are kept by default'
     )
     clean_parser.add_argument(
         '-e,'
         '--delete-extras-data', dest='delete_extras_data', action='store_true', help='Also delete extras data files. They are kept by default'
     )
 
     info_parser.add_argument('--offline', dest='offline', action='store_true', help='Only print info available offline')
     info_parser.add_argument('--json', dest='json', action='store_true', help='Output information in JSON format')
-    info_parser.add_argument('-f', '--force-refresh', dest='force_refresh', action='store_true', help='Force a refresh of all assets metadata')
+    info_parser.add_argument(
+        '-f',
+        '--force-refresh',
+        dest='force_refresh',
+        action='store_true',
+        help='Force a refresh of all assets metadata. It could take some time ! If not forced, the cached data will be used'
+    )
+    info_parser.add_argument('-g', '--gui', dest='gui', action='store_true', help='Display the output in a windows instead of using the console')
 
     get_token_parser.add_argument('--json', dest='json', action='store_true', help='Output information in JSON format')
     get_token_parser.add_argument('--bearer', dest='bearer', action='store_true', help='Return fresh bearer token rather than an exchange code')
 
     edit_parser.add_argument(
         '-i', '--input', dest='input', metavar='<path/name>', action='store', help='The file name (with path) where the list should be read from'
     )
     # not use for now
     # edit_parser.add_argument('--csv', dest='csv', action='store_true', help='Input file is in CSV format')
     # edit_parser.add_argument('--tsv', dest='tsv', action='store_true', help='Input file is in TSV format')
     # edit_parser.add_argument('--json', dest='json', action='store_true', help='Input file is in JSON format')
 
+    # Note: this line prints the full help and quit if not other command is available
     args, extra = parser.parse_known_args()
 
     if args.version:
-        print(f'UEVaultManager version "{__version__}", codename "{__codename__}"')
+        print(f'UEVaultManager version "{UEVM_version}", codename "{UEVM_codename}"')
         exit(0)
 
+    cli = UEVaultManagerCLI(override_config=args.config_file, api_timeout=args.api_timeout)
     if not args.subparser_name or args.full_help:
-        print(parser.format_help())
-
-        if args.full_help:
-            # Commands that should not be shown in full help/list of commands (e.g. aliases)
-            _hidden_commands = {'download', 'update', 'repair', 'get-token', 'verify-asset', 'list-assets'}
-            # Print the help for all the subparsers. Thanks stackoverflow!
-            print('Individual command help:')
-            # noinspection PyProtectedMember,PyUnresolvedReferences
-            subparsers = next(a for a in parser._actions if isinstance(a, argparse._SubParsersAction))
-            # noinspection PyUnresolvedReferences
-            for choice, subparser in subparsers.choices.items():
-                if choice in _hidden_commands:
-                    continue
-                print(f'\nCommand: {choice}')
-                print(subparser.format_help())
-        elif os.name == 'nt':
-            from UEVaultManager.lfs.windows_helpers import double_clicked
-            if double_clicked():
-                print('Please note that this is not the intended way to run UEVaultManager.')
-                print('Follow https://github.com/LaurentOngaro/UEVaultManager#readme to set it up properly')
-                subprocess.Popen(['cmd', '/K', 'echo>nul'])
+        cli.print_help(args=args, parser=parser)
         return
 
-    cli = UEVaultManagerCLI(override_config=args.config_file, api_timeout=args.api_timeout)
     ql = cli.setup_threaded_logging()
 
     conf_log_level = cli.core.uevmlfs.config.get('UEVaultManager', 'log_level', fallback='info')
     if conf_log_level == 'debug' or args.debug:
         cli.core.verbose_mode = True
         logging.getLogger().setLevel(level=logging.DEBUG)
         # keep requests quiet
```

### Comparing `UEVaultManager-1.3.0/UEVaultManager/core.py` & `UEVaultManager-1.4.0/UEVaultManager/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,79 +1,45 @@
 # coding=utf-8
 """
 Implementation for:
 - AppCore: handles most of the lower level interaction with the downloader, lfs, and api components to make writing CLI/GUI code easier and cleaner and avoid duplication.
-- CSV_headings: contains the title of each column and a boolean value to know if its contents must be preserved if it already exists in the output file (To Avoid overwriting data changed by the user in the file)
 """
 import json
 import logging
 import os
 import time
 from base64 import b64decode
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime, timedelta
 from hashlib import sha1
 from locale import getlocale, LC_CTYPE
 from platform import system
 from threading import current_thread, enumerate as thread_enumerate
 from urllib.parse import urlparse
 
-from requests import session, __version__
+from requests import session
 from requests.exceptions import HTTPError, ConnectionError
 
 import UEVaultManager.tkgui.modules.globals as gui_g  # using the shortest variable name for globals for convenience
+# noinspection PyPep8Naming
+from UEVaultManager import __version__ as UEVM_version
 from UEVaultManager.api.egs import EPCAPI, GrabResult
 from UEVaultManager.api.uevm import UEVMAPI
 from UEVaultManager.lfs.egl import EPCLFS
 from UEVaultManager.lfs.uevmlfs import UEVMLFS
 from UEVaultManager.models.app import *
 from UEVaultManager.models.exceptions import *
 from UEVaultManager.models.json_manifest import JSONManifest
 from UEVaultManager.models.manifest import Manifest
+from UEVaultManager.tkgui.modules.functions import box_message
 from UEVaultManager.utils.cli import check_and_create_path
 from UEVaultManager.utils.egl_crypt import decrypt_epic_data
 from UEVaultManager.utils.env import is_windows_mac_or_pyi
 
 # The heading dict contains the title of each column and a boolean value to know if its contents must be preserved if it already exists in the output file (To Avoid overwriting data changed by the user in the file)
-CSV_headings = {
-    'Asset_id': False,  # ! important: Do not Rename => this field is used as main key for each asset
-    'App name': False,
-    'App title': False,
-    'Category': False,
-    'UE Version': False,
-    'Review': False,
-    'Developer': False,
-    'Description': False,
-    'Status': False,
-    'Discount Price': False,
-    'On sale': False,
-    'Purchased': False,
-    'Obsolete': True,
-    'Supported Versions': False,
-    'Grab result': False,
-    'Price': False,  # ! important: Rename Wisely => this field is searched by text in the next lines
-    'Old Price': False,  # ! important: always place it after the Price field in the list
-    # User Fields
-    'Comment': True,
-    'Stars': True,
-    'Must Buy': True,
-    'Test result': True,
-    'Installed Folder': True,
-    'Alternative': True,
-    'Asset Folder': True,
-    # less important fields
-    'Page title': False,
-    'Image': False,
-    'Url': True,  # could be kept if a better url that can be used to download the asset is found
-    'Compatible Versions': False,
-    'Date Added': True,
-    'Creation Date': False,
-    'Update Date': False,
-    'Uid': False
-}
 
 # ToDo: instead of true/false return values for success/failure actually raise an exception that the CLI/GUI
 #  can handle to give the user more details. (Not required yet since there's no GUI so log output is fine)
 
 
 class AppCore:
     """
@@ -242,15 +208,19 @@
             self.uevmlfs.userdata = self.egs.start_session(exchange_token=code)
             return True
         except Exception as error:
             self.log.error(f'Logging in failed with {error!r}, please try again.')
             return False
 
     def auth_import(self) -> bool:
-        """Import refresh token from EGL installation and use it for logging in"""
+        """
+        Import refresh token from EGL installation and use it for logging in
+        :return: True if successful, False otherwise
+        :raises ValueError
+        """
         self.egl.read_config()
         remember_me_data = self.egl.config.get('RememberMe', 'Data')
         raw_data = b64decode(remember_me_data)
         # data is encrypted
         if raw_data[0] != '{':
             for data_key in self.egl.data_keys:
                 try:
@@ -273,16 +243,17 @@
         except Exception as error:
             self.log.error(f'Logging in failed with {error!r}, please try again.')
             return False
 
     def login(self, force_refresh=False) -> bool:
         """
         Attempts logging in with existing credentials.
-
-        raises ValueError if no existing credentials or InvalidCredentialsError if the API return an error
+        :param force_refresh: if True, force a refresh of the session
+        :return: True if successful, False otherwise
+        :raises ValueError if no existing credentials or InvalidCredentialsError if the API return an error
         """
         if not self.uevmlfs.userdata:
             raise ValueError('No saved credentials')
         elif self.logged_in and self.uevmlfs.userdata['expires_at']:
             dt_exp = datetime.fromisoformat(self.uevmlfs.userdata['expires_at'][:-1])
             dt_now = datetime.utcnow()
             td = dt_now - dt_exp
@@ -367,16 +338,15 @@
         cached = self.uevmlfs.get_cached_version()
         version_info = cached['data']
         if force or not version_info or (datetime.now().timestamp() - cached['last_update']) > 24 * 3600:
             version_info = self.uevm_api.get_version_information()
             self.uevmlfs.set_cached_version(version_info)
 
         web_version = version_info['version']
-        self.update_available = version_tuple(web_version) > version_tuple(__version__)
-        self.update_available = False
+        self.update_available = version_tuple(web_version) > version_tuple(UEVM_version)
 
     def get_update_info(self) -> dict:
         """
         Returns update info dict
         :return: update info dict
         """
         return self.uevmlfs.get_cached_version()['data']
@@ -416,14 +386,15 @@
     def get_asset(self, app_name: str, platform='Windows', update=False) -> AppAsset:
         """
         Returns an AppAsset object for the given app name and platform
         :param app_name: app name to get
         :param platform: platform to get asset for
         :param update: force update of asset list
         :return: AppAsset object
+        :raises ValueError: if no asset is found for the given app name and platform
         """
         if update or platform not in self.uevmlfs.assets:
             self.get_assets(update_assets=True, platform=platform)
 
         try:
             return next(i for i in self.uevmlfs.assets[platform] if i.app_name == app_name)
         except StopIteration:
@@ -495,22 +466,35 @@
             self.log.debug(f'--- START fetching data {name}{thread_data}')
 
             currently_fetching[name] = True
             start_time = datetime.now()
             name, namespace, catalog_item_id, _process_meta, _process_extras = fetch_list[name]
 
             if _process_meta:
-                eg_meta = self.egs.get_item_info(namespace, catalog_item_id, timeout=10.0)
+                eg_meta, status_code = self.egs.get_item_info(namespace, catalog_item_id, timeout=10.0)
+                if status_code != 200:
+                    self.log.warning(f'Failed to fetch metadata for {name}: reponse code = {status_code}')
+                    return False
+
                 app = App(app_name=name, app_title=eg_meta['title'], metadata=eg_meta, asset_infos=assets[name])
                 self.uevmlfs.set_item_meta(app.app_name, app)
                 apps[name] = app
 
             if _process_extras:
                 # we use title because it's less ambiguous than a name when searching an asset
                 eg_extras = self.egs.get_assets_extras(asset_name=name, asset_title=apps[name].app_title, verbose_mode=self.verbose_mode)
+
+                # check for data consistency
+                if 'stomt' in app_name.lower() or 'terrainmagic' in app_name.lower():
+                    if eg_extras.get('grab_result', '') != GrabResult.NO_ERROR.name or not eg_extras.get('purchased', False):
+                        box_message(
+                            msg=f'Some results in extras data are inconsistants for {app_name}. Please check the data and try again. Exiting...',
+                            level='error'
+                        )
+
                 self.uevmlfs.set_item_extras(app_name=name, extras=eg_extras, update_global_dict=True)
 
                 # log the asset if the title in metadata and the title in the marketplace grabbed page are not identical
                 if eg_extras['page_title'] != '' and eg_extras['page_title'] != apps[name].app_title:
                     self.log.warning(f'{name} has incoherent data. It has been added to the bad_data_logger file')
                     eg_extras['grab_result'] = GrabResult.INCONSISTANT_DATA.name
                     if self.bad_data_logger:
@@ -676,19 +660,19 @@
                     new_value=0, new_text="Fetching missing metadata...\nIt could take some time. Be patient.", new_max_value=len(fetch_list)
                 )
                 # gui_g.progress_window_ref.hide_progress_bar()
                 # gui_g.progress_window_ref.hide_stop_button()
 
             self.log.info(f'Fetching metadata for {len(fetch_list)} app(s).')
             if self.use_threads:
-                # note:  unreal engine API limits the number of connection to 16. So no more than 16 threads !
+                # note:  unreal engine API limits the number of connection to 16. So no more than 15 threads to avoid connection refused
 
                 # with ThreadPoolExecutor(max_workers=min(16, os.cpu_count() - 2), thread_name_prefix="Asset_Fetcher") as executor:
                 #    executor.map(fetch_asset_meta, fetch_list.keys(), timeout=30.0)
-                self.thread_executor = ThreadPoolExecutor(max_workers=min(16, os.cpu_count() + 2), thread_name_prefix="Asset_Fetcher")
+                self.thread_executor = ThreadPoolExecutor(max_workers=min(15, os.cpu_count() + 2), thread_name_prefix="Asset_Fetcher")
                 # Dictionary that maps each key to its corresponding Future object
                 futures = {}
                 for key in fetch_list.keys():
                     # Submit the task and add its Future to the dictionary
                     future = self.thread_executor.submit(fetch_asset_meta, key)
                     futures[key] = future
                     if self.thread_executor_must_stop:
@@ -700,36 +684,44 @@
         self.log.info(f'======\nSTARTING phase 3: emptying the List of assets to be fetched \n')
         if gui_g.progress_window_ref is not None:
             # gui_g.progress_window_ref.show_progress_bar()  # show progress bar, must be before reset
             gui_g.progress_window_ref.show_stop_button()
             gui_g.progress_window_ref.reset(new_value=0, new_text="Checking and Fetching assets data...", new_max_value=len(filtered_items))
         # loop through valid and filtered items
         meta_updated = (bypass_count == 0) and meta_updated  # to avoid deleting metadata files or assets that have been filtered
+        fetch_try_count = {}
+        fetch_try_limit = 3
         while len(filtered_items) > 0:
             if gui_g.progress_window_ref is not None and not gui_g.progress_window_ref.update_and_continue(increment=1):
                 return []
             item = filtered_items.pop()
             app_name = item['name']
             app_assets = item['asset']
+            if fetch_try_count.get(app_name):
+                fetch_try_count[app_name] += 1
+            else:
+                fetch_try_count[app_name] = 1
             if self.verbose_mode:
-                self.log.info(f'Checking {app_name}. Still {len(filtered_items)} assets to check')
+                self.log.info(f'Checking {app_name} Try number = {fetch_try_count[app_name] }. Still {len(filtered_items)} assets to check')
             try:
                 app_item = apps.get(app_name)
             except (KeyError, IndexError):
                 self.log.debug(f'{app_name} has not been found int the app list. Bypassing')
                 # item not found in app, ignore and pass to next one
                 continue
-
             # retry if the asset is still in fetch list (with active fetcher treads)
             if fetch_list.get(app_name) and (not currently_fetching.get(app_name) or 'Asset_Fetcher' not in thread_enumerate()):
                 self.log.info(f'Fetching metadata for {app_name} is still no done, retrying')
                 if currently_fetching.get(app_name):
                     del currently_fetching[app_name]
                 fetch_asset_meta(app_name)
 
+            if fetch_try_count[app_name] > fetch_try_limit:
+                self.log.error(f'Fetching metadata for {app_name} has failed {fetch_try_limit} times. Skipping')
+                continue
             try:
                 is_bypassed = (app_name in assets_bypassed) and (assets_bypassed[app_name])
                 is_a_mod = any(i['path'] == 'mods' for i in app_item.metadata.get('categories', []))
             except (KeyError, IndexError, AttributeError):
                 self.log.debug(f'{app_name} has no metadata. Adding to the fetch list (again)')
                 try:
                     fetch_list[app_name] = (app_name, item.namespace, item.catalog_item_id, True, True)
@@ -750,21 +742,22 @@
             if not is_bypassed and not is_still_fetching and not is_a_mod and has_valid_platform:
                 _ret.append(app_item)
 
         self.log.info(f'A total of {len(_ret)} assets have been analysed and kept in phase 3')
 
         self.update_aliases(force=meta_updated)
 
+        if gui_g.s.never_update_data_files:
+            meta_updated = False
         if meta_updated:
             if gui_g.progress_window_ref is not None:
                 gui_g.progress_window_ref.reset(new_value=0, new_text="Updating metadata files...", new_max_value=len(_ret))
             # delete old files
             self._prune_metadata()
             self._save_metadata(_ret)
-        #  meta_updated = True  # test only
         if meta_updated:
             if gui_g.progress_window_ref is not None:
                 gui_g.progress_window_ref.reset(new_value=0, new_text="Updating extras data files...", new_max_value=len(_ret))
             # save new ones
             self._prune_extras_data(update_global_dict=False)
             self._save_extras_data(self.uevmlfs.assets_extras_data, update_global_dict=False)
         return _ret
@@ -833,15 +826,18 @@
             if lib_item['namespace'] == 'ue' and skip_ue:
                 continue
             if lib_item['appName'] in ignore:
                 continue
 
             item = self.uevmlfs.get_item_meta(lib_item['appName'])
             if not item or force_refresh:
-                eg_meta = self.egs.get_item_info(lib_item['namespace'], lib_item['catalogItemId'])
+                eg_meta, status_code = self.egs.get_item_info(lib_item['namespace'], lib_item['catalogItemId'])
+                if status_code != 200:
+                    self.log.warning(f'Failed to fetch metadata for {lib_item["appName"]}: reponse code = {status_code}')
+                    continue
                 item = App(app_name=lib_item['appName'], app_title=eg_meta['title'], metadata=eg_meta)
                 self.uevmlfs.set_item_meta(item.app_name, item)
 
             if not any(i['path'] == 'mods' for i in item.metadata.get('categories', [])):
                 _ret.append(item)
 
         # Force refresh to make sure these titles are included in aliasing
@@ -892,14 +888,15 @@
     def get_cdn_manifest(self, item, platform='Windows', disable_https=False):
         """
         Get the CDN manifest
         :param item: Item to get the CDN manifest for
         :param platform: Platform to get the CDN manifest for
         :param disable_https: Disable HTTPS for the manifest URLs
         :return: list of base URLs, manifest hash
+        :raises ValueError
         """
         manifest_urls, base_urls, manifest_hash = self.get_cdn_urls(item, platform)
         if not manifest_urls:
             raise ValueError('No manifest URLs returned by API')
 
         if disable_https:
             manifest_urls = [url.replace('https://', 'http://') for url in manifest_urls]
```

### Comparing `UEVaultManager-1.3.0/UEVaultManager/downloader/mp/manager.py` & `UEVaultManager-1.4.0/UEVaultManager/downloader/mp/manager.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/downloader/mp/workers.py` & `UEVaultManager-1.4.0/UEVaultManager/downloader/mp/workers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/lfs/egl.py` & `UEVaultManager-1.4.0/UEVaultManager/lfs/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/lfs/eos.py` & `UEVaultManager-1.4.0/UEVaultManager/lfs/eos.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/lfs/uevmlfs.py` & `UEVaultManager-1.4.0/UEVaultManager/lfs/uevmlfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import logging
 import os
 from collections import defaultdict
 from pathlib import Path
 from time import time
 
 from UEVaultManager.models.app import *
-from UEVaultManager.models.config import LGDConf
+from UEVaultManager.models.config import AppConf
 from UEVaultManager.utils.aliasing import generate_aliases
 from UEVaultManager.utils.env import is_windows_mac_or_pyi
 from .utils import clean_filename
 
 
 class UEVMLFS:
     """
@@ -43,15 +43,15 @@
         self.assets_extras_data = dict()
         # UEVaultManager update check info
         self._update_info = None
         # UE assets metadata cache data
         self._ue_assets_cache_data = None
 
         # Config with item specific settings (e.g. start parameters, env variables)
-        self.config = LGDConf(comment_prefixes='/', allow_no_value=True)
+        self.config = AppConf(comment_prefixes='/', allow_no_value=True)
 
         # Folders used by the app
         self.manifests_folder = 'manifests'
         self.metadata_folder = 'metadata'
         self.tmp_folder = 'tmp'
         self.extras_folder = 'extras'
 
@@ -208,14 +208,15 @@
             return None
 
     @userdata.setter
     def userdata(self, userdata: dict) -> None:
         """
         Set the user data
         :param userdata: User data
+        :raises ValueError: If userdata is None
         """
         if userdata is None:
             raise ValueError('Userdata is none!')
 
         self._user_data = userdata
         json.dump(userdata, open(os.path.join(self.path, 'user.json'), 'w'), indent=2, sort_keys=True)
 
@@ -243,15 +244,16 @@
 
         return self._assets
 
     @assets.setter
     def assets(self, assets) -> None:
         """
         Set the assets data
-        :param assets: data
+        :param assets: assets
+        :raises ValueError: If assets is None
         """
         if assets is None:
             raise ValueError('Assets is none!')
 
         self._assets = assets
         json.dump(
             {platform: [a.__dict__ for a in assets] for platform, assets in self._assets.items()},
@@ -300,14 +302,15 @@
         meta_file = os.path.join(self.path, 'metadata', f'{app_name}.json')
         json.dump(json_meta, open(meta_file, 'w'), indent=2, sort_keys=True)
 
     def delete_item_meta(self, app_name: str) -> None:
         """
         Delete the metadata for an item
         :param app_name: The name of the item
+        :raises ValueError: If the item does not exist
         """
         if app_name not in self.assets_metadata:
             raise ValueError(f'Item {app_name} does not exist in metadata DB!')
 
         del self.assets_metadata[app_name]
         meta_file = os.path.join(self.path, 'metadata', f'{app_name}.json')
         if os.path.exists(meta_file):
```

### Comparing `UEVaultManager-1.3.0/UEVaultManager/lfs/utils.py` & `UEVaultManager-1.4.0/UEVaultManager/lfs/utils.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/lfs/windows_helpers.py` & `UEVaultManager-1.4.0/UEVaultManager/lfs/windows_helpers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/models/app.py` & `UEVaultManager-1.4.0/UEVaultManager/models/app.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/models/chunk.py` & `UEVaultManager-1.4.0/UEVaultManager/models/chunk.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/models/downloading.py` & `UEVaultManager-1.4.0/UEVaultManager/models/downloading.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/models/egl.py` & `UEVaultManager-1.4.0/UEVaultManager/models/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/models/json_manifest.py` & `UEVaultManager-1.4.0/UEVaultManager/models/json_manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/models/manifest.py` & `UEVaultManager-1.4.0/UEVaultManager/models/manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/tkgui/main.py` & `UEVaultManager-1.4.0/UEVaultManager/tkgui/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 # coding=utf-8
 """
 GUI module for UEVaultManager
 this can be run directly by executing this script
 or by the --edit command option for the UEVaultManager cli application, for instance by running `cli --edit --input <my_source_file>'
 """
+import os.path
+
 import UEVaultManager.tkgui.modules.functions as gui_f  # using the shortest variable name for globals for convenience
 import UEVaultManager.tkgui.modules.globals as gui_g  # using the shortest variable name for globals for convenience
 from UEVaultManager.tkgui.modules.UEVMGuiClass import UEVMGui
 
 if __name__ == '__main__':
     app_icon_filename = gui_f.path_from_relative_to_absolute(gui_g.s.app_icon_filename)
     csv_filename = gui_f.path_from_relative_to_absolute(gui_g.s.csv_filename)
+    rebuild = False
+    if not os.path.isfile(csv_filename):
+        gui_f.create_empty_file(csv_filename)
+        rebuild = True
     main_window = UEVMGui(
-        title=gui_g.s.app_title, width=gui_g.s.app_width, height=gui_g.s.app_height, icon=app_icon_filename, screen_index=0, file=csv_filename
+        title=gui_g.s.app_title, width=gui_g.s.app_width, height=gui_g.s.app_height, icon=app_icon_filename, screen_index=0, file=csv_filename, rebuild_data=rebuild
     )
     main_window.mainloop()
```

### Comparing `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py` & `UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     :param height: the height of the window
     :param icon: the icon of the window
     :param screen_index: the index of the screen on which the window will be displayed
     :param quit_on_close: whether to quit the application when the window is closed
 
     """
 
-    def __init__(self, title: str, width: int = 400, height: int = 430, icon=None, screen_index=0, quit_on_close=False):
+    def __init__(self, title: str, width: int = 600, height: int = 430, icon=None, screen_index=0, quit_on_close=False):
         super().__init__()
         self.title(title)
         style = gui_f.set_custom_style(gui_g.s.theme_name, gui_g.s.theme_font)
         self.style = style
         # if tk._default_root == self :
         #     style = gui_f.set_custom_style(gui_g.s.theme_name, gui_g.s.theme_font)
         #     print(f"style SELF = {style.theme_use()}")
@@ -50,15 +50,15 @@
         else:
             # windows only (remove the minimize/maximize buttons and the icon)
             icon = gui_f.path_from_relative_to_absolute(icon)
             if icon != '' and os.path.isfile(icon):
                 self.iconbitmap(icon)
         self.resizable(True, False)
         self.quit_on_close = quit_on_close
-
+        self.keep_existing = False  # whether to keep the existing content when adding a new one
         self.content_frame = self.ContentFrame(self)
         self.control_frame = self.ControlFrame(self)
 
         self.content_frame.pack(ipadx=5, ipady=5, padx=5, pady=5, fill=tk.X)
         self.control_frame.pack(ipadx=5, ipady=5, padx=5, pady=5, fill=tk.X)
 
         self.bind('<Key>', self.on_key_press)
@@ -70,18 +70,24 @@
         """
         The frame containing the content of the window
         :param container: the container of the frame
         """
 
         def __init__(self, container):
             super().__init__(container)
-            pack_def_options = {'ipadx': 3, 'ipady': 3, 'padx': 5, 'pady': 5, 'fill': tk.X}
+            pack_def_options = {'ipadx': 3, 'ipady': 3}
 
             text_content = ExtendedText(self)
-            text_content.pack(**pack_def_options)
+            scrollbar = ttk.Scrollbar(self)
+            scrollbar.pack(side="right", fill="y")
+            scrollbar.config(command=text_content.yview)
+            text_content.config(yscrollcommand=scrollbar.set)
+            scrollbar.pack(side=tk.RIGHT, fill=tk.Y, **pack_def_options)
+            text_content.pack(side=tk.LEFT, fill=tk.BOTH, expand=True, **pack_def_options)
+
             self.text_content = text_content
 
     class ControlFrame(ttk.Frame):
         """
         The frame containing the control buttons of the window
         :param container: the container of the frame
         """
@@ -120,21 +126,29 @@
         """
         gui_g.display_content_window_ref = None
         if self.quit_on_close:
             self.quit()
         else:
             self.destroy()
 
-    def display(self, content: str) -> None:
+    def display(self, content='', keep_mode=True) -> None:
         """
-        Display the content in the window
+        Display the content in the window. By default, ie. keep_mode==True, each new call adds the content to the existing content with a new line.
         :param content: the text to print
+        :param keep_mode: whether to keep the existing content when a new one is added
         """
-        self.content_frame.text_content.delete('1.0', tk.END)
-        self.content_frame.text_content.insert(tk.END, content)
+
+        if self.keep_existing:
+            content += '\n'
+            self.content_frame.text_content.insert(tk.END, content)
+        else:
+            self.content_frame.text_content.delete('1.0', tk.END)
+            self.content_frame.text_content.insert(tk.END, content)
+        # set the mode at the end to allow using display() to be used to change the mode for the next call
+        self.keep_existing = keep_mode
 
     def clean(self) -> None:
         """
         Clean the content of the window
         """
         self.content_frame.text_content.delete('1.0', tk.END)
```

### Comparing `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/EditCellWindowClass.py` & `UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/EditCellWindowClass.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,20 +70,23 @@
         """
         The frame containing the control buttons of the window
         :param container: the container of the frame
         """
 
         def __init__(self, container):
             super().__init__(container)
-            pack_def_options = {'ipadx': 3, 'ipady': 3, 'fill': tk.X}
+            grid_def_options = {'ipadx': 5, 'ipady': 5, 'padx': 2, 'pady': 2, 'sticky': tk.NSEW}
             # (bootstyle is not recognized by PyCharm)
+            ttk.Label(self, text='Respect the initial format when changing a value').grid(row=0, column=0, columnspan=2, **grid_def_options)
             # noinspection PyArgumentList
-            ttk.Button(self, text='Close', command=container.on_close, bootstyle=WARNING).pack(**pack_def_options, side=tk.RIGHT)
+            ttk.Button(self, text='Save Changes', command=container.save_change, bootstyle=INFO).grid(row=1, column=0, **grid_def_options)
             # noinspection PyArgumentList
-            ttk.Button(self, text='Save Changes', command=container.save_change, bootstyle=INFO).pack(**pack_def_options, side=tk.RIGHT)
+            ttk.Button(self, text='Close', command=container.on_close, bootstyle=WARNING).grid(row=1, column=1, **grid_def_options)
+            self.columnconfigure('all', weight=1)
+            self.rowconfigure('all', weight=1)
 
     def on_key_press(self, event) -> None:
         """
         Event when a key is pressed
         :param event: the event that triggered the call of this function
         """
         if event.keysym == 'Escape':
```

### Comparing `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/EditRowWindowClass.py` & `UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/EditRowWindowClass.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             self.canvas_image = canvas_image
 
     def on_close(self, _event=None) -> None:
         """
         Event when the window is closing
         :param _event: the event that triggered the call of this function
         """
-        current_values = self.editable_table.get_selected_row_values()
+        current_values = self.editable_table.get_edited_row_values()
         # current_values is empty is save_button has been pressed because global variables have been cleared in save_changes()
         self.must_save = current_values and self.initial_values != current_values
         if self.must_save:
             if gui_f.box_yesno('Changes have been made in the window. Do you want to keep them ?'):
                 self.save_change()
         self.close_window()
```

### Comparing `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/EditableTableClass.py` & `UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/EditableTableClass.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # coding=utf-8
 """
 Implementation for:
 - EditableTable is a custom class that extends the pandastable.Table class, providing additional functionality
 """
+import io
 import webbrowser
 from tkinter import ttk
 
 import pandas as pd
-from pandastable import Table, TableModel
+from pandas.errors import EmptyDataError
+from pandastable import Table, TableModel, config
 
+from UEVaultManager.models.csv import create_emty_csv_row, CSV_headings
 from UEVaultManager.tkgui.modules.EditCellWindowClass import EditCellWindow
 from UEVaultManager.tkgui.modules.EditRowWindowClass import EditRowWindow
-from UEVaultManager.tkgui.modules.ExtendedWidgetClasses import ExtendedText
+from UEVaultManager.tkgui.modules.ExtendedWidgetClasses import ExtendedText, ExtendedCheckButton
 from UEVaultManager.tkgui.modules.functions import *
 from UEVaultManager.tkgui.modules.TaggedLabelFrameClass import TaggedLabelFrame
 
 
 class EditableTable(Table):
     """
     EditableTable is a custom class that extends the pandastable.Table class, providing additional functionality
@@ -24,23 +27,27 @@
     :param file: The path to the CSV file containing the table data.
     :param fontsize: The font size for the table.
     :param show_toolbar: Whether to show the toolbar.
     :param show_statusbar: Whether to show the status bar.
     :param kwargs: Additional arguments to pass to the pandastable.Table class.
     """
 
-    def __init__(self, container_frame=None, file=None, fontsize=10, show_toolbar=False, show_statusbar=False, **kwargs):
+    def __init__(self, container_frame=None, file=None, rows_per_page=36, show_toolbar=False, show_statusbar=False, **kwargs):
         self._last_selected_row = -1
         self._last_selected_col = -1
 
         self.file = file
         self.must_save = False
+        self.must_rebuild = False
+        self.container_frame = container_frame
+        self.show_toolbar = show_toolbar
+        self.show_statusbar = show_statusbar
 
         self.pagination_enabled = True
-        self.rows_per_page = 35
+        self.rows_per_page = rows_per_page
         self.current_page = 0
         self.total_pages = 0
 
         self.data = None
         self.data_filtered = None
 
         self.edit_row_window = None
@@ -50,31 +57,144 @@
         self.edit_cell_window = None
         self.edit_cell_row_index = None
         self.edit_cell_col_index = None
         self.edit_cell_entry = None
 
         self.load_data()
         Table.__init__(self, container_frame, dataframe=self.data, showtoolbar=show_toolbar, showstatusbar=show_statusbar, **kwargs)
-        self.fontsize = fontsize
-        self.setFont()
-
         self.bind('<Double-Button-1>', self.create_edit_cell_window)
 
     def _generate_cell_selection_changed_event(self) -> None:
         """
         Creates the event bindings for the table.
         """
         selected_row = self.currentrow
         selected_col = self.currentcol
 
         if (selected_row != self._last_selected_row) or (selected_col != self._last_selected_col):
             self._last_selected_row = selected_row
             self._last_selected_col = selected_col
             self.event_generate('<<CellSelectionChanged>>')
 
+    def gradient_color_cells(self, col_names=None, cmap='sunset', alpha=1) -> None:
+        """
+        Creates a gradient color for the cells os specified columns. The gradient depends on the cell value between min and max values for that column.
+        :param col_names: The names of the columns to create a gradient color for.
+        :param cmap: name of the colormap to use
+        :param alpha: alpha value for the color
+        """
+        # import pylab as plt
+        # cmaps = sorted(m for m in plt.cm.datad if not m.endswith("_r"))
+        # print(cmaps)
+        # possible cmaps:
+        # 'Accent', 'Blues', 'BrBG', 'BuGn', 'BuPu', 'CMRmap', 'Dark2', 'GnBu', 'Greens', 'Greys', 'OrRd', 'Oranges', 'PRGn', 'Paired', 'Pastel1',
+        #  'Pastel2', 'PiYG', 'PuBu', 'PuBuGn', 'PuOr', 'PuRd', 'Purples', 'RdBu', 'RdGy', 'RdPu', 'RdYlBu', 'RdYlGn', 'Reds', 'Set1', 'Set2', 'Set3',
+        #  'Spectral', 'Wistia', 'YlGn', 'YlGnBu', 'YlOrBr', 'YlOrRd', 'afmhot', 'autumn', 'binary', 'bone', 'brg', 'bwr', 'cool', 'coolwarm', 'copper',
+        #  'cubehelix', 'flag', 'gist_earth', 'gist_gray', 'gist_heat', 'gist_ncar', 'gist_rainbow', 'gist_stern', 'gist_yarg', 'gnuplot', 'gnuplot2',
+        #  'gray', 'hot', 'hsv', 'jet', 'nipy_spectral', 'ocean', 'pink', 'prism', 'rainbow', 'seismic', 'spring', 'summer', 'tab10', 'tab20', 'tab20b',
+        #  'tab20c', 'terrain', 'winter'
+
+        if col_names is None:
+            return
+        df = self.data_filtered if self.data_filtered is not None else self.model.df
+        for colname in col_names:
+            x = df[colname]
+            clrs = self.values_to_colors(x, cmap, alpha)
+            clrs = pd.Series(clrs, index=df.index)
+            rc = self.rowcolors
+            rc[colname] = clrs
+
+    def color_cells_if(self, col_names=None, color='green', value_to_check='True') -> None:
+        """
+        Set the cell color for the specified columns and the cell with a given value.
+        :param col_names: The names of the columns to create a gradient color for.
+        :param color: The color to set the cell to.
+        :param value_to_check: The value to check for.
+        """
+
+        if col_names is None:
+            return
+        df = self.data_filtered if self.data_filtered is not None else self.model.df
+        for col_name in col_names:
+            if col_name not in df.columns:
+                continue
+            mask = df[col_name] == value_to_check
+            self.setColorByMask(col=col_name, mask=mask, clr=color)
+
+    def color_cells_if_not(self, col_names=None, color='grey', value_to_check='False') -> None:
+        """
+        Set the cell color for the specified columns and the cell with NOT a given value.
+        :param col_names: The names of the columns to create a gradient color for.
+        :param color: The color to set the cell to.
+        :param value_to_check: The value to check for.
+        """
+        if col_names is None:
+            return
+        df = self.data_filtered if self.data_filtered is not None else self.model.df
+        for col_name in col_names:
+            if col_name not in df.columns:
+                continue
+            mask = df[col_name] != value_to_check
+            self.setColorByMask(col=col_name, mask=mask, clr=color)
+
+    def color_rows_if(self, col_names=None, color='#55555', value_to_check='True') -> None:
+        """
+        Set the row color for the specified columns and the rows with a given value.
+        :param col_names: The names of the columns to check for the value.
+        :param color: The color to set the row to.
+        :param value_to_check: The value to check for.
+        """
+        if col_names is None:
+            return
+        df = self.data_filtered if self.data_filtered is not None else self.model.df
+
+        for col_name in col_names:
+            if col_name not in df.columns:
+                continue
+            row_indices = []
+            mask = df[col_name]
+            for i in range(min(self.rows_per_page, len(mask))):
+                try:
+                    if str(mask[i]) == value_to_check:
+                        row_indices.append(i)
+                except KeyError:
+                    log_debug(f'KeyError for row {i} in color_rows_if')
+            if len(row_indices) > 0:  # Check if there are any row indices
+                self.setRowColors(rows=row_indices, clr=color, cols='all')
+            return
+
+    def set_preferences(self, default_pref=None) -> None:
+        """
+        Initializes the table preferences.
+        :param default_pref: The default preferences to apply to the table.
+        """
+        # remove the warning: "A value is trying to be set on a copy of a slice from a DataFrame"
+        # when sorting the table with pagination enabled
+        # see: https://stackoverflow.com/questions/20625582/how-to-deal-with-settingwithcopywarning-in-pandas
+        pd.options.mode.chained_assignment = None
+
+        if default_pref is not None:
+            config.apply_options(default_pref, self)
+
+    def set_colors(self) -> None:
+        """
+        Initializes the colors of some cells depending on their values.
+        """
+        if not gui_g.s.use_colors_for_data:
+            self.redraw()
+            return
+        log_debug(f'set_colors')
+        self.gradient_color_cells(col_names=['Review'], cmap='Set3', alpha=1)
+        self.color_cells_if(col_names=['Purchased', 'On sale'], color='lightgreen', value_to_check='True')
+        self.color_cells_if(col_names=['Grab result'], color='lightblue', value_to_check='NO_ERROR')
+        self.color_cells_if_not(col_names=['Status'], color='#555555', value_to_check='ACTIVE')
+        self.color_rows_if(col_names=['Status'], color='#555555', value_to_check='SUNSET')
+        self.color_rows_if(col_names=['Obsolete'], color='#777777', value_to_check='True')
+        self.redraw()
+
     def handle_left_click(self, event) -> None:
         """
         Handles left-click events on the table.
         :param event: The event that triggered the function call.
         """
         super().handle_left_click(event)
         self._generate_cell_selection_changed_event()
@@ -103,22 +223,23 @@
             self.current_page = page
             start = page * self.rows_per_page
             end = start + self.rows_per_page
             try:
                 # Update table with data for current page
                 self.model.df = self.data.iloc[start:end]
             except AttributeError:
-                self.redraw()
+                # self.redraw()
+                self.set_colors()
                 return
         else:
             # Update table with all data
             self.model.df = self.data_filtered
             self.current_page = 0
-        # self.updateModel(TableModel(data))
-        self.redraw()
+        # self.redraw()
+        self.set_colors()
 
     def next_page(self) -> None:
         """
         Navigates to the next page of the table data.
         """
         if self.current_page <= self.total_pages:
             self.show_page(self.current_page + 1)
@@ -148,49 +269,66 @@
         """
         csv_options = {
             'converters': {
                 'Asset_id': str,  #
                 'App name': str,  #
                 'Review': float,  #
                 'Price': float,  #
-                'Old Price': float,  #
+                'Old price': float,  #
                 'Purchased': convert_to_bool,  #
-                'Must Buy': convert_to_bool,  #
-                'Date Added': convert_to_datetime,  #
+                'Must buy': convert_to_bool,  #
+                'Date added': convert_to_datetime,  #
             },
             'on_bad_lines': 'warn',
             'encoding': "utf-8",
         }
         if not os.path.isfile(self.file):
             log_warning(f'File not found: {self.file}')
             return
 
-        self.data = pd.read_csv(self.file, **csv_options)
+        self.must_rebuild = False
+        try:
+            self.data = pd.read_csv(self.file, **csv_options)
+        except EmptyDataError:
+            # will create an empty row with the correct columns
+            str_data = ','.join(str(value) for value in CSV_headings.keys())  # column names
+            str_data += '\n'
+            str_data += create_emty_csv_row(return_as_string=True)  # dummy row
+            self.data = pd.read_csv(io.StringIO(str_data))
+            self.must_rebuild = True
+
+        self.init_data_format()
+
         # log_debug("\nCOL TYPES AFTER LOADING CSV\n")
-        # self.data.info() # direct print info
+        # self.data.info()  # direct print info
 
         self.total_pages = (len(self.data) - 1) // self.rows_per_page + 1
+        self.data_filtered = self.data
 
+    def init_data_format(self) -> None:
+        """
+        Initializes the data format for the table.
+        """
         for col in self.data.columns:
             try:
                 self.data[col] = self.data[col].astype(str)
             except (KeyError, ValueError) as error:
                 log_error(f'Could not convert column "{col}" to string. Error: {error}')
 
-        col_to_convert = ['Creation Date', 'Update Date']
+        col_to_convert = ['Creation date', 'Update date']
         # note "date added" does not use the same format as the other date columns
         for col in col_to_convert:
             col_type = self.data.get(col, None)
             if col_type is not None:
                 try:
-                    self.data[col] = pd.to_datetime(self.data[col], format='ISO8601')
+                    self.data[col] = pd.to_datetime(self.data[col], format='ISO8601', errors='ignore')
                 except (KeyError, ValueError) as error:
                     log_error(f'Could not convert column "{col}" to datetime. Error: {error}')
 
-        col_to_convert = ['Review', 'Price', 'Old Price', 'Discount Price']
+        col_to_convert = ['Review', 'Price', 'Old price', 'Discount price']
         for col in col_to_convert:
             col_type = self.data.get(col, None)
             if col_type is not None:
                 try:
                     self.data[col] = self.data[col].astype(float)
                 except (KeyError, ValueError) as error:
                     log_error(f'Could not convert column "{col}" to float. Error: {error}')
@@ -224,14 +362,15 @@
 
         # we use a string comparison here to avoid to import of the module to check the real class of UEVM_cli_ref
         if gui_g.UEVM_cli_ref is None or 'UEVaultManagerCLI' not in str(type(gui_g.UEVM_cli_ref)):
             from_cli_only_message()
             return False
         else:
             gui_g.UEVM_cli_ref.list_assets(gui_g.UEVM_cli_args)
+            self.current_page = 0
             self.load_data()
             self.show_page(self.current_page)
             return True
 
     def save_data(self) -> None:
         """
         Saves the current table data to the CSV file.
@@ -303,28 +442,28 @@
 
     def zoom_out(self) -> None:
         """
         Decreases the font size of the table.
         """
         self.zoomOut()
 
-    def get_selected_row_values(self) -> dict:
+    def get_edited_row_values(self) -> dict:
         """
         Returns the values of the selected row in the table.
         :return: A dictionary containing the column names and their corresponding values for the selected row.
         """
         if self.edit_row_entries is None or self.edit_row_index is None:
             return {}
         entries_values = {}
         for key, entry in self.edit_row_entries.items():
             try:
-                # get value for an entry tk widget
                 value = entry.get()
+            except AttributeError:
+                value = entry.get_content()  # for extendedWidgets
             except TypeError:
-                # get value for a text tk widget
                 value = entry.get('1.0', 'end')
             entries_values[key] = value
         return entries_values
 
     def create_edit_record_window(self) -> None:
         """
         Creates the edit row window for the selected row in the table.
@@ -380,17 +519,20 @@
                 inner_frame_url.grid(row=i, column=1, sticky=tk.EW)
                 entry = ttk.Entry(inner_frame_url)
                 entry.insert(0, value)
                 entry.pack(side=tk.LEFT, fill=tk.X, expand=True)
                 button = ttk.Button(inner_frame_url, text="Open URL", command=self.open_asset_url)
                 button.pack(side=tk.RIGHT)
             elif lower_key in ('description', 'comment'):
-                # description and comment fields are text
                 entry = ExtendedText(edit_row_window.content_frame, height=3)
-                entry.insert('1.0', value)
+                entry.set_content(value)
+                entry.grid(row=i, column=1, sticky=tk.EW)
+            elif lower_key in ('must buy', 'obsolete', 'purchased', 'on sale'):
+                entry = ExtendedCheckButton(edit_row_window.content_frame, label='')
+                entry.set_content(value)
                 entry.grid(row=i, column=1, sticky=tk.EW)
             else:
                 # other field is just a usual entry
                 entry = ttk.Entry(edit_row_window.content_frame)
                 entry.insert(0, value)
                 entry.grid(row=i, column=1, sticky=tk.EW)
 
@@ -398,27 +540,28 @@
 
         # image preview
         show_asset_image(image_url=image_url, canvas_image=edit_row_window.control_frame.canvas_image)
 
         self.edit_row_entries = entries
         self.edit_row_index = row_selected
         self.edit_row_window = edit_row_window
-        edit_row_window.initial_values = self.get_selected_row_values()
+        edit_row_window.initial_values = self.get_edited_row_values()
 
     def save_edit_row_record(self) -> None:
         """
         Saves the edited row values to the table data.
         """
-        for key, value in self.get_selected_row_values().items():
+        for key, value in self.get_edited_row_values().items():
             self.model.df.at[self.edit_row_index, key] = value
         self.edit_row_entries = None
         self.edit_row_index = None
         self.redraw()
         self.must_save = True
         self.edit_row_window.close_window()
+        self.update_quick_edit()
 
     def move_to_prev_record(self) -> None:
         """
         Navigates to the previous row in the table and opens the edit row window.
         """
         row_selected = self.getSelectedRow()
         if row_selected is None or row_selected == 0:
@@ -449,15 +592,15 @@
         col_index = self.get_col_clicked(event)
         if row_index is None or col_index is None:
             return None
         cell_value = self.model.df.iat[row_index, col_index]
 
         title = 'Edit current cell values'
         width = 300
-        height = 90
+        height = 110
         # window is displayed at mouse position
         # x = self.master.winfo_rootx()
         # y = self.master.winfo_rooty()
         edit_cell_window = EditCellWindow(parent=self.master, title=title, width=width, height=height, editable_table=self)
         edit_cell_window.grab_set()
         edit_cell_window.minsize(width, height)
 
@@ -505,74 +648,86 @@
             self.edit_cell_entry = None
             self.edit_cell_row_index = None
             self.edit_cell_col_index = None
         except TypeError:
             log_warning(f'Failed to get content of {widget}')
         self.redraw()
         self.edit_cell_window.close_window()
+        self.update_quick_edit()
 
-    def quit_edit_content(self, quick_edit_frame: TaggedLabelFrame = None, row: int = None) -> None:
+    def update_quick_edit(self, quick_edit_frame: TaggedLabelFrame = None, row: int = None) -> None:
         """
         Quick edit the content some cells of the selected row.
         :param quick_edit_frame: The frame to display the cell content preview in.
         :param row: The row index of the selected cell.
         """
         if row is None or row >= len(self.model.df) or quick_edit_frame is None:
             return
-        # url
+        # Url
         col = self.model.df.columns.get_loc('Url')
-        value = self.model.getValueAt(row, col)
-        quick_edit_frame.set_child_values(tag='url', content=value, row=row, col=col)
-        # stars
-        col = self.model.df.columns.get_loc('Stars')
-        value = self.model.getValueAt(row, col)
-        quick_edit_frame.set_child_values(tag='stars', content=value, row=row, col=col)
-        # comment
+        value = self.model.getValueAt(row=row, col=col)
+        quick_edit_frame.set_child_values(tag='Url', content=value, row=row, col=col)
+        # Comment
         col = self.model.df.columns.get_loc('Comment')
-        value = self.model.getValueAt(row, col)
-        quick_edit_frame.set_child_values(tag='comment', content=value, row=row, col=col)
-        # test_result
+        value = self.model.getValueAt(row=row, col=col)
+        quick_edit_frame.set_child_values(tag='Comment', content=value, row=row, col=col)
+        # Stars
+        col = self.model.df.columns.get_loc('Stars')
+        value = self.model.getValueAt(row=row, col=col)
+        quick_edit_frame.set_child_values(tag='Stars', content=value, row=row, col=col)
+        # Test
         col = self.model.df.columns.get_loc('Test result')
-        value = self.model.getValueAt(row, col)
-        quick_edit_frame.set_child_values(tag='test_result', content=value, row=row, col=col)
-        # alternative
+        value = self.model.getValueAt(row=row, col=col)
+        quick_edit_frame.set_child_values(tag='Test result', content=value, row=row, col=col)
+        # Must buy
+        col = self.model.df.columns.get_loc('Must buy')
+        value = self.model.getValueAt(row=row, col=col)
+        quick_edit_frame.set_child_values(tag='Must buy', label='', content=value, row=row, col=col)
+        # Alternative
         col = self.model.df.columns.get_loc('Alternative')
-        value = self.model.getValueAt(row, col)
-        quick_edit_frame.set_child_values(tag='alternative', content=value, row=row, col=col)
-        # Installed folder
-        col = self.model.df.columns.get_loc('Installed Folder')
-        value = self.model.getValueAt(row, col)
-        quick_edit_frame.set_child_values(tag='folder', content=value, row=row, col=col)
+        value = self.model.getValueAt(row=row, col=col)
+        quick_edit_frame.set_child_values(tag='Alternative', content=value, row=row, col=col)
+        # Installed
+        col = self.model.df.columns.get_loc('Installed folder')
+        value = self.model.getValueAt(row=row, col=col)
+        quick_edit_frame.set_child_values(tag='Installed folder', content=value, row=row, col=col)
+        # Origin
+        col = self.model.df.columns.get_loc('Origin')
+        value = self.model.getValueAt(row=row, col=col)
+        quick_edit_frame.set_child_values(tag='Origin', content=value, row=row, col=col)
 
     @staticmethod
     def quick_edit(quick_edit_frame: TaggedLabelFrame = None) -> None:
         """
         Resets the cell content preview.
         :param quick_edit_frame: The frame to reset the cell content preview in.
         """
-        quick_edit_frame.set_default_content('asset_url')
-        quick_edit_frame.set_default_content('asset_comment')
-        quick_edit_frame.set_default_content('asset_test_result')
-        quick_edit_frame.set_default_content('asset_alternative')
-        quick_edit_frame.set_default_content('asset_folder')
+        quick_edit_frame.set_default_content('Url')
+        quick_edit_frame.set_default_content('Comments')
+        quick_edit_frame.set_default_content('Stars')
+        quick_edit_frame.set_default_content('Test result')
+        quick_edit_frame.set_default_content('Must buy')
+        quick_edit_frame.set_default_content('Installed folder')
+        quick_edit_frame.set_default_content('Origin')
+        quick_edit_frame.set_default_content('Alternative')
 
     def quick_edit_save_value(self, value: str, row: int = None, col: int = None) -> None:
         """
         Saves the cell content preview.
         :param value: The value to save.
         :param row: The row index of the cell.
         :param col: The column index of the cell.
         """
         if row is None or row >= len(self.model.df) or col is None:
             return
         try:
             self.model.df.iat[row, col] = value
             self.redraw()
             self.must_save = True
-            log_info(f'Save preview value {value} at row={row} col={col}')
+            log_debug(f'Save preview value {value} at row={row} col={col}')
         except IndexError:
             log_warning(f'Failed to save preview value {value} at row={row} col={col}')
 
     def get_image_url(self, row: int = None) -> str:
         """
         Returns the image URL of the selected row.
         :param row: The row index of the selected cell.
@@ -593,15 +748,16 @@
         if url is None:
             if self.edit_row_entries is None:
                 return
             asset_url = self.edit_row_entries['Url'].get()
         else:
             asset_url = url
         log_info(f'calling open_asset_url={asset_url}')
-        if asset_url is None or asset_url == '' or asset_url == 'nan':
+        if asset_url is None or asset_url == '' or asset_url == gui_g.s.empty_cell:
+            log_info('asset URL is empty for this asset')
             return
         webbrowser.open(asset_url)
 
     def reset_style(self) -> None:
         """
         Resets the table style. Usefull when style of the main ttk window has changed.
         """
```

### Comparing `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py` & `UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 - ExtendedEntry: extended entry widget
 - ExtendedText: extended text widget
 - ExtendedLabel: extended label widget
 - ExtendedCheckButton: extended checkbutton widget
 """
 
 import inspect
+import os
 import tkinter as tk
 from enum import Enum
 from tkinter import ttk
 from tkinter.font import nametofont
 
 from UEVaultManager.tkgui.modules.functions import log_warning, tag_to_label
 
@@ -38,14 +39,16 @@
     """
 
     def __init__(self, tag=None, row=-1, col=-1, default_content=''):
         self.tag = tag
         self.col = col
         self.row = row
         self.default_content = default_content if default_content else tag_to_label(tag)
+        # can't call this here because the set_content function is specific and overridden in the derived classes
+        # self.reset_content()
 
     @staticmethod
     def _remove_extended_args(kwargs, function_signature) -> None:
         """
         Removes the extended args from the kwargs.
         :param kwargs: args to extract from.
         :param function_signature: function to get the signature from. We can't use a non-static method because the init function will be the derived class's init function.
@@ -132,52 +135,58 @@
 
         return default_font
 
 
 class ExtendedEntry(ExtendedWidget, ttk.Entry):
     """
     Extended widget version of a ttk.Entry class.
-    :param master: master widget
+    :param master: container for the widget
     :param kwargs: kwargs to pass to the widget
     :return: ExtendedEntry instance
     """
 
     def __init__(self, master=None, **kwargs):
+        if master is None:
+            print('A container is needed to display this widget')
+            return
         ext_args = self._extract_extended_args(kwargs, function_signature=ExtendedWidget.__init__)
         ExtendedWidget.__init__(self, **ext_args)
         # already made with _extract_extended_args
         # self._remove_extended_args(kwargs, function_signature=ExtendedWidget.__init__)
         ttk.Entry.__init__(self, master, **kwargs)
-        self.type: WidgetType.ENTRY
+        self.widget_type = WidgetType.ENTRY
 
     def set_content(self, content='') -> None:
         """
         Sets the content of the widget.
         :param content: content to set
         """
         self.delete(0, tk.END)
         self.insert(0, content)
 
 
 class ExtendedText(ExtendedWidget, tk.Text):
     """
     Extended widget version of a ttk.Text. Also add a "ttk.style" like property to the widget.
-    :param master: master widget
+    :param master: container for the widget
     :param kwargs: kwargs to pass to the widget
     :return: ExtendedText instance
     """
 
     def __init__(self, master=None, **kwargs):
+        if master is None:
+            print('A container is needed to display this widget')
+            return
         ext_args = self._extract_extended_args(kwargs, function_signature=ExtendedWidget.__init__)
         ExtendedWidget.__init__(self, **ext_args)
 
         # already made with _extract_extended_args
         # self._remove_extended_args(kwargs, function_signature=ExtendedWidget.__init__)
         tk.Text.__init__(self, master, **kwargs)
-        self.type: WidgetType.TEXT
+        self.widget_type = WidgetType.TEXT
         self.update_style()
 
     def update_style(self) -> None:
         """
         Update the style of the widget based on a ttk.Entry widget.
         """
         style = self.get_style()
@@ -214,64 +223,146 @@
             log_warning(f'Failed to get content of {self}: {error!r}')
             return ''
 
 
 class ExtendedLabel(ExtendedWidget, ttk.Label):
     """
     Extended widget version of a ttk.Label.
-    :param master: master widget
+    :param master: container for the widget
+    :param text: Text to display next to the checkbutton
     :param kwargs: kwargs to pass to the widget
     :return: ExtendedLabel instance
     """
 
     def __init__(self, master=None, **kwargs):
+        if master is None:
+            print('A container is needed to display this widget')
+            return
         ext_args = self._extract_extended_args(kwargs, function_signature=ExtendedWidget.__init__)
         ExtendedWidget.__init__(self, **ext_args)
         # already made with _extract_extended_args
         # self._remove_extended_args(kwargs, function_signature=ExtendedWidget.__init__)
         ttk.Label.__init__(self, master, **kwargs)
-        self.type: WidgetType.LABEL
+        self.widget_type = WidgetType.LABEL
 
 
-class ExtendedCheckButton(ExtendedWidget, ttk.Checkbutton):
+class ExtendedCheckButton(ExtendedWidget):
     """
-    Extended widget version of a ttk.Checkbutton.
-    :param master: master widget
+    Create a new widget version of a ttk.Checkbutton.
+    Note: We don't use the ttk.Checkbutton because it's hard to sync its state when using the on_click event.
+    :param master: Parent widget
+    :param label: Text to display next to the checkbutton
+    :param images_folder: Path to the folder containing the images for the checkbutton. If empty, the './assets' folder will be used
+    :param change_state_on_click: If True, the state of the checkbutton will change when clicking on the text or the checkbutton. if not, the change must be done manually by calling the switch_state method
     :param kwargs: kwargs to pass to the widget
     :return: ExtendedCheckButton instance
     """
 
-    def __init__(self, master=None, **kwargs):
+    def __init__(self, master, label=None, images_folder=None, change_state_on_click=True, **kwargs):
+        if master is None:
+            print('A container is needed to display this widget')
+            return
         ext_args = self._extract_extended_args(kwargs, function_signature=ExtendedWidget.__init__)
         ExtendedWidget.__init__(self, **ext_args)
-        # already made with _extract_extended_args
-        # self._remove_extended_args(kwargs, function_signature=ExtendedWidget.__init__)
-        ttk.Checkbutton.__init__(self, master, **kwargs)
-        self.type: WidgetType.CHECKBUTTON
+        if images_folder is None:
+            images_folder = './assets/'
+        self._img_checked = tk.PhotoImage(file=os.path.join(images_folder, 'checked_16.png'))  # Path to the checked image
+        self._img_uncheckked = tk.PhotoImage(file=os.path.join(images_folder, 'unchecked_16.png'))  # Path to the unchecked image
+        self.widget_type = WidgetType.CHECKBUTTON
         self.default_content = False
+        self._var = tk.BooleanVar(value=self.default_content)
+        frm_inner = ttk.Frame(master)
+        lbl_text = ttk.Label(frm_inner, text='')  # no text bydefault
+        check_label = ttk.Label(frm_inner, image=self._img_uncheckked, cursor='hand2')
+        lbl_text.pack(side=tk.LEFT)
+        check_label.pack(side=tk.LEFT)
+        self._frm_inner = frm_inner
+        self._lbl_text = lbl_text
+        self._check_label = check_label
+
+        if label is not None:
+            self.set_label(label)
+        # noinspection PyTypeChecker
+        # keep "bad" type to keep compatible signatures with overriden methods
+        self.set_content(self.default_content)
+
+        if change_state_on_click:
+            self.bind("<Button-1>", self.switch_state)
 
-    def set_content(self, content=''):
+    def _update_state(self) -> None:
         """
-        Sets the content of the widget.
+        Updates the image of the checkbutton
+        """
+        current_state = self._var.get()
+        if current_state:
+            self._check_label.config(image=self._img_checked)
+        else:
+            self._check_label.config(image=self._img_uncheckked)
+
+    def pack(self, **kwargs) -> None:
+        """
+        Packs the widget
+        :param kwargs: kwargs to pass to the widget
+        """
+        self._frm_inner.pack(**kwargs)
+
+    def grid(self, **kwargs) -> None:
+        """
+        Grids the widget
+        :param kwargs: kwargs to pass to the widget
+        """
+        self._frm_inner.grid(**kwargs)
+
+    def bind(self, sequence=None, command=None) -> None:
+        """
+        Binds a callback to the widget
+        :param sequence: Sequence to bind to
+        :param command:  function to bind
+        """
+        self._lbl_text.bind(sequence, command)
+        self._check_label.bind(sequence, command)
+
+    # noinspection PyUnusedLocal
+    def switch_state(self, event=None) -> bool:
+        """
+        Switches the state of the checkbutton
+        :param event: event that triggered the call
+        """
+        value = bool(self._var.get())
+        # print(f'Current state: {value} event: {event}   ')
+        value = not value
+        self._var.set(value)
+        self._update_state()
+        return value
+
+    def set_label(self, text='') -> None:
+        """
+        Sets the label of the widget
+        :param text: text to set
+        """
+        self._check_label.config(text=text)
+
+    def set_content(self, content='') -> None:
+        """
+        Sets the content of the widget. True, 'True' and '1' will be considered as True, everything else will be considered as False
         :param content: content to set
         """
         try:
-            content = str(content).capitalize()
-            if content or (content == 'True') or (content == '1'):
-                # noinspection PyUnresolvedReferences
-                self.select()
+            if type(content) is bool:
+                # noinspection PyTypeChecker
+                # keep "bad" type to keep compatible signatures with overriden methods
+                self._var.set(content)
+            elif (content.lower() == 'true') or (content == '1'):
+                self._var.set(True)
             else:
-                # noinspection PyUnresolvedReferences
-                self.deselect()
+                self._var.set(False)
+
+            self._update_state()
         except (AttributeError, tk.TclError) as error:
             log_warning(f'Failed to set content of {self} to {content}: {error!r}')
 
-    def get_content(self):
+    def get_content(self) -> bool:
         """
         Gets the content of the widget.
-        :return: content of the widget
+        :return: True if the checkbutton is checked, False otherwise
         """
-        try:
-            return self.instate(['selected'])
-        except (AttributeError, tk.TclError) as error:
-            log_warning(f'Failed to get content of {self}: {error!r}')
-            return None
+        return self._var.get()
```

### Comparing `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/ProgressWindowsClass.py` & `UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/ProgressWindowsClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/SaferDictClass.py` & `UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/SaferDictClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,14 @@
         :param default: the default value to return if the key doesn't exist
         """
         return super().get(key, default)
 
     def copy_from(self, source: dict):
         """
         Copies the content of the given source dictionary into the SaferDict.
-        If the source is not a dictionary, raises a TypeError.
         :param source: the source dictionary to copy from
+        :raises TypeError: if the source is not a dictionary
         """
         if not isinstance(source, dict):
             raise TypeError("source must be a dictionary")
         self.clear()
         self.update({k: v for k, v in source.items()})
```

### Comparing `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py` & `UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 """
 Implementation for:
 - TaggedLabelFrame: a custom LabelFrame widget that allows child widgets to be identified by tags
 """
 import tkinter as tk
 from tkinter import ttk
 
+import UEVaultManager.tkgui.modules.globals as gui_g  # using the shortest variable name for globals for convenience
 from UEVaultManager.tkgui.modules.ExtendedWidgetClasses import WidgetType, ExtendedEntry, ExtendedText, ExtendedLabel, ExtendedCheckButton
-from UEVaultManager.tkgui.modules.functions import log_error, tag_to_label
+from UEVaultManager.tkgui.modules.functions import log_error, tag_to_label, log_warning, path_from_relative_to_absolute, log_debug
 
 
 class TaggedLabelFrame(ttk.LabelFrame):
     """
     A custom LabelFrame widget that allows child widgets to be identified by tags.
     :param args: Args to pass to the widget
     :param kwargs: Kwargs to pass to the widget
@@ -26,56 +27,62 @@
         self.lblf_fw_options = {'ipadx': 2, 'ipady': 2, 'fill': tk.X, 'expand': True}
 
     def add_child(
         self,
         tag: str,
         widget_type: WidgetType.ENTRY,
         default_content=None,
-        height=None,
         width=None,
+        height=None,
+        label=None,
         layout_option='',
-        focus_out_callback=None
+        focus_out_callback=None,
+        click_on_callback=None
     ) -> None:
         """
         Adds a child widget to the LabelFrame and associates it with the given tag.
+        Note: we can not use command parameter to manage callback here because it should be transmited
+        to the parent widget and in that case tag won't be available as an indentificator
         :param tag: Tag to search for (case-insensitive)
         :param widget_type: Type of widget to add. A string value of 'text', 'checkbutton', or 'entry'
         :param width: Width of the child widget. Only used for text widgets
         :param height: Height of the child widget. Only used for text widgets
+        :param label: Text to display in the child widget.
         :param default_content: Default content of the child widget
         :param layout_option: Layout options to use. Default, full width.
         :param focus_out_callback: Callback to call when the child widget loses focus
+        :param click_on_callback: Callback to call when the child widget is clicked or checked
         """
         tag = tag.lower()
         frame = ttk.Frame(self)
         frame.pack(**self.lblf_fw_options)
         label = ttk.Label(frame, text=tag_to_label(tag))
         label.pack(side=tk.LEFT, **self.pack_options)
-
-        widget_class = {
-            WidgetType.ENTRY: (lambda **kwargs: ExtendedEntry)(master=frame, tag=tag, default_content=default_content, height=height, width=width),
-            WidgetType.TEXT:
-            (lambda **kwargs: ExtendedText)(master=frame, wrap=tk.WORD, tag=tag, default_content=default_content, height=height, width=width),
-            WidgetType.LABEL: (lambda **kwargs: ExtendedLabel)(master=frame, tag=tag, default_content=default_content, height=height, width=width),
-            WidgetType.CHECKBUTTON:
-            (lambda **kwargs: ExtendedCheckButton)(master=frame, tag=tag, default_content=default_content, height=height, width=width)
-        }.get(widget_type)
-        if widget_class is None:
+        asset_folder = path_from_relative_to_absolute(gui_g.s.assets_folder)
+        if widget_type == WidgetType.ENTRY:
+            child = ExtendedEntry(master=frame, tag=tag, default_content=default_content, height=height, width=width)
+        elif widget_type == WidgetType.TEXT:
+            child = ExtendedText(master=frame, tag=tag, default_content=default_content, wrap=tk.WORD, height=height, width=width)
+        elif widget_type == WidgetType.LABEL:
+            child = ExtendedLabel(master=frame, tag=tag, default_content=default_content)
+        elif widget_type == WidgetType.CHECKBUTTON:
+            child = ExtendedCheckButton(master=frame, tag=tag, default_content=default_content, label=label, images_folder=asset_folder)
+        else:
             log_error(f'Invalid widget type: {widget_type}')
             return
 
-        child = widget_class(frame, tag=tag, default_content=default_content, height=height, width=width)
         self._tagged_child[tag] = child
-        child.reset_content()
 
         layout_option = self.pack_fw_options if layout_option == '' else layout_option
         child.pack(side=tk.LEFT, **layout_option)
 
         if focus_out_callback is not None:
             child.bind('<FocusOut>', lambda event: focus_out_callback(event=event, tag=tag))
+        if click_on_callback is not None:
+            child.bind('<Button-1>', lambda event: click_on_callback(event=event, tag=tag))
 
     def get_child_by_tag(self, tag: str):
         """
         Returns the child widget associated with the given tag.
         :param tag: Tag to search for (case-insensitive)
         :return: Child widget
         """
@@ -85,32 +92,40 @@
     def get_children(self) -> dict:
         """
         Returns the dictionary of tagged children.
         :return: A dictionary of tagged children
         """
         return self._tagged_child
 
-    def set_default_content(self, tag: str = '') -> None:
+    def set_default_content(self, tag='') -> None:
         """
         Sets the default content of the child widget associated with the given tag.
         :param tag: Tag to search for (case-insensitive)
         """
         tag = tag.lower()
         widget = self.get_child_by_tag(tag)
         if widget is not None:
             widget.set_content(widget.default_content)
 
-    def set_child_values(self, tag: str = '', content: str = '', row: int = -1, col: int = -1) -> None:
+    def set_child_values(self, tag='', content='', label=None, row=-1, col=-1) -> None:
         """
         Sets the content of the child widget associated with the given tag.
         Also sets its row and column index.
         :param tag: Tag to search for (case-insensitive)
+        :param label: Text to set (only for CheckButton widget)
         :param content: Content to set
         :param row: Row index to set
         :param col: Column index to set
         """
         tag = tag.lower()
         widget = self.get_child_by_tag(tag)
         if widget is not None:
             widget.set_content(content)
             widget.row = row
             widget.col = col
+            if label is not None:
+                try:
+                    widget.set_label(label)
+                except AttributeError:
+                    log_debug(f'Widget with tag {tag} does not have a set_label method')
+        else:
+            log_warning(f'Widget with tag {tag} not found')
```

### Comparing `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/UEVMGuiClass.py` & `UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/UEVMGuiClass.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     :param height: The height
     :param icon: The icon
     :param screen_index: The screen index
     :param file: The file where the data is stored or read from
     :param show_open_file_dialog: If True, the open file dialog will be shown at startup
     """
 
-    def __init__(self, title: str, width=1200, height=800, icon='', screen_index=0, file='', show_open_file_dialog=False):
+    def __init__(self, title: str, width=1200, height=800, icon='', screen_index=0, file='', show_open_file_dialog=False, rebuild_data=False):
         super().__init__()
         self.title(title)
         style = set_custom_style(gui_g.s.theme_name, gui_g.s.theme_font)
         self.style = style
         geometry = gui_f.center_window_on_screen(screen_index, height, width)
         self.geometry(geometry)
         if icon is None:
@@ -45,40 +45,62 @@
                 self.iconbitmap(icon)
         self.resizable(True, False)
         self.editable_table = None
         self.do_not_launch_search = False
         pack_def_options = {'ipadx': 5, 'ipady': 5, 'padx': 3, 'pady': 3}
 
         table_frame = self.TableFrame(self)
-        self.editable_table = EditableTable(container_frame=table_frame, file=file, fontsize=gui_g.s.table_font_size, show_statusbar=True)
+
+        # gui_g.UEVM_gui_ref = self  # important ! Must be donne before any use of a ProgressWindow. If not, an UEVMGuiHiddenRootClass will be created and the ProgressWindow still be displayed after the init
+        self.editable_table = EditableTable(container_frame=table_frame, file=file, rows_per_page=36, show_statusbar=True)
+        self.editable_table.set_preferences(gui_g.s.datatable_default_pref)
+
+        # done in the rebuild_data() method
         self.editable_table.show()
         self.editable_table.show_page(0)
 
         self.table_frame = table_frame
         toolbar_frame = self.ToolbarFrame(self)
         self.toolbar_frame = toolbar_frame
         control_frame = self.ControlFrame(self)
         self.control_frame = control_frame
+        options_frame = self.OptionsFrame(self)
+        self.options_frame = options_frame
+        self.editable_table.set_colors()
 
         toolbar_frame.pack(**pack_def_options, fill=tk.X, side=tk.TOP, anchor=tk.NW)
         table_frame.pack(**pack_def_options, fill=tk.BOTH, side=tk.LEFT, anchor=tk.NW, expand=True)
         control_frame.pack(**pack_def_options, fill=tk.BOTH, side=tk.RIGHT, anchor=tk.NW)
+        # not displayed at start
+        # options_frame.pack(**pack_def_options, fill=tk.BOTH, side=tk.RIGHT, anchor=tk.NW)
 
         self.bind('<Key>', self.on_key_press)
         # Bind the table to the mouse motion event
         self.editable_table.bind('<Motion>', self.on_mouse_over_cell)
         self.editable_table.bind('<Leave>', self.on_mouse_leave_cell)
         self.editable_table.bind('<<CellSelectionChanged>>', self.on_selection_change)
         self.protocol('WM_DELETE_WINDOW', self.on_close)
 
         if show_open_file_dialog:
             if self.load_file() == '':
                 gui_f.log_error(f'This application could not run without a file to read data from')
                 self.quit()
 
+        # Quick edit the first row
+        self.editable_table.update_quick_edit(quick_edit_frame=self.control_frame.lbtf_quick_edit, row=0)
+
+        if rebuild_data or self.editable_table.must_rebuild:
+            if gui_f.box_okcancel('Data are invalid or empty. They will be rebuilt from sources files. Do you want to continue ?'):
+                if not self.editable_table.rebuild_data():
+                    gui_f.log_error(f'Rebuild data error. This application could not run without a file to read from or some data to build from it')
+                    self.destroy()  # self.quit() won't work here
+                    return
+            else:
+                self.destroy()  # self.quit() won't work here
+
     class ToolbarFrame(ttk.Frame):
         """
         This class is used to create the toolbar frame
         :param container: The parent container
         """
 
         def __init__(self, container):
@@ -124,21 +146,29 @@
             btn_zoom_in = ttk.Button(lblf_display, text='Zoom In', command=container.editable_table.zoom_in)
             btn_zoom_in.pack(**pack_def_options, side=tk.LEFT)
             btn_zoom_out = ttk.Button(lblf_display, text='Zoom Out', command=container.editable_table.zoom_out)
             btn_zoom_out.pack(**pack_def_options, side=tk.LEFT)
 
             lblf_commands = ttk.LabelFrame(self, text='Cli commands')
             lblf_commands.pack(side=tk.LEFT, **lblf_def_options)
-            # noinspection PyArgumentList
-            btn_status = ttk.Button(lblf_commands, text='Run Status', command=container.run_cli_status)
+            btn_help = ttk.Button(lblf_commands, text='Help', command=lambda: container.run_cli_command('print_help'))
+            btn_help.pack(**pack_def_options, side=tk.LEFT)
+            btn_status = ttk.Button(lblf_commands, text='Status', command=lambda: container.run_cli_command('status'))
             btn_status.pack(**pack_def_options, side=tk.LEFT)
+            btn_info = ttk.Button(lblf_commands, text='Info', command=lambda: container.run_cli_command('info'))
+            btn_info.pack(**pack_def_options, side=tk.LEFT)
+            btn_info = ttk.Button(lblf_commands, text='List Files', command=lambda: container.run_cli_command('list_files'))
+            btn_info.pack(**pack_def_options, side=tk.LEFT)
 
             lblf_actions = ttk.LabelFrame(self, text='Actions')
             lblf_actions.pack(side=tk.RIGHT, **lblf_def_options)
             # noinspection PyArgumentList
+            btn_toggle_options = ttk.Button(lblf_actions, text='Show Options', command=container.toggle_options_pane, state=tk.DISABLED)
+            btn_toggle_options.pack(**pack_def_options, side=tk.LEFT)
+            # noinspection PyArgumentList
             btn_toggle_controls = ttk.Button(lblf_actions, text='Hide Controls', command=container.toggle_controls_pane)
             btn_toggle_controls.pack(**pack_def_options, side=tk.LEFT)
             # noinspection PyArgumentList
             btn_on_close = ttk.Button(lblf_actions, text='Quit', command=container.on_close, bootstyle=WARNING)
             btn_on_close.pack(**pack_def_options, side=tk.RIGHT)
 
             # Bind events for the Entry widget
@@ -146,50 +176,36 @@
             entry_page_num.bind('<Return>', container.on_entry_page_num_changed)
 
             self.btn_toggle_pagination = btn_toggle_pagination
             self.btn_first_page = btn_first_page
             self.btn_prev_page = btn_prev_page
             self.btn_next_page = btn_next_page
             self.btn_last_page = btn_last_page
+            self.btn_toggle_options = btn_toggle_options
             self.btn_toggle_controls = btn_toggle_controls
             self.lbl_page_count = lbl_page_count
             self.entry_page_num = entry_page_num
             self.entry_page_num_var = entry_page_num_var
 
     class TableFrame(ttk.Frame):
         """
         The TableFrame is a container for the Table widget.
         :param container: The parent container.
         """
 
         def __init__(self, container):
             super().__init__(container)
+            self.container = container
 
     class ControlFrame(ttk.Frame):
         """
         The ControlFrame is a container for the filter controls.
         :param container: The parent container.
         """
 
-        # delete the temporary text in filter value entry
-        def reset_entry_search(self, _event=None) -> None:
-            """
-            Reset the search entry to the default text.
-            :param _event: 
-            """
-            self.entry_search.delete(0, 'end')
-            self.entry_search.insert(0, gui_g.s.default_global_search)
-
-        def del_entry_search(self, _event=None) -> None:
-            """
-            Delete the text in the search entry.
-            :param _event:
-            """
-            self.entry_search.delete(0, 'end')
-
         def __init__(self, container):
             super().__init__()
 
             # grid_def_options = {'ipadx': 2, 'ipady': 2, 'padx': 2, 'pady': 2, 'sticky': tk.NW}
             pack_def_options = {'ipadx': 2, 'ipady': 2, 'fill': tk.BOTH, 'expand': False}
             grid_fw_options = {'ipadx': 2, 'ipady': 2, 'padx': 2, 'pady': 2, 'sticky': tk.EW}  # full width
             lblf_def_options = {'ipadx': 2, 'ipady': 2, 'padx': 2, 'pady': 2, 'fill': tk.X, 'expand': False}
@@ -240,15 +256,15 @@
             cur_col += 1
             var_category = tk.StringVar(value=categories[0])
             opt_category = ttk.Combobox(lbf_filter_cat, textvariable=var_category, values=categories)
             opt_category.grid(row=cur_row, column=cur_col, columnspan=3, **grid_fw_options)
             # row 2
             cur_row += 1
             cur_col = 0
-            lbl_grab_results = ttk.Label(lbf_filter_cat, text='Grab Result')
+            lbl_grab_results = ttk.Label(lbf_filter_cat, text='Grab result')
             lbl_grab_results.grid(row=cur_row, column=cur_col, **grid_fw_options)
             cur_col += 1
             var_grab_results = tk.StringVar(value=grab_results[0])
             opt_grab_results = ttk.Combobox(lbf_filter_cat, textvariable=var_grab_results, values=grab_results)
             opt_grab_results.grid(row=cur_row, column=cur_col, columnspan=3, **grid_fw_options)
             # row 3
             cur_row += 1
@@ -288,16 +304,20 @@
             lbl_desc = ttk.Label(lbtf_quick_edit, text='Changing this values will change the values of \nthe selected row when losing focus')
             lbl_desc.pack(**pack_def_options)
             lbtf_quick_edit.add_child(widget_type=WidgetType.ENTRY, tag='Url', focus_out_callback=container.on_quick_edit_focus_out)
             lbtf_quick_edit.add_child(
                 widget_type=WidgetType.TEXT, tag='Comment', focus_out_callback=container.on_quick_edit_focus_out, width=10, height=4
             )
             lbtf_quick_edit.add_child(widget_type=WidgetType.ENTRY, tag='Stars', focus_out_callback=container.on_quick_edit_focus_out)
-            lbtf_quick_edit.add_child(widget_type=WidgetType.ENTRY, tag='Test_result', focus_out_callback=container.on_quick_edit_focus_out)
-            lbtf_quick_edit.add_child(widget_type=WidgetType.ENTRY, tag='Folder', default_content='Installed in')
+            lbtf_quick_edit.add_child(widget_type=WidgetType.ENTRY, tag='Test result', focus_out_callback=container.on_quick_edit_focus_out)
+            lbtf_quick_edit.add_child(
+                widget_type=WidgetType.CHECKBUTTON, tag='Must buy', label='', click_on_callback=container.on_switch_edit_flag, default_content=False
+            )
+            lbtf_quick_edit.add_child(widget_type=WidgetType.ENTRY, tag='Installed folder', default_content='Installed in')
+            lbtf_quick_edit.add_child(widget_type=WidgetType.ENTRY, tag='Origin', focus_out_callback=container.on_quick_edit_focus_out)
             lbtf_quick_edit.add_child(widget_type=WidgetType.ENTRY, tag='Alternative', focus_out_callback=container.on_quick_edit_focus_out)
 
             lbt_image_preview = ttk.LabelFrame(self, text='Image Preview')
             lbt_image_preview.pack(**lblf_fw_options, anchor=tk.SW)
             canvas_image = tk.Canvas(lbt_image_preview, width=gui_g.s.preview_max_width, height=gui_g.s.preview_max_height, highlightthickness=0)
             canvas_image.pack(side=tk.BOTTOM, expand=True, anchor=tk.CENTER)
             canvas_image.create_rectangle((0, 0), (gui_g.s.preview_max_width, gui_g.s.preview_max_height), fill='black')
@@ -316,58 +336,125 @@
             self.var_on_sale = var_on_sale
             self.var_grab_results = var_grab_results
 
             self.entry_search = entry_search
             self.lbtf_quick_edit = lbtf_quick_edit
             self.canvas_image = canvas_image
 
-    def _open_file_dialog(self, save_mode=False) -> str:
+        def reset_entry_search(self, _event=None) -> None:
+            """
+            Reset the search entry to the default text.
+            :param _event:
+            """
+            self.entry_search.delete(0, 'end')
+            self.entry_search.insert(0, gui_g.s.default_global_search)
+
+        def del_entry_search(self, _event=None) -> None:
+            """
+            Delete the text in the search entry.
+            :param _event:
+            """
+            self.entry_search.delete(0, 'end')
+
+    class OptionsFrame(ttk.Frame):
+        """
+        This class is used to create the toolbar frame
+        :param _container: The parent container
+        """
+
+        def __init__(self, _container):
+            super().__init__()
+            # pack_def_options = {'ipadx': 2, 'ipady': 2, 'padx': 2, 'pady': 2, 'fill': tk.BOTH, 'expand': False}
+            lblf_def_options = {'ipadx': 1, 'ipady': 1, 'expand': False}
+            grid_fw_options = {'ipadx': 2, 'ipady': 2, 'padx': 2, 'pady': 2, 'sticky': tk.EW}  # full width
+
+            lblf_options = ttk.LabelFrame(self, text='Command Options')
+            lblf_options.pack(side=tk.TOP, **lblf_def_options)
+            # row 0
+            cur_col = 0
+            cur_row = 0
+            force_refresh_var = tk.BooleanVar(value=gui_g.UEVM_cli_args.get('force', False))
+            force_refresh_var.trace_add('write', lambda name, index, mode: gui_g.set_args_force_refresh(force_refresh_var.get()))
+            ck_force_refresh = ttk.Checkbutton(lblf_options, text='Force refresh', variable=force_refresh_var)
+            ck_force_refresh.grid(row=cur_row, column=cur_col, **grid_fw_options)
+            # row 1
+            cur_row += 1
+            cur_col = 0
+            offline_var = tk.BooleanVar(value=gui_g.UEVM_cli_args.get('offli', False))
+            offline_var.trace_add('write', lambda name, index, mode: gui_g.set_args_offline(offline_var.get()))
+            ck_offline = ttk.Checkbutton(lblf_options, text='Offline Mode', variable=offline_var)
+            ck_offline.grid(row=cur_row, column=cur_col, **grid_fw_options)
+            # row 2
+            cur_row += 1
+            cur_col = 0
+            debug_var = tk.BooleanVar(value=gui_g.UEVM_cli_args.get('debug', False))
+            debug_var.trace_add('write', lambda name, index, mode: gui_g.set_args_debug(debug_var.get()))
+            ck_debug = ttk.Checkbutton(lblf_options, text='Debug mode', variable=debug_var)
+            ck_debug.grid(row=cur_row, column=cur_col, **grid_fw_options)
+
+    def _open_file_dialog(self, save_mode=False, filename=None) -> str:
         """
         Open a file dialog to choose a file to save or load data to/from
         :param save_mode: if True, the dialog will be in saving mode, else in loading mode
+        :param filename: the default filename to use
         :return: the chosen filename
         """
         # adding category to the default filename
-        initial_dir = os.path.dirname(gui_g.s.csv_filename)
-        default_filename = os.path.basename(gui_g.s.csv_filename)  # remove dir
+        if not filename:
+            filename = gui_g.s.default_filename
+        initial_dir = os.path.dirname(filename)
+        default_filename = os.path.basename(filename)  # remove dir
         default_ext = os.path.splitext(default_filename)[1]  # get extension
         default_filename = os.path.splitext(default_filename)[0]  # get filename without extension
         try:
             # if the file is empty or absent or invalid when creating the class, the control_frame is not defined
             category = self.control_frame.var_category.get().replace('/', '_')
         except AttributeError:
             category = None
         if category and category != gui_g.s.default_category_for_all:
             default_filename = default_filename + '_' + category + default_ext
+        else:
+            default_filename = default_filename + default_ext
         if save_mode:
             filename = fd.asksaveasfilename(
                 title='Choose a file to save data to', initialdir=initial_dir, filetypes=gui_g.s.data_filetypes, initialfile=default_filename
             )
         else:
             filename = fd.askopenfilename(
                 title='Choose a file to read data from', initialdir=initial_dir, filetypes=gui_g.s.data_filetypes, initialfile=default_filename
             )
         return filename
 
+    def _change_navigation_state(self, state: str) -> None:
+        """
+        Change the state of the navigation buttons
+        :param state: 'normal' or 'disabled'
+        """
+        self.toolbar_frame.btn_first_page.config(state=state)
+        self.toolbar_frame.btn_prev_page.config(state=state)
+        self.toolbar_frame.btn_next_page.config(state=state)
+        self.toolbar_frame.btn_last_page.config(state=state)
+        self.toolbar_frame.entry_page_num.config(state=state)
+
     def on_key_press(self, event) -> None:
         """
         Handle key press events
         :param event:
         """
         if event.keysym == 'Escape':
             if gui_g.edit_cell_window_ref:
-                gui_g.edit_cell_window_ref.destroy()
+                gui_g.edit_cell_window_ref.quit()
                 gui_g.edit_cell_window_ref = None
             elif gui_g.edit_row_window_ref:
-                gui_g.edit_row_window_ref.destroy()
+                gui_g.edit_row_window_ref.quit()
                 gui_g.edit_row_window_ref = None
             else:
                 self.on_close()
-        elif event.keysym == 'Return':
-            self.editable_table.create_edit_record_window()
+        # elif event.keysym == 'Return':
+        #    self.editable_table.create_edit_record_window()
 
     def on_mouse_over_cell(self, event=None) -> None:
         """
         Show the image of the asset when the mouse is over the cell
         :param event:
         """
         if event is None:
@@ -389,15 +476,15 @@
 
     def on_selection_change(self, event=None) -> None:
         """
         When the selection changes, show the selected row in the quick edit frame
         :param event:
         """
         selected_row = event.widget.currentrow
-        self.editable_table.quit_edit_content(quick_edit_frame=self.control_frame.lbtf_quick_edit, row=selected_row)
+        self.editable_table.update_quick_edit(quick_edit_frame=self.control_frame.lbtf_quick_edit, row=selected_row)
 
     def on_entry_page_num_changed(self, _event=None) -> None:
         """
         When the page number changes, show the corresponding page
         :param _event:
         """
         page_num = 0
@@ -428,37 +515,59 @@
         if col is None or row is None or col < 0 or row < 0:
             gui_f.log_debug(f'invalid values for row={row} and col={col}')
             return
         value = widget.get_content()
         self.editable_table.quick_edit_save_value(col=col, row=row, value=value)
 
     # noinspection PyUnusedLocal
+    def on_switch_edit_flag(self, event=None, tag='') -> None:
+        """
+        When the focus leaves a quick edit widget, save the value
+        :param event: event that triggered the call
+        :param tag: tag of the widget that triggered the event
+        """
+        if tag == '':
+            return
+        widget = self.control_frame.lbtf_quick_edit.get_child_by_tag(tag)
+        if widget is None or widget.widget_type != WidgetType.CHECKBUTTON:
+            gui_f.log_warning(f'Could not find a CHECKBUTTON widget with tag {tag}')
+            return
+        col = widget.col
+        row = widget.row
+        if col is None or row is None or col < 0 or row < 0:
+            gui_f.log_debug(f'invalid values for row={row} and col={col}')
+            return
+
+        value = widget.switch_state(event=event)
+        self.editable_table.quick_edit_save_value(col=col, row=row, value=value)
+
+    # noinspection PyUnusedLocal
     def on_check_change(self, *args) -> None:
         """
         When a checkbutton is changed, launch a search
         :param args:
         """
         if not self.do_not_launch_search:
             self.apply_filters()
 
     def on_close(self) -> None:
         """
         When the window is closed, check if there are unsaved changes and ask the user if he wants to save them
         """
-        if self.editable_table.must_save:
+        if self.editable_table is not None and self.editable_table.must_save:
             if gui_f.box_yesno('Changes have been made. Do you want to save them in the source file ?'):
                 self.save_file(show_dialog=False)
         self.quit()
 
     def load_file(self) -> str:
         """
         Load a file
         :return: the name of the file that was loaded
         """
-        filename = self._open_file_dialog()
+        filename = self._open_file_dialog(filename=self.editable_table.file)
         if filename and os.path.isfile(filename):
             self.editable_table.file = filename
             self.editable_table.load_data()
             self.editable_table.show_page(0)
             self.update_page_numbers()
             self.update_file_name()
             gui_f.box_message(f'The file {filename} as been read')
@@ -466,15 +575,15 @@
 
     def save_file(self, show_dialog=True) -> str:
         """
         Save the data to a file
         :param show_dialog: if True, show a dialog to select the file to save to, if False, use the current file
         """
         if show_dialog:
-            filename = self._open_file_dialog(save_mode=True)
+            filename = self._open_file_dialog(filename=self.editable_table.file, save_mode=True)
             if filename:
                 self.editable_table.file = filename
         else:
             filename = self.editable_table.file
 
         if filename:
             self.editable_table.save_data()
@@ -486,15 +595,15 @@
         """
         Export the selected rows to a file
         """
         # Get selected row indices
         selected_row_indices = self.editable_table.multiplerowlist
         if selected_row_indices:
             selected_rows = self.editable_table.data_filtered.iloc[selected_row_indices]
-            filename = self._open_file_dialog(save_mode=True)
+            filename = self._open_file_dialog(save_mode=True, filename=self.editable_table.file)
             if filename:
                 selected_rows.to_csv(filename, index=False)
                 gui_f.box_message(f'Selected rows exported to "{filename}"')
         else:
             gui_f.box_message('Select at least one row first')
 
     def apply_filters(self, _event=None) -> None:
@@ -527,17 +636,17 @@
         if not_obsolete:
             filter_dict['Obsolete'] = False
             filter_dict['Status'] = 'active'
         else:
             filter_dict.pop('Obsolete', None)
             filter_dict.pop('Status', None)
         if must_buy:
-            filter_dict['Must Buy'] = True
+            filter_dict['Must buy'] = True
         else:
-            filter_dict.pop('Must Buy', None)
+            filter_dict.pop('Must buy', None)
         if on_sale:
             filter_dict['On sale'] = True
         else:
             filter_dict.pop('On sale', None)
         self.editable_table.apply_filters(filter_dict, global_search=search_text)
         # self.control_frame.reset_entry_search()
 
@@ -562,19 +671,15 @@
         if forced_value is not None:
             self.editable_table.pagination_enabled = forced_value
         else:
             self.editable_table.pagination_enabled = not self.editable_table.pagination_enabled
         self.editable_table.show_page()
         if not self.editable_table.pagination_enabled:
             # Disable prev/next buttons when pagination is disabled
-            self.toolbar_frame.btn_first_page.config(state=tk.DISABLED)
-            self.toolbar_frame.btn_prev_page.config(state=tk.DISABLED)
-            self.toolbar_frame.btn_next_page.config(state=tk.DISABLED)
-            self.toolbar_frame.btn_last_page.config(state=tk.DISABLED)
-            self.toolbar_frame.entry_page_num.config(state=tk.DISABLED)
+            self._change_navigation_state(tk.DISABLED)
             self.toolbar_frame.btn_toggle_pagination.config(text='Enable  Pagination')
         else:
             self.update_page_numbers()  # will also update buttons status
             self.toolbar_frame.btn_toggle_pagination.config(text='Disable Pagination')
 
     def show_first_page(self) -> None:
         """
@@ -614,36 +719,50 @@
         """
         Move to the next asset in the table
         """
         self.editable_table.move_to_next_record()
 
     def toggle_controls_pane(self) -> None:
         """
-        Toggle the visibility of the controls on the right side of the table
+        Toggle the visibility of the controls pane on the right side of the table
         """
         # Toggle visibility of filter controls frame
         if self.control_frame.winfo_ismapped():
             self.control_frame.pack_forget()
             self.toolbar_frame.btn_toggle_controls.config(text='Show Control')
+            self.toolbar_frame.btn_toggle_options.config(state=tk.NORMAL)
+
         else:
             self.control_frame.pack(side=tk.RIGHT, fill=tk.BOTH)
             self.toolbar_frame.btn_toggle_controls.config(text='Hide Control')
+            self.toolbar_frame.btn_toggle_options.config(state=tk.DISABLED)
+
+    def toggle_options_pane(self) -> None:
+        """
+        Toggle the visibility of the Options pane on the right side of the table
+        """
+        # Toggle visibility of filter controls frame
+        if self.options_frame.winfo_ismapped():
+            self.options_frame.pack_forget()
+            self.toolbar_frame.btn_toggle_options.config(text='Show Options')
+            self.toolbar_frame.btn_toggle_controls.config(state=tk.NORMAL)
+        else:
+            self.options_frame.pack(side=tk.RIGHT, fill=tk.BOTH)
+            self.toolbar_frame.btn_toggle_options.config(text='Hide Options')
+            self.toolbar_frame.btn_toggle_controls.config(state=tk.DISABLED)
 
     def update_page_numbers(self) -> None:
         """
         Update the page numbers in the toolbar
         """
         page_num = self.editable_table.current_page + 1
         self.toolbar_frame.entry_page_num_var.set(page_num)
         self.toolbar_frame.lbl_page_count.config(text=f' / {self.editable_table.total_pages}')
         # enable all buttons by default
-        self.toolbar_frame.btn_first_page.config(state=tk.NORMAL)
-        self.toolbar_frame.btn_prev_page.config(state=tk.NORMAL)
-        self.toolbar_frame.btn_next_page.config(state=tk.NORMAL)
-        self.toolbar_frame.btn_last_page.config(state=tk.NORMAL)
+        self._change_navigation_state(tk.NORMAL)
 
         if not self.editable_table.pagination_enabled:
             self.toolbar_frame.entry_page_num.config(state=tk.NORMAL)
         if page_num == 1:
             self.toolbar_frame.btn_first_page.config(state=tk.DISABLED)
             self.toolbar_frame.btn_prev_page.config(state=tk.DISABLED)
         elif page_num == self.editable_table.total_pages:
@@ -676,35 +795,53 @@
         grab_results.insert(0, gui_g.s.default_category_for_all)
         return {'categories': categories, 'grab_results': grab_results}
 
     def reload_data(self) -> None:
         """
         Reload the data from the file
         """
-        if self.editable_table.must_save:
-            if gui_f.box_yesno('Changes have been made, they will be lost. Are you sure you want to continue ?'):
-                self.editable_table.reload_data()
-                gui_f.box_message(f'Data Reloaded from {self.editable_table.file}')
-                self.update_page_numbers()
-                self.update_category_var()
+        if not self.editable_table.must_save or (
+            self.editable_table.must_save and gui_f.box_yesno('Changes have been made, they will be lost. Are you sure you want to continue ?')
+        ):
+            self.editable_table.reload_data()
+            gui_f.box_message(f'Data Reloaded from {self.editable_table.file}')
+            self.update_page_numbers()
+            self.update_category_var()
 
     def rebuild_data(self) -> None:
         """
         Rebuild the data from the file. Will ask for confirmation before rebuilding
         """
         if gui_f.box_yesno(
             f'The process will change the content of the windows and the {self.editable_table.file} file.\nAre you sure you want to continue ?'
         ):
             if self.editable_table.rebuild_data():
                 gui_f.box_message(f'Data rebuilt from {self.editable_table.file}')
                 self.update_page_numbers()
                 self.update_category_var()
 
-    @staticmethod
-    def run_cli_status() -> None:
+    def run_cli_command(self, command_name='') -> None:
         """
         Execute the 'status' command and display the result in DisplayContentWindow
+        :param command_name: the name of the command to execute
         """
-        gui_g.UEVM_cli_args['offline'] = True  # we don't need an update of the data
+        if command_name == '':
+            return
+        row = self.editable_table.getSelectedRow()
+        col = self.editable_table.model.df.columns.get_loc('App name')
+        app_name = self.editable_table.model.getValueAt(row, col)
+
+        # gui_g.UEVM_cli_args['offline'] = True  # speed up some commands
+        # set default options for the cli command to execute
+        gui_g.UEVM_cli_args['gui'] = True
+        gui_g.UEVM_cli_args['full_help'] = True
+        gui_g.UEVM_cli_args['csv'] = False  # mandatory for displaying the result in the DisplayContentWindow
+        gui_g.UEVM_cli_args['tcsv'] = False  # mandatory for displaying the result in the DisplayContentWindow
+        gui_g.UEVM_cli_args['json'] = False  # mandatory for displaying the result in the DisplayContentWindow
+
+        if app_name != '':
+            gui_g.UEVM_cli_args['app_name'] = app_name
+
         if gui_g.display_content_window_ref is None or not gui_g.display_content_window_ref.winfo_viewable():
             # we display the window only if it is not already displayed
-            gui_g.UEVM_cli_ref.status(gui_g.UEVM_cli_args)
+            function_to_call = getattr(gui_g.UEVM_cli_ref, command_name)
+            function_to_call(gui_g.UEVM_cli_args)
```

### Comparing `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py` & `UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/WebImageClass.py` & `UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/WebImageClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/functions.py` & `UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import requests
 import ttkbootstrap as ttk
 from PIL import ImageTk, Image
 from screeninfo import get_monitors
 from termcolor import colored
 
 from UEVaultManager.tkgui.modules import globals as gui_g
-from UEVaultManager.tkgui.modules.SaferDictClass import SaferDict
 
 
 def log_format_message(name: str, levelname: str, message: str) -> str:
     """
     Format the log message
     :param name: the name of the logger
     :param levelname: the level of log
@@ -48,21 +47,30 @@
     else:
         log_info(msg)
         messagebox.showinfo(title=gui_g.s.app_title, message=msg)
 
 
 def box_yesno(msg: str) -> bool:
     """
-    Display a message box with the given message and return True if the user clicked on Yes, False otherwise
+    Display a YES/NO message box with the given message
     :param msg: the message to display 
     :return:  True if the user clicked on Yes, False otherwise
     """
     return messagebox.askyesno(title=gui_g.s.app_title, message=msg)
 
 
+def box_okcancel(msg: str) -> bool:
+    """
+    Display an OK/CANCEL message box with the given message
+    :param msg: the message to display
+    :return:  True if the user clicked on Yes, False otherwise
+    """
+    return messagebox.askokcancel(title=gui_g.s.app_title, message=msg)
+
+
 def todo_message() -> None:
     """
     Display a message box with a message saying that the feature is not implemented yet
     """
     msg = 'Not implemented yet'
     msg = log_format_message(gui_g.s.app_title, 'info', colored(msg, 'yellow'))
     print(msg)
@@ -123,14 +131,16 @@
     :param msg: the message to log. Note that the app will exit after logging the message
     """
     if gui_g.UEVM_log_ref is not None:
         gui_g.UEVM_log_ref.error(msg)
     else:
         msg = log_format_message(gui_g.s.app_title, 'Error', colored(msg, 'red', 'bold'))
         print(msg)
+    if gui_g.UEVM_gui_ref is not None:
+        gui_g.UEVM_gui_ref.quit()
     exit(1)
 
 
 def convert_to_bool(value) -> bool:
     """
     Convert a value to a boolean
     :param value: the value to convert. If the value is not a boolean, it will be converted to a string and then to a boolean.
@@ -213,15 +223,15 @@
 
 def show_asset_image(image_url: str, canvas_image=None) -> None:
     """
     Show the image of the given asset in the given canvas
     :param image_url: the url of the image to display
     :param canvas_image: the canvas to display the image in
     """
-    if canvas_image is None or image_url == '' or str(image_url).lower() == 'nan':
+    if canvas_image is None or image_url == '' or str(image_url).lower() == gui_g.s.empty_cell:
         return
     try:
         # noinspection DuplicatedCode
         if not os.path.isdir(gui_g.s.cache_folder):
             os.mkdir(gui_g.s.cache_folder)
         image_filename = os.path.join(gui_g.s.cache_folder, os.path.basename(image_url))
         # Check if the image is already cached
@@ -232,15 +242,15 @@
             response = requests.get(image_url)
             image = Image.open(BytesIO(response.content))
 
             with open(image_filename, "wb") as f:
                 f.write(response.content)
         resize_and_show_image(image, canvas_image)
     except Exception as error:
-        log_error(f"Error showing image: {error}")
+        log_warning(f"Error showing image: {error}")
 
 
 def show_default_image(canvas_image=None) -> None:
     """
     Show the default image in the given canvas
     :param canvas_image: the canvas to display the image in
     """
@@ -280,14 +290,17 @@
     # Horizontal.TProgressbar or Vertical.TProgressbar (depending on the orient option),
     # Horizontal.TScale or Vertical.TScale (depending on the orient option),
     # Horizontal.TScrollbar or Vertical.TScrollbar (depending on the orient option)
     style.configure('TLabel', font=font, spacing=1, padding=2)
     style.configure('TButton', font=font, spacing=1, padding=2)
     style.configure('TEntry', font=font, spacing=1, padding=2)
     style.configure('TFrame', font=font, spacing=1, padding=1)
+    style.configure('TCombobox', font=font, spacing=1, padding=1)
+    style.configure('TLabelFrame', font=font, spacing=1, padding=1)
+
     return style
 
 
 def json_print_key_val(json_obj, indent=4, print_result=True, output_on_gui=False) -> None:
     """
     Pretty prints a JSON object in a simple 'key: value' format.
     :param json_obj:  The JSON object to print.
@@ -321,25 +334,25 @@
     if print_result:
         if output_on_gui and gui_g.display_content_window_ref is not None:
             gui_g.display_content_window_ref.display(result)
         else:
             print(result)
 
 
-def init_gui_args(args, additional_args=None) -> None:
+def custom_print(text='', keep_mode=True) -> None:
+    """
+    Print the given text on the GUI if it's available, otherwise print it on the console²
+    :param text: the text to print
+    :param keep_mode: whether to keep the existing content when adding a new one
+    """
+    if gui_g.display_content_window_ref is not None:
+        gui_g.display_content_window_ref.display(content=text, keep_mode=keep_mode)
+    else:
+        print(text)
+
+
+def create_empty_file(file_path: str) -> None:
+    """
+    Create an empty file
+    :param file_path: the path of the file to create
     """
-    Initialize the GUI arguments using the CLI arguments
-    :param args:
-    :param additional_args: dict of additional arguments to add
-    """
-
-    # args can not be used as it because it's an object that mainly run as a dict (but it's not)
-    # so we need to convert it to a dict first
-    temp_dict = vars(args)
-    temp_dict['csv'] = True  # force csv output
-    temp_dict['gui'] = True
-    if additional_args is not None:
-        temp_dict.update(additional_args)
-    # create a SaferDict object from the dict (it will avoid errors when trying to access non-existing keys)
-    gui_g.UEVM_cli_args = SaferDict({})
-    # copy the dict content to the SaferDict object
-    gui_g.UEVM_cli_args.copy_from(temp_dict)
+    open(file_path, 'a').close()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/globals.py` & `UEVaultManager-1.4.0/UEVaultManager/tkgui/modules/globals.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,14 +23,41 @@
 # noinspection PyTypeChecker
 UEVM_cli_ref = None  # avoid importing classes from the UEVM main app here because it can cause circular dependencies when importing the module
 # noinspection PyTypeChecker
 UEVM_gui_ref = None  # avoid importing classes from the UEVM GUI class here because it can cause circular dependencies when importing the module
 #  reference to the log object of the UEVM main app.
 #  If empty, log will be message printed in the console
 UEVM_log_ref = None
+#  reference to the default command line parser (used for help button in gui).
+UEVM_parser_ref = None
 
 # global variables
 # noinspection PyTypeChecker
 UEVM_cli_args: SaferDict = None
 UEVM_filter_category = ''
 
 s = GUISettings()  # using the shortest variable name for GUISettings for convenience
+
+
+# options that can be changed in the GUI
+def set_args_force_refresh(value: bool) -> None:
+    """
+    Set the value of the argument force_refresh. Mandadory fot the associated ttk.ckbutton to work
+    :param value: True or False
+    """
+    UEVM_cli_args['force_refresh'] = value
+
+
+def set_args_debug(value: bool) -> None:
+    """
+    Set the value of the argument debug. Mandadory fot the associated ttk.ckbutton to work
+    :param value: True or False
+    """
+    UEVM_cli_args['debug'] = value
+
+
+def set_args_offline(value: bool) -> None:
+    """
+    Set the value of the argument offline. Mandadory fot the associated ttk.ckbutton to work
+    :param value:  True or False
+    """
+    UEVM_cli_args['offline'] = value
```

### Comparing `UEVaultManager-1.3.0/UEVaultManager/utils/aliasing.py` & `UEVaultManager-1.4.0/UEVaultManager/utils/aliasing.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/utils/cli.py` & `UEVaultManager-1.4.0/UEVaultManager/utils/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,41 @@
 # coding=utf-8
 """
 CLI interface functions
 """
 import os
 
 
-def get_boolean_choice(prompt, default=True):
+def get_boolean_choice(prompt: str, default=True) -> bool:
     """
     Prompts the user with a yes/no question and returns a boolean value based on their choice.
-
-    Args:
-        prompt (str): The question prompt.
-        default (bool, optional): The default choice. Defaults to True.
-
-    Returns:
-        bool: True if the user chooses yes, False if they choose no.
-
+    :param prompt: The question prompt.
+    :param default: The default choice. Defaults to True.
+    :return: True if the user chooses yes, False if they choose no.
     """
     yn = 'Y/n' if default else 'y/N'
 
     choice = input(f'{prompt} [{yn}]: ')
     if not choice:
         return default
     elif choice[0].lower() == 'y':
         return True
     else:
         return False
 
 
-def get_int_choice(prompt, default=None, min_choice=None, max_choice=None, return_on_invalid=False):
+def get_int_choice(prompt: str, default=None, min_choice=None, max_choice=None, return_on_invalid=False) -> any:
     """
     Prompts the user to enter an integer choice within a specified range.
-
-    Args:
-        prompt (str): The question prompt.
-        default (int, optional): The default choice. Defaults to None.
-        min_choice (int, optional): The minimum allowed choice. Defaults to None.
-        max_choice (int, optional): The maximum allowed choice. Defaults to None.
-        return_on_invalid (bool, optional): Determines whether to return None on an invalid choice. Defaults to False.
-
-    Returns:
-        int or None: The user's integer choice or None if return_on_invalid is True.
-
+    :param prompt: The question prompt.
+    :param default: The default choice. Defaults to None.
+    :param min_choice: The minimum allowed choice. Defaults to None.
+    :param max_choice: The maximum allowed choice. Defaults to None.
+    :param return_on_invalid: Determines whether to return None on an invalid choice. Defaults to False.
+    :return: The user's integer choice or None if return_on_invalid is True.
     """
     if default is not None:
         prompt = f'{prompt} [{default}]: '
     else:
         prompt = f'{prompt}: '
 
     while True:
@@ -71,107 +61,95 @@
                 if return_on_invalid:
                     return None
                 return_on_invalid = True
                 continue
             return choice
 
 
-def str_to_bool(val):
+def str_to_bool(val: str) -> bool:
     """
     Convert a string representation of truth to a boolean value.
-
     True values are 'y', 'yes', 't', 'true', 'on', and '1'; false values
     are 'n', 'no', 'f', 'false', 'off', and '0'. Raises ValueError if
     'val' is anything else.
-
-    Args:
-        val (str): The string representation of truth.
-
-    Returns:
-        bool: True or False based on the string representation of truth.
-
-    Raises:
-        ValueError: If the input value is not a valid truth representation.
-
+    :param val: The string representation of truth.
+    :return: True or False based on the string representation of truth.
+    :raises ValueError: If the input value is not a valid truth representation.
     """
     val = val.lower()
     if val in ('y', 'yes', 't', 'true', 'on', '1'):
         return True
     elif val in ('n', 'no', 'f', 'false', 'off', '0'):
         return False
     else:
         raise ValueError('Invalid truth value %r' % (val,))
 
 
-def check_and_create_path(full_file_name: str) -> bool:
+def str_is_bool(val: str) -> bool:
     """
-    Checks if the given file path exists and creates it if it doesn't.
-
-    Args:
-        full_file_name (str): The full path of the file.
+    Check if a string could be a boolean value.
+    Boolean values are 'y', 'yes', 't', 'true', 'on', '1', 'n', 'no', 'f', 'false', 'off', and '0'.
+    :param val: The string representation of truth.
+    :return: True if the string could be a boolean value, False otherwise.
+    """
+    val = val.lower()
+    if val in ('y', 'yes', 't', 'true', 'on', '1', 'n', 'no', 'f', 'false', 'off', '0'):
+        return True
+    else:
+        return False
 
-    Returns:
-        bool: True if the path exists or is successfully created, False otherwise.
 
+def check_and_create_path(full_file_name: str) -> bool:
+    """
+    Checks if the given file path exists and creates it if it doesn't.
+    :param full_file_name: The full path of the file.
+    :return: True if the path exists or is successfully created, False otherwise.
     """
     # Split the file path and name
     file_path, file_name = os.path.split(full_file_name)
 
     # Check if the folder exists, create it if it doesn't
     if not os.path.isdir(file_path):
         try:
             os.makedirs(file_path, exist_ok=True)
         except OSError:
             return False
 
     return True
 
 
-def convert_string_to_float_list(string, increment=0.01):
+def convert_string_to_float_list(string: str, increment=0.01) -> list:
     """
     Converts a string in the format 'start - end' to a list of float values.
-
-    Args:
-        string (str): The string in the format 'start - end'.
-        increment: The increment between each float value. Defaults to 0.1.
-
-    Returns:
-        list: A list of float values between the start and end values (inclusive).
+    :param string: The string in the format 'start - end'.
+    :param increment: The increment between each float value. Defaults to 0.1.
+    :return: A list of float values between the start and end values (inclusive).
     """
     start, end = map(float, string.split('-'))
     return [round(i, 2) for i in float_range(start, end, increment)]
 
 
-def float_range(start, stop, step):
+def float_range(start: float, stop: float, step: float) -> iter:
     """
     Generator function that yields a sequence of floating-point numbers from start to stop (inclusive) with a given step size.
-
-    Args:
-        start (float): The starting value of the sequence.
-        stop (float): The ending value of the sequence.
-        step (float): The step size between each number in the sequence.
-
-    Yields:
-        float: The next floating-point number in the sequence.
+    :param start: The starting value of the sequence.
+    :param stop: The ending value of the sequence.
+    :param step: The step size between each number in the sequence.
+    :return: (yield) The next floating-point number in the sequence.
     """
     while start <= stop:
         yield start
         start += step
 
 
-def create_list_from_string(string):
+def create_list_from_string(string: str) -> list:
     """
     Creates a list from a string using ',' as a separator. If an item contains a '-', it is converted into a string of float values.
-
-    Args:
-        string (str): The input string.
-
-    Returns:
-        list: The resulting list.
-
+    :param  string: The input string.
+    :return: The resulting list.
     """
     items = string.split(',')
     result_str = ''
 
     for item in items:
         if '-' in item:
             float_values = convert_string_to_float_list(item)
```

### Comparing `UEVaultManager-1.3.0/UEVaultManager/utils/custom_parser.py` & `UEVaultManager-1.4.0/UEVaultManager/utils/custom_parser.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/utils/egl_crypt.py` & `UEVaultManager-1.4.0/UEVaultManager/utils/egl_crypt.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/utils/rolling_hash.py` & `UEVaultManager-1.4.0/UEVaultManager/utils/rolling_hash.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.3.0/UEVaultManager/utils/webview_login.py` & `UEVaultManager-1.4.0/UEVaultManager/utils/webview_login.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 - do_webview_login() : launch the webview login
 """
 import json
 import logging
 import os
 import webbrowser
 
-from UEVaultManager import __version__
+# noinspection PyPep8Naming
+from UEVaultManager import __version__ as UEVM_version
 
 logger = logging.getLogger('WebViewHelper')
 webview_available = True
 
 try:
     # note : webview don't came with the obsolete webview package but with [pywebview](https://pywebview.flowrl.com/)
     import webview
@@ -175,15 +176,15 @@
         # Additionally, we have to disable JS injection for the first load, as otherwise the user
         # will get an error for some reason.
         url = logout_url
         api.inject_js = False
 
     logger.info('Opening Epic Games login window...')
     # Open logout URL first to remove existing cookies, then redirect to log in.
-    window = webview.create_window(f'UEVaultManager {__version__} - Epic Games Account Login', url=url, width=768, height=1024, js_api=api)
+    window = webview.create_window(f'UEVaultManager {UEVM_version} - Epic Games Account Login', url=url, width=768, height=1024, js_api=api)
     api.window = window
     window.events.loaded += api.on_loaded
 
     try:
         webview.start()
     except Exception as we:
         logger.error(
```

### Comparing `UEVaultManager-1.3.0/UEVaultManager.egg-info/PKG-INFO` & `UEVaultManager-1.4.0/UEVaultManager.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.3.0
+Version: 1.4.0
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -64,8 +64,8 @@
   * [The individual json files](https://uevaultmanager.readthedocs.io/en/latest/output.html#the-individual-json-files)
   * [how to fix invalid search result during the grabbing process](https://uevaultmanager.readthedocs.io/en/latest/output.html#how-to-fix-invalid-search-result-during-the-grabbing-process)
   * [possible values in the error Field](https://uevaultmanager.readthedocs.io/en/latest/output.html#possible-values-in-the-error-field)
 
 [Next](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
 
 
- UEVaultManager ## version:1.3.0 ## codename: Andromeda
+ UEVaultManager ## version:1.4.0 ## codename: Phoenix
```

### Comparing `UEVaultManager-1.3.0/UEVaultManager.egg-info/SOURCES.txt` & `UEVaultManager-1.4.0/UEVaultManager.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,33 +10,35 @@
 UEVaultManager.egg-info/entry_points.txt
 UEVaultManager.egg-info/requires.txt
 UEVaultManager.egg-info/top_level.txt
 UEVaultManager/api/__init__.py
 UEVaultManager/api/egs.py
 UEVaultManager/api/uevm.py
 UEVaultManager/assets/UEVM_200x200.png
+UEVaultManager/assets/checked_16.png
 UEVaultManager/assets/main.ico
+UEVaultManager/assets/unchecked_16.png
 UEVaultManager/downloader/__init__.py
 UEVaultManager/downloader/mp/__init__.py
 UEVaultManager/downloader/mp/manager.py
 UEVaultManager/downloader/mp/workers.py
 UEVaultManager/lfs/__init__.py
 UEVaultManager/lfs/egl.py
 UEVaultManager/lfs/eos.py
 UEVaultManager/lfs/uevmlfs.py
 UEVaultManager/lfs/utils.py
 UEVaultManager/lfs/windows_helpers.py
 UEVaultManager/models/__init__.py
 UEVaultManager/models/app.py
 UEVaultManager/models/chunk.py
 UEVaultManager/models/config.py
+UEVaultManager/models/csv.py
 UEVaultManager/models/downloading.py
 UEVaultManager/models/egl.py
 UEVaultManager/models/exceptions.py
-UEVaultManager/models/gql.py
 UEVaultManager/models/json_manifest.py
 UEVaultManager/models/manifest.py
 UEVaultManager/tkgui/__init__.py
 UEVaultManager/tkgui/main.py
 UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
 UEVaultManager/tkgui/modules/EditCellWindowClass.py
 UEVaultManager/tkgui/modules/EditRowWindowClass.py
```

### Comparing `UEVaultManager-1.3.0/setup.py` & `UEVaultManager-1.4.0/setup.py`

 * *Files identical despite different names*

