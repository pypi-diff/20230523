# Comparing `tmp/pyflame-0.3.0.tar.gz` & `tmp/pyflame-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflame-0.3.0.tar", last modified: Mon May 23 18:02:46 2022, max compression
+gzip compressed data, was "pyflame-0.3.1.tar", last modified: Tue May 23 13:10:14 2023, max compression
```

## Comparing `pyflame-0.3.0.tar` & `pyflame-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2022-05-23 18:02:46.796986 pyflame-0.3.0/
--rw-r--r--   0 dharding  (1000) dharding  (1000)       33 2021-05-19 13:20:43.000000 pyflame-0.3.0/.gitignore
--rw-r--r--   0 dharding  (1000) dharding  (1000)      495 2022-05-23 18:00:37.000000 pyflame-0.3.0/CHANGELOG.rst
--rw-r--r--   0 dharding  (1000) dharding  (1000)     1059 2022-02-17 13:57:58.000000 pyflame-0.3.0/LICENSE
--rw-r--r--   0 dharding  (1000) dharding  (1000)       43 2021-12-02 18:05:59.000000 pyflame-0.3.0/MANIFEST.in
--rw-r--r--   0 dharding  (1000) dharding  (1000)     5897 2022-05-23 18:02:46.796986 pyflame-0.3.0/PKG-INFO
--rw-r--r--   0 dharding  (1000) dharding  (1000)     4975 2022-02-17 13:57:58.000000 pyflame-0.3.0/README.rst
-drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2022-05-23 18:02:46.793653 pyflame-0.3.0/pyflame/
--rw-r--r--   0 dharding  (1000) dharding  (1000)      169 2022-02-17 13:57:58.000000 pyflame-0.3.0/pyflame/__init__.py
--rw-r--r--   0 dharding  (1000) dharding  (1000)      158 2022-02-17 13:57:58.000000 pyflame-0.3.0/pyflame/__main__.py
-drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2022-05-23 18:02:46.796986 pyflame-0.3.0/pyflame/djdt/
--rw-r--r--   0 dharding  (1000) dharding  (1000)        0 2021-05-19 13:20:43.000000 pyflame-0.3.0/pyflame/djdt/__init__.py
--rw-r--r--   0 dharding  (1000) dharding  (1000)     1376 2022-02-17 13:57:58.000000 pyflame-0.3.0/pyflame/djdt/panel.py
--rw-r--r--   0 dharding  (1000) dharding  (1000)      421 2022-02-17 13:57:58.000000 pyflame-0.3.0/pyflame/djdt/settings.py
--rw-r--r--   0 dharding  (1000) dharding  (1000)      170 2022-02-17 13:57:58.000000 pyflame-0.3.0/pyflame/exceptions.py
--rw-r--r--   0 dharding  (1000) dharding  (1000)     3255 2022-02-20 12:55:14.000000 pyflame-0.3.0/pyflame/ipython.py
--rw-r--r--   0 dharding  (1000) dharding  (1000)     1865 2022-02-20 12:58:37.000000 pyflame-0.3.0/pyflame/render.py
--rw-r--r--   0 dharding  (1000) dharding  (1000)     3110 2022-02-21 09:43:00.000000 pyflame-0.3.0/pyflame/runner.py
--rw-r--r--   0 dharding  (1000) dharding  (1000)     1370 2022-02-17 13:57:58.000000 pyflame-0.3.0/pyflame/sampler.py
--rw-r--r--   0 dharding  (1000) dharding  (1000)      733 2022-02-17 13:57:58.000000 pyflame-0.3.0/pyflame/stack.py
-drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2022-05-23 18:02:46.793653 pyflame-0.3.0/pyflame/templates/
-drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2022-05-23 18:02:46.796986 pyflame-0.3.0/pyflame/templates/pyflame/
--rw-r--r--   0 dharding  (1000) dharding  (1000)      883 2022-02-20 13:22:15.000000 pyflame-0.3.0/pyflame/templates/pyflame/panel.html
-drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2022-05-23 18:02:46.796986 pyflame-0.3.0/pyflame.egg-info/
--rw-rw-r--   0 dharding  (1000) dharding  (1000)     5897 2022-05-23 18:02:46.000000 pyflame-0.3.0/pyflame.egg-info/PKG-INFO
--rw-rw-r--   0 dharding  (1000) dharding  (1000)      535 2022-05-23 18:02:46.000000 pyflame-0.3.0/pyflame.egg-info/SOURCES.txt
--rw-rw-r--   0 dharding  (1000) dharding  (1000)        1 2022-05-23 18:02:46.000000 pyflame-0.3.0/pyflame.egg-info/dependency_links.txt
--rw-rw-r--   0 dharding  (1000) dharding  (1000)        1 2021-05-16 13:26:47.000000 pyflame-0.3.0/pyflame.egg-info/not-zip-safe
--rw-r--r--   0 dharding  (1000) dharding  (1000)       75 2022-05-23 18:02:46.000000 pyflame-0.3.0/pyflame.egg-info/requires.txt
--rw-rw-r--   0 dharding  (1000) dharding  (1000)        8 2022-05-23 18:02:46.000000 pyflame-0.3.0/pyflame.egg-info/top_level.txt
--rw-r--r--   0 dharding  (1000) dharding  (1000)      105 2021-05-19 13:20:43.000000 pyflame-0.3.0/pyproject.toml
--rw-r--r--   0 dharding  (1000) dharding  (1000)      984 2022-05-23 18:02:46.796986 pyflame-0.3.0/setup.cfg
--rwxr-xr-x   0 dharding  (1000) dharding  (1000)       62 2022-05-23 17:36:57.000000 pyflame-0.3.0/setup.py
+drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2023-05-23 13:10:14.130819 pyflame-0.3.1/
+-rw-r--r--   0 dharding  (1000) dharding  (1000)       33 2021-05-19 13:20:43.000000 pyflame-0.3.1/.gitignore
+-rw-r--r--   0 dharding  (1000) dharding  (1000)      635 2023-05-23 13:08:33.000000 pyflame-0.3.1/CHANGELOG.rst
+-rw-r--r--   0 dharding  (1000) dharding  (1000)     1059 2022-02-17 13:57:58.000000 pyflame-0.3.1/LICENSE
+-rw-r--r--   0 dharding  (1000) dharding  (1000)       43 2021-12-02 18:05:59.000000 pyflame-0.3.1/MANIFEST.in
+-rw-r--r--   0 dharding  (1000) dharding  (1000)     5947 2023-05-23 13:10:14.130819 pyflame-0.3.1/PKG-INFO
+-rw-r--r--   0 dharding  (1000) dharding  (1000)     5025 2023-05-23 11:42:38.000000 pyflame-0.3.1/README.rst
+drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2023-05-23 13:10:14.127485 pyflame-0.3.1/pyflame/
+-rw-r--r--   0 dharding  (1000) dharding  (1000)      207 2023-05-23 13:08:33.000000 pyflame-0.3.1/pyflame/__init__.py
+-rw-r--r--   0 dharding  (1000) dharding  (1000)      158 2022-02-17 13:57:58.000000 pyflame-0.3.1/pyflame/__main__.py
+drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2023-05-23 13:10:14.127485 pyflame-0.3.1/pyflame/djdt/
+-rw-r--r--   0 dharding  (1000) dharding  (1000)        0 2021-05-19 13:20:43.000000 pyflame-0.3.1/pyflame/djdt/__init__.py
+-rw-r--r--   0 dharding  (1000) dharding  (1000)     1376 2022-02-17 13:57:58.000000 pyflame-0.3.1/pyflame/djdt/panel.py
+-rw-r--r--   0 dharding  (1000) dharding  (1000)      421 2022-02-17 13:57:58.000000 pyflame-0.3.1/pyflame/djdt/settings.py
+-rw-r--r--   0 dharding  (1000) dharding  (1000)      170 2022-02-17 13:57:58.000000 pyflame-0.3.1/pyflame/exceptions.py
+-rw-r--r--   0 dharding  (1000) dharding  (1000)     3255 2022-02-20 12:55:14.000000 pyflame-0.3.1/pyflame/ipython.py
+-rw-r--r--   0 dharding  (1000) dharding  (1000)     1865 2022-02-20 12:58:37.000000 pyflame-0.3.1/pyflame/render.py
+-rw-r--r--   0 dharding  (1000) dharding  (1000)     3110 2022-02-21 09:43:00.000000 pyflame-0.3.1/pyflame/runner.py
+-rw-r--r--   0 dharding  (1000) dharding  (1000)     1370 2022-02-17 13:57:58.000000 pyflame-0.3.1/pyflame/sampler.py
+-rw-r--r--   0 dharding  (1000) dharding  (1000)      733 2022-02-17 13:57:58.000000 pyflame-0.3.1/pyflame/stack.py
+drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2023-05-23 13:10:14.124152 pyflame-0.3.1/pyflame/templates/
+drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2023-05-23 13:10:14.127485 pyflame-0.3.1/pyflame/templates/pyflame/
+-rw-r--r--   0 dharding  (1000) dharding  (1000)      883 2022-02-20 13:22:15.000000 pyflame-0.3.1/pyflame/templates/pyflame/panel.html
+drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2023-05-23 13:10:14.127485 pyflame-0.3.1/pyflame.egg-info/
+-rw-rw-r--   0 dharding  (1000) dharding  (1000)     5947 2023-05-23 13:10:14.000000 pyflame-0.3.1/pyflame.egg-info/PKG-INFO
+-rw-rw-r--   0 dharding  (1000) dharding  (1000)      535 2023-05-23 13:10:14.000000 pyflame-0.3.1/pyflame.egg-info/SOURCES.txt
+-rw-rw-r--   0 dharding  (1000) dharding  (1000)        1 2023-05-23 13:10:14.000000 pyflame-0.3.1/pyflame.egg-info/dependency_links.txt
+-rw-rw-r--   0 dharding  (1000) dharding  (1000)        1 2021-05-16 13:26:47.000000 pyflame-0.3.1/pyflame.egg-info/not-zip-safe
+-rw-r--r--   0 dharding  (1000) dharding  (1000)       75 2023-05-23 13:10:14.000000 pyflame-0.3.1/pyflame.egg-info/requires.txt
+-rw-rw-r--   0 dharding  (1000) dharding  (1000)        8 2023-05-23 13:10:14.000000 pyflame-0.3.1/pyflame.egg-info/top_level.txt
+-rw-r--r--   0 dharding  (1000) dharding  (1000)      105 2021-05-19 13:20:43.000000 pyflame-0.3.1/pyproject.toml
+-rw-r--r--   0 dharding  (1000) dharding  (1000)      984 2023-05-23 13:10:14.130819 pyflame-0.3.1/setup.cfg
+-rwxr-xr-x   0 dharding  (1000) dharding  (1000)       62 2023-05-23 11:34:03.000000 pyflame-0.3.1/setup.py
```

### Comparing `pyflame-0.3.0/LICENSE` & `pyflame-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflame-0.3.0/PKG-INFO` & `pyflame-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflame
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Flamegraph generator for Python
 Home-page: https://gitlab.com/living180/pyflame
 Author: Daniel Harding
 Author-email: dharding@living180.net
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Django
@@ -63,15 +63,16 @@
 * ``-o path``, ``--output-file path``: the location to save the flamegraph. If not
   specified, save in the current directory using the name of the Python script with an
   ``.svg`` extension appended.
 
 Django Debug Toolbar Configuration
 ----------------------------------
 
-To enable, add ``pyflame.djdt.panel.FlamegraphPanel`` to ``DEBUG_TOOLBAR_PANELS`` in the
+To enable, add ``pyflame`` to ``INSTALLED_APPS`` and
+``pyflame.djdt.panel.FlamegraphPanel`` to ``DEBUG_TOOLBAR_PANELS`` in the
 project's Django settings module.
 
 pyflame uses a similar configuration mechanism to that of Django Debug Toolbar.  To
 modify the default configuration, add a ``PYFLAME_CONFIG`` setting to the project's
 Django settings module. This must be a dictionary which may contain any of the following
 options:
 
@@ -149,12 +150,12 @@
 it).  The approach of spawning a separate thread to sample stack traces using
 ``sys._current_frames()`` was drawn from Evan Hempel's python-flamegraph_ project.
 
 .. _FlameGraph: https://github.com/brendangregg/FlameGraph
 .. _Django Debug Toolbar: https://github.com/jazzband/django-debug-toolbar
 .. _IPython: https://ipython.readthedocs.io/en/stable/overview.html
 .. _Jupyter Notebook: https://jupyter-notebook.readthedocs.io/en/stable/
-.. _flamegraph.pl: https://github.com/brendangregg/FlameGraph/flamegraph.pl
+.. _flamegraph.pl: https://github.com/brendangregg/FlameGraph/blob/master/flamegraph.pl
 .. _MIT license: https://opensource.org/licenses/MIT
 .. _LICENSE: https://gitlab.com/living180/pyflame/-/blob/main/LICENSE
 .. _djdt-flamegraph: https://github.com/23andMe/djdt-flamegraph
 .. _python-flamegraph: https://github.com/evanhempel/python-flamegraph
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_jw8ayris_/tmppazeq904_TarContainer/0/5", line 161, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_jw8ayris_/tmppazeq904_TarContainer/0/5", line 161, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyflame Version: 0.3.0 Summary: A Flamegraph
+Metadata-Version: 2.1 Name: pyflame Version: 0.3.1 Summary: A Flamegraph
 generator for Python Home-page: https://gitlab.com/living180/pyflame Author:
 Daniel Harding Author-email: dharding@living180.net Classifier: Development
 Status :: 4 - Beta Classifier: Environment :: Console Classifier: Framework ::
 Django Classifier: Framework :: Jupyter Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `pyflame-0.3.0/README.rst` & `pyflame-0.3.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,16 @@
 * ``-o path``, ``--output-file path``: the location to save the flamegraph. If not
   specified, save in the current directory using the name of the Python script with an
   ``.svg`` extension appended.
 
 Django Debug Toolbar Configuration
 ----------------------------------
 
-To enable, add ``pyflame.djdt.panel.FlamegraphPanel`` to ``DEBUG_TOOLBAR_PANELS`` in the
+To enable, add ``pyflame`` to ``INSTALLED_APPS`` and
+``pyflame.djdt.panel.FlamegraphPanel`` to ``DEBUG_TOOLBAR_PANELS`` in the
 project's Django settings module.
 
 pyflame uses a similar configuration mechanism to that of Django Debug Toolbar.  To
 modify the default configuration, add a ``PYFLAME_CONFIG`` setting to the project's
 Django settings module. This must be a dictionary which may contain any of the following
 options:
 
@@ -123,12 +124,12 @@
 it).  The approach of spawning a separate thread to sample stack traces using
 ``sys._current_frames()`` was drawn from Evan Hempel's python-flamegraph_ project.
 
 .. _FlameGraph: https://github.com/brendangregg/FlameGraph
 .. _Django Debug Toolbar: https://github.com/jazzband/django-debug-toolbar
 .. _IPython: https://ipython.readthedocs.io/en/stable/overview.html
 .. _Jupyter Notebook: https://jupyter-notebook.readthedocs.io/en/stable/
-.. _flamegraph.pl: https://github.com/brendangregg/FlameGraph/flamegraph.pl
+.. _flamegraph.pl: https://github.com/brendangregg/FlameGraph/blob/master/flamegraph.pl
 .. _MIT license: https://opensource.org/licenses/MIT
 .. _LICENSE: https://gitlab.com/living180/pyflame/-/blob/main/LICENSE
 .. _djdt-flamegraph: https://github.com/23andMe/djdt-flamegraph
 .. _python-flamegraph: https://github.com/evanhempel/python-flamegraph
```

### Comparing `pyflame-0.3.0/pyflame/djdt/panel.py` & `pyflame-0.3.1/pyflame/djdt/panel.py`

 * *Files identical despite different names*

### Comparing `pyflame-0.3.0/pyflame/ipython.py` & `pyflame-0.3.1/pyflame/ipython.py`

 * *Files identical despite different names*

### Comparing `pyflame-0.3.0/pyflame/render.py` & `pyflame-0.3.1/pyflame/render.py`

 * *Files identical despite different names*

### Comparing `pyflame-0.3.0/pyflame/runner.py` & `pyflame-0.3.1/pyflame/runner.py`

 * *Files identical despite different names*

### Comparing `pyflame-0.3.0/pyflame/sampler.py` & `pyflame-0.3.1/pyflame/sampler.py`

 * *Files identical despite different names*

### Comparing `pyflame-0.3.0/pyflame/stack.py` & `pyflame-0.3.1/pyflame/stack.py`

 * *Files identical despite different names*

### Comparing `pyflame-0.3.0/pyflame/templates/pyflame/panel.html` & `pyflame-0.3.1/pyflame/templates/pyflame/panel.html`

 * *Files identical despite different names*

### Comparing `pyflame-0.3.0/pyflame.egg-info/PKG-INFO` & `pyflame-0.3.1/pyflame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflame
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Flamegraph generator for Python
 Home-page: https://gitlab.com/living180/pyflame
 Author: Daniel Harding
 Author-email: dharding@living180.net
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Django
@@ -63,15 +63,16 @@
 * ``-o path``, ``--output-file path``: the location to save the flamegraph. If not
   specified, save in the current directory using the name of the Python script with an
   ``.svg`` extension appended.
 
 Django Debug Toolbar Configuration
 ----------------------------------
 
-To enable, add ``pyflame.djdt.panel.FlamegraphPanel`` to ``DEBUG_TOOLBAR_PANELS`` in the
+To enable, add ``pyflame`` to ``INSTALLED_APPS`` and
+``pyflame.djdt.panel.FlamegraphPanel`` to ``DEBUG_TOOLBAR_PANELS`` in the
 project's Django settings module.
 
 pyflame uses a similar configuration mechanism to that of Django Debug Toolbar.  To
 modify the default configuration, add a ``PYFLAME_CONFIG`` setting to the project's
 Django settings module. This must be a dictionary which may contain any of the following
 options:
 
@@ -149,12 +150,12 @@
 it).  The approach of spawning a separate thread to sample stack traces using
 ``sys._current_frames()`` was drawn from Evan Hempel's python-flamegraph_ project.
 
 .. _FlameGraph: https://github.com/brendangregg/FlameGraph
 .. _Django Debug Toolbar: https://github.com/jazzband/django-debug-toolbar
 .. _IPython: https://ipython.readthedocs.io/en/stable/overview.html
 .. _Jupyter Notebook: https://jupyter-notebook.readthedocs.io/en/stable/
-.. _flamegraph.pl: https://github.com/brendangregg/FlameGraph/flamegraph.pl
+.. _flamegraph.pl: https://github.com/brendangregg/FlameGraph/blob/master/flamegraph.pl
 .. _MIT license: https://opensource.org/licenses/MIT
 .. _LICENSE: https://gitlab.com/living180/pyflame/-/blob/main/LICENSE
 .. _djdt-flamegraph: https://github.com/23andMe/djdt-flamegraph
 .. _python-flamegraph: https://github.com/evanhempel/python-flamegraph
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_jw8ayris_/tmppazeq904_TarContainer/0/24", line 161, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_jw8ayris_/tmppazeq904_TarContainer/0/24", line 161, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyflame Version: 0.3.0 Summary: A Flamegraph
+Metadata-Version: 2.1 Name: pyflame Version: 0.3.1 Summary: A Flamegraph
 generator for Python Home-page: https://gitlab.com/living180/pyflame Author:
 Daniel Harding Author-email: dharding@living180.net Classifier: Development
 Status :: 4 - Beta Classifier: Environment :: Console Classifier: Framework ::
 Django Classifier: Framework :: Jupyter Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `pyflame-0.3.0/pyflame.egg-info/SOURCES.txt` & `pyflame-0.3.1/pyflame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyflame-0.3.0/setup.cfg` & `pyflame-0.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyflame
-version = 0.3.0
+version = 0.3.1
 url = https://gitlab.com/living180/pyflame
 author = Daniel Harding
 author_email = dharding@living180.net
 description = A Flamegraph generator for Python
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 classifiers =
```

