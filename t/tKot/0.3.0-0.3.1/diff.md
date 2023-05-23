# Comparing `tmp/tKot-0.3.0.tar.gz` & `tmp/tKot-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tKot-0.3.0.tar", last modified: Tue May 23 06:07:24 2023, max compression
+gzip compressed data, was "tKot-0.3.1.tar", last modified: Tue May 23 06:50:30 2023, max compression
```

## Comparing `tKot-0.3.0.tar` & `tKot-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 06:07:24.749444 tKot-0.3.0/
--rw-rw-rw-   0        0        0      483 2023-05-23 06:07:24.748443 tKot-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       30 2023-02-27 11:57:31.000000 tKot-0.3.0/README.md
--rw-rw-rw-   0        0        0      602 2023-05-23 06:00:55.000000 tKot-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 06:07:24.749444 tKot-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      311 2023-02-27 12:07:32.000000 tKot-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 06:07:24.724443 tKot-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 06:07:24.735463 tKot-0.3.0/src/tKot/
--rw-rw-rw-   0        0        0       60 2023-02-28 12:42:47.000000 tKot-0.3.0/src/tKot/__init__.py
--rw-rw-rw-   0        0        0     2487 2023-05-23 06:06:44.000000 tKot-0.3.0/src/tKot/buttons.py
--rw-rw-rw-   0        0        0     2972 2023-05-03 11:19:55.000000 tKot-0.3.0/src/tKot/frames.py
-drwxrwxrwx   0        0        0        0 2023-05-23 06:07:24.746443 tKot-0.3.0/src/tKot.egg-info/
--rw-rw-rw-   0        0        0      483 2023-05-23 06:07:24.000000 tKot-0.3.0/src/tKot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-05-23 06:07:24.000000 tKot-0.3.0/src/tKot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 06:07:24.000000 tKot-0.3.0/src/tKot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-23 06:07:24.000000 tKot-0.3.0/src/tKot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-23 06:07:24.000000 tKot-0.3.0/src/tKot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 06:50:30.547057 tKot-0.3.1/
+-rw-rw-rw-   0        0        0      483 2023-05-23 06:50:30.546058 tKot-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2023-02-27 11:57:31.000000 tKot-0.3.1/README.md
+-rw-rw-rw-   0        0        0      602 2023-05-23 06:50:19.000000 tKot-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 06:50:30.547057 tKot-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      311 2023-02-27 12:07:32.000000 tKot-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 06:50:30.484266 tKot-0.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 06:50:30.497762 tKot-0.3.1/src/tKot/
+-rw-rw-rw-   0        0        0       60 2023-02-28 12:42:47.000000 tKot-0.3.1/src/tKot/__init__.py
+-rw-rw-rw-   0        0        0     2482 2023-05-23 06:50:19.000000 tKot-0.3.1/src/tKot/buttons.py
+-rw-rw-rw-   0        0        0      324 2023-05-23 06:47:52.000000 tKot-0.3.1/src/tKot/common.py
+-rw-rw-rw-   0        0        0     2972 2023-05-03 11:19:55.000000 tKot-0.3.1/src/tKot/frames.py
+drwxrwxrwx   0        0        0        0 2023-05-23 06:50:30.544062 tKot-0.3.1/src/tKot.egg-info/
+-rw-rw-rw-   0        0        0      483 2023-05-23 06:50:30.000000 tKot-0.3.1/src/tKot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-05-23 06:50:30.000000 tKot-0.3.1/src/tKot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 06:50:30.000000 tKot-0.3.1/src/tKot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-23 06:50:30.000000 tKot-0.3.1/src/tKot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-23 06:50:30.000000 tKot-0.3.1/src/tKot.egg-info/top_level.txt
```

### Comparing `tKot-0.3.0/pyproject.toml` & `tKot-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backed = "setuptools.build_meta"
 
 [project]
 name = "tKot"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `tKot-0.3.0/src/tKot/buttons.py` & `tKot-0.3.1/src/tKot/buttons.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import tkinter as tk
 from PIL import Image, ImageTk
+from .common import Point
 
 
 class Icon(tk.Widget):
     p_im: Image.Image | None
     im: ImageTk.PhotoImage | None
     info: str | None
 
@@ -28,49 +29,47 @@
 
 class StatusIcon:
     """Icon with status properties"""
     __c: tk.Canvas
     c_id: int
     __current: int
     __im: ImageTk
-    __h: int
-    __w: int
+    __size = Point
 
     def __init__(self,
                  canvas: tk.Canvas,
                  images: dict[int, Image],
                  default: int = None):
         self.__c = canvas
         """ canvas for widget """
         self.__c_id = -1
         """ Image canvas ID. -1 if not place """
         self.__images = images
         self.__current = 0
-        self.__h = 100
-        """icon height"""
-        self.__w = 100
-        """icon width"""
+        self.__size = Point(100, 100)
+        """icon size"""
         self.set_status(tuple(self.__images.keys())[0] if default is None else self.__images[default])
 
     def get_status(self) -> int:
         """return current status"""
         return self.__current
 
     def set_status(self, value: int):
         """set status with change image"""
-        self.__im = ImageTk.PhotoImage(self.__images[value].resize((self.__h, self.__w)))
+        self.__im = ImageTk.PhotoImage(self.__images[value].resize((self.__size.x, self.__size.y)))
         self.__current = value
         if self.__c_id != -1:
             self.__c.itemconfigure(self.__c_id, image=self.__im)
 
-    def set_width(self, value: int):
-        self.__w = value
+    def set_size(self, value: Point):
+        self.__size = value
 
-    def set_height(self, value: int):
-        self.__h = value
+    @property
+    def size(self):
+        return self.__size
 
     def place(self, x: int, y: int):
         """ replace on canvas by (x, y). Old canvas id shall delete"""
         if self.__c_id != -1:
             self.__c.delete(self.__c_id)
         self.__c_id = self.__c.create_image(x, y,
                                             anchor=tk.NW,
```

### Comparing `tKot-0.3.0/src/tKot/frames.py` & `tKot-0.3.1/src/tKot/frames.py`

 * *Files identical despite different names*

