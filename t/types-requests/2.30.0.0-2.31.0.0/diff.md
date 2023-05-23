# Comparing `tmp/types-requests-2.30.0.0.tar.gz` & `tmp/types-requests-2.31.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-requests-2.30.0.0.tar", last modified: Fri May  5 12:27:47 2023, max compression
+gzip compressed data, was "types-requests-2.31.0.0.tar", last modified: Tue May 23 09:14:57 2023, max compression
```

## Comparing `types-requests-2.30.0.0.tar` & `types-requests-2.31.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:27:47.462063 types-requests-2.30.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-05 12:27:46.000000 types-requests-2.30.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 12:27:46.000000 types-requests-2.30.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-05 12:27:47.462063 types-requests-2.30.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:27:47.462063 types-requests-2.30.0.0/requests-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-05 12:27:46.000000 types-requests-2.30.0.0/requests-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-05 12:27:32.000000 types-requests-2.30.0.0/requests-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-05 12:27:32.000000 types-requests-2.30.0.0/requests-stubs/__version__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-05 12:27:32.000000 types-requests-2.30.0.0/requests-stubs/adapters.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-05-05 12:27:32.000000 types-requests-2.30.0.0/requests-stubs/api.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-05 12:27:32.000000 types-requests-2.30.0.0/requests-stubs/auth.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 12:27:32.000000 types-requests-2.30.0.0/requests-stubs/certs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-05 12:27:32.000000 types-requests-2.30.0.0/requests-stubs/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-05 12:27:32.000000 types-requests-2.30.0.0/requests-stubs/cookies.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-05 12:27:32.000000 types-requests-2.30.0.0/requests-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-05 12:27:32.000000 types-requests-2.30.0.0/requests-stubs/help.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 12:27:32.000000 types-requests-2.30.0.0/requests-stubs/hooks.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-05-05 12:27:32.000000 types-requests-2.30.0.0/requests-stubs/models.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-05 12:27:32.000000 types-requests-2.30.0.0/requests-stubs/packages.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-05-05 12:27:32.000000 types-requests-2.30.0.0/requests-stubs/sessions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-05 12:27:32.000000 types-requests-2.30.0.0/requests-stubs/status_codes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-05 12:27:32.000000 types-requests-2.30.0.0/requests-stubs/structures.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-05 12:27:32.000000 types-requests-2.30.0.0/requests-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:27:47.462063 types-requests-2.30.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-05 12:27:46.000000 types-requests-2.30.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:27:47.462063 types-requests-2.30.0.0/types_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-05 12:27:47.000000 types-requests-2.30.0.0/types_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-05 12:27:47.000000 types-requests-2.30.0.0/types_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:27:47.000000 types-requests-2.30.0.0/types_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 12:27:47.000000 types-requests-2.30.0.0/types_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 12:27:47.000000 types-requests-2.30.0.0/types_requests.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:14:57.436358 types-requests-2.31.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-05-23 09:14:56.000000 types-requests-2.31.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 09:14:56.000000 types-requests-2.31.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-23 09:14:57.436358 types-requests-2.31.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:14:57.432358 types-requests-2.31.0.0/requests-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-23 09:14:56.000000 types-requests-2.31.0.0/requests-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-23 09:14:32.000000 types-requests-2.31.0.0/requests-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-23 09:14:32.000000 types-requests-2.31.0.0/requests-stubs/__version__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-23 09:14:32.000000 types-requests-2.31.0.0/requests-stubs/adapters.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-05-23 09:14:32.000000 types-requests-2.31.0.0/requests-stubs/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-23 09:14:32.000000 types-requests-2.31.0.0/requests-stubs/auth.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 09:14:32.000000 types-requests-2.31.0.0/requests-stubs/certs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-23 09:14:32.000000 types-requests-2.31.0.0/requests-stubs/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-23 09:14:32.000000 types-requests-2.31.0.0/requests-stubs/cookies.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-23 09:14:32.000000 types-requests-2.31.0.0/requests-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-23 09:14:32.000000 types-requests-2.31.0.0/requests-stubs/help.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-23 09:14:32.000000 types-requests-2.31.0.0/requests-stubs/hooks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-05-23 09:14:32.000000 types-requests-2.31.0.0/requests-stubs/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-23 09:14:32.000000 types-requests-2.31.0.0/requests-stubs/packages.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-05-23 09:14:32.000000 types-requests-2.31.0.0/requests-stubs/sessions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-23 09:14:32.000000 types-requests-2.31.0.0/requests-stubs/status_codes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-23 09:14:32.000000 types-requests-2.31.0.0/requests-stubs/structures.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-23 09:14:32.000000 types-requests-2.31.0.0/requests-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 09:14:57.436358 types-requests-2.31.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-23 09:14:56.000000 types-requests-2.31.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:14:57.436358 types-requests-2.31.0.0/types_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-23 09:14:57.000000 types-requests-2.31.0.0/types_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-23 09:14:57.000000 types-requests-2.31.0.0/types_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:14:57.000000 types-requests-2.31.0.0/types_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 09:14:57.000000 types-requests-2.31.0.0/types_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 09:14:57.000000 types-requests-2.31.0.0/types_requests.egg-info/top_level.txt
```

### Comparing `types-requests-2.30.0.0/CHANGELOG.md` & `types-requests-2.31.0.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+## 2.31.0.0 (2023-05-23)
+
+[stubsabot] Bump requests to 2.31.* (#10199)
+
+Release: https://pypi.org/pypi/requests/2.31.0
+Homepage: https://requests.readthedocs.io
+Diff: https://github.com/psf/requests/compare/v2.30.0...v2.31.0
+
+Stubsabot analysis of the diff between the two releases:
+ - 0 public Python files have been added.
+ - 0 files included in typeshed's stubs have been deleted.
+ - 2 files included in typeshed's stubs have been modified or renamed: `requests/__version__.py`, `requests/sessions.py`.
+ - Total lines of Python code added: 26.
+ - Total lines of Python code deleted: 4.
+
 ## 2.30.0.0 (2023-05-05)
 
 [requests] Update stubs to 2.30 (#10141)
 
 ## 2.29.0.0 (2023-04-29)
 
 Update `requests` for v2.29 (#10097)
```

### Comparing `types-requests-2.30.0.0/PKG-INFO` & `types-requests-2.31.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-requests
-Version: 2.30.0.0
+Version: 2.31.0.0
 Summary: Typing stubs for requests
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/requests.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `requests`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/requests. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `5fdbf37c1f59968a18667843c157da66d43dddbd`.
+This package was generated from typeshed commit `e821090926dcb06d5b53e0a81f29508bbe3a911b`.
```

### Comparing `types-requests-2.30.0.0/requests-stubs/__init__.pyi` & `types-requests-2.31.0.0/requests-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.30.0.0/requests-stubs/adapters.pyi` & `types-requests-2.31.0.0/requests-stubs/adapters.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.30.0.0/requests-stubs/api.pyi` & `types-requests-2.31.0.0/requests-stubs/api.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.30.0.0/requests-stubs/auth.pyi` & `types-requests-2.31.0.0/requests-stubs/auth.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.30.0.0/requests-stubs/compat.pyi` & `types-requests-2.31.0.0/requests-stubs/compat.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.30.0.0/requests-stubs/cookies.pyi` & `types-requests-2.31.0.0/requests-stubs/cookies.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.30.0.0/requests-stubs/exceptions.pyi` & `types-requests-2.31.0.0/requests-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.30.0.0/requests-stubs/help.pyi` & `types-requests-2.31.0.0/requests-stubs/help.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.30.0.0/requests-stubs/models.pyi` & `types-requests-2.31.0.0/requests-stubs/models.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.30.0.0/requests-stubs/sessions.pyi` & `types-requests-2.31.0.0/requests-stubs/sessions.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.30.0.0/requests-stubs/structures.pyi` & `types-requests-2.31.0.0/requests-stubs/structures.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.30.0.0/requests-stubs/utils.pyi` & `types-requests-2.31.0.0/requests-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.30.0.0/setup.py` & `types-requests-2.31.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `requests`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/requests. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `5fdbf37c1f59968a18667843c157da66d43dddbd`.
+This package was generated from typeshed commit `e821090926dcb06d5b53e0a81f29508bbe3a911b`.
 '''.lstrip()
 
 setup(name=name,
-      version="2.30.0.0",
+      version="2.31.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/requests.md",
```

### Comparing `types-requests-2.30.0.0/types_requests.egg-info/PKG-INFO` & `types-requests-2.31.0.0/types_requests.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-requests
-Version: 2.30.0.0
+Version: 2.31.0.0
 Summary: Typing stubs for requests
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/requests.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `requests`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/requests. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `5fdbf37c1f59968a18667843c157da66d43dddbd`.
+This package was generated from typeshed commit `e821090926dcb06d5b53e0a81f29508bbe3a911b`.
```

### Comparing `types-requests-2.30.0.0/types_requests.egg-info/SOURCES.txt` & `types-requests-2.31.0.0/types_requests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

