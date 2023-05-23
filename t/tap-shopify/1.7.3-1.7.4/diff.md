# Comparing `tmp/tap-shopify-1.7.3.tar.gz` & `tmp/tap-shopify-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-shopify-1.7.3.tar", last modified: Wed May 10 10:05:31 2023, max compression
+gzip compressed data, was "tap-shopify-1.7.4.tar", last modified: Tue May 23 12:34:07 2023, max compression
```

## Comparing `tap-shopify-1.7.3.tar` & `tap-shopify-1.7.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 10:05:31.395802 tap-shopify-1.7.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32387 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      329 2023-05-10 10:05:31.395802 tap-shopify-1.7.3/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2548 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-05-10 10:05:31.395802 tap-shopify-1.7.3/setup.cfg
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      840 2023-05-10 09:42:36.000000 tap-shopify-1.7.3/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 10:05:31.391802 tap-shopify-1.7.3/tap_shopify/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8700 2023-05-04 18:16:17.000000 tap-shopify-1.7.3/tap_shopify/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1321 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/context.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      143 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/exceptions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 10:05:31.395802 tap-shopify-1.7.3/tap_shopify/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10539 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/schemas/abandoned_checkouts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      690 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/schemas/collects.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1518 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/schemas/custom_collections.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       43 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/schemas/customers.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27088 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/schemas/definitions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1147 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/schemas/events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1577 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/schemas/inventory_items.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      394 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/schemas/inventory_levels.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       43 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/schemas/locations.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1160 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/schemas/metafields.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20799 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/schemas/order_refunds.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23571 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/schemas/orders.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6059 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/schemas/products.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3294 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/schemas/transactions.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 10:05:31.395802 tap-shopify-1.7.3/tap_shopify/streams/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      513 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      277 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/abandoned_checkouts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13353 2023-05-10 09:42:36.000000 tap-shopify-1.7.3/tap_shopify/streams/base.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1873 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/collects.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      283 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/custom_collections.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      241 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/customers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/events.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2037 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/inventory_items.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2486 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/inventory_levels.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1381 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/locations.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3810 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/streams/metafields.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2583 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/streams/order_refunds.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/orders.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      272 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/products.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3513 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/streams/transactions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 10:05:31.391802 tap-shopify-1.7.3/tap_shopify.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      329 2023-05-10 10:05:31.000000 tap-shopify-1.7.3/tap_shopify.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1378 2023-05-10 10:05:31.000000 tap-shopify-1.7.3/tap_shopify.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-10 10:05:31.000000 tap-shopify-1.7.3/tap_shopify.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       60 2023-05-10 10:05:31.000000 tap-shopify-1.7.3/tap_shopify.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       89 2023-05-10 10:05:31.000000 tap-shopify-1.7.3/tap_shopify.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2023-05-10 10:05:31.000000 tap-shopify-1.7.3/tap_shopify.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-23 12:34:07.052371 tap-shopify-1.7.4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32387 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      329 2023-05-23 12:34:07.052371 tap-shopify-1.7.4/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2548 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-05-23 12:34:07.052371 tap-shopify-1.7.4/setup.cfg
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      840 2023-05-23 12:23:15.000000 tap-shopify-1.7.4/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-23 12:34:07.048371 tap-shopify-1.7.4/tap_shopify/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8700 2023-05-04 18:16:17.000000 tap-shopify-1.7.4/tap_shopify/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1321 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/tap_shopify/context.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      143 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/tap_shopify/exceptions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-23 12:34:07.052371 tap-shopify-1.7.4/tap_shopify/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10539 2023-05-04 05:21:45.000000 tap-shopify-1.7.4/tap_shopify/schemas/abandoned_checkouts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      690 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/tap_shopify/schemas/collects.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1518 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/tap_shopify/schemas/custom_collections.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       43 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/tap_shopify/schemas/customers.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27088 2023-05-04 05:21:45.000000 tap-shopify-1.7.4/tap_shopify/schemas/definitions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1147 2023-05-04 05:21:45.000000 tap-shopify-1.7.4/tap_shopify/schemas/events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1577 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/tap_shopify/schemas/inventory_items.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      394 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/tap_shopify/schemas/inventory_levels.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       43 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/tap_shopify/schemas/locations.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1160 2023-05-04 05:21:45.000000 tap-shopify-1.7.4/tap_shopify/schemas/metafields.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20799 2023-05-04 05:21:45.000000 tap-shopify-1.7.4/tap_shopify/schemas/order_refunds.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23571 2023-05-04 05:21:45.000000 tap-shopify-1.7.4/tap_shopify/schemas/orders.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6059 2023-05-04 05:21:45.000000 tap-shopify-1.7.4/tap_shopify/schemas/products.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3294 2023-05-04 05:21:45.000000 tap-shopify-1.7.4/tap_shopify/schemas/transactions.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-23 12:34:07.052371 tap-shopify-1.7.4/tap_shopify/streams/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      513 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/tap_shopify/streams/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      277 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/tap_shopify/streams/abandoned_checkouts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13574 2023-05-23 12:23:15.000000 tap-shopify-1.7.4/tap_shopify/streams/base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1873 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/tap_shopify/streams/collects.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      283 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/tap_shopify/streams/custom_collections.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      241 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/tap_shopify/streams/customers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/tap_shopify/streams/events.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2037 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/tap_shopify/streams/inventory_items.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2486 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/tap_shopify/streams/inventory_levels.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1381 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/tap_shopify/streams/locations.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3810 2023-05-04 05:21:45.000000 tap-shopify-1.7.4/tap_shopify/streams/metafields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2583 2023-05-04 05:21:45.000000 tap-shopify-1.7.4/tap_shopify/streams/order_refunds.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/tap_shopify/streams/orders.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      272 2023-01-25 09:00:08.000000 tap-shopify-1.7.4/tap_shopify/streams/products.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3513 2023-05-04 05:21:45.000000 tap-shopify-1.7.4/tap_shopify/streams/transactions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-23 12:34:07.048371 tap-shopify-1.7.4/tap_shopify.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      329 2023-05-23 12:34:06.000000 tap-shopify-1.7.4/tap_shopify.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1378 2023-05-23 12:34:07.000000 tap-shopify-1.7.4/tap_shopify.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-23 12:34:06.000000 tap-shopify-1.7.4/tap_shopify.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       60 2023-05-23 12:34:06.000000 tap-shopify-1.7.4/tap_shopify.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       89 2023-05-23 12:34:06.000000 tap-shopify-1.7.4/tap_shopify.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2023-05-23 12:34:06.000000 tap-shopify-1.7.4/tap_shopify.egg-info/top_level.txt
```

### Comparing `tap-shopify-1.7.3/LICENSE` & `tap-shopify-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/README.md` & `tap-shopify-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/setup.py` & `tap-shopify-1.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="tap-shopify",
-    version="1.7.3",
+    version="1.7.4",
     description="Singer.io tap for extracting Shopify data",
     author="Stitch",
     url="http://github.com/singer-io/tap-shopify",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     python_requires='>=3.5.2',
     py_modules=["tap_shopify"],
     install_requires=[
```

### Comparing `tap-shopify-1.7.3/tap_shopify/__init__.py` & `tap-shopify-1.7.4/tap_shopify/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify/context.py` & `tap-shopify-1.7.4/tap_shopify/context.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify/schemas/abandoned_checkouts.json` & `tap-shopify-1.7.4/tap_shopify/schemas/abandoned_checkouts.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify/schemas/collects.json` & `tap-shopify-1.7.4/tap_shopify/schemas/collects.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify/schemas/custom_collections.json` & `tap-shopify-1.7.4/tap_shopify/schemas/custom_collections.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify/schemas/definitions.json` & `tap-shopify-1.7.4/tap_shopify/schemas/definitions.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify/schemas/events.json` & `tap-shopify-1.7.4/tap_shopify/schemas/events.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify/schemas/inventory_items.json` & `tap-shopify-1.7.4/tap_shopify/schemas/inventory_items.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify/schemas/metafields.json` & `tap-shopify-1.7.4/tap_shopify/schemas/metafields.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify/schemas/order_refunds.json` & `tap-shopify-1.7.4/tap_shopify/schemas/order_refunds.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify/schemas/orders.json` & `tap-shopify-1.7.4/tap_shopify/schemas/orders.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify/schemas/products.json` & `tap-shopify-1.7.4/tap_shopify/schemas/products.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify/schemas/transactions.json` & `tap-shopify-1.7.4/tap_shopify/schemas/transactions.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify/streams/__init__.py` & `tap-shopify-1.7.4/tap_shopify/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify/streams/base.py` & `tap-shopify-1.7.4/tap_shopify/streams/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 import functools
 import math
 import sys
 import socket
 from urllib.error import URLError
+import http
 import backoff
 import pyactiveresource
 import pyactiveresource.formats
 import simplejson
 import singer
 from singer import metrics, utils
 from singer.utils import strptime_to_utc
@@ -116,14 +117,18 @@
     """
     # retry if the error string contains 'timed out'
     if str(error_raised).__contains__('timed out'):
         return False
     return True
 
 def shopify_error_handling(fnc):
+    @backoff.on_exception(backoff.expo, # IncompleteRead error raised
+                          http.client.IncompleteRead,
+                          max_tries=MAX_RETRIES,
+                          factor=2)
     @backoff.on_exception(backoff.expo, # timeout error raise by Shopify
                           (pyactiveresource.connection.Error, socket.timeout),
                           giveup=is_timeout_error,
                           max_tries=MAX_RETRIES,
                           factor=2)
     @backoff.on_exception(backoff.expo,
                           (pyactiveresource.connection.ServerError,
```

### Comparing `tap-shopify-1.7.3/tap_shopify/streams/collects.py` & `tap-shopify-1.7.4/tap_shopify/streams/collects.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify/streams/events.py` & `tap-shopify-1.7.4/tap_shopify/streams/events.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify/streams/inventory_items.py` & `tap-shopify-1.7.4/tap_shopify/streams/inventory_items.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify/streams/inventory_levels.py` & `tap-shopify-1.7.4/tap_shopify/streams/inventory_levels.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify/streams/locations.py` & `tap-shopify-1.7.4/tap_shopify/streams/locations.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify/streams/metafields.py` & `tap-shopify-1.7.4/tap_shopify/streams/metafields.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify/streams/order_refunds.py` & `tap-shopify-1.7.4/tap_shopify/streams/order_refunds.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify/streams/transactions.py` & `tap-shopify-1.7.4/tap_shopify/streams/transactions.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.3/tap_shopify.egg-info/SOURCES.txt` & `tap-shopify-1.7.4/tap_shopify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

