# Comparing `tmp/wmwpy-0.2.0b0.tar.gz` & `tmp/wmwpy-0.3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wmwpy-0.2.0b0.tar", last modified: Tue May 16 03:17:25 2023, max compression
+gzip compressed data, was "wmwpy-0.3.0b0.tar", last modified: Tue May 23 20:25:37 2023, max compression
```

## Comparing `wmwpy-0.2.0b0.tar` & `wmwpy-0.3.0b0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:17:25.113730 wmwpy-0.2.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42049 2023-05-16 03:17:25.113730 wmwpy-0.2.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 03:17:25.113730 wmwpy-0.2.0b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:17:25.105730 wmwpy-0.2.0b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:17:25.105730 wmwpy-0.2.0b0/src/wmwpy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:17:25.105730 wmwpy-0.2.0b0/src/wmwpy/Font/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Font/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:17:25.109730 wmwpy-0.2.0b0/src/wmwpy/Utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:17:25.109730 wmwpy-0.2.0b0/src/wmwpy/Utils/Types/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Utils/Types/Documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Utils/Types/Images.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Utils/Types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Utils/XMLTools.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21714 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Utils/rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Utils/textures.py
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Utils/waltex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:17:25.109730 wmwpy-0.2.0b0/src/wmwpy/classes/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/Widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    22504 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/imagelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/level.py
--rw-r--r--   0 runner    (1001) docker     (123)    19156 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/sprite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:17:25.109730 wmwpy-0.2.0b0/src/wmwpy/classes/widget/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_CANVAS.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_FINGER_CATCHER.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_GROUP.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_ICON_LIST.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_LABEL.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_PROGRESS_BAR.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_PUSH_BUTTON.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_SCROLLABLE_CAMERA.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_SCROLLABLE_SET.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_SLIDER.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_TOGGLE.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/game.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/gameobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/gametemplate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:17:25.105730 wmwpy-0.2.0b0/src/wmwpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42049 2023-05-16 03:17:25.000000 wmwpy-0.2.0b0/src/wmwpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-16 03:17:25.000000 wmwpy-0.2.0b0/src/wmwpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 03:17:25.000000 wmwpy-0.2.0b0/src/wmwpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-16 03:17:25.000000 wmwpy-0.2.0b0/src/wmwpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 03:17:25.000000 wmwpy-0.2.0b0/src/wmwpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:25:37.018346 wmwpy-0.3.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42049 2023-05-23 20:25:37.018346 wmwpy-0.3.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 20:25:37.018346 wmwpy-0.3.0b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:25:37.010346 wmwpy-0.3.0b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:25:37.014346 wmwpy-0.3.0b0/src/wmwpy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:25:37.014346 wmwpy-0.3.0b0/src/wmwpy/Font/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Font/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:25:37.014346 wmwpy-0.3.0b0/src/wmwpy/Utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:25:37.014346 wmwpy-0.3.0b0/src/wmwpy/Utils/Types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/Types/Documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/Types/Images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/Types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/XMLTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21854 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/textures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/Utils/waltex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:25:37.014346 wmwpy-0.3.0b0/src/wmwpy/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/Widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22504 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/imagelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14141 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/sprite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:25:37.018346 wmwpy-0.3.0b0/src/wmwpy/classes/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_CANVAS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_FINGER_CATCHER.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_GROUP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_ICON_LIST.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_LABEL.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_PROGRESS_BAR.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_PUSH_BUTTON.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_SCROLLABLE_CAMERA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_SCROLLABLE_SET.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_SLIDER.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/WT_TOGGLE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/classes/widget/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/gameobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-05-23 20:25:25.000000 wmwpy-0.3.0b0/src/wmwpy/gametemplate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:25:37.014346 wmwpy-0.3.0b0/src/wmwpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42049 2023-05-23 20:25:37.000000 wmwpy-0.3.0b0/src/wmwpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-23 20:25:37.000000 wmwpy-0.3.0b0/src/wmwpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:25:37.000000 wmwpy-0.3.0b0/src/wmwpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 20:25:37.000000 wmwpy-0.3.0b0/src/wmwpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 20:25:37.000000 wmwpy-0.3.0b0/src/wmwpy.egg-info/top_level.txt
```

### Comparing `wmwpy-0.2.0b0/LICENSE` & `wmwpy-0.3.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `wmwpy-0.2.0b0/PKG-INFO` & `wmwpy-0.3.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmwpy
-Version: 0.2.0b0
+Version: 0.3.0b0
 Summary: Python module to work with Where's My...? games files.
 Author: ego-lay-atman-bay
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `wmwpy-0.2.0b0/README.md` & `wmwpy-0.3.0b0/README.md`

 * *Files identical despite different names*

### Comparing `wmwpy-0.2.0b0/pyproject.toml` & `wmwpy-0.3.0b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 ]
 dependencies = [
   "lxml",
   "numpy",
   "Pillow",
   "natsort",
   "filetype",
+  "tk",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/wmw-modding/wmwpy"
 "Bug Tracker" = "https://github.com/wmw-modding/wmwpy/issues"
 "Documentation" = "https://wmw-modding.github.io/wmwpy/"
```

### Comparing `wmwpy-0.2.0b0/src/wmwpy/Utils/Types/Documents.py` & `wmwpy-0.3.0b0/src/wmwpy/Utils/Types/Documents.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.2.0b0/src/wmwpy/Utils/Types/Images.py` & `wmwpy-0.3.0b0/src/wmwpy/Utils/Types/Images.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.2.0b0/src/wmwpy/Utils/XMLTools.py` & `wmwpy-0.3.0b0/src/wmwpy/Utils/XMLTools.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.2.0b0/src/wmwpy/Utils/filesystem.py` & `wmwpy-0.3.0b0/src/wmwpy/Utils/filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import io
 from filetype import filetype
 from PIL import Image
 import zipfile
 import natsort
 import typing
+import fnmatch
 
 from .path import joinPath
 # from . import Waltex
 # from . import ImageUtils
 # from ..classes import sprite
 # from ..classes import Object
 
@@ -155,25 +156,25 @@
             fp (str): File path.
 
         Returns:
             bool: Whether the path exists.
         """
         return this.root.exists(fp)
     
-    def listdir(this, path = '/', recursive = False) -> list:
+    def listdir(this, path = '/', recursive = False, search = r'*') -> list:
         """Returns a list of files and subfolders in path.
 
         Args:
             path (str, optional): Path to folder to list. Defaults to '/'.
             recursive (bool, optional): Whether to include subfolders. Defaults to False.
 
         Returns:
             list: List of files and subfolders.
         """
-        return this.get(path).listdir(recursive = recursive)
+        return this.get(path).listdir(recursive = recursive, search = search)
     
     def dump(this, output : str = None):
         """Dump the contents of the filesystem to the specified directory
 
         Args:
             output (str, optional): Path to output directory. Defaults to original path.
         """
@@ -518,25 +519,25 @@
         Returns:
             int: bytes written.
         """
         this.rawdata.truncate(0)
         this.rawdata.seek(0)
         return this.rawdata.write(data)
     
-    def listdir(this, recursive = False):
+    def listdir(this, recursive = False, search = r'*'):
         """Returns a list of files and subfolders in path.
 
         Args:
             path (str, optional): Path to folder to list. Defaults to '/'.
             recursive (bool, optional): Whether to include subfolders. Defaults to False.
 
         Returns:
             list: List of files and subfolders.
         """
-        return this.parent.listdir(recursive = recursive)
+        return this.parent.listdir(recursive = recursive, search = search)
     
 
 class Folder(FileBase):
     def __init__(this, parent = None, path: str = None):
         """Folder
 
         Args:
@@ -645,15 +646,15 @@
             path (str): Path to check.
 
         Returns:
             bool: Does path exist?
         """
         return this.get(path) != None
     
-    def listdir(this, recursive = False):
+    def listdir(this, recursive = False, search = r'*'):
         """Returns a list of files and subfolders in path.
 
         Args:
             path (str, optional): Path to folder to list. Defaults to '/'.
             recursive (bool, optional): Whether to include subfolders. Defaults to False.
 
         Returns:
@@ -662,14 +663,15 @@
         files = []
         for file in this.files:
             files.append(file.path)
             if recursive and file._type.value == this._Type.FOLDER:
                 files = files + file.listdir(recursive = recursive)
         
         files = natsort.natsorted(files)
+        files = fnmatch.filter(files, search)
         
         return files
 
 class Reader():
     MIME = 'text/'
     EXTENSION = 'txt'
```

### Comparing `wmwpy-0.2.0b0/src/wmwpy/Utils/path.py` & `wmwpy-0.3.0b0/src/wmwpy/Utils/path.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,33 +5,32 @@
     """Join a list of paths to create a new path, while ignoring any forward or backward slashes (`/` `\`)
 
     Args:
         *args: (str): str path
     Returns:
         str: New path
     """
+    
     if len(args) == 0:
         return ''
-    else:
-        return pathlib.Path(getRelPath(args[0]), joinPath(*args[1:])).as_posix()
-    # for p in args:
-    #     path = os.path.join(path, getRelPath(p))
-        
-    # return path
 
-def getRelPath(path : str) -> str:
+    path = pathlib.Path(args[0], *[makeRelativePath(p) for p in args[1:]])
+    return path.as_posix()
+
+def makeRelativePath(path : str) -> str:
     """Remove forward and backward slashes (`/` `\`) from the beginning of a path.
-    
-    (I really should rename this function)
 
     Args:
         path (str): Path to check
 
     Returns:
         str: New path without a forward or backward slash.
     """
     if path == '':
         return '.'
     parts = pathlib.Path(path).parts
+    if len(parts) == 0:
+        return path
+    
     if parts[0] in ['\\', '/']:
         return pathlib.Path(*parts[1::]).as_posix()
     return path
```

### Comparing `wmwpy-0.2.0b0/src/wmwpy/Utils/rotate.py` & `wmwpy-0.3.0b0/src/wmwpy/Utils/rotate.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.2.0b0/src/wmwpy/Utils/textures.py` & `wmwpy-0.3.0b0/src/wmwpy/Utils/textures.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.2.0b0/src/wmwpy/Utils/waltex.py` & `wmwpy-0.3.0b0/src/wmwpy/Utils/waltex.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.2.0b0/src/wmwpy/__init__.py` & `wmwpy-0.3.0b0/src/wmwpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.0-beta"
+__version__ = "0.3.0-beta"
 __author__ = 'ego-lay-atman-bay'
 
 import typing
 
 from .game import Game
 from . import classes
 from . import Font
@@ -16,15 +16,15 @@
     platform : typing.Literal['android', 'ios'] = 'android',
     game : str = 'WMW',
     assets : str = None,
     db : str = None,
     profile : str = None,
     baseassets : str = None,
     hook : typing.Callable[[int, str, int], typing.Any] = None,
-):
+) -> Game:
     """load game
 
     Args:
         gamepath (str): Folder to extracted game.
         platform (Literal['android', 'ios'], optional): What platform this game is for. Can be 'android' or 'ios'. Defaults to 'android'.
         game (str, optional): Which game is being loaded. A full list of games is in the `gametemplate.GAMES` variable. Defaults to 'WMW'. 
         assets (str, optional): Relative path to assets folder. Defaults to '/assets'.
```

### Comparing `wmwpy-0.2.0b0/src/wmwpy/classes/Widgets.py` & `wmwpy-0.3.0b0/src/wmwpy/classes/Widgets.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.2.0b0/src/wmwpy/classes/curves.py` & `wmwpy-0.3.0b0/src/wmwpy/classes/curves.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.2.0b0/src/wmwpy/classes/imagelist.py` & `wmwpy-0.3.0b0/src/wmwpy/classes/imagelist.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.2.0b0/src/wmwpy/classes/layout.py` & `wmwpy-0.3.0b0/src/wmwpy/classes/layout.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.2.0b0/src/wmwpy/classes/level.py` & `wmwpy-0.3.0b0/src/wmwpy/game.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,307 +1,233 @@
-import io
-from lxml import etree
-from PIL import Image, ImageTk
-import numpy
-
-from ..Utils.filesystem import *
-from .object import Object
-from ..gameobject import GameObject
-
-class Level(GameObject):
-    XML_TEMPLATE = b"""<?xml version="1.0"?>
-    <Objects>
-    </Objects>
-    """
+import os
+import typing
+
+from .Utils.filesystem import *
+from .Utils import Texture
+from .classes import *
+
+class Game():
+    _DB = '/Data/water.db'
+    _BASEASSETS = '/'
+    _PROFILE = None
     
-    IMAGE_TEMPLATE = Image.new('P', (90,127), 'white').quantize(colors=256)
-    IMAGE_FORMAT = 'PNG'
+    game = 'WMW'
     
     def __init__(
         this,
-        xml : str | bytes | File = None,
-        image : str | bytes | File = None,
-        filesystem : Filesystem | Folder = None,
-        gamepath : str = None,
-        assets : str = '/assets',
+        gamepath : str, assets : str = '/assets',
+        db : str = '/Data/water.db',
+        profile : str = None,
         baseassets : str = '/',
+        platform : typing.Literal['android', 'ios'] = 'android',
+        hook : typing.Callable[[int, str, int], typing.Any] = None,
     ) -> None:
-        """Load level
+        """load game
 
         Args:
-            xml (str | bytes | File): XML file for level.
-            image (str | bytes | File): Image file for level.
-            filesystem (Filesystem | Folder, optional): Filesystem to use. Defaults to None.
-            gamepath (str, optional): Game path. Only used if filesystem not specified. Defaults to None.
-            assets (str, optional): Assets path relative to game path. Only used if filesystem not specified. Defaults to '/assets'.
+            gamepath (str): Folder to extracted game.
+            assets (str, optional): Relative path to assets folder. Defaults to '/assets'.
+            db (str, optional): Relative path to database file from assets folder. Defaults to '/Data/water.db'.
+            profile (str, optional): Relative path to profile file in WMW2. Defaults to `None`
             baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `/`
+            platform (Literal['android', 'ios'], optional): What platform this game is for. Can be 'android' or 'ios'. Defaults to 'android'.
+            hook (Callable[[int, str, int], Any], optional): Hook for loading assets, useful for guis. The function gets called with the paramaters `(progress : int, current : str, max : int)`. Defaults to None.
         """
+        if gamepath == None:
+            return
         
-        this.gamepath = gamepath
+        this.gamepath = os.path.abspath(gamepath)
+        # print(f'{gamepath = }\n{this.gamepath = }')
         this.assets = assets
-        this.filename = ''
-        if this.assets == None:
-            this.assets = '/assets'
+        this.db = db or this._DB
+        this.profile = profile or this._PROFILE
+        this.baseassets = baseassets or this._BASEASSETS
+        this.platform = platform
         
-        super().__init__(filesystem, gamepath, assets, baseassets)
         
-        this.xml_file = super().get_file(xml, template = this.XML_TEMPLATE)
+        this.updateFilesystem(hook = hook)
         
-        this.xml = etree.parse(this.xml_file).getroot()
+    def updateFilesystem(this, hook : typing.Callable[[int, str, int], typing.Any] = None):
+        this.filesystem = Filesystem(this.gamepath, this.assets)
+        this.filesystem.getAssets(hook = hook)
         
-        this.image_file = super().get_file(image)
-        if this.image_file == None:
-            this.image = this.IMAGE_TEMPLATE.copy()
+    def Level(
+        this,
+        xmlPath : str = None,
+        imagePath : str = None,
+        load_callback : typing.Callable[[int, str, int], typing.Any] = None,
+        ignore_errors : bool = False,
+    ):
+        """
+        Load level
+
+        Args:
+            xmlPath (str, optional): Path to xml file. Defaults to None.
+            imagePath (str, optional): Path to image file. Defaults to None.
+        """
+        if isinstance(xmlPath, File):
+            xml = xmlPath
         else:
-            this.image = Image.open(this.image_file).quantize(colors=256)
-        
-        this.objects = []
-        this.properties = {}
-        this.room = (0,0)
+            xml = None
+            if xmlPath:
+                split = os.path.splitext(xmlPath)
+                if split[1] == '':
+                    if imagePath in ['', None]:
+                        imagePath = '.'.join([split[0], 'png'])
+                    xmlPath = '.'.join([split[0], 'xml'])
+                
+                xml = this.filesystem.get(xmlPath)
         
-        this.read()
+        if isinstance(imagePath, File):
+            image = imagePath
+        else:
+            image = None
+            if imagePath:
+                image = this.filesystem.get(imagePath)
+        
+        level = Level(
+            xml = xml,
+            image = image,
+            filesystem = this.filesystem,
+            load_callback = load_callback,
+            ignore_errors = ignore_errors,
+        )
+        if isinstance(xmlPath, File):
+            level.filename = xmlPath.path
+        else:
+            level.filename = xmlPath
         
-        this.scale = 5
+        return level
     
-    @property
-    def size(this) -> tuple[int,int]:
-        """Level image size
-
-        Returns:
-            tuple[int,int]: (width,height)
+    def Object(
+        this,
+        object : str,
+        **kwargs
+    ):
         """
-        return this._image.size
-    
-    @property
-    def image(this) -> Image.Image:
-        """Scaled up Level image
+        Loads object
+
+        Args:
+            object (str): Path to `.hs` object file.
 
         Returns:
-            PIL.Image.Image: PIL Image
+            classes.object.Object: Where's My Water? object.
         """
-        image = this._image.copy()
         
-        size = numpy.array(image.size)
-        size = size * this.scale
         
-        image = image.resize(size, resample = Image.NEAREST)
+        if not isinstance(object, File):
+            object = this.filesystem.get(object)
         
-        return image
+        obj = Object(
+            object,
+            filesystem = this.filesystem,
+            **kwargs
+        )
+        if isinstance(object, File):
+            obj.filename = object.path
+        else:
+            obj.filename = object
+            
         
-    @image.setter
-    def image(this, value : Image.Image):
-        this._image = value
+        return obj
     
-    @property
-    def PhotoImage(this) -> ImageTk.PhotoImage:
-        """Tkinter PhotoImage of the Level image
+    def Imagelist(
+        this,
+        imagelist : str = None,
+        HD = False,
+    ):
+        """
+        Load imagelist
+
+        Args:
+            imagelist (str): Path to `.imagelist` file. Defaults to None
+            HD (bool, optional): Whether to use HD textures. Defaults to False.
 
         Returns:
-            ImageTk.PhotoImage: Tkinter PhotoImage
+            classes.imagelist.Imagelist: Imagelist object.
         """
-        this._PhotoImage = ImageTk.PhotoImage(this.image)
-        return this._PhotoImage
-
-    @property
-    def scale(this) -> int:
-        """Level size scale
-        """
-        return this._scale
-    @scale.setter
-    def scale(this, value : int):
-        this._scale = value
         
-        for obj in this.objects:
-            obj.scale = this._scale
-    
-    def read(this):
-        """Read level XML
-        """
-        this.objects : list[Object] = []
-        this.properties = {}
+        if not isinstance(imagelist, File):
+            imagelist = this.filesystem.get(imagelist)
         
-        id = 0
+        imagelistObject = Imagelist(
+            imagelist,
+            filesystem = this.filesystem,
+            HD = False,
+        )
+        if isinstance(imagelist, File):
+            imagelistObject.filename = imagelist.path
+        else:
+            imagelistObject.filename = imagelist
         
-        for element in this.xml:
-            # comment safe-guard
-            if element is etree.Comment:
-                continue
-            
-            if element.tag == 'Object':
-                properties = {}
-                pos = (0,0)
-                name = element.get('name')
-                
-                for el in element:
-                    if not el is etree.Comment:
-                        if el.tag == 'AbsoluteLocation':
-                            pos = el.get('value')
-                        
-                        elif el.tag == 'Properties':
-                            for property in el:
-                                if not property is etree.Comment and property.tag == 'Property':
-                                    properties[property.get('name')] = property.get('value')
-                
-                obj = Object(
-                    this.filesystem.get(properties['Filename']), # get file because `Object` does not take filepath
-                    filesystem = this.filesystem,
-                    properties = properties,
-                    pos = pos,
-                    name = name,
-                )
-                
-                obj.id = id
-                
-                this.objects.append(obj)
-                
-                id += 1
-            
-            if element.tag == 'Properties':
-                for el in element:
-                    if el is etree.Comment:
-                        continue
-                    
-                    if el.tag == 'Property':
-                        this.properties[el.get('name')] = el.get('name')
-            
-            if element.tag == 'Room':
-                for el in element:
-                    if el is etree.Comment:
-                        continue
-                    
-                    if el.tag == 'AbsoluteLocation':
-                        this.room = tuple([float(_) for _ in el.get('value').split()])
+        return imagelistObject
     
-    def export(
+    def Sprite(
         this,
-        filename : str = None,
-        exportObjects : bool = False,
-    ) -> bytes:
-        """Export level
+        sprite : str,
+        **kwargs
+    ):
+        """
+        Loads sprite.
 
         Args:
-            filename (str, optional): Path to level. Defaults to Level.filename.
-            exportObjects (bool, optional): Whether to export objects. Defaults to False.
-
-        Raises:
-            TypeError: Path is not a file.
+            sprite (str): Path to `.sprite` file.`
 
         Returns:
-            bytes: XML file.
+            classes.sprite.Sprite: Sprite object.
         """
-        if filename == None:
-            if this.filename:
-                filename = this.filename
-        else:
-            this.filename = filename
-        
-        xml : etree.ElementBase = etree.Element('Objects')
-        for object in this.objects:
-            if exportObjects:
-                object.export()
-            
-            xml.append(object.getLevelXML())
-        
-        room = etree.Element('Room')
-        etree.SubElement(room, 'AbsoluteLocation', value = ' '.join([str(_) for _ in this.room]))
-
-        properties = etree.Element('Properties')
-        for name in this.properties:
-            value = this.properties[name]
-            etree.SubElement(properties, 'Property', name = name, value = value)
-        
-        if len(properties):
-            xml.append(properties)
         
-        this.xml = xml
+        if not isinstance(sprite, File):
+            sprite = this.filesystem.get(sprite)
         
-        output = etree.tostring(xml, pretty_print=True, xml_declaration=True, encoding='utf-8')
-        
-        if (file := this.filesystem.get(filename)) != None:
-            if isinstance(file, File):
-                file.write(output)
-            else:
-                raise TypeError(f'Path {filename} is not a file.')
-                
+        spriteObject = Sprite(
+            sprite,
+            filesystem = this.filesystem,
+            **kwargs
+        )
+        if isinstance(sprite, File):
+            spriteObject.filename = sprite.path
         else:
-            this.filesystem.add(filename, output)
+            spriteObject.filename = sprite.path
         
-        return output
+        return spriteObject
     
-    def addObject(
+    def Texture(
         this,
-        filename : str | Object,
-        properties : dict = {},
-        pos : tuple[float,float] = (0,0),
-        name : str = 'Obj'
+        texture : str,
     ):
-        """Add object to level.
+        """
+        Get image texture. Doesn't matter if it's a `.waltex` image or not.
 
         Args:
-            filename (str | Object): Filename for object. If it's a wmwpy.classes.Object class, then it will use that instead.
-            properties (dict, optional): Object properties. Defaults to {}.
-            pos (tuple[x,y], optional): Position of object in level. Defaults to (0,0).
-            name (str, optional): Name of object. May get renamed if object with name alread exists. Defaults to 'Obj'.
+            texture (str): Path to image file.
 
         Returns:
-            Object: wmwpy Object.
+            Utils.textures.Texture: Texture object.
         """
-        if not isinstance(filename, Object):
-            filename = Object(
-                filename,
-                filesystem = this.filesystem,
-                properties = properties,
-                pos = pos,
-                name = name,
-            )
-        else:
-            filename.name = name
-            filename.pos = pos
-            filename.setProperty(properties)
-        
-        obj = filename
-        
-        id = 0
-        while this.getObjectById(id) != None:
-            id += 1
-        
-        if this.getObject(obj.name) != None:
-            objnum = 0
-            name = obj.name
-            
-            while this.getObject(obj.name) != None:
-                objnum += 1
-                obj.name = f'{name}{str(objnum)}'
-        
-        obj.id = id
-        this.objects.append(obj)
-        obj.scale = this.scale
         
-        return obj
+        if not isinstance(texture, File):
+            texture = this.filesystem.get(texture)
+        
+        return Texture(
+            texture
+        )
+    
+    def Layout(this, layout : str):
+        raise NotImplementedError('load layout is not implemented yet.')
     
-    def getObjectById(this, id : int) -> Object:
-        """Get an Object by it's id
+    def generateFileManifest(this, writeFile : bool = True, filename : str = '/FileManifest.txt'):
+        """Generate the `FileManifest.txt` file needed for some games, such as WMM. This just generates a text file with the paths to every file in the `assets` folder (which includes the `FileManifest.txt` file).
 
         Args:
-            id (int): Object id to find
+            writeFile (bool, optional): Write the manifest to the `FileManifest.txt` file. Defaults to True.
+            filename (str, optional): Filename for FileManifest.txt. Defaults to 'filename'.
 
         Returns:
-            Object: wmwpy Object
-        """
-        for obj in this.objects:
-            if obj.id == id:
-                return obj
-        return None
-    
-    def getObject(this, name : str):
-        """
-        Get object by name
-
-        Args:
-            name (str): Object name.
+            str: Contents of `FileManifest.txt`
         """
+        manifest = '\n'.join(this.filesystem.listdir(recursive = True))
         
-        for obj in this.objects:
-            if obj.name == name:
-                return obj
+        if writeFile:
+            this.filesystem.add(filename, manifest, replace = True)
         
-        return None
+        return manifest
```

### Comparing `wmwpy-0.2.0b0/src/wmwpy/classes/object.py` & `wmwpy-0.3.0b0/src/wmwpy/classes/object.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,18 +379,21 @@
         return output
     
     def updateProperties(this):
         """Update properties. Deletes any properties that are the same as defaultProperties.
         """
         properties = list(this.properties.keys())
         
-        for property in properties:
-            if property in this.defaultProperties:
-                if this.properties[property] == this.defaultProperties[property]:
-                    del this.properties[property]
+        # for property in properties:
+        #     if property in this.defaultProperties:
+        #         if this.properties[property] == this.defaultProperties[property]:
+        #             del this.properties[property]
+        
+        # if this.type != None:
+        #     this.properties['Type'] = this.type
 
     def getLevelXML(
         this,
         filename : str = None,
     ) -> etree.ElementBase:
         """Gets XML to be used in levels.
 
@@ -439,15 +442,15 @@
         """The Object type, based off the `Type` property.
         """
         if 'Type' in this.properties:
             return this.properties['Type']
         elif 'Type' in this.defaultProperties:
             return this.defaultProperties['Type']
         else:
-            return None
+            return ''
     @type.setter
     def type(this, value : str):
         if not isinstance(value, str):
             raise TypeError('type is not a string')
         
         if not 'Type' in this.defaultProperties:
             this.defaultProperties['Type'] = value
```

### Comparing `wmwpy-0.2.0b0/src/wmwpy/classes/sprite.py` & `wmwpy-0.3.0b0/src/wmwpy/classes/sprite.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.2.0b0/src/wmwpy/classes/widget/__init__.py` & `wmwpy-0.3.0b0/src/wmwpy/classes/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.2.0b0/src/wmwpy/classes/widget/widget.py` & `wmwpy-0.3.0b0/src/wmwpy/classes/widget/widget.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.2.0b0/src/wmwpy/gameobject.py` & `wmwpy-0.3.0b0/src/wmwpy/gameobject.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.2.0b0/src/wmwpy/gametemplate.py` & `wmwpy-0.3.0b0/src/wmwpy/gametemplate.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.2.0b0/src/wmwpy.egg-info/PKG-INFO` & `wmwpy-0.3.0b0/src/wmwpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmwpy
-Version: 0.2.0b0
+Version: 0.3.0b0
 Summary: Python module to work with Where's My...? games files.
 Author: ego-lay-atman-bay
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `wmwpy-0.2.0b0/src/wmwpy.egg-info/SOURCES.txt` & `wmwpy-0.3.0b0/src/wmwpy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/wmwpy.egg-info/dependency_links.txt
 src/wmwpy.egg-info/requires.txt
 src/wmwpy.egg-info/top_level.txt
 src/wmwpy/Font/__init__.py
 src/wmwpy/Utils/XMLTools.py
 src/wmwpy/Utils/__init__.py
 src/wmwpy/Utils/filesystem.py
+src/wmwpy/Utils/logging_utils.py
 src/wmwpy/Utils/path.py
 src/wmwpy/Utils/rotate.py
 src/wmwpy/Utils/textures.py
 src/wmwpy/Utils/waltex.py
 src/wmwpy/Utils/Types/Documents.py
 src/wmwpy/Utils/Types/Images.py
 src/wmwpy/Utils/Types/__init__.py
```

