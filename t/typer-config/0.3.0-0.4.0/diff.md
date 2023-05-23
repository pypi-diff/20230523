# Comparing `tmp/typer_config-0.3.0.tar.gz` & `tmp/typer_config-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_config-0.3.0.tar", max compression
+gzip compressed data, was "typer_config-0.4.0.tar", max compression
```

## Comparing `typer_config-0.3.0.tar` & `typer_config-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-05-16 04:06:27.574721 typer_config-0.3.0/LICENSE
--rw-r--r--   0        0        0     1840 2023-05-18 01:01:35.696589 typer_config-0.3.0/README.md
--rw-r--r--   0        0        0     2454 2023-05-18 02:46:44.745316 typer_config-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3706 2023-05-18 02:25:55.528865 typer_config-0.3.0/typer_config/__init__.py
--rw-r--r--   0        0        0     1089 2023-05-16 04:06:27.578055 typer_config-0.3.0/typer_config/__typing.py
--rw-r--r--   0        0        0     5957 2023-05-18 02:33:38.242837 typer_config-0.3.0/typer_config/loaders.py
--rw-r--r--   0        0        0     3843 1970-01-01 00:00:00.000000 typer_config-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-16 04:06:27.574721 typer_config-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1840 2023-05-18 01:01:35.696589 typer_config-0.4.0/README.md
+-rw-r--r--   0        0        0     2612 2023-05-23 03:04:29.520702 typer_config-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3706 2023-05-18 02:25:55.528865 typer_config-0.4.0/typer_config/__init__.py
+-rw-r--r--   0        0        0     1355 2023-05-23 02:08:20.889710 typer_config-0.4.0/typer_config/__typing.py
+-rw-r--r--   0        0        0     8661 2023-05-23 02:08:20.899710 typer_config-0.4.0/typer_config/loaders.py
+-rw-r--r--   0        0        0     3843 1970-01-01 00:00:00.000000 typer_config-0.4.0/PKG-INFO
```

### Comparing `typer_config-0.3.0/LICENSE` & `typer_config-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typer_config-0.3.0/README.md` & `typer_config-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `typer_config-0.3.0/pyproject.toml` & `typer_config-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typer-config"
-version = "0.3.0"
+version = "0.4.0"
 description = "Utilities for working with configuration files in typer CLIs. "
 authors = ["Matt Anderson <matt@manderscience.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "typer_config"}]
 repository = "https://github.com/maxb2/typer-config"
 documentation = "https://maxb2.github.io/typer-config/"
@@ -62,21 +62,24 @@
 mypy = "^1.2.0"
 types-toml = "^0.10.8.6"
 types-pyyaml = "^6.0.12.9"
 git-changelog = "^1.0.1"
 duty = "^0.11.0"
 pytest-cov = "^4.0.0"
 safety = "^2.3.5"
-griffe = "^0.27.5"
+griffe = "^0.28.1"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.1.9"
 mkdocstrings = {extras = ["python"], version = "^0.21.2"}
 mike = "^1.1.2"
 mkdocs-gen-files = "^0.5.0"
+pydantic = "^1.10.7"
+blacken-docs = { git = "https://github.com/maxb2/blacken-docs.git", rev = "b3c82da4df8eaca840b101d0aeab12ae029b6364" }
+schema = "^0.7.5"
 
 [tool.isort]
 profile = "black"
 
 [tool.pylint.format]
 max-line-length = "88"
```

### Comparing `typer_config-0.3.0/typer_config/__init__.py` & `typer_config-0.4.0/typer_config/__init__.py`

 * *Files identical despite different names*

### Comparing `typer_config-0.3.0/typer_config/__typing.py` & `typer_config-0.4.0/typer_config/__typing.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,14 +23,22 @@
 ConfigDict: TypeAlias = Dict[TyperParameterName, Any]
 """Configuration dictionary to be applied to the click context default map."""
 
 ConfigDictAccessorPath: TypeAlias = Iterable[str]
 """Configuration dictionary accessor path."""
 
 # Function types
+TyperParameterValueTransformer: TypeAlias = Callable[
+    [TyperParameterValue], TyperParameterValue
+]
+"""Typer parameter value transforming function."""
+
+ConfigDictTransformer: TypeAlias = Callable[[ConfigDict], ConfigDict]
+"""ConfigDict transforming function."""
+
 ConfigLoader: TypeAlias = Callable[[TyperParameterValue], ConfigDict]
 """Configuration loader function."""
 
 ConfigParameterCallback: TypeAlias = Callable[
     [Context, CallbackParam, TyperParameterValue], TyperParameterValue
 ]
 """Typer config parameter callback function."""
```

### Comparing `typer_config-0.3.0/PKG-INFO` & `typer_config-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typer-config
-Version: 0.3.0
+Version: 0.4.0
 Summary: Utilities for working with configuration files in typer CLIs. 
 Home-page: https://maxb2.github.io/typer-config/
 License: MIT
 Keywords: typer,config,configuration,configuration-file,yaml,toml,json,dotenv,cli
 Author: Matt Anderson
 Author-email: matt@manderscience.com
 Requires-Python: >=3.8,<4.0
```

