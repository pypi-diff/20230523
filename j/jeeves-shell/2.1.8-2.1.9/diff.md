# Comparing `tmp/jeeves_shell-2.1.8.tar.gz` & `tmp/jeeves_shell-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeeves_shell-2.1.8.tar", max compression
+gzip compressed data, was "jeeves_shell-2.1.9.tar", max compression
```

## Comparing `jeeves_shell-2.1.8.tar` & `jeeves_shell-2.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1097 2022-11-04 16:58:55.671588 jeeves_shell-2.1.8/LICENSE
--rw-r--r--   0        0        0      956 2022-12-11 18:27:06.062169 jeeves_shell-2.1.8/README.md
--rw-r--r--   0        0        0       39 2022-12-11 18:23:17.084079 jeeves_shell-2.1.8/jeeves_shell/__init__.py
--rw-r--r--   0        0        0      797 2022-12-23 20:39:58.547042 jeeves_shell-2.1.8/jeeves_shell/cli.py
--rw-r--r--   0        0        0     3353 2023-04-15 21:43:00.746449 jeeves_shell-2.1.8/jeeves_shell/discover.py
--rw-r--r--   0        0        0      189 2022-12-09 17:35:01.246912 jeeves_shell-2.1.8/jeeves_shell/entry_points.py
--rw-r--r--   0        0        0      420 2022-12-09 20:33:49.924243 jeeves_shell-2.1.8/jeeves_shell/errors.py
--rw-r--r--   0        0        0      256 2023-05-05 17:26:27.544054 jeeves_shell-2.1.8/jeeves_shell/import_by_path.py
--rw-r--r--   0        0        0      307 2022-12-23 20:35:47.874000 jeeves_shell-2.1.8/jeeves_shell/jeeves.py
--rw-r--r--   0        0        0     1685 2023-05-18 19:56:46.496379 jeeves_shell-2.1.8/pyproject.toml
--rw-r--r--   0        0        0     1925 1970-01-01 00:00:00.000000 jeeves_shell-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1097 2022-11-04 16:58:55.671588 jeeves_shell-2.1.9/LICENSE
+-rw-r--r--   0        0        0      956 2022-12-11 18:27:06.062169 jeeves_shell-2.1.9/README.md
+-rw-r--r--   0        0        0       39 2022-12-11 18:23:17.084079 jeeves_shell-2.1.9/jeeves_shell/__init__.py
+-rw-r--r--   0        0        0      797 2022-12-23 20:39:58.547042 jeeves_shell-2.1.9/jeeves_shell/cli.py
+-rw-r--r--   0        0        0     3353 2023-04-15 21:43:00.746449 jeeves_shell-2.1.9/jeeves_shell/discover.py
+-rw-r--r--   0        0        0      189 2022-12-09 17:35:01.246912 jeeves_shell-2.1.9/jeeves_shell/entry_points.py
+-rw-r--r--   0        0        0      420 2022-12-09 20:33:49.924243 jeeves_shell-2.1.9/jeeves_shell/errors.py
+-rw-r--r--   0        0        0      256 2023-05-05 17:26:27.544054 jeeves_shell-2.1.9/jeeves_shell/import_by_path.py
+-rw-r--r--   0        0        0      307 2022-12-23 20:35:47.874000 jeeves_shell-2.1.9/jeeves_shell/jeeves.py
+-rw-r--r--   0        0        0     1719 2023-05-18 20:15:19.119192 jeeves_shell-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1925 1970-01-01 00:00:00.000000 jeeves_shell-2.1.9/PKG-INFO
```

### Comparing `jeeves_shell-2.1.8/LICENSE` & `jeeves_shell-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.1.8/README.md` & `jeeves_shell-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.1.8/jeeves_shell/cli.py` & `jeeves_shell-2.1.9/jeeves_shell/cli.py`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.1.8/jeeves_shell/discover.py` & `jeeves_shell-2.1.9/jeeves_shell/discover.py`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.1.8/pyproject.toml` & `jeeves_shell-2.1.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "jeeves-shell"
 description = "Pythonic replacement for GNU Make"
-version = "2.1.8"
+version = "2.1.9"
 license = "MIT"
 
 authors = []
 
 readme = "README.md"
 
 repository = "https://github.com/jeeves-sh/jeeves-shell"
@@ -45,14 +45,15 @@
 mkdocstrings = "^0.19.1"
 
 markupsafe = "<2.1"   # Otherwise, `jinja2` will fail
 importlib-metadata = "<5.0"
 mkdocs-macros-plugin = "^0.7.0"
 dominate = "^2.7.0"
 iolanta-tables = "^0.1.7"
+jeeves-yeti-pyproject = "^0.2.16"
 
 [tool.flakeheaven.exceptions."jeeves_shell/jeeves.py"]
 wemake-python-styleguide = [
   "-WPS115",
   "-WPS600",
 ]
```

### Comparing `jeeves_shell-2.1.8/PKG-INFO` & `jeeves_shell-2.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeeves-shell
-Version: 2.1.8
+Version: 2.1.9
 Summary: Pythonic replacement for GNU Make
 Home-page: https://github.com/jeeves-sh/jeeves-shell
 License: MIT
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

