# Comparing `tmp/asgihandler-0.4.1.tar.gz` & `tmp/asgihandler-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgihandler-0.4.1.tar", last modified: Mon May 22 22:41:26 2023, max compression
+gzip compressed data, was "asgihandler-0.4.2.tar", last modified: Tue May 23 17:55:15 2023, max compression
```

## Comparing `asgihandler-0.4.1.tar` & `asgihandler-0.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 22:41:26.044002 asgihandler-0.4.1/
--rw-rw-rw-   0        0        0     1067 2022-07-16 23:50:52.000000 asgihandler-0.4.1/LICENSE
--rw-rw-rw-   0        0        0       27 2022-07-16 23:50:52.000000 asgihandler-0.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3035 2023-05-22 22:41:26.044002 asgihandler-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     2403 2022-07-16 23:50:52.000000 asgihandler-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 22:41:25.994005 asgihandler-0.4.1/asgihandler/
--rw-rw-rw-   0        0        0       21 2022-07-16 23:50:52.000000 asgihandler-0.4.1/asgihandler/__init__.py
--rw-rw-rw-   0        0        0       68 2022-07-16 23:55:07.000000 asgihandler-0.4.1/asgihandler/__version__.py
--rw-rw-rw-   0        0        0     1287 2022-08-05 19:34:25.000000 asgihandler-0.4.1/asgihandler/core.py
--rw-rw-rw-   0        0        0      424 2023-05-22 22:36:31.000000 asgihandler-0.4.1/asgihandler/userCheck.py
-drwxrwxrwx   0        0        0        0 2023-05-22 22:41:26.042001 asgihandler-0.4.1/asgihandler.egg-info/
--rw-rw-rw-   0        0        0     3035 2023-05-22 22:41:25.000000 asgihandler-0.4.1/asgihandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-05-22 22:41:25.000000 asgihandler-0.4.1/asgihandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 22:41:25.000000 asgihandler-0.4.1/asgihandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 22:41:25.000000 asgihandler-0.4.1/asgihandler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-22 22:41:25.000000 asgihandler-0.4.1/asgihandler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 22:41:26.045004 asgihandler-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     3878 2023-05-22 22:39:37.000000 asgihandler-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:55:15.441125 asgihandler-0.4.2/
+-rw-rw-rw-   0        0        0     1067 2022-07-16 23:50:52.000000 asgihandler-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0       27 2022-07-16 23:50:52.000000 asgihandler-0.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3117 2023-05-23 17:55:15.440125 asgihandler-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2483 2023-05-02 06:18:39.000000 asgihandler-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 17:55:15.426124 asgihandler-0.4.2/asgihandler/
+-rw-rw-rw-   0        0        0       21 2022-07-16 23:50:52.000000 asgihandler-0.4.2/asgihandler/__init__.py
+-rw-rw-rw-   0        0        0       68 2022-07-16 23:55:07.000000 asgihandler-0.4.2/asgihandler/__version__.py
+-rw-rw-rw-   0        0        0     1287 2022-08-05 19:34:25.000000 asgihandler-0.4.2/asgihandler/core.py
+-rw-rw-rw-   0        0        0      424 2023-05-23 17:48:05.000000 asgihandler-0.4.2/asgihandler/userCheck.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:55:15.439124 asgihandler-0.4.2/asgihandler.egg-info/
+-rw-rw-rw-   0        0        0     3117 2023-05-23 17:55:15.000000 asgihandler-0.4.2/asgihandler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-05-23 17:55:15.000000 asgihandler-0.4.2/asgihandler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 17:55:15.000000 asgihandler-0.4.2/asgihandler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 17:55:15.000000 asgihandler-0.4.2/asgihandler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-23 17:55:15.000000 asgihandler-0.4.2/asgihandler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 17:55:15.441125 asgihandler-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     3878 2023-05-23 17:54:45.000000 asgihandler-0.4.2/setup.py
```

### Comparing `asgihandler-0.4.1/LICENSE` & `asgihandler-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asgihandler-0.4.1/PKG-INFO` & `asgihandler-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: asgihandler
-Version: 0.4.1
+Version: 0.4.2
 Summary: ASGIHandler
 Home-page: https://github.com/GreaterWMS/GreaterWMS
 Author: Singosgu
 Author-email: singosgu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 📦 setup.py (for humans)
 =======================
 
@@ -78,7 +78,11 @@
   [an example setup.py]: https://github.com/navdeep-G/setup.py/blob/master/setup.py
   [PyPi]: https://docs.python.org/3/distutils/packageindex.html
   [Twine]: https://pypi.python.org/pypi/twine
   [image]: https://farm1.staticflickr.com/628/33173824932_58add34581_k_d.jpg
   [What is setup.py?]: https://stackoverflow.com/questions/1471994/what-is-setup-py
   [The Hitchhiker's Guide to Packaging]: https://the-hitchhikers-guide-to-packaging.readthedocs.io/en/latest/creation.html
   [Cookiecutter template for a Python package]: https://github.com/audreyr/cookiecutter-pypackage
+
+python setup.py sdist bdist_wheel
+
+twine upload -u coco56 -p password dist/*
```

### Comparing `asgihandler-0.4.1/README.md` & `asgihandler-0.4.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -59,7 +59,11 @@
   [an example setup.py]: https://github.com/navdeep-G/setup.py/blob/master/setup.py
   [PyPi]: https://docs.python.org/3/distutils/packageindex.html
   [Twine]: https://pypi.python.org/pypi/twine
   [image]: https://farm1.staticflickr.com/628/33173824932_58add34581_k_d.jpg
   [What is setup.py?]: https://stackoverflow.com/questions/1471994/what-is-setup-py
   [The Hitchhiker's Guide to Packaging]: https://the-hitchhikers-guide-to-packaging.readthedocs.io/en/latest/creation.html
   [Cookiecutter template for a Python package]: https://github.com/audreyr/cookiecutter-pypackage
+
+python setup.py sdist bdist_wheel
+
+twine upload -u coco56 -p password dist/*
```

### Comparing `asgihandler-0.4.1/asgihandler/core.py` & `asgihandler-0.4.2/asgihandler/core.py`

 * *Files identical despite different names*

### Comparing `asgihandler-0.4.1/asgihandler.egg-info/PKG-INFO` & `asgihandler-0.4.2/asgihandler.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: asgihandler
-Version: 0.4.1
+Version: 0.4.2
 Summary: ASGIHandler
 Home-page: https://github.com/GreaterWMS/GreaterWMS
 Author: Singosgu
 Author-email: singosgu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 📦 setup.py (for humans)
 =======================
 
@@ -78,7 +78,11 @@
   [an example setup.py]: https://github.com/navdeep-G/setup.py/blob/master/setup.py
   [PyPi]: https://docs.python.org/3/distutils/packageindex.html
   [Twine]: https://pypi.python.org/pypi/twine
   [image]: https://farm1.staticflickr.com/628/33173824932_58add34581_k_d.jpg
   [What is setup.py?]: https://stackoverflow.com/questions/1471994/what-is-setup-py
   [The Hitchhiker's Guide to Packaging]: https://the-hitchhikers-guide-to-packaging.readthedocs.io/en/latest/creation.html
   [Cookiecutter template for a Python package]: https://github.com/audreyr/cookiecutter-pypackage
+
+python setup.py sdist bdist_wheel
+
+twine upload -u coco56 -p password dist/*
```

### Comparing `asgihandler-0.4.1/setup.py` & `asgihandler-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 # Package meta-data.
 NAME = 'asgihandler'
 DESCRIPTION = 'ASGIHandler'
 URL = 'https://github.com/GreaterWMS/GreaterWMS'
 EMAIL = 'singosgu@gmail.com'
 AUTHOR = 'Singosgu'
-REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.4.1'
+REQUIRES_PYTHON = '>=3.7.0'
+VERSION = '0.4.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
 ]
 
 # What packages are optional?
@@ -116,15 +116,15 @@
     license='MIT',
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy'
     ],
     # $ setup.py publish support.
     cmdclass={
         'upload': UploadCommand,
     },
```

