# Comparing `tmp/tKot-0.3.4.tar.gz` & `tmp/tKot-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tKot-0.3.4.tar", last modified: Tue May 23 08:02:55 2023, max compression
+gzip compressed data, was "tKot-0.3.5.tar", last modified: Tue May 23 08:12:40 2023, max compression
```

## Comparing `tKot-0.3.4.tar` & `tKot-0.3.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 08:02:55.860141 tKot-0.3.4/
--rw-rw-rw-   0        0        0      483 2023-05-23 08:02:55.860141 tKot-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0       30 2023-02-27 11:57:31.000000 tKot-0.3.4/README.md
--rw-rw-rw-   0        0        0      602 2023-05-23 08:02:23.000000 tKot-0.3.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 08:02:55.861173 tKot-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      311 2023-02-27 12:07:32.000000 tKot-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:02:55.805924 tKot-0.3.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 08:02:55.819018 tKot-0.3.4/src/tKot/
--rw-rw-rw-   0        0        0       60 2023-02-28 12:42:47.000000 tKot-0.3.4/src/tKot/__init__.py
--rw-rw-rw-   0        0        0     2827 2023-05-23 07:38:30.000000 tKot-0.3.4/src/tKot/buttons.py
--rw-rw-rw-   0        0        0      707 2023-05-23 08:02:23.000000 tKot-0.3.4/src/tKot/common.py
--rw-rw-rw-   0        0        0     2972 2023-05-03 11:19:55.000000 tKot-0.3.4/src/tKot/frames.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:02:55.857139 tKot-0.3.4/src/tKot.egg-info/
--rw-rw-rw-   0        0        0      483 2023-05-23 08:02:55.000000 tKot-0.3.4/src/tKot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-05-23 08:02:55.000000 tKot-0.3.4/src/tKot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 08:02:55.000000 tKot-0.3.4/src/tKot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-23 08:02:55.000000 tKot-0.3.4/src/tKot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-23 08:02:55.000000 tKot-0.3.4/src/tKot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 08:12:40.235607 tKot-0.3.5/
+-rw-rw-rw-   0        0        0      483 2023-05-23 08:12:40.234644 tKot-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2023-02-27 11:57:31.000000 tKot-0.3.5/README.md
+-rw-rw-rw-   0        0        0      602 2023-05-23 08:11:47.000000 tKot-0.3.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 08:12:40.236608 tKot-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      311 2023-02-27 12:07:32.000000 tKot-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:12:40.180285 tKot-0.3.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 08:12:40.194315 tKot-0.3.5/src/tKot/
+-rw-rw-rw-   0        0        0       60 2023-02-28 12:42:47.000000 tKot-0.3.5/src/tKot/__init__.py
+-rw-rw-rw-   0        0        0     2827 2023-05-23 07:38:30.000000 tKot-0.3.5/src/tKot/buttons.py
+-rw-rw-rw-   0        0        0      666 2023-05-23 08:11:47.000000 tKot-0.3.5/src/tKot/common.py
+-rw-rw-rw-   0        0        0     2972 2023-05-03 11:19:55.000000 tKot-0.3.5/src/tKot/frames.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:12:40.232607 tKot-0.3.5/src/tKot.egg-info/
+-rw-rw-rw-   0        0        0      483 2023-05-23 08:12:40.000000 tKot-0.3.5/src/tKot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-05-23 08:12:40.000000 tKot-0.3.5/src/tKot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 08:12:40.000000 tKot-0.3.5/src/tKot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-23 08:12:40.000000 tKot-0.3.5/src/tKot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-23 08:12:40.000000 tKot-0.3.5/src/tKot.egg-info/top_level.txt
```

### Comparing `tKot-0.3.4/pyproject.toml` & `tKot-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backed = "setuptools.build_meta"
 
 [project]
 name = "tKot"
-version = "0.3.4"
+version = "0.3.5"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `tKot-0.3.4/src/tKot/buttons.py` & `tKot-0.3.5/src/tKot/buttons.py`

 * *Files identical despite different names*

### Comparing `tKot-0.3.4/src/tKot/common.py` & `tKot-0.3.5/src/tKot/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,12 +17,10 @@
 
     def __str__(self):
         return F'<{self.x},{self.y}>'
 
     def __mul__(self, other: int | float) -> Self:
         """:return Point with scaler x and y by other value"""
         if isinstance(other, (int, float)):
-            self.x = int(self.x*other)
-            self.y = int(self.y*other)
-            return self
+            return Point(int(self.x*other), int(self.y*other))
         else:
             ValueError(F"got unsupport type: {other}, expected int or float")
```

### Comparing `tKot-0.3.4/src/tKot/frames.py` & `tKot-0.3.5/src/tKot/frames.py`

 * *Files identical despite different names*

