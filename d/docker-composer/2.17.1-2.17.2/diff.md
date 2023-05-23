# Comparing `tmp/docker_composer-2.17.1.tar.gz` & `tmp/docker_composer-2.17.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_composer-2.17.1.tar", max compression
+gzip compressed data, was "docker_composer-2.17.2.tar", max compression
```

## Comparing `docker_composer-2.17.1.tar` & `docker_composer-2.17.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11358 2023-05-22 17:40:30.205463 docker_composer-2.17.1/LICENSE.txt
--rw-r--r--   0        0        0     1978 2023-05-22 17:40:30.205594 docker_composer-2.17.1/README.md
--rw-r--r--   0        0        0     1358 2023-05-23 01:33:53.042705 docker_composer-2.17.1/pyproject.toml
--rw-r--r--   0        0        0       60 2023-05-22 19:40:35.299994 docker_composer-2.17.1/src/docker_composer/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 17:40:30.206343 docker_composer-2.17.1/src/docker_composer/_utils/__init__.py
--rw-r--r--   0        0        0     4557 2023-05-22 20:35:25.788589 docker_composer-2.17.1/src/docker_composer/_utils/argument.py
--rw-r--r--   0        0        0     7241 2023-05-22 20:35:25.789294 docker_composer-2.17.1/src/docker_composer/_utils/generate_class.py
--rw-r--r--   0        0        0     3238 2023-05-22 17:40:30.206770 docker_composer-2.17.1/src/docker_composer/base.py
--rw-r--r--   0        0        0        0 2023-05-22 17:40:30.206821 docker_composer-2.17.1/src/docker_composer/py.typed
--rw-r--r--   0        0        0        0 2023-05-22 17:40:30.206931 docker_composer-2.17.1/src/docker_composer/runner/__init__.py
--rw-r--r--   0        0        0     1227 2023-05-22 20:35:25.790242 docker_composer-2.17.1/src/docker_composer/runner/cmd/build.py
--rw-r--r--   0        0        0     1811 2023-05-22 20:35:25.790760 docker_composer-2.17.1/src/docker_composer/runner/cmd/config.py
--rw-r--r--   0        0        0      937 2023-05-22 20:35:25.791110 docker_composer-2.17.1/src/docker_composer/runner/cmd/cp.py
--rw-r--r--   0        0        0     1414 2023-05-22 20:35:25.791824 docker_composer-2.17.1/src/docker_composer/runner/cmd/create.py
--rw-r--r--   0        0        0     1029 2023-05-22 20:35:25.792441 docker_composer-2.17.1/src/docker_composer/runner/cmd/down.py
--rw-r--r--   0        0        0      608 2023-05-22 20:35:25.792940 docker_composer-2.17.1/src/docker_composer/runner/cmd/events.py
--rw-r--r--   0        0        0     1234 2023-05-22 20:35:25.793552 docker_composer-2.17.1/src/docker_composer/runner/cmd/exec.py
--rw-r--r--   0        0        0      690 2023-05-22 20:35:25.794073 docker_composer-2.17.1/src/docker_composer/runner/cmd/images.py
--rw-r--r--   0        0        0      729 2023-05-22 20:35:25.794481 docker_composer-2.17.1/src/docker_composer/runner/cmd/kill.py
--rw-r--r--   0        0        0     1250 2023-05-22 20:35:25.795147 docker_composer-2.17.1/src/docker_composer/runner/cmd/logs.py
--rw-r--r--   0        0        0      830 2023-05-22 20:35:25.795508 docker_composer-2.17.1/src/docker_composer/runner/cmd/ls.py
--rw-r--r--   0        0        0      463 2023-05-22 20:35:25.795972 docker_composer-2.17.1/src/docker_composer/runner/cmd/pause.py
--rw-r--r--   0        0        0      687 2023-05-22 20:35:25.796437 docker_composer-2.17.1/src/docker_composer/runner/cmd/port.py
--rw-r--r--   0        0        0     1112 2023-05-22 20:35:25.797054 docker_composer-2.17.1/src/docker_composer/runner/cmd/ps.py
--rw-r--r--   0        0        0      964 2023-05-22 20:35:25.797590 docker_composer-2.17.1/src/docker_composer/runner/cmd/pull.py
--rw-r--r--   0        0        0      856 2023-05-22 20:35:25.798080 docker_composer-2.17.1/src/docker_composer/runner/cmd/push.py
--rw-r--r--   0        0        0      689 2023-05-22 20:35:25.798685 docker_composer-2.17.1/src/docker_composer/runner/cmd/restart.py
--rw-r--r--   0        0        0     1012 2023-05-22 20:35:25.799207 docker_composer-2.17.1/src/docker_composer/runner/cmd/rm.py
--rw-r--r--   0        0        0     2329 2023-05-22 20:35:25.799746 docker_composer-2.17.1/src/docker_composer/runner/cmd/run.py
--rw-r--r--   0        0        0      463 2023-05-22 20:35:25.800293 docker_composer-2.17.1/src/docker_composer/runner/cmd/start.py
--rw-r--r--   0        0        0      564 2023-05-22 20:35:25.800735 docker_composer-2.17.1/src/docker_composer/runner/cmd/stop.py
--rw-r--r--   0        0        0      473 2023-05-22 20:35:25.801329 docker_composer-2.17.1/src/docker_composer/runner/cmd/top.py
--rw-r--r--   0        0        0      471 2023-05-22 20:35:25.801939 docker_composer-2.17.1/src/docker_composer/runner/cmd/unpause.py
--rw-r--r--   0        0        0     3410 2023-05-22 20:35:25.802415 docker_composer-2.17.1/src/docker_composer/runner/cmd/up.py
--rw-r--r--   0        0        0      702 2023-05-22 20:35:25.802883 docker_composer-2.17.1/src/docker_composer/runner/cmd/version.py
--rw-r--r--   0        0        0    27397 2023-05-22 20:35:25.803600 docker_composer-2.17.1/src/docker_composer/runner/root.py
--rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 docker_composer-2.17.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-22 17:40:30.205463 docker_composer-2.17.2/LICENSE.txt
+-rw-r--r--   0        0        0     1978 2023-05-22 17:40:30.205594 docker_composer-2.17.2/README.md
+-rw-r--r--   0        0        0     1369 2023-05-23 04:08:51.031016 docker_composer-2.17.2/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-05-22 19:40:35.299994 docker_composer-2.17.2/src/docker_composer/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 17:40:30.206343 docker_composer-2.17.2/src/docker_composer/_utils/__init__.py
+-rw-r--r--   0        0        0     4557 2023-05-22 20:35:25.788589 docker_composer-2.17.2/src/docker_composer/_utils/argument.py
+-rw-r--r--   0        0        0     7241 2023-05-22 20:35:25.789294 docker_composer-2.17.2/src/docker_composer/_utils/generate_class.py
+-rw-r--r--   0        0        0     3238 2023-05-22 17:40:30.206770 docker_composer-2.17.2/src/docker_composer/base.py
+-rw-r--r--   0        0        0        0 2023-05-22 17:40:30.206821 docker_composer-2.17.2/src/docker_composer/py.typed
+-rw-r--r--   0        0        0        0 2023-05-22 17:40:30.206931 docker_composer-2.17.2/src/docker_composer/runner/__init__.py
+-rw-r--r--   0        0        0     1227 2023-05-22 20:35:25.790242 docker_composer-2.17.2/src/docker_composer/runner/cmd/build.py
+-rw-r--r--   0        0        0     1811 2023-05-22 20:35:25.790760 docker_composer-2.17.2/src/docker_composer/runner/cmd/config.py
+-rw-r--r--   0        0        0      937 2023-05-22 20:35:25.791110 docker_composer-2.17.2/src/docker_composer/runner/cmd/cp.py
+-rw-r--r--   0        0        0     1414 2023-05-22 20:35:25.791824 docker_composer-2.17.2/src/docker_composer/runner/cmd/create.py
+-rw-r--r--   0        0        0     1029 2023-05-22 20:35:25.792441 docker_composer-2.17.2/src/docker_composer/runner/cmd/down.py
+-rw-r--r--   0        0        0      608 2023-05-22 20:35:25.792940 docker_composer-2.17.2/src/docker_composer/runner/cmd/events.py
+-rw-r--r--   0        0        0     1234 2023-05-22 20:35:25.793552 docker_composer-2.17.2/src/docker_composer/runner/cmd/exec.py
+-rw-r--r--   0        0        0      690 2023-05-22 20:35:25.794073 docker_composer-2.17.2/src/docker_composer/runner/cmd/images.py
+-rw-r--r--   0        0        0      729 2023-05-22 20:35:25.794481 docker_composer-2.17.2/src/docker_composer/runner/cmd/kill.py
+-rw-r--r--   0        0        0     1250 2023-05-22 20:35:25.795147 docker_composer-2.17.2/src/docker_composer/runner/cmd/logs.py
+-rw-r--r--   0        0        0      830 2023-05-22 20:35:25.795508 docker_composer-2.17.2/src/docker_composer/runner/cmd/ls.py
+-rw-r--r--   0        0        0      463 2023-05-22 20:35:25.795972 docker_composer-2.17.2/src/docker_composer/runner/cmd/pause.py
+-rw-r--r--   0        0        0      687 2023-05-22 20:35:25.796437 docker_composer-2.17.2/src/docker_composer/runner/cmd/port.py
+-rw-r--r--   0        0        0     1112 2023-05-22 20:35:25.797054 docker_composer-2.17.2/src/docker_composer/runner/cmd/ps.py
+-rw-r--r--   0        0        0      964 2023-05-22 20:35:25.797590 docker_composer-2.17.2/src/docker_composer/runner/cmd/pull.py
+-rw-r--r--   0        0        0      856 2023-05-22 20:35:25.798080 docker_composer-2.17.2/src/docker_composer/runner/cmd/push.py
+-rw-r--r--   0        0        0      689 2023-05-22 20:35:25.798685 docker_composer-2.17.2/src/docker_composer/runner/cmd/restart.py
+-rw-r--r--   0        0        0     1012 2023-05-22 20:35:25.799207 docker_composer-2.17.2/src/docker_composer/runner/cmd/rm.py
+-rw-r--r--   0        0        0     2329 2023-05-22 20:35:25.799746 docker_composer-2.17.2/src/docker_composer/runner/cmd/run.py
+-rw-r--r--   0        0        0      463 2023-05-22 20:35:25.800293 docker_composer-2.17.2/src/docker_composer/runner/cmd/start.py
+-rw-r--r--   0        0        0      564 2023-05-22 20:35:25.800735 docker_composer-2.17.2/src/docker_composer/runner/cmd/stop.py
+-rw-r--r--   0        0        0      473 2023-05-22 20:35:25.801329 docker_composer-2.17.2/src/docker_composer/runner/cmd/top.py
+-rw-r--r--   0        0        0      471 2023-05-22 20:35:25.801939 docker_composer-2.17.2/src/docker_composer/runner/cmd/unpause.py
+-rw-r--r--   0        0        0     3410 2023-05-22 20:35:25.802415 docker_composer-2.17.2/src/docker_composer/runner/cmd/up.py
+-rw-r--r--   0        0        0      702 2023-05-22 20:35:25.802883 docker_composer-2.17.2/src/docker_composer/runner/cmd/version.py
+-rw-r--r--   0        0        0    27397 2023-05-22 20:35:25.803600 docker_composer-2.17.2/src/docker_composer/runner/root.py
+-rw-r--r--   0        0        0     3060 1970-01-01 00:00:00.000000 docker_composer-2.17.2/PKG-INFO
```

### Comparing `docker_composer-2.17.1/LICENSE.txt` & `docker_composer-2.17.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/README.md` & `docker_composer-2.17.2/README.md`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/pyproject.toml` & `docker_composer-2.17.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docker-composer"
-version = "2.17.1"
+version = "2.17.2"
 description = "Use docker-compose from within Python"
 authors = ["Micha <schollm-git@gmx.com>"]
 readme = "README.md"
 homepage = "https://github.com/schollm/docker-composer"
 repository = "https://github.com/schollm/docker-composer"
 license = "Apache-2.0"
 packages = [
@@ -14,20 +14,20 @@
   "Intended Audience :: Developers",
   "Intended Audience :: System Administrators",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3",
   "Topic :: Software Development :: Build Tools",
   "Topic :: Software Development :: Libraries :: Application Frameworks",
   "Operating System :: OS Independent",
-  "Development Status :: 4 - Beta"
+  "Development Status :: 5 - Production/Stable"
 ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<4.0"
+python = ">=3.9,<4.0"
 attrs = ">=20.3.0"
 loguru = ">=0.5.3"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^6.0.0"
 pytest = ">=6.1.2"
 black = ">=20.8b1"
```

### Comparing `docker_composer-2.17.1/src/docker_composer/_utils/argument.py` & `docker_composer-2.17.2/src/docker_composer/_utils/argument.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/_utils/generate_class.py` & `docker_composer-2.17.2/src/docker_composer/_utils/generate_class.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/base.py` & `docker_composer-2.17.2/src/docker_composer/base.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/cmd/build.py` & `docker_composer-2.17.2/src/docker_composer/runner/cmd/build.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/cmd/config.py` & `docker_composer-2.17.2/src/docker_composer/runner/cmd/config.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/cmd/cp.py` & `docker_composer-2.17.2/src/docker_composer/runner/cmd/cp.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/cmd/create.py` & `docker_composer-2.17.2/src/docker_composer/runner/cmd/create.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/cmd/down.py` & `docker_composer-2.17.2/src/docker_composer/runner/cmd/down.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/cmd/events.py` & `docker_composer-2.17.2/src/docker_composer/runner/cmd/events.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/cmd/exec.py` & `docker_composer-2.17.2/src/docker_composer/runner/cmd/exec.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/cmd/images.py` & `docker_composer-2.17.2/src/docker_composer/runner/cmd/images.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/cmd/kill.py` & `docker_composer-2.17.2/src/docker_composer/runner/cmd/kill.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/cmd/logs.py` & `docker_composer-2.17.2/src/docker_composer/runner/cmd/logs.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/cmd/ls.py` & `docker_composer-2.17.2/src/docker_composer/runner/cmd/ls.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/cmd/port.py` & `docker_composer-2.17.2/src/docker_composer/runner/cmd/port.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/cmd/ps.py` & `docker_composer-2.17.2/src/docker_composer/runner/cmd/ps.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/cmd/pull.py` & `docker_composer-2.17.2/src/docker_composer/runner/cmd/pull.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/cmd/push.py` & `docker_composer-2.17.2/src/docker_composer/runner/cmd/push.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/cmd/restart.py` & `docker_composer-2.17.2/src/docker_composer/runner/cmd/restart.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/cmd/rm.py` & `docker_composer-2.17.2/src/docker_composer/runner/cmd/rm.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/cmd/run.py` & `docker_composer-2.17.2/src/docker_composer/runner/cmd/run.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/cmd/stop.py` & `docker_composer-2.17.2/src/docker_composer/runner/cmd/stop.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/cmd/up.py` & `docker_composer-2.17.2/src/docker_composer/runner/cmd/up.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/cmd/version.py` & `docker_composer-2.17.2/src/docker_composer/runner/cmd/version.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/src/docker_composer/runner/root.py` & `docker_composer-2.17.2/src/docker_composer/runner/root.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.1/PKG-INFO` & `docker_composer-2.17.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: docker-composer
-Version: 2.17.1
+Version: 2.17.2
 Summary: Use docker-compose from within Python
 Home-page: https://github.com/schollm/docker-composer
 License: Apache-2.0
 Author: Micha
 Author-email: schollm-git@gmx.com
-Requires-Python: >=3.8.1,<4.0
-Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

