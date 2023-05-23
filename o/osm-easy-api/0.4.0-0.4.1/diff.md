# Comparing `tmp/osm_easy_api-0.4.0.tar.gz` & `tmp/osm_easy_api-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osm_easy_api-0.4.0.tar", last modified: Wed May  3 18:27:08 2023, max compression
+gzip compressed data, was "osm_easy_api-0.4.1.tar", last modified: Tue May 23 19:15:56 2023, max compression
```

## Comparing `osm_easy_api-0.4.0.tar` & `osm_easy_api-0.4.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 18:27:08.301620 osm_easy_api-0.4.0/
--rw-rw-rw-   0        0        0     2741 2023-05-03 18:26:26.000000 osm_easy_api-0.4.0/CHANGELOG.md
--rw-rw-rw-   0        0        0    35821 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/LICENSE.md
--rw-rw-rw-   0        0        0    44021 2023-05-03 18:27:08.301620 osm_easy_api-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     4542 2023-03-23 20:46:05.000000 osm_easy_api-0.4.0/README.md
--rw-rw-rw-   0        0        0       97 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0     1197 2023-05-03 18:27:08.308134 osm_easy_api-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:27:08.242055 osm_easy_api-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 18:27:08.254380 osm_easy_api-0.4.0/src/osm_easy_api/
--rw-rw-rw-   0        0        0      107 2023-05-03 18:26:45.000000 osm_easy_api-0.4.0/src/osm_easy_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:27:08.276668 osm_easy_api-0.4.0/src/osm_easy_api/api/
--rw-rw-rw-   0        0        0     3033 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/_URLs.py
--rw-rw-rw-   0        0        0      101 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/__init__.py
--rw-rw-rw-   0        0        0     4336 2023-03-08 21:18:46.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/api.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:27:08.284231 osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/
--rw-rw-rw-   0        0        0      520 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/__init__.py
--rw-rw-rw-   0        0        0    14405 2023-04-02 18:15:22.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/changeset.py
--rw-rw-rw-   0        0        0     4369 2023-04-02 18:15:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/changeset_discussion.py
--rw-rw-rw-   0        0        0    17037 2023-04-02 18:17:01.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/elements.py
--rw-rw-rw-   0        0        0     1062 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/gpx.py
--rw-rw-rw-   0        0        0     5540 2023-04-02 18:17:21.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/misc.py
--rw-rw-rw-   0        0        0    11406 2023-04-02 18:18:10.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/notes.py
--rw-rw-rw-   0        0        0     7047 2023-04-02 18:18:25.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/user.py
--rw-rw-rw-   0        0        0     1025 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/api/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:27:08.295442 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/
--rw-rw-rw-   0        0        0     4381 2023-03-23 20:30:50.000000 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/OsmChange.py
--rw-rw-rw-   0        0        0      432 2023-03-22 23:03:24.000000 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/__init__.py
--rw-rw-rw-   0        0        0     1785 2023-03-14 14:11:03.000000 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/changeset.py
--rw-rw-rw-   0        0        0     1183 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/node.py
--rw-rw-rw-   0        0        0     4022 2023-03-22 21:29:55.000000 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/note.py
--rw-rw-rw-   0        0        0     2635 2023-05-03 15:23:00.000000 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/osm_object_primitive.py
--rw-rw-rw-   0        0        0     2683 2023-05-03 17:59:51.000000 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/relation.py
--rw-rw-rw-   0        0        0     1403 2023-03-22 23:13:07.000000 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/tags.py
--rw-rw-rw-   0        0        0     2099 2023-03-22 20:09:45.000000 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/user.py
--rw-rw-rw-   0        0        0     1707 2023-05-03 17:48:59.000000 osm_easy_api-0.4.0/src/osm_easy_api/data_classes/way.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:27:08.297624 osm_easy_api-0.4.0/src/osm_easy_api/diff/
--rw-rw-rw-   0        0        0      111 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/diff/__init__.py
--rw-rw-rw-   0        0        0     6164 2023-04-01 19:34:36.000000 osm_easy_api-0.4.0/src/osm_easy_api/diff/diff.py
--rw-rw-rw-   0        0        0     9075 2023-03-07 21:24:24.000000 osm_easy_api-0.4.0/src/osm_easy_api/diff/diff_parser.py
--rw-rw-rw-   0        0        0        0 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-03 18:27:08.300625 osm_easy_api-0.4.0/src/osm_easy_api/utils/
--rw-rw-rw-   0        0        0       82 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/utils/__init__.py
--rw-rw-rw-   0        0        0      166 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/utils/join_url.py
--rw-rw-rw-   0        0        0      397 2023-03-07 21:14:41.000000 osm_easy_api-0.4.0/src/osm_easy_api/utils/write_gzip_to_file.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:27:08.272122 osm_easy_api-0.4.0/src/osm_easy_api.egg-info/
--rw-rw-rw-   0        0        0    44021 2023-05-03 18:27:08.000000 osm_easy_api-0.4.0/src/osm_easy_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2023-05-03 18:27:08.000000 osm_easy_api-0.4.0/src/osm_easy_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 18:27:08.000000 osm_easy_api-0.4.0/src/osm_easy_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-07 21:15:07.000000 osm_easy_api-0.4.0/src/osm_easy_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       90 2023-05-03 18:27:08.000000 osm_easy_api-0.4.0/src/osm_easy_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-03 18:27:08.000000 osm_easy_api-0.4.0/src/osm_easy_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 19:15:56.551484 osm_easy_api-0.4.1/
+-rw-rw-rw-   0        0        0     2817 2023-05-23 19:14:41.000000 osm_easy_api-0.4.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35821 2023-03-07 21:14:41.000000 osm_easy_api-0.4.1/LICENSE.md
+-rw-rw-rw-   0        0        0    44069 2023-05-23 19:15:56.552480 osm_easy_api-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4514 2023-05-03 21:30:36.000000 osm_easy_api-0.4.1/README.md
+-rw-rw-rw-   0        0        0       97 2023-03-07 21:14:41.000000 osm_easy_api-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1197 2023-05-23 19:15:56.555479 osm_easy_api-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-03-07 21:14:41.000000 osm_easy_api-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:15:56.468774 osm_easy_api-0.4.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 19:15:56.482128 osm_easy_api-0.4.1/src/osm_easy_api/
+-rw-rw-rw-   0        0        0      107 2023-05-23 19:15:01.000000 osm_easy_api-0.4.1/src/osm_easy_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:15:56.512804 osm_easy_api-0.4.1/src/osm_easy_api/api/
+-rw-rw-rw-   0        0        0     3033 2023-03-07 21:14:41.000000 osm_easy_api-0.4.1/src/osm_easy_api/api/_URLs.py
+-rw-rw-rw-   0        0        0      101 2023-03-07 21:14:41.000000 osm_easy_api-0.4.1/src/osm_easy_api/api/__init__.py
+-rw-rw-rw-   0        0        0     4336 2023-03-08 21:18:46.000000 osm_easy_api-0.4.1/src/osm_easy_api/api/api.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:15:56.521866 osm_easy_api-0.4.1/src/osm_easy_api/api/endpoints/
+-rw-rw-rw-   0        0        0      520 2023-03-07 21:14:41.000000 osm_easy_api-0.4.1/src/osm_easy_api/api/endpoints/__init__.py
+-rw-rw-rw-   0        0        0    14405 2023-04-02 18:15:22.000000 osm_easy_api-0.4.1/src/osm_easy_api/api/endpoints/changeset.py
+-rw-rw-rw-   0        0        0     4369 2023-04-02 18:15:41.000000 osm_easy_api-0.4.1/src/osm_easy_api/api/endpoints/changeset_discussion.py
+-rw-rw-rw-   0        0        0    17037 2023-04-02 18:17:01.000000 osm_easy_api-0.4.1/src/osm_easy_api/api/endpoints/elements.py
+-rw-rw-rw-   0        0        0     1062 2023-03-07 21:14:41.000000 osm_easy_api-0.4.1/src/osm_easy_api/api/endpoints/gpx.py
+-rw-rw-rw-   0        0        0     5540 2023-04-02 18:17:21.000000 osm_easy_api-0.4.1/src/osm_easy_api/api/endpoints/misc.py
+-rw-rw-rw-   0        0        0    11406 2023-04-02 18:18:10.000000 osm_easy_api-0.4.1/src/osm_easy_api/api/endpoints/notes.py
+-rw-rw-rw-   0        0        0     7047 2023-04-02 18:18:25.000000 osm_easy_api-0.4.1/src/osm_easy_api/api/endpoints/user.py
+-rw-rw-rw-   0        0        0     1025 2023-03-07 21:14:41.000000 osm_easy_api-0.4.1/src/osm_easy_api/api/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:15:56.532389 osm_easy_api-0.4.1/src/osm_easy_api/data_classes/
+-rw-rw-rw-   0        0        0     4381 2023-03-23 20:30:50.000000 osm_easy_api-0.4.1/src/osm_easy_api/data_classes/OsmChange.py
+-rw-rw-rw-   0        0        0      432 2023-03-22 23:03:24.000000 osm_easy_api-0.4.1/src/osm_easy_api/data_classes/__init__.py
+-rw-rw-rw-   0        0        0     1785 2023-03-14 14:11:03.000000 osm_easy_api-0.4.1/src/osm_easy_api/data_classes/changeset.py
+-rw-rw-rw-   0        0        0     1183 2023-03-07 21:14:41.000000 osm_easy_api-0.4.1/src/osm_easy_api/data_classes/node.py
+-rw-rw-rw-   0        0        0     4022 2023-03-22 21:29:55.000000 osm_easy_api-0.4.1/src/osm_easy_api/data_classes/note.py
+-rw-rw-rw-   0        0        0     2635 2023-05-03 15:23:00.000000 osm_easy_api-0.4.1/src/osm_easy_api/data_classes/osm_object_primitive.py
+-rw-rw-rw-   0        0        0     2683 2023-05-03 17:59:51.000000 osm_easy_api-0.4.1/src/osm_easy_api/data_classes/relation.py
+-rw-rw-rw-   0        0        0     1403 2023-03-22 23:13:07.000000 osm_easy_api-0.4.1/src/osm_easy_api/data_classes/tags.py
+-rw-rw-rw-   0        0        0     2099 2023-03-22 20:09:45.000000 osm_easy_api-0.4.1/src/osm_easy_api/data_classes/user.py
+-rw-rw-rw-   0        0        0     1707 2023-05-03 17:48:59.000000 osm_easy_api-0.4.1/src/osm_easy_api/data_classes/way.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:15:56.536393 osm_easy_api-0.4.1/src/osm_easy_api/diff/
+-rw-rw-rw-   0        0        0      111 2023-03-07 21:14:41.000000 osm_easy_api-0.4.1/src/osm_easy_api/diff/__init__.py
+-rw-rw-rw-   0        0        0     6164 2023-04-01 19:34:36.000000 osm_easy_api-0.4.1/src/osm_easy_api/diff/diff.py
+-rw-rw-rw-   0        0        0     9075 2023-03-07 21:24:24.000000 osm_easy_api-0.4.1/src/osm_easy_api/diff/diff_parser.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 21:14:41.000000 osm_easy_api-0.4.1/src/osm_easy_api/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-23 19:15:56.550477 osm_easy_api-0.4.1/src/osm_easy_api/utils/
+-rw-rw-rw-   0        0        0       82 2023-03-07 21:14:41.000000 osm_easy_api-0.4.1/src/osm_easy_api/utils/__init__.py
+-rw-rw-rw-   0        0        0      166 2023-03-07 21:14:41.000000 osm_easy_api-0.4.1/src/osm_easy_api/utils/join_url.py
+-rw-rw-rw-   0        0        0      397 2023-03-07 21:14:41.000000 osm_easy_api-0.4.1/src/osm_easy_api/utils/write_gzip_to_file.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:15:56.507682 osm_easy_api-0.4.1/src/osm_easy_api.egg-info/
+-rw-rw-rw-   0        0        0    44069 2023-05-23 19:15:56.000000 osm_easy_api-0.4.1/src/osm_easy_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2023-05-23 19:15:56.000000 osm_easy_api-0.4.1/src/osm_easy_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 19:15:56.000000 osm_easy_api-0.4.1/src/osm_easy_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-07 21:15:07.000000 osm_easy_api-0.4.1/src/osm_easy_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       90 2023-05-23 19:15:56.000000 osm_easy_api-0.4.1/src/osm_easy_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-23 19:15:56.000000 osm_easy_api-0.4.1/src/osm_easy_api.egg-info/top_level.txt
```

### Comparing `osm_easy_api-0.4.0/CHANGELOG.md` & `osm_easy_api-0.4.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.4.1]
+### Changed
+- Updated `requests` from `2.28.1` to `2.31.0`.
+
 ## [0.4.0]
 ### Added
 - `to_dict()` method and `from_dict()` class method to `Note`.  
 - `to_dict()` method and `from_dict()` class method to `Comment`.
 - `to_dict()` method and `from_dict()` class method to `User`.
 - Documentation about `Meta` and `Action` class.
 - Assert error (with information to report it on github) when api returns an error code not described on the wiki.
```

### Comparing `osm_easy_api-0.4.0/LICENSE.md` & `osm_easy_api-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/PKG-INFO` & `osm_easy_api-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm_easy_api
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python package for parsing osm diffs and communicating with the osm api.
 Home-page: https://github.com/docentYT/osm_easy_api
 License: GPLv3
 Keywords: openstreetmap,osm,api,wrapper,diff
 Platform: unix
 Platform: linux
 Platform: osx
@@ -153,23 +153,27 @@
     print(node.id)
 ```
 but it can consume large amounts of ram and use of this method is not recommended for large diff's.
 
 # Tests
 
 You will need to install `test-requirements.txt`. You can use tox.
-To run tests manually use `python -m unittest discover` or `run_tests_<module>.bat`.
+To run tests manually use `python -m unittest discover`.
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.4.1]
+### Changed
+- Updated `requests` from `2.28.1` to `2.31.0`.
+
 ## [0.4.0]
 ### Added
 - `to_dict()` method and `from_dict()` class method to `Note`.  
 - `to_dict()` method and `from_dict()` class method to `Comment`.
 - `to_dict()` method and `from_dict()` class method to `User`.
 - Documentation about `Meta` and `Action` class.
 - Assert error (with information to report it on github) when api returns an error code not described on the wiki.
```

### Comparing `osm_easy_api-0.4.0/README.md` & `osm_easy_api-0.4.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -128,8 +128,8 @@
     print(node.id)
 ```
 but it can consume large amounts of ram and use of this method is not recommended for large diff's.
 
 # Tests
 
 You will need to install `test-requirements.txt`. You can use tox.
-To run tests manually use `python -m unittest discover` or `run_tests_<module>.bat`.
+To run tests manually use `python -m unittest discover`.
```

### Comparing `osm_easy_api-0.4.0/setup.cfg` & `osm_easy_api-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/api/_URLs.py` & `osm_easy_api-0.4.1/src/osm_easy_api/api/_URLs.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/api/api.py` & `osm_easy_api-0.4.1/src/osm_easy_api/api/api.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/__init__.py` & `osm_easy_api-0.4.1/src/osm_easy_api/api/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/changeset.py` & `osm_easy_api-0.4.1/src/osm_easy_api/api/endpoints/changeset.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/changeset_discussion.py` & `osm_easy_api-0.4.1/src/osm_easy_api/api/endpoints/changeset_discussion.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/elements.py` & `osm_easy_api-0.4.1/src/osm_easy_api/api/endpoints/elements.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/gpx.py` & `osm_easy_api-0.4.1/src/osm_easy_api/api/endpoints/gpx.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/misc.py` & `osm_easy_api-0.4.1/src/osm_easy_api/api/endpoints/misc.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/notes.py` & `osm_easy_api-0.4.1/src/osm_easy_api/api/endpoints/notes.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/api/endpoints/user.py` & `osm_easy_api-0.4.1/src/osm_easy_api/api/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/api/exceptions.py` & `osm_easy_api-0.4.1/src/osm_easy_api/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/data_classes/OsmChange.py` & `osm_easy_api-0.4.1/src/osm_easy_api/data_classes/OsmChange.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/data_classes/changeset.py` & `osm_easy_api-0.4.1/src/osm_easy_api/data_classes/changeset.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/data_classes/node.py` & `osm_easy_api-0.4.1/src/osm_easy_api/data_classes/node.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/data_classes/note.py` & `osm_easy_api-0.4.1/src/osm_easy_api/data_classes/note.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/data_classes/osm_object_primitive.py` & `osm_easy_api-0.4.1/src/osm_easy_api/data_classes/osm_object_primitive.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/data_classes/relation.py` & `osm_easy_api-0.4.1/src/osm_easy_api/data_classes/relation.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/data_classes/tags.py` & `osm_easy_api-0.4.1/src/osm_easy_api/data_classes/tags.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/data_classes/user.py` & `osm_easy_api-0.4.1/src/osm_easy_api/data_classes/user.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/data_classes/way.py` & `osm_easy_api-0.4.1/src/osm_easy_api/data_classes/way.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/diff/diff.py` & `osm_easy_api-0.4.1/src/osm_easy_api/diff/diff.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api/diff/diff_parser.py` & `osm_easy_api-0.4.1/src/osm_easy_api/diff/diff_parser.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api.egg-info/PKG-INFO` & `osm_easy_api-0.4.1/src/osm_easy_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm-easy-api
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python package for parsing osm diffs and communicating with the osm api.
 Home-page: https://github.com/docentYT/osm_easy_api
 License: GPLv3
 Keywords: openstreetmap,osm,api,wrapper,diff
 Platform: unix
 Platform: linux
 Platform: osx
@@ -153,23 +153,27 @@
     print(node.id)
 ```
 but it can consume large amounts of ram and use of this method is not recommended for large diff's.
 
 # Tests
 
 You will need to install `test-requirements.txt`. You can use tox.
-To run tests manually use `python -m unittest discover` or `run_tests_<module>.bat`.
+To run tests manually use `python -m unittest discover`.
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.4.1]
+### Changed
+- Updated `requests` from `2.28.1` to `2.31.0`.
+
 ## [0.4.0]
 ### Added
 - `to_dict()` method and `from_dict()` class method to `Note`.  
 - `to_dict()` method and `from_dict()` class method to `Comment`.
 - `to_dict()` method and `from_dict()` class method to `User`.
 - Documentation about `Meta` and `Action` class.
 - Assert error (with information to report it on github) when api returns an error code not described on the wiki.
```

### Comparing `osm_easy_api-0.4.0/src/osm_easy_api.egg-info/SOURCES.txt` & `osm_easy_api-0.4.1/src/osm_easy_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

