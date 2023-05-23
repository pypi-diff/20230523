# Comparing `tmp/tKot-0.3.6.tar.gz` & `tmp/tKot-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tKot-0.3.6.tar", last modified: Tue May 23 09:23:14 2023, max compression
+gzip compressed data, was "tKot-0.3.7.tar", last modified: Tue May 23 11:04:04 2023, max compression
```

## Comparing `tKot-0.3.6.tar` & `tKot-0.3.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 09:23:14.657084 tKot-0.3.6/
--rw-rw-rw-   0        0        0      483 2023-05-23 09:23:14.656084 tKot-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0       30 2023-02-27 11:57:31.000000 tKot-0.3.6/README.md
--rw-rw-rw-   0        0        0      602 2023-05-23 09:21:19.000000 tKot-0.3.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 09:23:14.657084 tKot-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0      311 2023-02-27 12:07:32.000000 tKot-0.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:23:14.602515 tKot-0.3.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 09:23:14.615549 tKot-0.3.6/src/tKot/
--rw-rw-rw-   0        0        0       60 2023-02-28 12:42:47.000000 tKot-0.3.6/src/tKot/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-05-23 09:00:46.000000 tKot-0.3.6/src/tKot/buttons.py
--rw-rw-rw-   0        0        0      666 2023-05-23 08:11:47.000000 tKot-0.3.6/src/tKot/common.py
--rw-rw-rw-   0        0        0     2972 2023-05-03 11:19:55.000000 tKot-0.3.6/src/tKot/frames.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:23:14.654084 tKot-0.3.6/src/tKot.egg-info/
--rw-rw-rw-   0        0        0      483 2023-05-23 09:23:14.000000 tKot-0.3.6/src/tKot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-05-23 09:23:14.000000 tKot-0.3.6/src/tKot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 09:23:14.000000 tKot-0.3.6/src/tKot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-23 09:23:14.000000 tKot-0.3.6/src/tKot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-23 09:23:14.000000 tKot-0.3.6/src/tKot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 11:04:04.349532 tKot-0.3.7/
+-rw-rw-rw-   0        0        0      483 2023-05-23 11:04:04.348533 tKot-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2023-02-27 11:57:31.000000 tKot-0.3.7/README.md
+-rw-rw-rw-   0        0        0      602 2023-05-23 11:03:27.000000 tKot-0.3.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 11:04:04.349532 tKot-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      311 2023-02-27 12:07:32.000000 tKot-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:04:04.295579 tKot-0.3.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 11:04:04.308579 tKot-0.3.7/src/tKot/
+-rw-rw-rw-   0        0        0       60 2023-02-28 12:42:47.000000 tKot-0.3.7/src/tKot/__init__.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 11:03:27.000000 tKot-0.3.7/src/tKot/buttons.py
+-rw-rw-rw-   0        0        0      666 2023-05-23 08:11:47.000000 tKot-0.3.7/src/tKot/common.py
+-rw-rw-rw-   0        0        0     2972 2023-05-03 11:19:55.000000 tKot-0.3.7/src/tKot/frames.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:04:04.345567 tKot-0.3.7/src/tKot.egg-info/
+-rw-rw-rw-   0        0        0      483 2023-05-23 11:04:04.000000 tKot-0.3.7/src/tKot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-05-23 11:04:04.000000 tKot-0.3.7/src/tKot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 11:04:04.000000 tKot-0.3.7/src/tKot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-23 11:04:04.000000 tKot-0.3.7/src/tKot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-23 11:04:04.000000 tKot-0.3.7/src/tKot.egg-info/top_level.txt
```

### Comparing `tKot-0.3.6/pyproject.toml` & `tKot-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backed = "setuptools.build_meta"
 
 [project]
 name = "tKot"
-version = "0.3.6"
+version = "0.3.7"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `tKot-0.3.6/src/tKot/buttons.py` & `tKot-0.3.7/src/tKot/buttons.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,7 +81,11 @@
                                             anchor=tk.NW,
                                             image=self.__im)
 
     def delete(self):
         """delete from canvas"""
         self.__c.delete(self.__c_id)
         self.__c_id = -1
+
+    @property
+    def c_id(self) -> int:
+        return self.__c_id
```

### Comparing `tKot-0.3.6/src/tKot/common.py` & `tKot-0.3.7/src/tKot/common.py`

 * *Files identical despite different names*

### Comparing `tKot-0.3.6/src/tKot/frames.py` & `tKot-0.3.7/src/tKot/frames.py`

 * *Files identical despite different names*

