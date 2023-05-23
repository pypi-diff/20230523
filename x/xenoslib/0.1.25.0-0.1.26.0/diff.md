# Comparing `tmp/xenoslib-0.1.25.0.tar.gz` & `tmp/xenoslib-0.1.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenoslib-0.1.25.0.tar", last modified: Thu Mar 30 05:13:28 2023, max compression
+gzip compressed data, was "xenoslib-0.1.26.0.tar", last modified: Tue May 23 02:51:19 2023, max compression
```

## Comparing `xenoslib-0.1.25.0.tar` & `xenoslib-0.1.26.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:13:28.429117 xenoslib-0.1.25.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-30 05:13:16.000000 xenoslib-0.1.25.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-30 05:13:28.429117 xenoslib-0.1.25.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-03-30 05:13:16.000000 xenoslib-0.1.25.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 05:13:28.429117 xenoslib-0.1.25.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-03-30 05:13:16.000000 xenoslib-0.1.25.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:13:28.429117 xenoslib-0.1.25.0/xenoslib/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-30 05:13:16.000000 xenoslib-0.1.25.0/xenoslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-30 05:13:16.000000 xenoslib-0.1.25.0/xenoslib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-30 05:13:16.000000 xenoslib-0.1.25.0/xenoslib/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-03-30 05:13:16.000000 xenoslib-0.1.25.0/xenoslib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-03-30 05:13:16.000000 xenoslib-0.1.25.0/xenoslib/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-03-30 05:13:16.000000 xenoslib-0.1.25.0/xenoslib/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-03-30 05:13:16.000000 xenoslib-0.1.25.0/xenoslib/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-03-30 05:13:16.000000 xenoslib-0.1.25.0/xenoslib/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-03-30 05:13:16.000000 xenoslib-0.1.25.0/xenoslib/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-03-30 05:13:16.000000 xenoslib-0.1.25.0/xenoslib/win_trayicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-03-30 05:13:16.000000 xenoslib-0.1.25.0/xenoslib/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:13:28.429117 xenoslib-0.1.25.0/xenoslib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-30 05:13:28.000000 xenoslib-0.1.25.0/xenoslib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-30 05:13:28.000000 xenoslib-0.1.25.0/xenoslib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 05:13:28.000000 xenoslib-0.1.25.0/xenoslib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-30 05:13:28.000000 xenoslib-0.1.25.0/xenoslib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-30 05:13:28.000000 xenoslib-0.1.25.0/xenoslib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:51:19.647269 xenoslib-0.1.26.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 02:51:08.000000 xenoslib-0.1.26.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-23 02:51:19.647269 xenoslib-0.1.26.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-23 02:51:08.000000 xenoslib-0.1.26.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 02:51:19.647269 xenoslib-0.1.26.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-23 02:51:08.000000 xenoslib-0.1.26.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:51:19.643269 xenoslib-0.1.26.0/xenoslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-23 02:51:08.000000 xenoslib-0.1.26.0/xenoslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-23 02:51:08.000000 xenoslib-0.1.26.0/xenoslib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-23 02:51:08.000000 xenoslib-0.1.26.0/xenoslib/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-23 02:51:08.000000 xenoslib-0.1.26.0/xenoslib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-23 02:51:08.000000 xenoslib-0.1.26.0/xenoslib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-23 02:51:08.000000 xenoslib-0.1.26.0/xenoslib/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-23 02:51:08.000000 xenoslib-0.1.26.0/xenoslib/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-23 02:51:08.000000 xenoslib-0.1.26.0/xenoslib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-23 02:51:08.000000 xenoslib-0.1.26.0/xenoslib/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-23 02:51:08.000000 xenoslib-0.1.26.0/xenoslib/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-23 02:51:08.000000 xenoslib-0.1.26.0/xenoslib/win_trayicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-23 02:51:08.000000 xenoslib-0.1.26.0/xenoslib/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:51:19.647269 xenoslib-0.1.26.0/xenoslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-23 02:51:19.000000 xenoslib-0.1.26.0/xenoslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-23 02:51:19.000000 xenoslib-0.1.26.0/xenoslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 02:51:19.000000 xenoslib-0.1.26.0/xenoslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-23 02:51:19.000000 xenoslib-0.1.26.0/xenoslib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 02:51:19.000000 xenoslib-0.1.26.0/xenoslib.egg-info/top_level.txt
```

### Comparing `xenoslib-0.1.25.0/LICENSE` & `xenoslib-0.1.26.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.25.0/README.md` & `xenoslib-0.1.26.0/README.md`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.25.0/setup.py` & `xenoslib-0.1.26.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     long_description_content_type="text/markdown",
     author=about.__author__,
     author_email=about.__author_email__,
     license=about.__license__,
     url=about.__url__,
     install_requires=[
         "PyYAML>=5.4",
+        "IMAPClient>=2.3.1",
     ],
     python_requires=">=3.7",
     extras_require={
         ':"linux" in sys_platform': [],
         ':sys_platform == "win32"': ["pywin32>=225"],
         ':python_version >= "3.10"': ["requests>=2.19"],
         ':python_version <= "3.9"': ["requests>=2.0.0"],
```

### Comparing `xenoslib-0.1.25.0/xenoslib/base.py` & `xenoslib-0.1.26.0/xenoslib/base.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.25.0/xenoslib/dev.py` & `xenoslib-0.1.26.0/xenoslib/dev.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.25.0/xenoslib/extend.py` & `xenoslib-0.1.26.0/xenoslib/extend.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.25.0/xenoslib/linux.py` & `xenoslib-0.1.26.0/xenoslib/linux.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.25.0/xenoslib/mock.py` & `xenoslib-0.1.26.0/xenoslib/mock.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.25.0/xenoslib/onedrive.py` & `xenoslib-0.1.26.0/xenoslib/onedrive.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.25.0/xenoslib/win_trayicon.py` & `xenoslib-0.1.26.0/xenoslib/win_trayicon.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.25.0/xenoslib/windows.py` & `xenoslib-0.1.26.0/xenoslib/windows.py`

 * *Files identical despite different names*

