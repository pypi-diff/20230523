# Comparing `tmp/crabpy_pyramid-1.4.0.tar.gz` & `tmp/crabpy_pyramid-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crabpy_pyramid-1.4.0.tar", last modified: Tue May  9 05:35:56 2023, max compression
+gzip compressed data, was "crabpy_pyramid-1.5.0.tar", last modified: Tue May 23 09:30:17 2023, max compression
```

## Comparing `crabpy_pyramid-1.4.0.tar` & `crabpy_pyramid-1.5.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-09 05:35:56.965313 crabpy_pyramid-1.4.0/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     4606 2023-05-09 05:35:34.000000 crabpy_pyramid-1.4.0/CHANGES.rst
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/LICENSE
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/MANIFEST.in
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6636 2023-05-09 05:35:56.969313 crabpy_pyramid-1.4.0/PKG-INFO
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1326 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/README.rst
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-09 05:35:56.965313 crabpy_pyramid-1.4.0/crabpy_pyramid/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    11605 2023-05-05 13:21:30.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/__init__.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-09 05:35:56.965313 crabpy_pyramid-1.4.0/crabpy_pyramid/renderers/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/renderers/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6935 2023-05-09 05:35:34.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/renderers/adressenregister.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3726 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/renderers/capakey.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    15765 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/renderers/crab.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-09 05:35:56.965313 crabpy_pyramid-1.4.0/crabpy_pyramid/routes/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/routes/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3498 2023-05-05 13:21:30.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/routes/adressenregister.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1901 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/routes/capakey.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     4825 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/routes/crab.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2735 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/utils.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-09 05:35:56.965313 crabpy_pyramid-1.4.0/crabpy_pyramid/views/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/views/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    11433 2023-05-09 05:35:34.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/views/adressenregister.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     5610 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/views/capakey.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    13969 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/views/crab.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      599 2023-05-05 13:21:30.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/views/exceptions.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-09 05:35:56.965313 crabpy_pyramid-1.4.0/crabpy_pyramid.egg-info/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6636 2023-05-09 05:35:56.000000 crabpy_pyramid-1.4.0/crabpy_pyramid.egg-info/PKG-INFO
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      839 2023-05-09 05:35:56.000000 crabpy_pyramid-1.4.0/crabpy_pyramid.egg-info/SOURCES.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-05-09 05:35:56.000000 crabpy_pyramid-1.4.0/crabpy_pyramid.egg-info/dependency_links.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       47 2023-05-09 05:35:56.000000 crabpy_pyramid-1.4.0/crabpy_pyramid.egg-info/entry_points.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 13:30:20.000000 crabpy_pyramid-1.4.0/crabpy_pyramid.egg-info/not-zip-safe
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       42 2023-05-09 05:35:56.000000 crabpy_pyramid-1.4.0/crabpy_pyramid.egg-info/requires.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       15 2023-05-09 05:35:56.000000 crabpy_pyramid-1.4.0/crabpy_pyramid.egg-info/top_level.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      173 2023-05-09 05:35:56.969313 crabpy_pyramid-1.4.0/setup.cfg
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1484 2023-05-09 05:35:34.000000 crabpy_pyramid-1.4.0/setup.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-23 09:30:17.489079 crabpy_pyramid-1.5.0/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     4699 2023-05-23 09:30:14.000000 crabpy_pyramid-1.5.0/CHANGES.rst
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/LICENSE
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/MANIFEST.in
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6729 2023-05-23 09:30:17.489079 crabpy_pyramid-1.5.0/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1326 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/README.rst
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-23 09:30:17.489079 crabpy_pyramid-1.5.0/crabpy_pyramid/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    11585 2023-05-23 09:30:14.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/__init__.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-23 09:30:17.489079 crabpy_pyramid-1.5.0/crabpy_pyramid/renderers/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/renderers/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6935 2023-05-09 05:35:34.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/renderers/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3726 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/renderers/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    15765 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/renderers/crab.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-23 09:30:17.489079 crabpy_pyramid-1.5.0/crabpy_pyramid/routes/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/routes/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3685 2023-05-23 09:30:14.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/routes/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1901 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/routes/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     4825 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/routes/crab.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2735 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/utils.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-23 09:30:17.489079 crabpy_pyramid-1.5.0/crabpy_pyramid/views/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/views/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    12235 2023-05-23 09:30:14.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/views/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     5610 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/views/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    13969 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/views/crab.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      599 2023-05-05 13:21:30.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/views/exceptions.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-23 09:30:17.489079 crabpy_pyramid-1.5.0/crabpy_pyramid.egg-info/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6729 2023-05-23 09:30:17.000000 crabpy_pyramid-1.5.0/crabpy_pyramid.egg-info/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      839 2023-05-23 09:30:17.000000 crabpy_pyramid-1.5.0/crabpy_pyramid.egg-info/SOURCES.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-05-23 09:30:17.000000 crabpy_pyramid-1.5.0/crabpy_pyramid.egg-info/dependency_links.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       47 2023-05-23 09:30:17.000000 crabpy_pyramid-1.5.0/crabpy_pyramid.egg-info/entry_points.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 13:30:20.000000 crabpy_pyramid-1.5.0/crabpy_pyramid.egg-info/not-zip-safe
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       42 2023-05-23 09:30:17.000000 crabpy_pyramid-1.5.0/crabpy_pyramid.egg-info/requires.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       15 2023-05-23 09:30:17.000000 crabpy_pyramid-1.5.0/crabpy_pyramid.egg-info/top_level.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      173 2023-05-23 09:30:17.489079 crabpy_pyramid-1.5.0/setup.cfg
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1484 2023-05-23 09:30:14.000000 crabpy_pyramid-1.5.0/setup.py
```

### Comparing `crabpy_pyramid-1.4.0/CHANGES.rst` & `crabpy_pyramid-1.5.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+1.5.0 (23-05-2023)
+------------------
+
+- Nice to haves (#184)
+- Support voor py3.10+ (#187)
+
 1.4.0 (09-05-2023)
 ------------------
 
 - Adressenregister fixes (#179)
 - Verschil tss return HttpNotfound en raise HttpNotfound wegwerken (#178)
 
 1.3.0 (05-05-2023)
```

### Comparing `crabpy_pyramid-1.4.0/LICENSE` & `crabpy_pyramid-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.4.0/PKG-INFO` & `crabpy_pyramid-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crabpy_pyramid
-Version: 1.4.0
+Version: 1.5.0
 Summary: Bindings for the CRABpy webservices and the Pyramid framework.
 Home-page: http://github.com/OnroerendErfgoed/crabpy_pyramid
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Keywords: web wsgi pyramid CRAB CAPAKEY AGIV
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,20 @@
     # activate your virtual env
     $ pip install sphinx sphinxcontrib-httpdomain
     $ python setup.py develop
     $ cd docs
     $ make html
 
 
+1.5.0 (23-05-2023)
+------------------
+
+- Nice to haves (#184)
+- Support voor py3.10+ (#187)
+
 1.4.0 (09-05-2023)
 ------------------
 
 - Adressenregister fixes (#179)
 - Verschil tss return HttpNotfound en raise HttpNotfound wegwerken (#178)
 
 1.3.0 (05-05-2023)
```

### Comparing `crabpy_pyramid-1.4.0/README.rst` & `crabpy_pyramid-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.4.0/crabpy_pyramid/__init__.py` & `crabpy_pyramid-1.5.0/crabpy_pyramid/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-# -*- coding: utf-8 -*-
-
 import logging
 import os
-from collections import Sequence
+from  collections.abc import Sequence
 
 from crabpy.client import AdressenRegisterClient
 from crabpy.client import crab_factory
 from crabpy.gateway.adressenregister import Gateway
 from crabpy.gateway.capakey import CapakeyRestGateway
 from crabpy.gateway.crab import CrabGateway
 from pyramid.config import Configurator
```

### Comparing `crabpy_pyramid-1.4.0/crabpy_pyramid/renderers/adressenregister.py` & `crabpy_pyramid-1.5.0/crabpy_pyramid/renderers/adressenregister.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.4.0/crabpy_pyramid/renderers/capakey.py` & `crabpy_pyramid-1.5.0/crabpy_pyramid/renderers/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.4.0/crabpy_pyramid/renderers/crab.py` & `crabpy_pyramid-1.5.0/crabpy_pyramid/renderers/crab.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.4.0/crabpy_pyramid/routes/adressenregister.py` & `crabpy_pyramid-1.5.0/crabpy_pyramid/routes/adressenregister.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,19 +94,23 @@
         "/adressenregister/adressen/{adres_id}/percelen",
     )
     crabpy_pyramid.add_route(
         config,
         "adressenregister_get_perceel_by_id",
         "/adressenregister/percelen/{perceel_id}",
     )
-
+    crabpy_pyramid.add_route(
+        config,
+        "adressenregister_get_perceel_by_id_parts",
+        "/adressenregister/percelen/{perceel_id_part1}/{perceel_id_part2}",
+    )
     crabpy_pyramid.add_route(
         config,
         "adressenregister_list_postinfo_by_gemeente",
-        "/adressenregister/gemeenten/{gemeente_naam}/postinfo",
+        "/adressenregister/gemeenten/{gemeente_naam_niscode}/postinfo",
     )
     crabpy_pyramid.add_route(
         config,
         "adressenregister_get_postinfo_by_postcode",
         "/adressenregister/postinfo/{postcode}",
     )
```

### Comparing `crabpy_pyramid-1.4.0/crabpy_pyramid/routes/capakey.py` & `crabpy_pyramid-1.5.0/crabpy_pyramid/routes/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.4.0/crabpy_pyramid/routes/crab.py` & `crabpy_pyramid-1.5.0/crabpy_pyramid/routes/crab.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.4.0/crabpy_pyramid/utils.py` & `crabpy_pyramid-1.5.0/crabpy_pyramid/utils.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.4.0/crabpy_pyramid/views/adressenregister.py` & `crabpy_pyramid-1.5.0/crabpy_pyramid/views/adressenregister.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import re
 
 import pycountry
 from crabpy.client import AdressenRegisterClientException
 from pyramid.httpexceptions import HTTPBadRequest
 from pyramid.httpexceptions import HTTPNotFound
 from pyramid.view import view_config
 
@@ -288,24 +289,45 @@
     request = set_http_caching(request, "adressenregister", "short")
     Gateway = request.adressenregister_gateway()
     perceel_id = request.matchdict.get("perceel_id")
     return handle_gateway_response(Gateway.get_perceel_by_id, perceel_id=perceel_id)
 
 
 @view_config(
+    route_name="adressenregister_get_perceel_by_id_parts",
+    renderer="adresreg_itemjson",
+    accept="application/json",
+)
+def adressenregister_get_perceel_by_id_parts(request):
+    request = set_http_caching(request, "adressenregister", "short")
+    Gateway = request.adressenregister_gateway()
+    perceel_id = (
+        f'{request.matchdict.get("perceel_id_part1")}'
+        f'-{request.matchdict.get("perceel_id_part2")}'
+    )
+    return handle_gateway_response(Gateway.get_perceel_by_id, perceel_id=perceel_id)
+
+
+@view_config(
     route_name="adressenregister_list_postinfo_by_gemeente",
     renderer="adresreg_listjson",
     accept="application/json",
 )
 def adressenregister_list_postinfo_by_gemeente(request):
     request = set_http_caching(request, "adressenregister", "long")
     Gateway = request.adressenregister_gateway()
-    gemeente_naam = request.matchdict.get("gemeente_naam")
+    gemeente_param = request.matchdict.get("gemeente_naam_niscode")
+    niscode_pattern = re.compile(r"^\d{5}$")
+    if niscode_pattern.match(gemeente_param):
+        gemeente = handle_gateway_response(
+            Gateway.get_gemeente_by_niscode, gemeente_param
+        )
+        gemeente_param = gemeente.naam()
     adressen = handle_gateway_response(
-        Gateway.get_postinfo_by_gemeentenaam, gemeente_naam
+        Gateway.get_postinfo_by_gemeentenaam, gemeente_param
     )
 
     return range_return(request, adressen)
 
 
 @view_config(
     route_name="adressenregister_get_postinfo_by_postcode",
```

### Comparing `crabpy_pyramid-1.4.0/crabpy_pyramid/views/capakey.py` & `crabpy_pyramid-1.5.0/crabpy_pyramid/views/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.4.0/crabpy_pyramid/views/crab.py` & `crabpy_pyramid-1.5.0/crabpy_pyramid/views/crab.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.4.0/crabpy_pyramid/views/exceptions.py` & `crabpy_pyramid-1.5.0/crabpy_pyramid/views/exceptions.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.4.0/crabpy_pyramid.egg-info/PKG-INFO` & `crabpy_pyramid-1.5.0/crabpy_pyramid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crabpy-pyramid
-Version: 1.4.0
+Version: 1.5.0
 Summary: Bindings for the CRABpy webservices and the Pyramid framework.
 Home-page: http://github.com/OnroerendErfgoed/crabpy_pyramid
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Keywords: web wsgi pyramid CRAB CAPAKEY AGIV
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,20 @@
     # activate your virtual env
     $ pip install sphinx sphinxcontrib-httpdomain
     $ python setup.py develop
     $ cd docs
     $ make html
 
 
+1.5.0 (23-05-2023)
+------------------
+
+- Nice to haves (#184)
+- Support voor py3.10+ (#187)
+
 1.4.0 (09-05-2023)
 ------------------
 
 - Adressenregister fixes (#179)
 - Verschil tss return HttpNotfound en raise HttpNotfound wegwerken (#178)
 
 1.3.0 (05-05-2023)
```

### Comparing `crabpy_pyramid-1.4.0/crabpy_pyramid.egg-info/SOURCES.txt` & `crabpy_pyramid-1.5.0/crabpy_pyramid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.4.0/setup.py` & `crabpy_pyramid-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     'coverage',
     'webtest'
 ]
 
 testing_extras = tests_requires + []
 
 setup(name='crabpy_pyramid',
-      version='1.4.0',
+      version='1.5.0',
       description='Bindings for the CRABpy webservices and the Pyramid framework.',
       long_description=README + '\n\n' + CHANGES,
       classifiers=[
         'Development Status :: 5 - Production/Stable',
         "Programming Language :: Python",
         'Programming Language :: Python :: 3.8',
         "Framework :: Pyramid",
```

