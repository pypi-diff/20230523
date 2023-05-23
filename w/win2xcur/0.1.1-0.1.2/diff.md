# Comparing `tmp/win2xcur-0.1.1.tar.gz` & `tmp/win2xcur-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "win2xcur-0.1.1.tar", last modified: Mon Mar 28 04:49:54 2022, max compression
+gzip compressed data, was "win2xcur-0.1.2.tar", last modified: Tue May 23 02:39:21 2023, max compression
```

## Comparing `win2xcur-0.1.1.tar` & `win2xcur-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 quantum   (1000) quantum   (1000)        0 2022-03-28 04:49:54.837281 win2xcur-0.1.1/
--rw-r--r--   0 quantum   (1000) quantum   (1000)     3231 2022-03-28 04:49:54.837281 win2xcur-0.1.1/PKG-INFO
--rw-r--r--   0 quantum   (1000) quantum   (1000)     2150 2022-03-24 05:37:17.000000 win2xcur-0.1.1/README.md
--rw-r--r--   0 quantum   (1000) quantum   (1000)       38 2022-03-28 04:49:54.837281 win2xcur-0.1.1/setup.cfg
--rw-r--r--   0 quantum   (1000) quantum   (1000)     1536 2022-03-28 04:49:36.000000 win2xcur-0.1.1/setup.py
-drwxr-xr-x   0 quantum   (1000) quantum   (1000)        0 2022-03-28 04:49:54.837281 win2xcur-0.1.1/win2xcur/
--rw-r--r--   0 quantum   (1000) quantum   (1000)        0 2020-09-26 19:43:32.000000 win2xcur-0.1.1/win2xcur/__init__.py
--rw-r--r--   0 quantum   (1000) quantum   (1000)     1027 2020-10-04 08:14:48.000000 win2xcur-0.1.1/win2xcur/cursor.py
-drwxr-xr-x   0 quantum   (1000) quantum   (1000)        0 2022-03-28 04:49:54.837281 win2xcur-0.1.1/win2xcur/main/
--rw-r--r--   0 quantum   (1000) quantum   (1000)        0 2020-10-03 05:53:27.000000 win2xcur-0.1.1/win2xcur/main/__init__.py
--rw-r--r--   0 quantum   (1000) quantum   (1000)     2674 2022-03-17 05:46:41.000000 win2xcur-0.1.1/win2xcur/main/win2xcur.py
--rw-r--r--   0 quantum   (1000) quantum   (1000)     1395 2020-10-04 08:11:26.000000 win2xcur-0.1.1/win2xcur/main/x2wincur.py
-drwxr-xr-x   0 quantum   (1000) quantum   (1000)        0 2022-03-28 04:49:54.837281 win2xcur-0.1.1/win2xcur/parser/
--rw-r--r--   0 quantum   (1000) quantum   (1000)      547 2020-10-03 05:53:27.000000 win2xcur-0.1.1/win2xcur/parser/__init__.py
--rw-r--r--   0 quantum   (1000) quantum   (1000)     4648 2021-03-09 20:46:00.000000 win2xcur-0.1.1/win2xcur/parser/ani.py
--rw-r--r--   0 quantum   (1000) quantum   (1000)      400 2020-09-27 04:50:10.000000 win2xcur-0.1.1/win2xcur/parser/base.py
--rw-r--r--   0 quantum   (1000) quantum   (1000)     1447 2020-10-04 07:13:04.000000 win2xcur-0.1.1/win2xcur/parser/cur.py
--rw-r--r--   0 quantum   (1000) quantum   (1000)     3954 2022-03-28 04:46:58.000000 win2xcur-0.1.1/win2xcur/parser/xcursor.py
--rw-r--r--   0 quantum   (1000) quantum   (1000)     1590 2020-10-04 07:13:04.000000 win2xcur-0.1.1/win2xcur/shadow.py
--rw-r--r--   0 quantum   (1000) quantum   (1000)      355 2022-03-17 05:46:41.000000 win2xcur-0.1.1/win2xcur/utils.py
-drwxr-xr-x   0 quantum   (1000) quantum   (1000)        0 2022-03-28 04:49:54.837281 win2xcur-0.1.1/win2xcur/writer/
--rw-r--r--   0 quantum   (1000) quantum   (1000)      255 2020-10-03 05:53:27.000000 win2xcur-0.1.1/win2xcur/writer/__init__.py
--rw-r--r--   0 quantum   (1000) quantum   (1000)     2502 2022-03-28 04:47:55.000000 win2xcur-0.1.1/win2xcur/writer/windows.py
--rw-r--r--   0 quantum   (1000) quantum   (1000)     1509 2020-10-04 07:57:27.000000 win2xcur-0.1.1/win2xcur/writer/x11.py
-drwxr-xr-x   0 quantum   (1000) quantum   (1000)        0 2022-03-28 04:49:54.837281 win2xcur-0.1.1/win2xcur.egg-info/
--rw-r--r--   0 quantum   (1000) quantum   (1000)     3231 2022-03-28 04:49:54.000000 win2xcur-0.1.1/win2xcur.egg-info/PKG-INFO
--rw-r--r--   0 quantum   (1000) quantum   (1000)      570 2022-03-28 04:49:54.000000 win2xcur-0.1.1/win2xcur.egg-info/SOURCES.txt
--rw-r--r--   0 quantum   (1000) quantum   (1000)        1 2022-03-28 04:49:54.000000 win2xcur-0.1.1/win2xcur.egg-info/dependency_links.txt
--rw-r--r--   0 quantum   (1000) quantum   (1000)       97 2022-03-28 04:49:54.000000 win2xcur-0.1.1/win2xcur.egg-info/entry_points.txt
--rw-r--r--   0 quantum   (1000) quantum   (1000)       11 2022-03-28 04:49:54.000000 win2xcur-0.1.1/win2xcur.egg-info/requires.txt
--rw-r--r--   0 quantum   (1000) quantum   (1000)        9 2022-03-28 04:49:54.000000 win2xcur-0.1.1/win2xcur.egg-info/top_level.txt
+drwxr-xr-x   0 quantum   (1000) quantum   (1000)        0 2023-05-23 02:39:21.925808 win2xcur-0.1.2/
+-rw-r--r--   0 quantum   (1000) quantum   (1000)     3231 2023-05-23 02:39:21.925808 win2xcur-0.1.2/PKG-INFO
+-rw-r--r--   0 quantum   (1000) quantum   (1000)     2150 2022-03-24 05:37:17.000000 win2xcur-0.1.2/README.md
+-rw-r--r--   0 quantum   (1000) quantum   (1000)       38 2023-05-23 02:39:21.925808 win2xcur-0.1.2/setup.cfg
+-rw-r--r--   0 quantum   (1000) quantum   (1000)     1536 2023-05-23 02:38:58.000000 win2xcur-0.1.2/setup.py
+drwxr-xr-x   0 quantum   (1000) quantum   (1000)        0 2023-05-23 02:39:21.925808 win2xcur-0.1.2/win2xcur/
+-rw-r--r--   0 quantum   (1000) quantum   (1000)        0 2020-09-26 19:43:32.000000 win2xcur-0.1.2/win2xcur/__init__.py
+-rw-r--r--   0 quantum   (1000) quantum   (1000)     1027 2020-10-04 08:14:48.000000 win2xcur-0.1.2/win2xcur/cursor.py
+drwxr-xr-x   0 quantum   (1000) quantum   (1000)        0 2023-05-23 02:39:21.925808 win2xcur-0.1.2/win2xcur/main/
+-rw-r--r--   0 quantum   (1000) quantum   (1000)        0 2020-10-03 05:53:27.000000 win2xcur-0.1.2/win2xcur/main/__init__.py
+-rw-r--r--   0 quantum   (1000) quantum   (1000)     2674 2022-03-17 05:46:41.000000 win2xcur-0.1.2/win2xcur/main/win2xcur.py
+-rw-r--r--   0 quantum   (1000) quantum   (1000)     1395 2020-10-04 08:11:26.000000 win2xcur-0.1.2/win2xcur/main/x2wincur.py
+drwxr-xr-x   0 quantum   (1000) quantum   (1000)        0 2023-05-23 02:39:21.925808 win2xcur-0.1.2/win2xcur/parser/
+-rw-r--r--   0 quantum   (1000) quantum   (1000)      547 2020-10-03 05:53:27.000000 win2xcur-0.1.2/win2xcur/parser/__init__.py
+-rw-r--r--   0 quantum   (1000) quantum   (1000)     4648 2021-03-09 20:46:00.000000 win2xcur-0.1.2/win2xcur/parser/ani.py
+-rw-r--r--   0 quantum   (1000) quantum   (1000)      400 2020-09-27 04:50:10.000000 win2xcur-0.1.2/win2xcur/parser/base.py
+-rw-r--r--   0 quantum   (1000) quantum   (1000)     1447 2020-10-04 07:13:04.000000 win2xcur-0.1.2/win2xcur/parser/cur.py
+-rw-r--r--   0 quantum   (1000) quantum   (1000)     3954 2022-03-28 04:46:58.000000 win2xcur-0.1.2/win2xcur/parser/xcursor.py
+-rw-r--r--   0 quantum   (1000) quantum   (1000)     1929 2022-04-24 06:04:08.000000 win2xcur-0.1.2/win2xcur/shadow.py
+-rw-r--r--   0 quantum   (1000) quantum   (1000)      355 2022-03-17 05:46:41.000000 win2xcur-0.1.2/win2xcur/utils.py
+drwxr-xr-x   0 quantum   (1000) quantum   (1000)        0 2023-05-23 02:39:21.925808 win2xcur-0.1.2/win2xcur/writer/
+-rw-r--r--   0 quantum   (1000) quantum   (1000)      255 2020-10-03 05:53:27.000000 win2xcur-0.1.2/win2xcur/writer/__init__.py
+-rw-r--r--   0 quantum   (1000) quantum   (1000)     2502 2022-03-28 04:47:55.000000 win2xcur-0.1.2/win2xcur/writer/windows.py
+-rw-r--r--   0 quantum   (1000) quantum   (1000)     1509 2020-10-04 07:57:27.000000 win2xcur-0.1.2/win2xcur/writer/x11.py
+drwxr-xr-x   0 quantum   (1000) quantum   (1000)        0 2023-05-23 02:39:21.925808 win2xcur-0.1.2/win2xcur.egg-info/
+-rw-r--r--   0 quantum   (1000) quantum   (1000)     3231 2023-05-23 02:39:21.000000 win2xcur-0.1.2/win2xcur.egg-info/PKG-INFO
+-rw-r--r--   0 quantum   (1000) quantum   (1000)      570 2023-05-23 02:39:21.000000 win2xcur-0.1.2/win2xcur.egg-info/SOURCES.txt
+-rw-r--r--   0 quantum   (1000) quantum   (1000)        1 2023-05-23 02:39:21.000000 win2xcur-0.1.2/win2xcur.egg-info/dependency_links.txt
+-rw-r--r--   0 quantum   (1000) quantum   (1000)       97 2023-05-23 02:39:21.000000 win2xcur-0.1.2/win2xcur.egg-info/entry_points.txt
+-rw-r--r--   0 quantum   (1000) quantum   (1000)       11 2023-05-23 02:39:21.000000 win2xcur-0.1.2/win2xcur.egg-info/requires.txt
+-rw-r--r--   0 quantum   (1000) quantum   (1000)        9 2023-05-23 02:39:21.000000 win2xcur-0.1.2/win2xcur.egg-info/top_level.txt
```

### Comparing `win2xcur-0.1.1/PKG-INFO` & `win2xcur-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: win2xcur
-Version: 0.1.1
+Version: 0.1.2
 Summary: win2xcur is a tool to convert Windows .cur and .ani cursors to Xcursor format.
 Home-page: https://github.com/quantum5/win2xcur
 Author: quantum
 Author-email: quantum2048@gmail.com
 License: UNKNOWN
 Keywords: cur ani x11 windows win32 cursor xcursor
 Platform: UNKNOWN
```

### Comparing `win2xcur-0.1.1/README.md` & `win2xcur-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `win2xcur-0.1.1/setup.py` & `win2xcur-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name='win2xcur',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=['numpy', 'Wand'],
 
     entry_points={
         'console_scripts': [
             'win2xcur = win2xcur.main.win2xcur:main',
             'x2wincur = win2xcur.main.x2wincur:main',
```

### Comparing `win2xcur-0.1.1/win2xcur/cursor.py` & `win2xcur-0.1.2/win2xcur/cursor.py`

 * *Files identical despite different names*

### Comparing `win2xcur-0.1.1/win2xcur/main/win2xcur.py` & `win2xcur-0.1.2/win2xcur/main/win2xcur.py`

 * *Files identical despite different names*

### Comparing `win2xcur-0.1.1/win2xcur/main/x2wincur.py` & `win2xcur-0.1.2/win2xcur/main/x2wincur.py`

 * *Files identical despite different names*

### Comparing `win2xcur-0.1.1/win2xcur/parser/__init__.py` & `win2xcur-0.1.2/win2xcur/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `win2xcur-0.1.1/win2xcur/parser/ani.py` & `win2xcur-0.1.2/win2xcur/parser/ani.py`

 * *Files identical despite different names*

### Comparing `win2xcur-0.1.1/win2xcur/parser/cur.py` & `win2xcur-0.1.2/win2xcur/parser/cur.py`

 * *Files identical despite different names*

### Comparing `win2xcur-0.1.1/win2xcur/parser/xcursor.py` & `win2xcur-0.1.2/win2xcur/parser/xcursor.py`

 * *Files identical despite different names*

### Comparing `win2xcur-0.1.1/win2xcur/shadow.py` & `win2xcur-0.1.2/win2xcur/shadow.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,47 @@
 from typing import List
 
 from wand.color import Color
-from wand.image import BaseImage, Image
+from wand.image import BaseImage, COMPOSITE_OPERATORS, Image
 
 from win2xcur.cursor import CursorFrame
 
+if 'copy_opacity' in COMPOSITE_OPERATORS:
+    COPY_ALPHA = 'copy_opacity'  # ImageMagick 6 name
+    NEEDS_NEGATE = False
+else:
+    COPY_ALPHA = 'copy_alpha'  # ImageMagick 7 name
+    NEEDS_NEGATE = True
+
 
 def apply_to_image(image: BaseImage, *, color: str, radius: float, sigma: float, xoffset: float,
                    yoffset: float) -> Image:
     xoffset = round(xoffset * image.width)
     yoffset = round(yoffset * image.height)
     new_width = image.width + 3 * xoffset
     new_height = image.height + 3 * yoffset
 
+    if NEEDS_NEGATE:
+        channel = image.channel_images['opacity'].clone()
+        channel.negate()
+    else:
+        channel = image.channel_images['opacity']
+
     opacity = Image(width=new_width, height=new_height, pseudo='xc:white')
-    opacity.composite(image.channel_images['opacity'], left=xoffset, top=yoffset)
+    opacity.composite(channel, left=xoffset, top=yoffset)
     opacity.gaussian_blur(radius * image.width, sigma * image.width)
     opacity.negate()
     opacity.modulate(50)
 
     shadow = Image(width=new_width, height=new_height, pseudo='xc:' + color)
-    shadow.composite(opacity, operator='copy_opacity')
+    shadow.composite(opacity, operator=COPY_ALPHA)
 
     result = Image(width=new_width, height=new_height, pseudo='xc:transparent')
+    result.composite(shadow)
     result.composite(image)
-    result.composite(shadow, operator='difference')
 
     trimmed = result.clone()
     trimmed.trim(color=Color('transparent'))
     result.crop(width=max(image.width, trimmed.width), height=max(image.height, trimmed.height))
     return result
```

### Comparing `win2xcur-0.1.1/win2xcur/writer/windows.py` & `win2xcur-0.1.2/win2xcur/writer/windows.py`

 * *Files identical despite different names*

### Comparing `win2xcur-0.1.1/win2xcur/writer/x11.py` & `win2xcur-0.1.2/win2xcur/writer/x11.py`

 * *Files identical despite different names*

### Comparing `win2xcur-0.1.1/win2xcur.egg-info/PKG-INFO` & `win2xcur-0.1.2/win2xcur.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: win2xcur
-Version: 0.1.1
+Version: 0.1.2
 Summary: win2xcur is a tool to convert Windows .cur and .ani cursors to Xcursor format.
 Home-page: https://github.com/quantum5/win2xcur
 Author: quantum
 Author-email: quantum2048@gmail.com
 License: UNKNOWN
 Keywords: cur ani x11 windows win32 cursor xcursor
 Platform: UNKNOWN
```

### Comparing `win2xcur-0.1.1/win2xcur.egg-info/SOURCES.txt` & `win2xcur-0.1.2/win2xcur.egg-info/SOURCES.txt`

 * *Files identical despite different names*

