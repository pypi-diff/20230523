# Comparing `tmp/aio.api.github-0.2.3.tar.gz` & `tmp/aio.api.github-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio.api.github-0.2.3.tar", last modified: Tue May 23 17:56:59 2023, max compression
+gzip compressed data, was "aio.api.github-0.2.4.tar", last modified: Tue May 23 19:12:32 2023, max compression
```

## Comparing `aio.api.github-0.2.3.tar` & `aio.api.github-0.2.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:59.376130 aio.api.github-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-23 17:56:59.376130 aio.api.github-0.2.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:59.372130 aio.api.github-0.2.3/aio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:59.372130 aio.api.github-0.2.3/aio/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:59.376130 aio.api.github-0.2.3/aio/api/github/
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:59.376130 aio.api.github-0.2.3/aio/api/github/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:59.376130 aio.api.github-0.2.3/aio/api/github/abstract/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/actions/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/commit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:59.376130 aio.api.github-0.2.3/aio/api/github/abstract/issues/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/issues/issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/issues/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/label.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/release.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15913 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:59.376130 aio.api.github-0.2.3/aio.api.github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio.api.github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio.api.github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio.api.github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio.api.github.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio.api.github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio.api.github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 17:56:59.376130 aio.api.github-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:12:32.979508 aio.api.github-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-23 19:12:32.979508 aio.api.github-0.2.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:12:32.971508 aio.api.github-0.2.4/aio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:12:32.971508 aio.api.github-0.2.4/aio/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:12:32.975508 aio.api.github-0.2.4/aio/api/github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio/api/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:12:32.975508 aio.api.github-0.2.4/aio/api/github/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio/api/github/abstract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:12:32.975508 aio.api.github-0.2.4/aio/api/github/abstract/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio/api/github/abstract/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio/api/github/abstract/actions/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio/api/github/abstract/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio/api/github/abstract/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio/api/github/abstract/commit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:12:32.979508 aio.api.github-0.2.4/aio/api/github/abstract/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio/api/github/abstract/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio/api/github/abstract/issues/issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio/api/github/abstract/issues/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio/api/github/abstract/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio/api/github/abstract/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio/api/github/abstract/release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio/api/github/abstract/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio/api/github/abstract/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio/api/github/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio/api/github/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16051 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio/api/github/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio/api/github/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio/api/github/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio/api/github/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:12:32.975508 aio.api.github-0.2.4/aio.api.github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio.api.github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio.api.github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio.api.github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio.api.github.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio.api.github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/aio.api.github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 19:12:32.979508 aio.api.github-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-23 19:12:32.000000 aio.api.github-0.2.4/setup.py
```

### Comparing `aio.api.github-0.2.3/aio/api/github/__init__.py` & `aio.api.github-0.2.4/aio/api/github/__init__.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.3/aio/api/github/abstract/__init__.py` & `aio.api.github-0.2.4/aio/api/github/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.3/aio/api/github/abstract/actions/actions.py` & `aio.api.github-0.2.4/aio/api/github/abstract/actions/actions.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.3/aio/api/github/abstract/api.py` & `aio.api.github-0.2.4/aio/api/github/abstract/api.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.3/aio/api/github/abstract/base.py` & `aio.api.github-0.2.4/aio/api/github/abstract/base.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.3/aio/api/github/abstract/commit.py` & `aio.api.github-0.2.4/aio/api/github/abstract/commit.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.3/aio/api/github/abstract/issues/issues.py` & `aio.api.github-0.2.4/aio/api/github/abstract/issues/issues.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.3/aio/api/github/abstract/issues/tracker.py` & `aio.api.github-0.2.4/aio/api/github/abstract/issues/tracker.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.3/aio/api/github/abstract/iterator.py` & `aio.api.github-0.2.4/aio/api/github/abstract/iterator.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.3/aio/api/github/abstract/release.py` & `aio.api.github-0.2.4/aio/api/github/abstract/release.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.3/aio/api/github/abstract/repo.py` & `aio.api.github-0.2.4/aio/api/github/abstract/repo.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.3/aio/api/github/abstract/tag.py` & `aio.api.github-0.2.4/aio/api/github/abstract/tag.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.3/aio/api/github/api.py` & `aio.api.github-0.2.4/aio/api/github/api.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.3/aio/api/github/interface.py` & `aio.api.github-0.2.4/aio/api/github/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,14 +167,19 @@
 
     @abstracts.interfacemethod
     def __init__(self, github: "IGithubAPI", name: str) -> None:
         raise NotImplementedError
 
     @property  # type:ignore
     @abstracts.interfacemethod
+    def actions(self) -> "IGithubActions":
+        raise NotImplementedError
+
+    @property  # type:ignore
+    @abstracts.interfacemethod
     def github(self) -> IGithubAPI:
         raise NotImplementedError
 
     @property  # type:ignore
     @abstracts.interfacemethod
     def issues(self) -> "IGithubIssues":
         """Github issues for this repo."""
```

### Comparing `aio.api.github-0.2.3/aio.api.github.egg-info/SOURCES.txt` & `aio.api.github-0.2.4/aio.api.github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.3/backend_shim.py` & `aio.api.github-0.2.4/backend_shim.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.3/setup.py` & `aio.api.github-0.2.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,9 +36,9 @@
         'aio.api.github',
         'aio.api.github.abstract',
         'aio.api.github.abstract.actions',
         'aio.api.github.abstract.issues',
     ),
     'python_requires': '>=3.10.0',
     'url': 'https://github.com/envoyproxy/toolshed/tree/main/aio.api.github',
-    'version': '0.2.3',
+    'version': '0.2.4',
 })
```

