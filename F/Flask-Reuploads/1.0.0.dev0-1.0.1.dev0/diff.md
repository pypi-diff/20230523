# Comparing `tmp/Flask-Reuploads-1.0.0.dev0.tar.gz` & `tmp/Flask-Reuploads-1.0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Reuploads-1.0.0.dev0.tar", last modified: Tue May 23 16:40:39 2023, max compression
+gzip compressed data, was "Flask-Reuploads-1.0.1.dev0.tar", last modified: Tue May 23 18:26:29 2023, max compression
```

## Comparing `Flask-Reuploads-1.0.0.dev0.tar` & `Flask-Reuploads-1.0.1.dev0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 16:40:39.989909 Flask-Reuploads-1.0.0.dev0/
--rw-rw-rw-   0        0        0      855 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.0.dev0/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      155 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.0.dev0/.readthedocs.yaml
--rw-rw-rw-   0        0        0     3822 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.0.dev0/CHANGES.rst
--rw-rw-rw-   0        0        0     1090 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.0.dev0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1071 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.0.dev0/LICENSE
--rw-rw-rw-   0        0        0      470 2023-05-23 15:32:28.000000 Flask-Reuploads-1.0.0.dev0/MANIFEST.in
--rw-rw-rw-   0        0        0     1718 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.0.dev0/PACKAGING.rst
--rw-rw-rw-   0        0        0    12067 2023-05-23 16:40:39.988903 Flask-Reuploads-1.0.0.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     6412 2023-05-23 16:24:09.000000 Flask-Reuploads-1.0.0.dev0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-23 16:40:39.897358 Flask-Reuploads-1.0.0.dev0/docs/
--rw-rw-rw-   0        0        0      761 2023-05-23 16:35:17.000000 Flask-Reuploads-1.0.0.dev0/docs/api.rst
--rw-rw-rw-   0        0        0       28 2023-05-23 14:18:04.000000 Flask-Reuploads-1.0.0.dev0/docs/changes.rst
--rw-rw-rw-   0        0        0     2136 2023-05-23 16:38:42.000000 Flask-Reuploads-1.0.0.dev0/docs/conf.py
--rw-rw-rw-   0        0        0     5382 2023-05-23 14:18:04.000000 Flask-Reuploads-1.0.0.dev0/docs/configuration.rst
--rw-rw-rw-   0        0        0       33 2023-05-23 14:18:04.000000 Flask-Reuploads-1.0.0.dev0/docs/contributing.rst
--rw-rw-rw-   0        0        0    10415 2023-05-23 14:18:04.000000 Flask-Reuploads-1.0.0.dev0/docs/explanation.rst
--rw-rw-rw-   0        0        0     1495 2023-05-23 16:38:38.000000 Flask-Reuploads-1.0.0.dev0/docs/getting_started.rst
--rw-rw-rw-   0        0        0     1290 2023-05-23 16:38:58.000000 Flask-Reuploads-1.0.0.dev0/docs/index.rst
--rw-rw-rw-   0        0        0     1465 2023-05-23 16:39:22.000000 Flask-Reuploads-1.0.0.dev0/docs/installation.rst
--rw-rw-rw-   0        0        0      268 2023-05-23 14:18:04.000000 Flask-Reuploads-1.0.0.dev0/docs/minimal_app.rst
--rw-rw-rw-   0        0        0      106 2023-05-23 14:18:04.000000 Flask-Reuploads-1.0.0.dev0/docs/requirements.in
--rw-rw-rw-   0        0        0     1515 2023-05-23 14:18:04.000000 Flask-Reuploads-1.0.0.dev0/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-23 16:40:39.900359 Flask-Reuploads-1.0.0.dev0/examples/
--rw-rw-rw-   0        0        0      473 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.0.dev0/examples/example.rst
-drwxrwxrwx   0        0        0        0 2023-05-23 16:40:39.902355 Flask-Reuploads-1.0.0.dev0/examples/example1/
--rw-rw-rw-   0        0        0     1350 2023-05-23 15:42:13.000000 Flask-Reuploads-1.0.0.dev0/examples/example1/app.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:40:39.907381 Flask-Reuploads-1.0.0.dev0/examples/example1/templates/
--rw-rw-rw-   0        0        0      205 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.0.dev0/examples/example1/templates/upload.html
-drwxrwxrwx   0        0        0        0 2023-05-23 16:40:39.911379 Flask-Reuploads-1.0.0.dev0/examples/example2/
--rw-rw-rw-   0        0        0     1534 2023-05-23 15:42:13.000000 Flask-Reuploads-1.0.0.dev0/examples/example2/app.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:40:39.916378 Flask-Reuploads-1.0.0.dev0/examples/example2/templates/
--rw-rw-rw-   0        0        0      205 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.0.dev0/examples/example2/templates/upload.html
--rw-rw-rw-   0        0        0       98 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.0.dev0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 16:40:39.990904 Flask-Reuploads-1.0.0.dev0/setup.cfg
--rw-rw-rw-   0        0        0     2455 2023-05-23 16:32:53.000000 Flask-Reuploads-1.0.0.dev0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:40:39.731572 Flask-Reuploads-1.0.0.dev0/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 16:40:39.960899 Flask-Reuploads-1.0.0.dev0/src/Flask_Reuploads.egg-info/
--rw-rw-rw-   0        0        0    12067 2023-05-23 16:40:39.000000 Flask-Reuploads-1.0.0.dev0/src/Flask_Reuploads.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1064 2023-05-23 16:40:39.000000 Flask-Reuploads-1.0.0.dev0/src/Flask_Reuploads.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 16:40:39.000000 Flask-Reuploads-1.0.0.dev0/src/Flask_Reuploads.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-23 16:40:39.000000 Flask-Reuploads-1.0.0.dev0/src/Flask_Reuploads.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       39 2023-05-23 16:40:39.000000 Flask-Reuploads-1.0.0.dev0/src/Flask_Reuploads.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-23 16:40:39.000000 Flask-Reuploads-1.0.0.dev0/src/Flask_Reuploads.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-23 16:40:39.977901 Flask-Reuploads-1.0.0.dev0/src/flask_reuploads/
--rw-rw-rw-   0        0        0     1346 2023-05-23 15:37:37.000000 Flask-Reuploads-1.0.0.dev0/src/flask_reuploads/__init__.py
--rw-rw-rw-   0        0        0      201 2023-05-23 14:11:19.000000 Flask-Reuploads-1.0.0.dev0/src/flask_reuploads/exceptions.py
--rw-rw-rw-   0        0        0     4231 2023-05-23 14:11:19.000000 Flask-Reuploads-1.0.0.dev0/src/flask_reuploads/extensions.py
--rw-rw-rw-   0        0        0    14290 2023-05-23 15:20:23.000000 Flask-Reuploads-1.0.0.dev0/src/flask_reuploads/flask_reuploads.py
--rw-rw-rw-   0        0        0        0 2023-05-23 14:11:19.000000 Flask-Reuploads-1.0.0.dev0/src/flask_reuploads/py.typed
--rw-rw-rw-   0        0        0     2504 2023-05-23 15:36:01.000000 Flask-Reuploads-1.0.0.dev0/src/flask_reuploads/test_helper.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:40:39.983903 Flask-Reuploads-1.0.0.dev0/tests/
--rw-rw-rw-   0        0        0        0 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.0.dev0/tests/__init__.py
--rw-rw-rw-   0        0        0     5328 2023-05-23 15:42:13.000000 Flask-Reuploads-1.0.0.dev0/tests/test_autoserve.py
--rw-rw-rw-   0        0        0    14890 2023-05-23 15:26:06.000000 Flask-Reuploads-1.0.0.dev0/tests/test_flask_reuploads.py
--rw-rw-rw-   0        0        0     1548 2023-05-23 15:40:01.000000 Flask-Reuploads-1.0.0.dev0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-05-23 18:26:29.872044 Flask-Reuploads-1.0.1.dev0/
+-rw-rw-rw-   0        0        0      855 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.1.dev0/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0      155 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.1.dev0/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     3822 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.1.dev0/CHANGES.rst
+-rw-rw-rw-   0        0        0     1090 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.1.dev0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1071 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.1.dev0/LICENSE
+-rw-rw-rw-   0        0        0      470 2023-05-23 15:32:28.000000 Flask-Reuploads-1.0.1.dev0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1718 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.1.dev0/PACKAGING.rst
+-rw-rw-rw-   0        0        0    12106 2023-05-23 18:26:29.870043 Flask-Reuploads-1.0.1.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     6412 2023-05-23 16:24:09.000000 Flask-Reuploads-1.0.1.dev0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-23 18:26:29.782037 Flask-Reuploads-1.0.1.dev0/docs/
+-rw-rw-rw-   0        0        0      761 2023-05-23 16:35:17.000000 Flask-Reuploads-1.0.1.dev0/docs/api.rst
+-rw-rw-rw-   0        0        0       28 2023-05-23 14:18:04.000000 Flask-Reuploads-1.0.1.dev0/docs/changes.rst
+-rw-rw-rw-   0        0        0     2136 2023-05-23 16:38:42.000000 Flask-Reuploads-1.0.1.dev0/docs/conf.py
+-rw-rw-rw-   0        0        0     5382 2023-05-23 14:18:04.000000 Flask-Reuploads-1.0.1.dev0/docs/configuration.rst
+-rw-rw-rw-   0        0        0       33 2023-05-23 14:18:04.000000 Flask-Reuploads-1.0.1.dev0/docs/contributing.rst
+-rw-rw-rw-   0        0        0    10415 2023-05-23 14:18:04.000000 Flask-Reuploads-1.0.1.dev0/docs/explanation.rst
+-rw-rw-rw-   0        0        0     1495 2023-05-23 16:38:38.000000 Flask-Reuploads-1.0.1.dev0/docs/getting_started.rst
+-rw-rw-rw-   0        0        0     1290 2023-05-23 16:38:58.000000 Flask-Reuploads-1.0.1.dev0/docs/index.rst
+-rw-rw-rw-   0        0        0     1465 2023-05-23 16:39:22.000000 Flask-Reuploads-1.0.1.dev0/docs/installation.rst
+-rw-rw-rw-   0        0        0      268 2023-05-23 14:18:04.000000 Flask-Reuploads-1.0.1.dev0/docs/minimal_app.rst
+-rw-rw-rw-   0        0        0      106 2023-05-23 14:18:04.000000 Flask-Reuploads-1.0.1.dev0/docs/requirements.in
+-rw-rw-rw-   0        0        0     1515 2023-05-23 14:18:04.000000 Flask-Reuploads-1.0.1.dev0/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 18:26:29.785044 Flask-Reuploads-1.0.1.dev0/examples/
+-rw-rw-rw-   0        0        0      473 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.1.dev0/examples/example.rst
+drwxrwxrwx   0        0        0        0 2023-05-23 18:26:29.788039 Flask-Reuploads-1.0.1.dev0/examples/example1/
+-rw-rw-rw-   0        0        0     1350 2023-05-23 15:42:13.000000 Flask-Reuploads-1.0.1.dev0/examples/example1/app.py
+drwxrwxrwx   0        0        0        0 2023-05-23 18:26:29.791042 Flask-Reuploads-1.0.1.dev0/examples/example1/templates/
+-rw-rw-rw-   0        0        0      205 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.1.dev0/examples/example1/templates/upload.html
+drwxrwxrwx   0        0        0        0 2023-05-23 18:26:29.796047 Flask-Reuploads-1.0.1.dev0/examples/example2/
+-rw-rw-rw-   0        0        0     1534 2023-05-23 15:42:13.000000 Flask-Reuploads-1.0.1.dev0/examples/example2/app.py
+drwxrwxrwx   0        0        0        0 2023-05-23 18:26:29.802038 Flask-Reuploads-1.0.1.dev0/examples/example2/templates/
+-rw-rw-rw-   0        0        0      205 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.1.dev0/examples/example2/templates/upload.html
+-rw-rw-rw-   0        0        0       98 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.1.dev0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 18:26:29.873037 Flask-Reuploads-1.0.1.dev0/setup.cfg
+-rw-rw-rw-   0        0        0     2494 2023-05-23 18:19:46.000000 Flask-Reuploads-1.0.1.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 18:26:29.702042 Flask-Reuploads-1.0.1.dev0/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 18:26:29.839043 Flask-Reuploads-1.0.1.dev0/src/Flask_Reuploads.egg-info/
+-rw-rw-rw-   0        0        0    12106 2023-05-23 18:26:29.000000 Flask-Reuploads-1.0.1.dev0/src/Flask_Reuploads.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1064 2023-05-23 18:26:29.000000 Flask-Reuploads-1.0.1.dev0/src/Flask_Reuploads.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 18:26:29.000000 Flask-Reuploads-1.0.1.dev0/src/Flask_Reuploads.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-23 16:40:39.000000 Flask-Reuploads-1.0.1.dev0/src/Flask_Reuploads.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       39 2023-05-23 18:26:29.000000 Flask-Reuploads-1.0.1.dev0/src/Flask_Reuploads.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-23 18:26:29.000000 Flask-Reuploads-1.0.1.dev0/src/Flask_Reuploads.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 18:26:29.857038 Flask-Reuploads-1.0.1.dev0/src/flask_reuploads/
+-rw-rw-rw-   0        0        0     1346 2023-05-23 15:37:37.000000 Flask-Reuploads-1.0.1.dev0/src/flask_reuploads/__init__.py
+-rw-rw-rw-   0        0        0      201 2023-05-23 14:11:19.000000 Flask-Reuploads-1.0.1.dev0/src/flask_reuploads/exceptions.py
+-rw-rw-rw-   0        0        0     4231 2023-05-23 14:11:19.000000 Flask-Reuploads-1.0.1.dev0/src/flask_reuploads/extensions.py
+-rw-rw-rw-   0        0        0    14290 2023-05-23 15:20:23.000000 Flask-Reuploads-1.0.1.dev0/src/flask_reuploads/flask_reuploads.py
+-rw-rw-rw-   0        0        0        0 2023-05-23 14:11:19.000000 Flask-Reuploads-1.0.1.dev0/src/flask_reuploads/py.typed
+-rw-rw-rw-   0        0        0     2504 2023-05-23 15:36:01.000000 Flask-Reuploads-1.0.1.dev0/src/flask_reuploads/test_helper.py
+drwxrwxrwx   0        0        0        0 2023-05-23 18:26:29.866045 Flask-Reuploads-1.0.1.dev0/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-23 12:59:21.000000 Flask-Reuploads-1.0.1.dev0/tests/__init__.py
+-rw-rw-rw-   0        0        0     5328 2023-05-23 15:42:13.000000 Flask-Reuploads-1.0.1.dev0/tests/test_autoserve.py
+-rw-rw-rw-   0        0        0    14890 2023-05-23 15:26:06.000000 Flask-Reuploads-1.0.1.dev0/tests/test_flask_reuploads.py
+-rw-rw-rw-   0        0        0     1548 2023-05-23 15:40:01.000000 Flask-Reuploads-1.0.1.dev0/tox.ini
```

### Comparing `Flask-Reuploads-1.0.0.dev0/.pre-commit-config.yaml` & `Flask-Reuploads-1.0.1.dev0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/CHANGES.rst` & `Flask-Reuploads-1.0.1.dev0/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/CONTRIBUTING.rst` & `Flask-Reuploads-1.0.1.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/LICENSE` & `Flask-Reuploads-1.0.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/PACKAGING.rst` & `Flask-Reuploads-1.0.1.dev0/PACKAGING.rst`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/PKG-INFO` & `Flask-Reuploads-1.0.1.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: Flask-Reuploads
-Version: 1.0.0.dev0
+Version: 1.0.1.dev0
 Summary: Flexible and efficient upload handling for Flask
 Home-page: https://github.com/picklu/flask-reuploads
 Author: Matthew "LeafStorm" Frazier
 Author-email: leafstormrush@gmail.com
-Maintainer: Jürgen Gmach
-Maintainer-email: juergen.gmach@googlemail.com
+Maintainer: Jürgen Gmach, Subrata Sarker
+Maintainer-email: juergen.gmach@googlemail.com, picklumithu@yahoo.com
 License: MIT
 Project-URL: Source, https://github.com/picklu/flask-reuploads
 Project-URL: Issue Tracker, https://github.com/jugmac00/flask-reuploaded/issues
 Project-URL: Documentation, https://flask-reuploaded.readthedocs.io/en/latest/
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `Flask-Reuploads-1.0.0.dev0/README.rst` & `Flask-Reuploads-1.0.1.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/docs/api.rst` & `Flask-Reuploads-1.0.1.dev0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/docs/conf.py` & `Flask-Reuploads-1.0.1.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/docs/configuration.rst` & `Flask-Reuploads-1.0.1.dev0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/docs/explanation.rst` & `Flask-Reuploads-1.0.1.dev0/docs/explanation.rst`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/docs/getting_started.rst` & `Flask-Reuploads-1.0.1.dev0/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/docs/index.rst` & `Flask-Reuploads-1.0.1.dev0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/docs/installation.rst` & `Flask-Reuploads-1.0.1.dev0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/docs/requirements.txt` & `Flask-Reuploads-1.0.1.dev0/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/examples/example1/app.py` & `Flask-Reuploads-1.0.1.dev0/examples/example1/app.py`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/examples/example2/app.py` & `Flask-Reuploads-1.0.1.dev0/examples/example2/app.py`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/setup.py` & `Flask-Reuploads-1.0.1.dev0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,26 +26,26 @@
         return f.read()
 
 
 LONG = read("README.rst") + "\n\n" + read("CHANGES.rst")
 
 setup(
     name="Flask-Reuploads",
-    version="1.0.0.dev0",
+    version="1.0.1.dev0",
     url="https://github.com/picklu/flask-reuploads",
     project_urls={
         "Source": "https://github.com/picklu/flask-reuploads",
         "Issue Tracker": "https://github.com/jugmac00/flask-reuploaded/issues",
         "Documentation": "https://flask-reuploaded.readthedocs.io/en/latest/",
     },
     license="MIT",
     author='Matthew "LeafStorm" Frazier',
     author_email="leafstormrush@gmail.com",
-    maintainer="Jürgen Gmach",
-    maintainer_email="juergen.gmach@googlemail.com",
+    maintainer="Jürgen Gmach, Subrata Sarker",
+    maintainer_email="juergen.gmach@googlemail.com, picklumithu@yahoo.com",
     description="Flexible and efficient upload handling for Flask",
     long_description=LONG,
     long_description_content_type="text/x-rst",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     zip_safe=False,
     platforms="any",
```

### Comparing `Flask-Reuploads-1.0.0.dev0/src/Flask_Reuploads.egg-info/PKG-INFO` & `Flask-Reuploads-1.0.1.dev0/src/Flask_Reuploads.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: Flask-Reuploads
-Version: 1.0.0.dev0
+Version: 1.0.1.dev0
 Summary: Flexible and efficient upload handling for Flask
 Home-page: https://github.com/picklu/flask-reuploads
 Author: Matthew "LeafStorm" Frazier
 Author-email: leafstormrush@gmail.com
-Maintainer: Jürgen Gmach
-Maintainer-email: juergen.gmach@googlemail.com
+Maintainer: Jürgen Gmach, Subrata Sarker
+Maintainer-email: juergen.gmach@googlemail.com, picklumithu@yahoo.com
 License: MIT
 Project-URL: Source, https://github.com/picklu/flask-reuploads
 Project-URL: Issue Tracker, https://github.com/jugmac00/flask-reuploaded/issues
 Project-URL: Documentation, https://flask-reuploaded.readthedocs.io/en/latest/
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `Flask-Reuploads-1.0.0.dev0/src/Flask_Reuploads.egg-info/SOURCES.txt` & `Flask-Reuploads-1.0.1.dev0/src/Flask_Reuploads.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/src/flask_reuploads/__init__.py` & `Flask-Reuploads-1.0.1.dev0/src/flask_reuploads/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/src/flask_reuploads/extensions.py` & `Flask-Reuploads-1.0.1.dev0/src/flask_reuploads/extensions.py`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/src/flask_reuploads/flask_reuploads.py` & `Flask-Reuploads-1.0.1.dev0/src/flask_reuploads/flask_reuploads.py`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/src/flask_reuploads/test_helper.py` & `Flask-Reuploads-1.0.1.dev0/src/flask_reuploads/test_helper.py`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/tests/test_autoserve.py` & `Flask-Reuploads-1.0.1.dev0/tests/test_autoserve.py`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/tests/test_flask_reuploads.py` & `Flask-Reuploads-1.0.1.dev0/tests/test_flask_reuploads.py`

 * *Files identical despite different names*

### Comparing `Flask-Reuploads-1.0.0.dev0/tox.ini` & `Flask-Reuploads-1.0.1.dev0/tox.ini`

 * *Files identical despite different names*

