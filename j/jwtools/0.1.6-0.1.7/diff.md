# Comparing `tmp/jwtools-0.1.6.tar.gz` & `tmp/jwtools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwtools-0.1.6.tar", last modified: Mon May 22 05:30:25 2023, max compression
+gzip compressed data, was "jwtools-0.1.7.tar", last modified: Tue May 23 06:30:47 2023, max compression
```

## Comparing `jwtools-0.1.6.tar` & `jwtools-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 05:30:25.662289 jwtools-0.1.6/
--rw-rw-rw-   0        0        0     1164 2023-05-17 09:27:51.000000 jwtools-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     1324 2023-05-22 05:30:25.661289 jwtools-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      771 2023-05-18 02:30:45.000000 jwtools-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 05:30:25.654283 jwtools-0.1.6/jwtools/
--rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 jwtools-0.1.6/jwtools/__init__.py
--rw-rw-rw-   0        0        0      142 2023-05-19 10:02:42.000000 jwtools-0.1.6/jwtools/dt.py
--rw-rw-rw-   0        0        0     1568 2023-05-22 05:29:30.000000 jwtools-0.1.6/jwtools/func.py
-drwxrwxrwx   0        0        0        0 2023-05-22 05:30:25.658285 jwtools-0.1.6/jwtools.egg-info/
--rw-rw-rw-   0        0        0     1324 2023-05-22 05:30:25.000000 jwtools-0.1.6/jwtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-22 05:30:25.000000 jwtools-0.1.6/jwtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 05:30:25.000000 jwtools-0.1.6/jwtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-22 05:30:25.000000 jwtools-0.1.6/jwtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 05:30:25.662289 jwtools-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-05-22 05:29:30.000000 jwtools-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 05:30:25.660291 jwtools-0.1.6/tests/
--rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 jwtools-0.1.6/tests/__init__.py
--rw-rw-rw-   0        0        0      209 2023-05-18 03:36:21.000000 jwtools-0.1.6/tests/test1.py
+drwxrwxrwx   0        0        0        0 2023-05-23 06:30:47.132418 jwtools-0.1.7/
+-rw-rw-rw-   0        0        0     1164 2023-05-17 09:27:51.000000 jwtools-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     1324 2023-05-23 06:30:47.131417 jwtools-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      771 2023-05-18 02:30:45.000000 jwtools-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 06:30:47.118419 jwtools-0.1.7/jwtools/
+-rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 jwtools-0.1.7/jwtools/__init__.py
+-rw-rw-rw-   0        0        0      142 2023-05-19 10:02:42.000000 jwtools-0.1.7/jwtools/dt.py
+-rw-rw-rw-   0        0        0     2963 2023-05-23 04:39:47.000000 jwtools-0.1.7/jwtools/func.py
+drwxrwxrwx   0        0        0        0 2023-05-23 06:30:47.123416 jwtools-0.1.7/jwtools/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 jwtools-0.1.7/jwtools/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 06:30:47.124416 jwtools-0.1.7/jwtools/tests/feature/
+-rw-rw-rw-   0        0        0        0 2023-05-23 04:43:26.000000 jwtools-0.1.7/jwtools/tests/feature/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 06:30:47.127420 jwtools-0.1.7/jwtools/tests/script/
+-rw-rw-rw-   0        0        0        0 2023-05-23 06:26:31.000000 jwtools-0.1.7/jwtools/tests/script/__init__.py
+-rw-rw-rw-   0        0        0      209 2023-05-18 03:36:21.000000 jwtools-0.1.7/jwtools/tests/script/test1.py
+-rw-rw-rw-   0        0        0      747 2023-05-23 04:42:50.000000 jwtools-0.1.7/jwtools/tests/script/test2.py
+-rw-rw-rw-   0        0        0      183 2023-05-22 03:25:04.000000 jwtools-0.1.7/jwtools/tests/test_base.py
+drwxrwxrwx   0        0        0        0 2023-05-23 06:30:47.130418 jwtools-0.1.7/jwtools/tests/unit/
+-rw-rw-rw-   0        0        0        0 2023-05-23 04:43:33.000000 jwtools-0.1.7/jwtools/tests/unit/__init__.py
+-rw-rw-rw-   0        0        0     1480 2023-05-23 06:24:25.000000 jwtools-0.1.7/jwtools/tests/unit/func_test.py
+drwxrwxrwx   0        0        0        0 2023-05-23 06:30:47.121417 jwtools-0.1.7/jwtools.egg-info/
+-rw-rw-rw-   0        0        0     1324 2023-05-23 06:30:46.000000 jwtools-0.1.7/jwtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2023-05-23 06:30:47.000000 jwtools-0.1.7/jwtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 06:30:46.000000 jwtools-0.1.7/jwtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-23 06:30:46.000000 jwtools-0.1.7/jwtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 06:30:47.132418 jwtools-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-05-23 06:30:31.000000 jwtools-0.1.7/setup.py
```

### Comparing `jwtools-0.1.6/LICENSE` & `jwtools-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jwtools-0.1.6/PKG-INFO` & `jwtools-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwtools
-Version: 0.1.6
+Version: 0.1.7
 Summary: It is a micro-toolbox that includes various common operations and will continue to be improved in the future.
 Home-page: https://github.com/jinghewang/python-jwtools.git
 Author: jinghewang
 Author-email: jinghewang@163.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jwtools-0.1.6/README.md` & `jwtools-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `jwtools-0.1.6/jwtools.egg-info/PKG-INFO` & `jwtools-0.1.7/jwtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwtools
-Version: 0.1.6
+Version: 0.1.7
 Summary: It is a micro-toolbox that includes various common operations and will continue to be improved in the future.
 Home-page: https://github.com/jinghewang/python-jwtools.git
 Author: jinghewang
 Author-email: jinghewang@163.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jwtools-0.1.6/setup.py` & `jwtools-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jwtools',
-    version='0.1.6',
+    version='0.1.7',
     description="It is a micro-toolbox that includes various common operations and will continue to be improved in the future.",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     include_package_data=True,
     author='jinghewang',
     author_email='jinghewang@163.com',
     license='MIT License',
```

