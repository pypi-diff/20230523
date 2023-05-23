# Comparing `tmp/chartmogul-3.1.1.tar.gz` & `tmp/chartmogul-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartmogul-3.1.1.tar", last modified: Mon Apr  3 12:43:54 2023, max compression
+gzip compressed data, was "chartmogul-3.1.2.tar", last modified: Tue May 23 11:49:38 2023, max compression
```

## Comparing `chartmogul-3.1.1.tar` & `chartmogul-3.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2023-04-03 12:43:54.200749 chartmogul-3.1.1/
--rw-r--r--   0 sebastian   (501) staff       (20)     1081 2022-04-25 14:08:25.000000 chartmogul-3.1.1/LICENSE.txt
--rw-r--r--   0 sebastian   (501) staff       (20)      693 2023-04-03 12:43:54.200844 chartmogul-3.1.1/PKG-INFO
--rw-r--r--   0 sebastian   (501) staff       (20)    15660 2023-04-03 12:41:37.000000 chartmogul-3.1.1/README.md
-drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2023-04-03 12:43:54.135089 chartmogul-3.1.1/chartmogul/
--rw-r--r--   0 sebastian   (501) staff       (20)     1300 2023-04-03 12:41:37.000000 chartmogul-3.1.1/chartmogul/__init__.py
-drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2023-04-03 12:43:54.186011 chartmogul-3.1.1/chartmogul/api/
--rw-r--r--   0 sebastian   (501) staff       (20)       85 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/api/__init__.py
--rw-r--r--   0 sebastian   (501) staff       (20)      648 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/api/account.py
--rw-r--r--   0 sebastian   (501) staff       (20)     1880 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/api/activities_export.py
--rw-r--r--   0 sebastian   (501) staff       (20)     1365 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/api/activity.py
--rw-r--r--   0 sebastian   (501) staff       (20)      551 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/api/attributes.py
--rw-r--r--   0 sebastian   (501) staff       (20)      361 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/api/config.py
--rw-r--r--   0 sebastian   (501) staff       (20)     1321 2023-04-03 12:41:37.000000 chartmogul-3.1.1/chartmogul/api/contact.py
--rw-r--r--   0 sebastian   (501) staff       (20)     1116 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/api/custom_attrs.py
--rw-r--r--   0 sebastian   (501) staff       (20)     3224 2023-04-03 12:41:37.000000 chartmogul-3.1.1/chartmogul/api/customer.py
-drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2023-04-03 12:43:54.192939 chartmogul-3.1.1/chartmogul/api/customers/
--rw-r--r--   0 sebastian   (501) staff       (20)       51 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/api/customers/__init__.py
--rw-r--r--   0 sebastian   (501) staff       (20)     1101 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/api/customers/activity.py
--rw-r--r--   0 sebastian   (501) staff       (20)     2770 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/api/customers/subscription.py
--rw-r--r--   0 sebastian   (501) staff       (20)      675 2022-08-29 13:07:01.000000 chartmogul-3.1.1/chartmogul/api/data_source.py
--rw-r--r--   0 sebastian   (501) staff       (20)     3194 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/api/invoice.py
--rw-r--r--   0 sebastian   (501) staff       (20)     3361 2022-08-29 13:07:01.000000 chartmogul-3.1.1/chartmogul/api/metrics.py
--rw-r--r--   0 sebastian   (501) staff       (20)      441 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/api/ping.py
--rw-r--r--   0 sebastian   (501) staff       (20)      727 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/api/plan.py
--rw-r--r--   0 sebastian   (501) staff       (20)     1115 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/api/plan_group.py
--rw-r--r--   0 sebastian   (501) staff       (20)      774 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/api/plan_group_plans.py
--rw-r--r--   0 sebastian   (501) staff       (20)     1711 2023-04-03 12:41:37.000000 chartmogul-3.1.1/chartmogul/api/subscription_event.py
--rw-r--r--   0 sebastian   (501) staff       (20)     1105 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/api/tags.py
--rw-r--r--   0 sebastian   (501) staff       (20)      650 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/api/transaction.py
--rw-r--r--   0 sebastian   (501) staff       (20)      352 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/errors.py
-drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2023-04-03 12:43:54.200577 chartmogul-3.1.1/chartmogul/imp/
--rw-r--r--   0 sebastian   (501) staff       (20)      118 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/imp/__init__.py
--rw-r--r--   0 sebastian   (501) staff       (20)      497 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/imp/invoice.py
--rw-r--r--   0 sebastian   (501) staff       (20)      580 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/imp/subscription.py
--rw-r--r--   0 sebastian   (501) staff       (20)      332 2022-04-25 14:08:25.000000 chartmogul-3.1.1/chartmogul/imp/transaction.py
--rw-r--r--   0 sebastian   (501) staff       (20)     7560 2023-04-03 12:41:37.000000 chartmogul-3.1.1/chartmogul/resource.py
--rw-r--r--   0 sebastian   (501) staff       (20)      812 2023-04-03 12:41:37.000000 chartmogul-3.1.1/chartmogul/retry_request.py
--rw-r--r--   0 sebastian   (501) staff       (20)       22 2023-04-03 12:41:37.000000 chartmogul-3.1.1/chartmogul/version.py
-drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2023-04-03 12:43:54.145427 chartmogul-3.1.1/chartmogul.egg-info/
--rw-r--r--   0 sebastian   (501) staff       (20)      693 2023-04-03 12:43:54.000000 chartmogul-3.1.1/chartmogul.egg-info/PKG-INFO
--rw-r--r--   0 sebastian   (501) staff       (20)     1124 2023-04-03 12:43:54.000000 chartmogul-3.1.1/chartmogul.egg-info/SOURCES.txt
--rw-r--r--   0 sebastian   (501) staff       (20)        1 2023-04-03 12:43:54.000000 chartmogul-3.1.1/chartmogul.egg-info/dependency_links.txt
--rw-r--r--   0 sebastian   (501) staff       (20)        1 2022-04-25 14:10:06.000000 chartmogul-3.1.1/chartmogul.egg-info/not-zip-safe
--rw-r--r--   0 sebastian   (501) staff       (20)       86 2023-04-03 12:43:54.000000 chartmogul-3.1.1/chartmogul.egg-info/requires.txt
--rw-r--r--   0 sebastian   (501) staff       (20)       11 2023-04-03 12:43:54.000000 chartmogul-3.1.1/chartmogul.egg-info/top_level.txt
--rw-r--r--   0 sebastian   (501) staff       (20)      224 2023-04-03 12:43:54.205172 chartmogul-3.1.1/setup.cfg
--rw-r--r--   0 sebastian   (501) staff       (20)     2213 2023-04-03 12:41:37.000000 chartmogul-3.1.1/setup.py
+drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2023-05-23 11:49:38.648505 chartmogul-3.1.2/
+-rw-r--r--   0 sebastian   (501) staff       (20)     1081 2022-04-25 14:08:25.000000 chartmogul-3.1.2/LICENSE.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)      693 2023-05-23 11:49:38.648573 chartmogul-3.1.2/PKG-INFO
+-rw-r--r--   0 sebastian   (501) staff       (20)    15660 2023-05-23 11:44:05.000000 chartmogul-3.1.2/README.md
+drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2023-05-23 11:49:38.644170 chartmogul-3.1.2/chartmogul/
+-rw-r--r--   0 sebastian   (501) staff       (20)     1300 2023-05-23 11:44:05.000000 chartmogul-3.1.2/chartmogul/__init__.py
+drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2023-05-23 11:49:38.647077 chartmogul-3.1.2/chartmogul/api/
+-rw-r--r--   0 sebastian   (501) staff       (20)       85 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/api/__init__.py
+-rw-r--r--   0 sebastian   (501) staff       (20)      648 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/api/account.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     1880 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/api/activities_export.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     1365 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/api/activity.py
+-rw-r--r--   0 sebastian   (501) staff       (20)      551 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/api/attributes.py
+-rw-r--r--   0 sebastian   (501) staff       (20)      361 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/api/config.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     1321 2023-05-23 11:44:05.000000 chartmogul-3.1.2/chartmogul/api/contact.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     1116 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/api/custom_attrs.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     3224 2023-05-23 11:44:05.000000 chartmogul-3.1.2/chartmogul/api/customer.py
+drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2023-05-23 11:49:38.647741 chartmogul-3.1.2/chartmogul/api/customers/
+-rw-r--r--   0 sebastian   (501) staff       (20)       51 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/api/customers/__init__.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     1101 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/api/customers/activity.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     2770 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/api/customers/subscription.py
+-rw-r--r--   0 sebastian   (501) staff       (20)      675 2022-08-29 13:07:01.000000 chartmogul-3.1.2/chartmogul/api/data_source.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     3194 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/api/invoice.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     3361 2022-08-29 13:07:01.000000 chartmogul-3.1.2/chartmogul/api/metrics.py
+-rw-r--r--   0 sebastian   (501) staff       (20)      441 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/api/ping.py
+-rw-r--r--   0 sebastian   (501) staff       (20)      727 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/api/plan.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     1115 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/api/plan_group.py
+-rw-r--r--   0 sebastian   (501) staff       (20)      774 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/api/plan_group_plans.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     1714 2023-05-23 11:44:05.000000 chartmogul-3.1.2/chartmogul/api/subscription_event.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     1105 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/api/tags.py
+-rw-r--r--   0 sebastian   (501) staff       (20)      650 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/api/transaction.py
+-rw-r--r--   0 sebastian   (501) staff       (20)      352 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/errors.py
+drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2023-05-23 11:49:38.648370 chartmogul-3.1.2/chartmogul/imp/
+-rw-r--r--   0 sebastian   (501) staff       (20)      118 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/imp/__init__.py
+-rw-r--r--   0 sebastian   (501) staff       (20)      497 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/imp/invoice.py
+-rw-r--r--   0 sebastian   (501) staff       (20)      580 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/imp/subscription.py
+-rw-r--r--   0 sebastian   (501) staff       (20)      332 2022-04-25 14:08:25.000000 chartmogul-3.1.2/chartmogul/imp/transaction.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     7560 2023-05-23 11:44:05.000000 chartmogul-3.1.2/chartmogul/resource.py
+-rw-r--r--   0 sebastian   (501) staff       (20)      812 2023-05-23 11:44:05.000000 chartmogul-3.1.2/chartmogul/retry_request.py
+-rw-r--r--   0 sebastian   (501) staff       (20)       22 2023-05-23 11:44:05.000000 chartmogul-3.1.2/chartmogul/version.py
+drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2023-05-23 11:49:38.644919 chartmogul-3.1.2/chartmogul.egg-info/
+-rw-r--r--   0 sebastian   (501) staff       (20)      693 2023-05-23 11:49:38.000000 chartmogul-3.1.2/chartmogul.egg-info/PKG-INFO
+-rw-r--r--   0 sebastian   (501) staff       (20)     1124 2023-05-23 11:49:38.000000 chartmogul-3.1.2/chartmogul.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)        1 2023-05-23 11:49:38.000000 chartmogul-3.1.2/chartmogul.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)        1 2022-04-25 14:10:06.000000 chartmogul-3.1.2/chartmogul.egg-info/not-zip-safe
+-rw-r--r--   0 sebastian   (501) staff       (20)       98 2023-05-23 11:49:38.000000 chartmogul-3.1.2/chartmogul.egg-info/requires.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)       11 2023-05-23 11:49:38.000000 chartmogul-3.1.2/chartmogul.egg-info/top_level.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)      224 2023-05-23 11:49:38.648822 chartmogul-3.1.2/setup.cfg
+-rw-r--r--   0 sebastian   (501) staff       (20)     2229 2023-05-23 11:44:05.000000 chartmogul-3.1.2/setup.py
```

### Comparing `chartmogul-3.1.1/LICENSE.txt` & `chartmogul-3.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/PKG-INFO` & `chartmogul-3.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chartmogul
-Version: 3.1.1
+Version: 3.1.2
 Summary: Python library for ChartMogul API.
 Home-page: https://chartmogul.com
-Download-URL: https://github.com/chartmogul/chartmogul-python/tarball/v3.1.1
+Download-URL: https://github.com/chartmogul/chartmogul-python/tarball/v3.1.2
 Author: Petr Kopac (ChartMogul Ltd.)
 Author-email: petr@chartmogul.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `chartmogul-3.1.1/README.md` & `chartmogul-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/chartmogul/__init__.py` & `chartmogul-3.1.2/chartmogul/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 
 
 """
 ChartMogul API Python Client
 
 Provides convenient Python bindings for ChartMogul's API.
 
-:copyright: (c) 2019 by ChartMogul Ltd.
+:copyright: (c) 2023 by ChartMogul Ltd.
 :license: MIT, see LICENSE for more details.
 """
 
 __title__ = 'chartmogul'
 __build__ = 0x000000
 __author__ = 'ChartMogul Ltd'
 __license__ = 'MIT'
-__copyright__ = 'Copyright 2021 ChartMogul Ltd'
+__copyright__ = 'Copyright 2023 ChartMogul Ltd'
```

### Comparing `chartmogul-3.1.1/chartmogul/api/account.py` & `chartmogul-3.1.2/chartmogul/api/account.py`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/chartmogul/api/activities_export.py` & `chartmogul-3.1.2/chartmogul/api/activities_export.py`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/chartmogul/api/activity.py` & `chartmogul-3.1.2/chartmogul/api/activity.py`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/chartmogul/api/attributes.py` & `chartmogul-3.1.2/chartmogul/api/attributes.py`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/chartmogul/api/contact.py` & `chartmogul-3.1.2/chartmogul/api/contact.py`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/chartmogul/api/custom_attrs.py` & `chartmogul-3.1.2/chartmogul/api/custom_attrs.py`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/chartmogul/api/customer.py` & `chartmogul-3.1.2/chartmogul/api/customer.py`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/chartmogul/api/customers/activity.py` & `chartmogul-3.1.2/chartmogul/api/customers/activity.py`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/chartmogul/api/customers/subscription.py` & `chartmogul-3.1.2/chartmogul/api/customers/subscription.py`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/chartmogul/api/data_source.py` & `chartmogul-3.1.2/chartmogul/api/data_source.py`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/chartmogul/api/invoice.py` & `chartmogul-3.1.2/chartmogul/api/invoice.py`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/chartmogul/api/metrics.py` & `chartmogul-3.1.2/chartmogul/api/metrics.py`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/chartmogul/api/plan.py` & `chartmogul-3.1.2/chartmogul/api/plan.py`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/chartmogul/api/plan_group.py` & `chartmogul-3.1.2/chartmogul/api/plan_group.py`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/chartmogul/api/plan_group_plans.py` & `chartmogul-3.1.2/chartmogul/api/plan_group_plans.py`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/chartmogul/api/subscription_event.py` & `chartmogul-3.1.2/chartmogul/api/subscription_event.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from marshmallow import Schema, fields, post_load, EXCLUDE
 from ..resource import Resource
 from collections import namedtuple
 
 
 class SubscriptionEvent(Resource):
     """
-    https://dev.chartmogul.com/v1.0/reference#subscription_events
+    https://dev.chartmogul.com/reference/subscription-events
     """
     _path = "/subscription_events"
     _root_key = 'subscription_events'
     _many = namedtuple('SubscriptionEvents', [_root_key, 'meta'])
 
     class _Schema(Schema):
         id = fields.Int(required=True)
         data_source_uuid = fields.String(required=True)
         customer_external_id = fields.String(required=True)
         event_type = fields.String(required=True)
-        event_date = fields.Date(required=True)
-        effective_date = fields.Date(required=True)
+        event_date = fields.DateTime(required=True)
+        effective_date = fields.DateTime(required=True)
         subscription_external_id = fields.String(allow_none=True)
         plan_external_id = fields.String(allow_none=True)
         currency = fields.String(allow_none=True)
         amount_in_cents = fields.Int(allow_none=True)
         quantity = fields.Int(allow_none=True)
         subscription_set_external_id = fields.String(allow_none=True)
         tax_amount_in_cents = fields.Int(allow_none=True)
```

### Comparing `chartmogul-3.1.1/chartmogul/api/tags.py` & `chartmogul-3.1.2/chartmogul/api/tags.py`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/chartmogul/api/transaction.py` & `chartmogul-3.1.2/chartmogul/api/transaction.py`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/chartmogul/imp/subscription.py` & `chartmogul-3.1.2/chartmogul/imp/subscription.py`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/chartmogul/resource.py` & `chartmogul-3.1.2/chartmogul/resource.py`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/chartmogul/retry_request.py` & `chartmogul-3.1.2/chartmogul/retry_request.py`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/chartmogul.egg-info/PKG-INFO` & `chartmogul-3.1.2/chartmogul.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chartmogul
-Version: 3.1.1
+Version: 3.1.2
 Summary: Python library for ChartMogul API.
 Home-page: https://chartmogul.com
-Download-URL: https://github.com/chartmogul/chartmogul-python/tarball/v3.1.1
+Download-URL: https://github.com/chartmogul/chartmogul-python/tarball/v3.1.2
 Author: Petr Kopac (ChartMogul Ltd.)
 Author-email: petr@chartmogul.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `chartmogul-3.1.1/chartmogul.egg-info/SOURCES.txt` & `chartmogul-3.1.2/chartmogul.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chartmogul-3.1.1/setup.py` & `chartmogul-3.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,25 @@
 
 requires = [
     'requests>=2.10.0',
     'uritemplate>=3.0.0',
     'promise>=1.0.1',
     'marshmallow>=3.10.0',
     'future>=0.18.3',
+    'urllib3<2.0'
 ]
 test_requirements = [
     # This is needed to circumvent a vcrpy dependency problem And can be
     # deleted once it is solved.
     'yarl; python_version>"3.5"',
     'yarl<1.4; python_version=="3.5"',
 
     'mock>=1.0.1',
     'requests-mock>=1.3.0',
-    'vcrpy>=1.11.1',
+    'vcrpy<3.0.0',
     'PyYAML>=5.1.2',
     'httpretty>=0.9.6',
     'wrapt>=1.11.2'
 ]
 
 with open('chartmogul/version.py', 'r') as fd:
     version = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]',
```

