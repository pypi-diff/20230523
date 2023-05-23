# Comparing `tmp/perprof-web-0.0.1.tar.gz` & `tmp/perprof-web-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perprof-web-0.0.1.tar", last modified: Sun May  7 10:18:18 2023, max compression
+gzip compressed data, was "perprof-web-0.0.2.tar", last modified: Tue May 23 20:38:03 2023, max compression
```

## Comparing `perprof-web-0.0.1.tar` & `perprof-web-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxr-xr-x   0 abel      (1000) abel      (1000)        0 2023-05-07 10:18:18.207328 perprof-web-0.0.1/
--rw-r--r--   0 abel      (1000) abel      (1000)    35278 2023-04-10 08:57:06.000000 perprof-web-0.0.1/LICENSE.md
--rw-r--r--   0 abel      (1000) abel      (1000)     2046 2023-05-07 10:18:18.207328 perprof-web-0.0.1/PKG-INFO
--rw-r--r--   0 abel      (1000) abel      (1000)     1498 2023-05-07 09:52:44.000000 perprof-web-0.0.1/README.md
-drwxr-xr-x   0 abel      (1000) abel      (1000)        0 2023-05-07 10:18:18.207328 perprof-web-0.0.1/perprof_web.egg-info/
--rw-r--r--   0 abel      (1000) abel      (1000)     2046 2023-05-07 10:18:18.000000 perprof-web-0.0.1/perprof_web.egg-info/PKG-INFO
--rw-r--r--   0 abel      (1000) abel      (1000)      209 2023-05-07 10:18:18.000000 perprof-web-0.0.1/perprof_web.egg-info/SOURCES.txt
--rw-r--r--   0 abel      (1000) abel      (1000)        1 2023-05-07 10:18:18.000000 perprof-web-0.0.1/perprof_web.egg-info/dependency_links.txt
--rw-r--r--   0 abel      (1000) abel      (1000)      200 2023-05-07 10:18:18.000000 perprof-web-0.0.1/perprof_web.egg-info/requires.txt
--rw-r--r--   0 abel      (1000) abel      (1000)        1 2023-05-07 10:18:18.000000 perprof-web-0.0.1/perprof_web.egg-info/top_level.txt
--rw-r--r--   0 abel      (1000) abel      (1000)     1191 2023-04-11 18:51:03.000000 perprof-web-0.0.1/pyproject.toml
--rw-r--r--   0 abel      (1000) abel      (1000)       38 2023-05-07 10:18:18.207328 perprof-web-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:38:03.114534 perprof-web-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35278 2023-05-23 20:37:20.000000 perprof-web-0.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-23 20:38:03.114534 perprof-web-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-23 20:37:20.000000 perprof-web-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:38:03.114534 perprof-web-0.0.2/perprof_web/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-23 20:37:20.000000 perprof-web-0.0.2/perprof_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-23 20:37:20.000000 perprof-web-0.0.2/perprof_web/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-23 20:37:20.000000 perprof-web-0.0.2/perprof_web/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:38:03.114534 perprof-web-0.0.2/perprof_web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-23 20:38:03.000000 perprof-web-0.0.2/perprof_web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-23 20:38:03.000000 perprof-web-0.0.2/perprof_web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:38:03.000000 perprof-web-0.0.2/perprof_web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-23 20:38:03.000000 perprof-web-0.0.2/perprof_web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 20:38:03.000000 perprof-web-0.0.2/perprof_web.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-23 20:37:20.000000 perprof-web-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 20:38:03.114534 perprof-web-0.0.2/setup.cfg
```

### Comparing `perprof-web-0.0.1/LICENSE.md` & `perprof-web-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `perprof-web-0.0.1/PKG-INFO` & `perprof-web-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perprof-web
-Version: 0.0.1
+Version: 0.0.2
 Summary: Web interface for perprof-py
 Author-email: Abel Soares Siqueira <abel.s.siqueira@gmail.com>
 Project-URL: repository, https://github.com/abelsiqueira/perprof-web
 Project-URL: documentation, https://abelsiqueira.com/perprof-web/
 Keywords: benchmark,comparison,performance profile,flask
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
@@ -31,16 +31,20 @@
 When using this software for publications, please cite the paper below, which
 describes this project:
 
 > Siqueira, A. S., Costa da Silva, R. G. and Santos, L.-R., (2016). Perprof-web: A Python Package for Performance Profile of Mathematical Optimization Software. Journal of Open Research Software. 4(1), p.e12. DOI: [10.5334/jors.81](http://doi.org/10.5334/jors.81).
 
 ## Install
 
-TODO: Add installation information for the end-user.
+Use `perprof-web` from Docker if you just want to use it.
 
 ## How to use
 
-TODO: Add a simple way to run for the end-user.
+Run perprof-web using Docker with
+
+```bash
+docker run -p 5000:5000 abelsiqueira/perprof-web
+```
 
 ## Getting Help
 
 If you didn't find something at the documentation, want to report a bug, or request a new feature, please open an [issue](https://github.com/abelsiqueira/perprof-web/issues).
```

### Comparing `perprof-web-0.0.1/README.md` & `perprof-web-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -15,16 +15,20 @@
 When using this software for publications, please cite the paper below, which
 describes this project:
 
 > Siqueira, A. S., Costa da Silva, R. G. and Santos, L.-R., (2016). Perprof-web: A Python Package for Performance Profile of Mathematical Optimization Software. Journal of Open Research Software. 4(1), p.e12. DOI: [10.5334/jors.81](http://doi.org/10.5334/jors.81).
 
 ## Install
 
-TODO: Add installation information for the end-user.
+Use `perprof-web` from Docker if you just want to use it.
 
 ## How to use
 
-TODO: Add a simple way to run for the end-user.
+Run perprof-web using Docker with
+
+```bash
+docker run -p 5000:5000 abelsiqueira/perprof-web
+```
 
 ## Getting Help
 
 If you didn't find something at the documentation, want to report a bug, or request a new feature, please open an [issue](https://github.com/abelsiqueira/perprof-web/issues).
```

### Comparing `perprof-web-0.0.1/perprof_web.egg-info/PKG-INFO` & `perprof-web-0.0.2/perprof_web.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perprof-web
-Version: 0.0.1
+Version: 0.0.2
 Summary: Web interface for perprof-py
 Author-email: Abel Soares Siqueira <abel.s.siqueira@gmail.com>
 Project-URL: repository, https://github.com/abelsiqueira/perprof-web
 Project-URL: documentation, https://abelsiqueira.com/perprof-web/
 Keywords: benchmark,comparison,performance profile,flask
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
@@ -31,16 +31,20 @@
 When using this software for publications, please cite the paper below, which
 describes this project:
 
 > Siqueira, A. S., Costa da Silva, R. G. and Santos, L.-R., (2016). Perprof-web: A Python Package for Performance Profile of Mathematical Optimization Software. Journal of Open Research Software. 4(1), p.e12. DOI: [10.5334/jors.81](http://doi.org/10.5334/jors.81).
 
 ## Install
 
-TODO: Add installation information for the end-user.
+Use `perprof-web` from Docker if you just want to use it.
 
 ## How to use
 
-TODO: Add a simple way to run for the end-user.
+Run perprof-web using Docker with
+
+```bash
+docker run -p 5000:5000 abelsiqueira/perprof-web
+```
 
 ## Getting Help
 
 If you didn't find something at the documentation, want to report a bug, or request a new feature, please open an [issue](https://github.com/abelsiqueira/perprof-web/issues).
```

### Comparing `perprof-web-0.0.1/pyproject.toml` & `perprof-web-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -16,21 +16,21 @@
   "Programming Language :: Python"
 ]
 dependencies = [
   "flask>=2,<3",
   "perprof-py>=1.1.4,<2",
   "matplotlib>=3,<4",
 ]
-version = "0.0.1"
+version = "0.0.2"
 
 [project.optional-dependencies]
 dev = [
   "black",
   "pre-commit",
-  "prospector[with_pyroma]",
+  "ruff",
   "pylint",
   "pytest",
   "pytest-cov",
 ]
 publishing = [
   "twine"
 ]
```

