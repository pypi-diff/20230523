# Comparing `tmp/nerevu-api-utils-0.0.3.tar.gz` & `tmp/nerevu-api-utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerevu-api-utils-0.0.3.tar", last modified: Thu Feb 24 08:23:29 2022, max compression
+gzip compressed data, was "nerevu-api-utils-0.0.4.tar", last modified: Mon May 22 23:34:54 2023, max compression
```

## Comparing `nerevu-api-utils-0.0.3.tar` & `nerevu-api-utils-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 reubano    (502) staff       (20)        0 2022-02-24 08:23:29.300920 nerevu-api-utils-0.0.3/
--rw-r--r--   0 reubano    (502) staff       (20)     1083 2022-02-24 00:54:13.000000 nerevu-api-utils-0.0.3/LICENSE
--rw-r--r--   0 reubano    (502) staff       (20)       66 2021-12-23 00:48:19.000000 nerevu-api-utils-0.0.3/MANIFEST.in
--rw-r--r--   0 reubano    (502) staff       (20)     1295 2022-02-24 08:23:29.300991 nerevu-api-utils-0.0.3/PKG-INFO
--rw-r--r--   0 reubano    (502) staff       (20)    19570 2022-02-24 08:23:21.000000 nerevu-api-utils-0.0.3/api_utils.py
--rw-r--r--   0 reubano    (502) staff       (20)      280 2022-02-24 04:17:56.000000 nerevu-api-utils-0.0.3/dev-requirements.txt
-drwxr-xr-x   0 reubano    (502) staff       (20)        0 2022-02-24 08:23:29.300492 nerevu-api-utils-0.0.3/nerevu_api_utils.egg-info/
--rw-r--r--   0 reubano    (502) staff       (20)     1295 2022-02-24 08:23:29.000000 nerevu-api-utils-0.0.3/nerevu_api_utils.egg-info/PKG-INFO
--rw-r--r--   0 reubano    (502) staff       (20)      391 2022-02-24 08:23:29.000000 nerevu-api-utils-0.0.3/nerevu_api_utils.egg-info/SOURCES.txt
--rw-r--r--   0 reubano    (502) staff       (20)        1 2022-02-24 08:23:29.000000 nerevu-api-utils-0.0.3/nerevu_api_utils.egg-info/dependency_links.txt
--rw-r--r--   0 reubano    (502) staff       (20)        1 2022-02-24 08:23:29.000000 nerevu-api-utils-0.0.3/nerevu_api_utils.egg-info/not-zip-safe
--rw-r--r--   0 reubano    (502) staff       (20)      372 2022-02-24 08:23:29.000000 nerevu-api-utils-0.0.3/nerevu_api_utils.egg-info/requires.txt
--rw-r--r--   0 reubano    (502) staff       (20)       10 2022-02-24 08:23:29.000000 nerevu-api-utils-0.0.3/nerevu_api_utils.egg-info/top_level.txt
--rw-r--r--   0 reubano    (502) staff       (20)      287 2022-02-24 04:09:18.000000 nerevu-api-utils-0.0.3/pyproject.toml
--rw-r--r--   0 reubano    (502) staff       (20)       81 2022-02-24 04:22:41.000000 nerevu-api-utils-0.0.3/requirements.txt
--rw-r--r--   0 reubano    (502) staff       (20)      461 2022-02-24 08:23:29.301252 nerevu-api-utils-0.0.3/setup.cfg
--rwxr-xr-x   0 reubano    (502) staff       (20)     2219 2022-02-24 06:37:30.000000 nerevu-api-utils-0.0.3/setup.py
-drwxr-xr-x   0 reubano    (502) staff       (20)        0 2022-02-24 08:23:29.300829 nerevu-api-utils-0.0.3/tests/
--rw-r--r--   0 reubano    (502) staff       (20)     6148 2015-06-12 14:55:05.000000 nerevu-api-utils-0.0.3/tests/.DS_Store
--rw-r--r--   0 reubano    (502) staff       (20)     6647 2021-12-23 01:02:03.000000 nerevu-api-utils-0.0.3/tests/pylintrc
--rw-r--r--   0 reubano    (502) staff       (20)     6486 2015-12-28 09:44:47.000000 nerevu-api-utils-0.0.3/tests/standard.rc
+drwxr-xr-x   0 reubano    (502) staff       (20)        0 2023-05-22 23:34:54.721634 nerevu-api-utils-0.0.4/
+-rw-r--r--   0 reubano    (502) staff       (20)     1083 2022-02-24 00:54:13.000000 nerevu-api-utils-0.0.4/LICENSE
+-rw-r--r--   0 reubano    (502) staff       (20)       66 2021-12-23 00:48:19.000000 nerevu-api-utils-0.0.4/MANIFEST.in
+-rw-r--r--   0 reubano    (502) staff       (20)     1295 2023-05-22 23:34:54.721721 nerevu-api-utils-0.0.4/PKG-INFO
+-rw-r--r--   0 reubano    (502) staff       (20)    19869 2023-05-22 23:34:26.000000 nerevu-api-utils-0.0.4/api_utils.py
+-rw-r--r--   0 reubano    (502) staff       (20)      280 2022-02-24 04:17:56.000000 nerevu-api-utils-0.0.4/dev-requirements.txt
+drwxr-xr-x   0 reubano    (502) staff       (20)        0 2023-05-22 23:34:54.720521 nerevu-api-utils-0.0.4/nerevu_api_utils.egg-info/
+-rw-r--r--   0 reubano    (502) staff       (20)     1295 2023-05-22 23:34:54.000000 nerevu-api-utils-0.0.4/nerevu_api_utils.egg-info/PKG-INFO
+-rw-r--r--   0 reubano    (502) staff       (20)      391 2023-05-22 23:34:54.000000 nerevu-api-utils-0.0.4/nerevu_api_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 reubano    (502) staff       (20)        1 2023-05-22 23:34:54.000000 nerevu-api-utils-0.0.4/nerevu_api_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 reubano    (502) staff       (20)        1 2023-05-22 23:34:54.000000 nerevu-api-utils-0.0.4/nerevu_api_utils.egg-info/not-zip-safe
+-rw-r--r--   0 reubano    (502) staff       (20)      372 2023-05-22 23:34:54.000000 nerevu-api-utils-0.0.4/nerevu_api_utils.egg-info/requires.txt
+-rw-r--r--   0 reubano    (502) staff       (20)       10 2023-05-22 23:34:54.000000 nerevu-api-utils-0.0.4/nerevu_api_utils.egg-info/top_level.txt
+-rw-r--r--   0 reubano    (502) staff       (20)      287 2022-02-24 04:09:18.000000 nerevu-api-utils-0.0.4/pyproject.toml
+-rw-r--r--   0 reubano    (502) staff       (20)       81 2023-05-22 23:34:26.000000 nerevu-api-utils-0.0.4/requirements.txt
+-rw-r--r--   0 reubano    (502) staff       (20)      461 2023-05-22 23:34:54.722000 nerevu-api-utils-0.0.4/setup.cfg
+-rwxr-xr-x   0 reubano    (502) staff       (20)     2219 2023-05-22 23:34:14.000000 nerevu-api-utils-0.0.4/setup.py
+drwxr-xr-x   0 reubano    (502) staff       (20)        0 2023-05-22 23:34:54.721383 nerevu-api-utils-0.0.4/tests/
+-rw-r--r--   0 reubano    (502) staff       (20)     6148 2015-06-12 14:55:05.000000 nerevu-api-utils-0.0.4/tests/.DS_Store
+-rw-r--r--   0 reubano    (502) staff       (20)     6647 2021-12-23 01:02:03.000000 nerevu-api-utils-0.0.4/tests/pylintrc
+-rw-r--r--   0 reubano    (502) staff       (20)     6486 2015-12-28 09:44:47.000000 nerevu-api-utils-0.0.4/tests/standard.rc
```

### Comparing `nerevu-api-utils-0.0.3/LICENSE` & `nerevu-api-utils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nerevu-api-utils-0.0.3/PKG-INFO` & `nerevu-api-utils-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: nerevu-api-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Flask API utility library
 Home-page: https://github.com/reubano/nerevu-api-utils
 Author: Reuben Cummings
 Author-email: reubano@gmail.com
 License: MIT
-Download-URL: https://github.com/reubano/nerevu-api-utils/archive/v0.0.3.tar.gz
+Download-URL: https://github.com/reubano/nerevu-api-utils/archive/v0.0.4.tar.gz
 Keywords: nerevu-api-utils,Flask,API,utility,library
 Platform: MacOS X
 Platform: Windows
 Platform: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `nerevu-api-utils-0.0.3/api_utils.py` & `nerevu-api-utils-0.0.4/api_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Attributes:
     LICENSES (dict): available python license classifiers.
 """
 import re
 from uuid import uuid4
 from hashlib import md5
-from datetime import datetime as dt, date, timedelta
+from datetime import datetime as dt, date, timedelta, timezone
 from functools import wraps, partial
 from json import loads, dumps
 from ast import literal_eval
 from os import path, listdir
 from inspect import isclass, getmembers
 from importlib import import_module
 from http.client import responses
@@ -28,15 +28,15 @@
 from meza import convert as cv, fntools as ft
 from sqlalchemy import event
 from sqlalchemy.inspection import inspect as sqlalchemy_inspect
 
 
 import inflect
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 __title__ = "nerevu-api-utils"
 __author__ = "Reuben Cummings"
 __description__ = "Flask API utility library"
 __email__ = "reubano@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022 Reuben Cummings"
@@ -170,15 +170,21 @@
             else:
                 # because some browsers don't respect the spec and treat no-cache like
                 # it was no-store (I'm looking at you chrome!)
                 response.cache_control.must_revalidate = True
 
             if _max_age and request.method == "GET":
                 extra = timedelta(seconds=_max_age)
-                response.expires = (response.last_modified or dt.utcnow()) + extra
+
+                if not (last_requested := response.last_modified):
+                    response_json = response.get_json() or {}
+                    timestamp = response_json.get("utc_requested", dt.now(timezone.utc).timestamp())
+                    last_requested = dt.fromtimestamp(timestamp, tz=timezone.utc)
+
+                response.expires = last_requested + extra
                 response.cache_control.public = True
                 response.add_etag()
 
                 if refresh_period:
                     # TODO: set stale-while-revalidate and stale-if-error
                     pass
             else:
```

### Comparing `nerevu-api-utils-0.0.3/nerevu_api_utils.egg-info/PKG-INFO` & `nerevu-api-utils-0.0.4/nerevu_api_utils.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: nerevu-api-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Flask API utility library
 Home-page: https://github.com/reubano/nerevu-api-utils
 Author: Reuben Cummings
 Author-email: reubano@gmail.com
 License: MIT
-Download-URL: https://github.com/reubano/nerevu-api-utils/archive/v0.0.3.tar.gz
+Download-URL: https://github.com/reubano/nerevu-api-utils/archive/v0.0.4.tar.gz
 Keywords: nerevu-api-utils,Flask,API,utility,library
 Platform: MacOS X
 Platform: Windows
 Platform: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `nerevu-api-utils-0.0.3/setup.py` & `nerevu-api-utils-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `nerevu-api-utils-0.0.3/tests/.DS_Store` & `nerevu-api-utils-0.0.4/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `nerevu-api-utils-0.0.3/tests/pylintrc` & `nerevu-api-utils-0.0.4/tests/pylintrc`

 * *Files identical despite different names*

### Comparing `nerevu-api-utils-0.0.3/tests/standard.rc` & `nerevu-api-utils-0.0.4/tests/standard.rc`

 * *Files identical despite different names*

