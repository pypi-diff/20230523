# Comparing `tmp/docker_composer-2.17.3.tar.gz` & `tmp/docker_composer-2.17.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_composer-2.17.3.tar", max compression
+gzip compressed data, was "docker_composer-2.17.4.tar", max compression
```

## Comparing `docker_composer-2.17.3.tar` & `docker_composer-2.17.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11358 2023-05-22 17:40:30.205463 docker_composer-2.17.3/LICENSE.txt
--rw-r--r--   0        0        0     1978 2023-05-22 17:40:30.205594 docker_composer-2.17.3/README.md
--rw-r--r--   0        0        0     1369 2023-05-23 04:26:04.917641 docker_composer-2.17.3/pyproject.toml
--rw-r--r--   0        0        0       60 2023-05-22 19:40:35.299994 docker_composer-2.17.3/src/docker_composer/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 17:40:30.206343 docker_composer-2.17.3/src/docker_composer/_utils/__init__.py
--rw-r--r--   0        0        0     4557 2023-05-22 20:35:25.788589 docker_composer-2.17.3/src/docker_composer/_utils/argument.py
--rw-r--r--   0        0        0     7241 2023-05-22 20:35:25.789294 docker_composer-2.17.3/src/docker_composer/_utils/generate_class.py
--rw-r--r--   0        0        0     3238 2023-05-22 17:40:30.206770 docker_composer-2.17.3/src/docker_composer/base.py
--rw-r--r--   0        0        0        0 2023-05-22 17:40:30.206821 docker_composer-2.17.3/src/docker_composer/py.typed
--rw-r--r--   0        0        0        0 2023-05-22 17:40:30.206931 docker_composer-2.17.3/src/docker_composer/runner/__init__.py
--rw-r--r--   0        0        0     1227 2023-05-23 04:26:04.918719 docker_composer-2.17.3/src/docker_composer/runner/cmd/build.py
--rw-r--r--   0        0        0     1811 2023-05-23 04:26:04.920419 docker_composer-2.17.3/src/docker_composer/runner/cmd/config.py
--rw-r--r--   0        0        0      937 2023-05-23 04:26:04.921067 docker_composer-2.17.3/src/docker_composer/runner/cmd/cp.py
--rw-r--r--   0        0        0     1414 2023-05-23 04:26:04.923573 docker_composer-2.17.3/src/docker_composer/runner/cmd/create.py
--rw-r--r--   0        0        0     1029 2023-05-23 04:26:04.924300 docker_composer-2.17.3/src/docker_composer/runner/cmd/down.py
--rw-r--r--   0        0        0      608 2023-05-23 04:26:04.924787 docker_composer-2.17.3/src/docker_composer/runner/cmd/events.py
--rw-r--r--   0        0        0     1234 2023-05-23 04:26:04.925252 docker_composer-2.17.3/src/docker_composer/runner/cmd/exec.py
--rw-r--r--   0        0        0      690 2023-05-23 04:26:04.925715 docker_composer-2.17.3/src/docker_composer/runner/cmd/images.py
--rw-r--r--   0        0        0      729 2023-05-23 04:26:04.926585 docker_composer-2.17.3/src/docker_composer/runner/cmd/kill.py
--rw-r--r--   0        0        0     1250 2023-05-23 04:26:04.927212 docker_composer-2.17.3/src/docker_composer/runner/cmd/logs.py
--rw-r--r--   0        0        0      830 2023-05-23 04:26:04.927781 docker_composer-2.17.3/src/docker_composer/runner/cmd/ls.py
--rw-r--r--   0        0        0      463 2023-05-23 04:26:04.928480 docker_composer-2.17.3/src/docker_composer/runner/cmd/pause.py
--rw-r--r--   0        0        0      687 2023-05-23 04:26:04.929044 docker_composer-2.17.3/src/docker_composer/runner/cmd/port.py
--rw-r--r--   0        0        0     1112 2023-05-23 04:26:04.929585 docker_composer-2.17.3/src/docker_composer/runner/cmd/ps.py
--rw-r--r--   0        0        0      964 2023-05-23 04:26:04.930252 docker_composer-2.17.3/src/docker_composer/runner/cmd/pull.py
--rw-r--r--   0        0        0      856 2023-05-23 04:26:04.930719 docker_composer-2.17.3/src/docker_composer/runner/cmd/push.py
--rw-r--r--   0        0        0      689 2023-05-23 04:26:04.931180 docker_composer-2.17.3/src/docker_composer/runner/cmd/restart.py
--rw-r--r--   0        0        0     1012 2023-05-23 04:26:04.931614 docker_composer-2.17.3/src/docker_composer/runner/cmd/rm.py
--rw-r--r--   0        0        0     2329 2023-05-23 04:26:04.932024 docker_composer-2.17.3/src/docker_composer/runner/cmd/run.py
--rw-r--r--   0        0        0      463 2023-05-23 04:26:04.932460 docker_composer-2.17.3/src/docker_composer/runner/cmd/start.py
--rw-r--r--   0        0        0      564 2023-05-23 04:26:04.932850 docker_composer-2.17.3/src/docker_composer/runner/cmd/stop.py
--rw-r--r--   0        0        0      473 2023-05-23 04:26:04.933272 docker_composer-2.17.3/src/docker_composer/runner/cmd/top.py
--rw-r--r--   0        0        0      471 2023-05-23 04:26:04.933590 docker_composer-2.17.3/src/docker_composer/runner/cmd/unpause.py
--rw-r--r--   0        0        0     3402 2023-05-23 04:26:04.933916 docker_composer-2.17.3/src/docker_composer/runner/cmd/up.py
--rw-r--r--   0        0        0      702 2023-05-23 04:26:04.934369 docker_composer-2.17.3/src/docker_composer/runner/cmd/version.py
--rw-r--r--   0        0        0    27385 2023-05-23 04:26:04.935079 docker_composer-2.17.3/src/docker_composer/runner/root.py
--rw-r--r--   0        0        0     3060 1970-01-01 00:00:00.000000 docker_composer-2.17.3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-22 17:40:30.205463 docker_composer-2.17.4/LICENSE.txt
+-rw-r--r--   0        0        0     1981 2023-05-23 04:32:05.445481 docker_composer-2.17.4/README.md
+-rw-r--r--   0        0        0     1374 2023-05-23 04:33:34.325529 docker_composer-2.17.4/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-05-22 19:40:35.299994 docker_composer-2.17.4/src/docker_composer/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 17:40:30.206343 docker_composer-2.17.4/src/docker_composer/_utils/__init__.py
+-rw-r--r--   0        0        0     4557 2023-05-22 20:35:25.788589 docker_composer-2.17.4/src/docker_composer/_utils/argument.py
+-rw-r--r--   0        0        0     7241 2023-05-22 20:35:25.789294 docker_composer-2.17.4/src/docker_composer/_utils/generate_class.py
+-rw-r--r--   0        0        0     3238 2023-05-22 17:40:30.206770 docker_composer-2.17.4/src/docker_composer/base.py
+-rw-r--r--   0        0        0        0 2023-05-22 17:40:30.206821 docker_composer-2.17.4/src/docker_composer/py.typed
+-rw-r--r--   0        0        0        0 2023-05-22 17:40:30.206931 docker_composer-2.17.4/src/docker_composer/runner/__init__.py
+-rw-r--r--   0        0        0     1227 2023-05-23 04:26:04.918719 docker_composer-2.17.4/src/docker_composer/runner/cmd/build.py
+-rw-r--r--   0        0        0     1811 2023-05-23 04:26:04.920419 docker_composer-2.17.4/src/docker_composer/runner/cmd/config.py
+-rw-r--r--   0        0        0      937 2023-05-23 04:26:04.921067 docker_composer-2.17.4/src/docker_composer/runner/cmd/cp.py
+-rw-r--r--   0        0        0     1414 2023-05-23 04:26:04.923573 docker_composer-2.17.4/src/docker_composer/runner/cmd/create.py
+-rw-r--r--   0        0        0     1029 2023-05-23 04:26:04.924300 docker_composer-2.17.4/src/docker_composer/runner/cmd/down.py
+-rw-r--r--   0        0        0      608 2023-05-23 04:26:04.924787 docker_composer-2.17.4/src/docker_composer/runner/cmd/events.py
+-rw-r--r--   0        0        0     1234 2023-05-23 04:26:04.925252 docker_composer-2.17.4/src/docker_composer/runner/cmd/exec.py
+-rw-r--r--   0        0        0      690 2023-05-23 04:26:04.925715 docker_composer-2.17.4/src/docker_composer/runner/cmd/images.py
+-rw-r--r--   0        0        0      729 2023-05-23 04:26:04.926585 docker_composer-2.17.4/src/docker_composer/runner/cmd/kill.py
+-rw-r--r--   0        0        0     1250 2023-05-23 04:26:04.927212 docker_composer-2.17.4/src/docker_composer/runner/cmd/logs.py
+-rw-r--r--   0        0        0      830 2023-05-23 04:26:04.927781 docker_composer-2.17.4/src/docker_composer/runner/cmd/ls.py
+-rw-r--r--   0        0        0      463 2023-05-23 04:26:04.928480 docker_composer-2.17.4/src/docker_composer/runner/cmd/pause.py
+-rw-r--r--   0        0        0      687 2023-05-23 04:26:04.929044 docker_composer-2.17.4/src/docker_composer/runner/cmd/port.py
+-rw-r--r--   0        0        0     1112 2023-05-23 04:26:04.929585 docker_composer-2.17.4/src/docker_composer/runner/cmd/ps.py
+-rw-r--r--   0        0        0      964 2023-05-23 04:26:04.930252 docker_composer-2.17.4/src/docker_composer/runner/cmd/pull.py
+-rw-r--r--   0        0        0      856 2023-05-23 04:26:04.930719 docker_composer-2.17.4/src/docker_composer/runner/cmd/push.py
+-rw-r--r--   0        0        0      689 2023-05-23 04:26:04.931180 docker_composer-2.17.4/src/docker_composer/runner/cmd/restart.py
+-rw-r--r--   0        0        0     1012 2023-05-23 04:26:04.931614 docker_composer-2.17.4/src/docker_composer/runner/cmd/rm.py
+-rw-r--r--   0        0        0     2329 2023-05-23 04:26:04.932024 docker_composer-2.17.4/src/docker_composer/runner/cmd/run.py
+-rw-r--r--   0        0        0      463 2023-05-23 04:26:04.932460 docker_composer-2.17.4/src/docker_composer/runner/cmd/start.py
+-rw-r--r--   0        0        0      564 2023-05-23 04:26:04.932850 docker_composer-2.17.4/src/docker_composer/runner/cmd/stop.py
+-rw-r--r--   0        0        0      473 2023-05-23 04:26:04.933272 docker_composer-2.17.4/src/docker_composer/runner/cmd/top.py
+-rw-r--r--   0        0        0      471 2023-05-23 04:26:04.933590 docker_composer-2.17.4/src/docker_composer/runner/cmd/unpause.py
+-rw-r--r--   0        0        0     3402 2023-05-23 04:26:04.933916 docker_composer-2.17.4/src/docker_composer/runner/cmd/up.py
+-rw-r--r--   0        0        0      702 2023-05-23 04:26:04.934369 docker_composer-2.17.4/src/docker_composer/runner/cmd/version.py
+-rw-r--r--   0        0        0    27385 2023-05-23 04:26:04.935079 docker_composer-2.17.4/src/docker_composer/runner/root.py
+-rw-r--r--   0        0        0     3068 1970-01-01 00:00:00.000000 docker_composer-2.17.4/PKG-INFO
```

### Comparing `docker_composer-2.17.3/LICENSE.txt` & `docker_composer-2.17.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/README.md` & `docker_composer-2.17.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Docker Composer
-A library to interact with `docker-compose` from a python Program.
+A library to interact with `docker-compose` V2 from a python Program.
 All commands and parameters are exposed as python classes and attributes
 to allow for full auto-completion of its parameters with IDEs
 that support it.
 
 
 ## Install
 ```shell script
```

### Comparing `docker_composer-2.17.3/pyproject.toml` & `docker_composer-2.17.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "docker-composer"
-version = "2.17.3"
-description = "Use docker-compose from within Python"
+version = "2.17.4"
+description = "Use docker-compose (V2) from within Python"
 authors = ["Micha <schollm-git@gmx.com>"]
 readme = "README.md"
 homepage = "https://github.com/schollm/docker-composer"
 repository = "https://github.com/schollm/docker-composer"
 license = "Apache-2.0"
 packages = [
     { include = "docker_composer", from = "src" },
```

### Comparing `docker_composer-2.17.3/src/docker_composer/_utils/argument.py` & `docker_composer-2.17.4/src/docker_composer/_utils/argument.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/_utils/generate_class.py` & `docker_composer-2.17.4/src/docker_composer/_utils/generate_class.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/base.py` & `docker_composer-2.17.4/src/docker_composer/base.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/cmd/build.py` & `docker_composer-2.17.4/src/docker_composer/runner/cmd/build.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/cmd/config.py` & `docker_composer-2.17.4/src/docker_composer/runner/cmd/config.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/cmd/cp.py` & `docker_composer-2.17.4/src/docker_composer/runner/cmd/cp.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/cmd/create.py` & `docker_composer-2.17.4/src/docker_composer/runner/cmd/create.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/cmd/down.py` & `docker_composer-2.17.4/src/docker_composer/runner/cmd/down.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/cmd/events.py` & `docker_composer-2.17.4/src/docker_composer/runner/cmd/events.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/cmd/exec.py` & `docker_composer-2.17.4/src/docker_composer/runner/cmd/exec.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/cmd/images.py` & `docker_composer-2.17.4/src/docker_composer/runner/cmd/images.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/cmd/kill.py` & `docker_composer-2.17.4/src/docker_composer/runner/cmd/kill.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/cmd/logs.py` & `docker_composer-2.17.4/src/docker_composer/runner/cmd/logs.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/cmd/ls.py` & `docker_composer-2.17.4/src/docker_composer/runner/cmd/ls.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/cmd/port.py` & `docker_composer-2.17.4/src/docker_composer/runner/cmd/port.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/cmd/ps.py` & `docker_composer-2.17.4/src/docker_composer/runner/cmd/ps.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/cmd/pull.py` & `docker_composer-2.17.4/src/docker_composer/runner/cmd/pull.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/cmd/push.py` & `docker_composer-2.17.4/src/docker_composer/runner/cmd/push.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/cmd/restart.py` & `docker_composer-2.17.4/src/docker_composer/runner/cmd/restart.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/cmd/rm.py` & `docker_composer-2.17.4/src/docker_composer/runner/cmd/rm.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/cmd/run.py` & `docker_composer-2.17.4/src/docker_composer/runner/cmd/run.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/cmd/stop.py` & `docker_composer-2.17.4/src/docker_composer/runner/cmd/stop.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/cmd/up.py` & `docker_composer-2.17.4/src/docker_composer/runner/cmd/up.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/cmd/version.py` & `docker_composer-2.17.4/src/docker_composer/runner/cmd/version.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/src/docker_composer/runner/root.py` & `docker_composer-2.17.4/src/docker_composer/runner/root.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.3/PKG-INFO` & `docker_composer-2.17.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: docker-composer
-Version: 2.17.3
-Summary: Use docker-compose from within Python
+Version: 2.17.4
+Summary: Use docker-compose (V2) from within Python
 Home-page: https://github.com/schollm/docker-composer
 License: Apache-2.0
 Author: Micha
 Author-email: schollm-git@gmx.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Dist: attrs (>=20.3.0)
 Requires-Dist: loguru (>=0.5.3)
 Project-URL: Repository, https://github.com/schollm/docker-composer
 Description-Content-Type: text/markdown
 
 # Docker Composer
-A library to interact with `docker-compose` from a python Program.
+A library to interact with `docker-compose` V2 from a python Program.
 All commands and parameters are exposed as python classes and attributes
 to allow for full auto-completion of its parameters with IDEs
 that support it.
 
 
 ## Install
 ```shell script
```

