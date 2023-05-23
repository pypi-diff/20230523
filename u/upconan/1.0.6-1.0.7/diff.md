# Comparing `tmp/upconan-1.0.6.tar.gz` & `tmp/upconan-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upconan-1.0.6.tar", last modified: Tue May 23 11:46:26 2023, max compression
+gzip compressed data, was "upconan-1.0.7.tar", last modified: Tue May 23 11:48:50 2023, max compression
```

## Comparing `upconan-1.0.6.tar` & `upconan-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 11:46:26.043022 upconan-1.0.6/
--rw-rw-rw-   0        0        0     1062 2023-05-19 13:12:37.000000 upconan-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      490 2023-05-23 11:46:26.042021 upconan-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-05-19 13:13:20.000000 upconan-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-23 11:46:26.043022 upconan-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      886 2023-05-23 11:45:59.000000 upconan-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 11:46:26.029021 upconan-1.0.6/src/
--rw-rw-rw-   0        0        0        0 2023-04-18 02:21:11.000000 upconan-1.0.6/src/__init__.py
--rw-rw-rw-   0        0        0     4799 2023-05-23 06:33:57.000000 upconan-1.0.6/src/upconan.py
-drwxrwxrwx   0        0        0        0 2023-05-23 11:46:26.042021 upconan-1.0.6/upconan.egg-info/
--rw-rw-rw-   0        0        0      490 2023-05-23 11:46:25.000000 upconan-1.0.6/upconan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-05-23 11:46:25.000000 upconan-1.0.6/upconan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 11:46:25.000000 upconan-1.0.6/upconan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-05-23 11:46:25.000000 upconan-1.0.6/upconan.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-23 11:46:25.000000 upconan-1.0.6/upconan.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2023-05-23 11:46:25.000000 upconan-1.0.6/upconan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-23 11:46:25.000000 upconan-1.0.6/upconan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 11:48:50.190582 upconan-1.0.7/
+-rw-rw-rw-   0        0        0     1062 2023-05-19 13:12:37.000000 upconan-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      490 2023-05-23 11:48:50.190582 upconan-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-05-19 13:13:20.000000 upconan-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 11:48:50.190582 upconan-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      895 2023-05-23 11:48:35.000000 upconan-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:48:50.182677 upconan-1.0.7/src/
+-rw-rw-rw-   0        0        0        0 2023-04-18 02:21:11.000000 upconan-1.0.7/src/__init__.py
+-rw-rw-rw-   0        0        0     4799 2023-05-23 06:33:57.000000 upconan-1.0.7/src/upconan.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:48:50.189582 upconan-1.0.7/upconan.egg-info/
+-rw-rw-rw-   0        0        0      490 2023-05-23 11:48:50.000000 upconan-1.0.7/upconan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-05-23 11:48:50.000000 upconan-1.0.7/upconan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 11:48:50.000000 upconan-1.0.7/upconan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-05-23 11:48:50.000000 upconan-1.0.7/upconan.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-23 11:48:50.000000 upconan-1.0.7/upconan.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2023-05-23 11:48:50.000000 upconan-1.0.7/upconan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-23 11:48:50.000000 upconan-1.0.7/upconan.egg-info/top_level.txt
```

### Comparing `upconan-1.0.6/LICENSE` & `upconan-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `upconan-1.0.6/setup.py` & `upconan-1.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name='upconan',
-    version="1.0.6",
+    version="1.0.7",
     description="一个更新conanfile的便捷工具",
     long_description="""从剪贴板复制conan包信息，更新当前路径下的conanfile.py或conanfile.txt文件中对应的conan包版本""",
     long_description_content_type='text/x-rst',
     keywords='python conan',
     author='leytou',
     author_email='hi_litao@163.com',
     url='https://github.com/leytou/upconan',
@@ -20,10 +20,10 @@
     install_requires=['GitPython','pyperclip'],
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
     entry_points={'console_scripts': [
         'upconan = src.upconan:main',
-        'upco = upconan'
+        'upco = src.upconan:main'
     ]},
 )
```

### Comparing `upconan-1.0.6/src/upconan.py` & `upconan-1.0.7/src/upconan.py`

 * *Files identical despite different names*

