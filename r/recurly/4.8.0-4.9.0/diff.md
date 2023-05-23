# Comparing `tmp/recurly-4.8.0.tar.gz` & `tmp/recurly-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recurly-4.8.0.tar", last modified: Wed Sep  1 18:53:59 2021, max compression
+gzip compressed data, was "dist/recurly-4.9.0.tar", last modified: Thu Sep 16 19:12:36 2021, max compression
```

## Comparing `recurly-4.8.0.tar` & `recurly-4.9.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-01 18:53:59.000000 recurly-4.8.0/
--rw-r--r--   0 root         (0) root         (0)     1074 2021-09-01 18:53:52.000000 recurly-4.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       60 2021-09-01 18:53:52.000000 recurly-4.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1337 2021-09-01 18:53:59.000000 recurly-4.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      891 2021-09-01 18:53:52.000000 recurly-4.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-01 18:53:59.000000 recurly-4.8.0/recurly/
--rw-r--r--   0 root         (0) root         (0)      928 2021-09-01 18:53:52.000000 recurly-4.8.0/recurly/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4520 2021-09-01 18:53:52.000000 recurly-4.8.0/recurly/base_client.py
--rw-r--r--   0 root         (0) root         (0)      353 2021-09-01 18:53:52.000000 recurly-4.8.0/recurly/base_errors.py
--rw-r--r--   0 root         (0) root         (0)   147341 2021-09-01 18:53:52.000000 recurly-4.8.0/recurly/client.py
--rw-r--r--   0 root         (0) root         (0)     2511 2021-09-01 18:53:52.000000 recurly-4.8.0/recurly/errors.py
--rw-r--r--   0 root         (0) root         (0)     3324 2021-09-01 18:53:52.000000 recurly-4.8.0/recurly/pager.py
--rw-r--r--   0 root         (0) root         (0)      194 2021-09-01 18:53:52.000000 recurly-4.8.0/recurly/request.py
--rw-r--r--   0 root         (0) root         (0)     6348 2021-09-01 18:53:52.000000 recurly-4.8.0/recurly/resource.py
--rw-r--r--   0 root         (0) root         (0)    94860 2021-09-01 18:53:52.000000 recurly-4.8.0/recurly/resources.py
--rw-r--r--   0 root         (0) root         (0)     1627 2021-09-01 18:53:52.000000 recurly-4.8.0/recurly/response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-01 18:53:59.000000 recurly-4.8.0/recurly.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1337 2021-09-01 18:53:59.000000 recurly-4.8.0/recurly.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      561 2021-09-01 18:53:59.000000 recurly-4.8.0/recurly.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-09-01 18:53:59.000000 recurly-4.8.0/recurly.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2021-09-01 18:53:59.000000 recurly-4.8.0/recurly.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-09-01 18:53:59.000000 recurly-4.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      822 2021-09-01 18:53:52.000000 recurly-4.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-01 18:53:59.000000 recurly-4.8.0/tests/
--rw-r--r--   0 root         (0) root         (0)      220 2021-09-01 18:53:52.000000 recurly-4.8.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      803 2021-09-01 18:53:52.000000 recurly-4.8.0/tests/mock_client.py
--rw-r--r--   0 root         (0) root         (0)      647 2021-09-01 18:53:52.000000 recurly-4.8.0/tests/mock_resources.py
--rw-r--r--   0 root         (0) root         (0)     9840 2021-09-01 18:53:52.000000 recurly-4.8.0/tests/test_base_client.py
--rw-r--r--   0 root         (0) root         (0)      218 2021-09-01 18:53:52.000000 recurly-4.8.0/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)     6025 2021-09-01 18:53:52.000000 recurly-4.8.0/tests/test_pager.py
--rw-r--r--   0 root         (0) root         (0)     5470 2021-09-01 18:53:52.000000 recurly-4.8.0/tests/test_resource.py
--rw-r--r--   0 root         (0) root         (0)     1681 2021-09-01 18:53:52.000000 recurly-4.8.0/tests/test_resources.py
--rw-r--r--   0 root         (0) root         (0)     3320 2021-09-01 18:53:52.000000 recurly-4.8.0/tests/test_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-16 19:12:36.000000 recurly-4.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1074 2021-09-16 19:12:30.000000 recurly-4.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       60 2021-09-16 19:12:30.000000 recurly-4.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1337 2021-09-16 19:12:36.000000 recurly-4.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      891 2021-09-16 19:12:30.000000 recurly-4.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-16 19:12:36.000000 recurly-4.9.0/recurly/
+-rw-r--r--   0 root         (0) root         (0)      928 2021-09-16 19:12:30.000000 recurly-4.9.0/recurly/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4520 2021-09-16 19:12:30.000000 recurly-4.9.0/recurly/base_client.py
+-rw-r--r--   0 root         (0) root         (0)      353 2021-09-16 19:12:30.000000 recurly-4.9.0/recurly/base_errors.py
+-rw-r--r--   0 root         (0) root         (0)   147341 2021-09-16 19:12:30.000000 recurly-4.9.0/recurly/client.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2021-09-16 19:12:30.000000 recurly-4.9.0/recurly/errors.py
+-rw-r--r--   0 root         (0) root         (0)     3324 2021-09-16 19:12:30.000000 recurly-4.9.0/recurly/pager.py
+-rw-r--r--   0 root         (0) root         (0)      194 2021-09-16 19:12:30.000000 recurly-4.9.0/recurly/request.py
+-rw-r--r--   0 root         (0) root         (0)     6348 2021-09-16 19:12:30.000000 recurly-4.9.0/recurly/resource.py
+-rw-r--r--   0 root         (0) root         (0)    95207 2021-09-16 19:12:30.000000 recurly-4.9.0/recurly/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1627 2021-09-16 19:12:30.000000 recurly-4.9.0/recurly/response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-16 19:12:36.000000 recurly-4.9.0/recurly.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1337 2021-09-16 19:12:36.000000 recurly-4.9.0/recurly.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      561 2021-09-16 19:12:36.000000 recurly-4.9.0/recurly.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-09-16 19:12:36.000000 recurly-4.9.0/recurly.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2021-09-16 19:12:36.000000 recurly-4.9.0/recurly.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-09-16 19:12:36.000000 recurly-4.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      822 2021-09-16 19:12:30.000000 recurly-4.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-16 19:12:36.000000 recurly-4.9.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      220 2021-09-16 19:12:30.000000 recurly-4.9.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      803 2021-09-16 19:12:30.000000 recurly-4.9.0/tests/mock_client.py
+-rw-r--r--   0 root         (0) root         (0)      647 2021-09-16 19:12:30.000000 recurly-4.9.0/tests/mock_resources.py
+-rw-r--r--   0 root         (0) root         (0)     9840 2021-09-16 19:12:30.000000 recurly-4.9.0/tests/test_base_client.py
+-rw-r--r--   0 root         (0) root         (0)      218 2021-09-16 19:12:30.000000 recurly-4.9.0/tests/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     6025 2021-09-16 19:12:30.000000 recurly-4.9.0/tests/test_pager.py
+-rw-r--r--   0 root         (0) root         (0)     5470 2021-09-16 19:12:30.000000 recurly-4.9.0/tests/test_resource.py
+-rw-r--r--   0 root         (0) root         (0)     1681 2021-09-16 19:12:30.000000 recurly-4.9.0/tests/test_resources.py
+-rw-r--r--   0 root         (0) root         (0)     3320 2021-09-16 19:12:30.000000 recurly-4.9.0/tests/test_response.py
```

### Comparing `recurly-4.8.0/LICENSE` & `recurly-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `recurly-4.8.0/PKG-INFO` & `recurly-4.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurly
-Version: 4.8.0
+Version: 4.9.0
 Summary: Recurly v4
 Home-page: https://github.com/recurly/recurly-client-python
 Author: Developer Experience
 Author-email: dx@recurly.com
 License: UNKNOWN
 Description: # Recurly
```

### Comparing `recurly-4.8.0/README.md` & `recurly-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `recurly-4.8.0/recurly/__init__.py` & `recurly-4.9.0/recurly/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 from os.path import dirname, basename, isfile
 import glob
 import ssl
 import sys
 
-__version__ = "4.8.0"
+__version__ = "4.9.0"
 __python_version__ = ".".join(map(str, sys.version_info[:3]))
 
 USER_AGENT = "Recurly/{}; python {}; {}".format(
     __version__, __python_version__, ssl.OPENSSL_VERSION
 )
 
 # Running in strict mode will throw exceptions
```

### Comparing `recurly-4.8.0/recurly/base_client.py` & `recurly-4.9.0/recurly/base_client.py`

 * *Files identical despite different names*

### Comparing `recurly-4.8.0/recurly/client.py` & `recurly-4.9.0/recurly/client.py`

 * *Files identical despite different names*

### Comparing `recurly-4.8.0/recurly/errors.py` & `recurly-4.9.0/recurly/errors.py`

 * *Files identical despite different names*

### Comparing `recurly-4.8.0/recurly/pager.py` & `recurly-4.9.0/recurly/pager.py`

 * *Files identical despite different names*

### Comparing `recurly-4.8.0/recurly/resource.py` & `recurly-4.9.0/recurly/resource.py`

 * *Files identical despite different names*

### Comparing `recurly-4.8.0/recurly/resources.py` & `recurly-4.9.0/recurly/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1524,14 +1524,16 @@
         The custom fields will only be altered when they are included in a request. Sending an empty array will not remove any existing values. To remove a field send the name with a null or empty value.
     customer_notes : str
         Customer notes
     expiration_reason : str
         Expiration reason
     expires_at : datetime
         Expires at
+    gateway_code : str
+        If present, this subscription's transactions will use the payment gateway with this code.
     id : str
         Subscription ID
     net_terms : int
         Integer representing the number of days after an invoice's creation that the invoice will become past due. If an invoice's net terms are set to '0', it is due 'On Receipt' and will become past due 24 hours after it’s created. If an invoice is due net 30, it will become past due at 31 days exactly.
     object : str
         Object type
     paused_at : datetime
@@ -1554,16 +1556,22 @@
         Revenue schedule type
     shipping : SubscriptionShipping
         Subscription shipping details
     state : str
         State
     subtotal : float
         Estimated total, before tax.
+    tax : float
+        Estimated tax
+    tax_info : TaxInfo
+        Tax info
     terms_and_conditions : str
         Terms and conditions
+    total : float
+        Estimated total
     total_billing_cycles : int
         The number of cycles/billing periods in a term. When `remaining_billing_cycles=0`, if `auto_renew=true` the subscription will renew and a new term will begin, otherwise the subscription will expire.
     trial_ends_at : datetime
         Trial period ends at
     trial_started_at : datetime
         Trial period started at
     unit_amount : float
@@ -1591,14 +1599,15 @@
         "current_period_started_at": datetime,
         "current_term_ends_at": datetime,
         "current_term_started_at": datetime,
         "custom_fields": ["CustomField"],
         "customer_notes": str,
         "expiration_reason": str,
         "expires_at": datetime,
+        "gateway_code": str,
         "id": str,
         "net_terms": int,
         "object": str,
         "paused_at": datetime,
         "pending_change": "SubscriptionChange",
         "plan": "PlanMini",
         "po_number": str,
@@ -1606,15 +1615,18 @@
         "remaining_billing_cycles": int,
         "remaining_pause_cycles": int,
         "renewal_billing_cycles": int,
         "revenue_schedule_type": str,
         "shipping": "SubscriptionShipping",
         "state": str,
         "subtotal": float,
+        "tax": float,
+        "tax_info": "TaxInfo",
         "terms_and_conditions": str,
+        "total": float,
         "total_billing_cycles": int,
         "trial_ends_at": datetime,
         "trial_started_at": datetime,
         "unit_amount": float,
         "updated_at": datetime,
         "uuid": str,
     }
```

### Comparing `recurly-4.8.0/recurly/response.py` & `recurly-4.9.0/recurly/response.py`

 * *Files identical despite different names*

### Comparing `recurly-4.8.0/recurly.egg-info/PKG-INFO` & `recurly-4.9.0/recurly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurly
-Version: 4.8.0
+Version: 4.9.0
 Summary: Recurly v4
 Home-page: https://github.com/recurly/recurly-client-python
 Author: Developer Experience
 Author-email: dx@recurly.com
 License: UNKNOWN
 Description: # Recurly
```

### Comparing `recurly-4.8.0/recurly.egg-info/SOURCES.txt` & `recurly-4.9.0/recurly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recurly-4.8.0/setup.py` & `recurly-4.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `recurly-4.8.0/tests/mock_client.py` & `recurly-4.9.0/tests/mock_client.py`

 * *Files identical despite different names*

### Comparing `recurly-4.8.0/tests/mock_resources.py` & `recurly-4.9.0/tests/mock_resources.py`

 * *Files identical despite different names*

### Comparing `recurly-4.8.0/tests/test_base_client.py` & `recurly-4.9.0/tests/test_base_client.py`

 * *Files identical despite different names*

### Comparing `recurly-4.8.0/tests/test_pager.py` & `recurly-4.9.0/tests/test_pager.py`

 * *Files identical despite different names*

### Comparing `recurly-4.8.0/tests/test_resource.py` & `recurly-4.9.0/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `recurly-4.8.0/tests/test_resources.py` & `recurly-4.9.0/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `recurly-4.8.0/tests/test_response.py` & `recurly-4.9.0/tests/test_response.py`

 * *Files identical despite different names*

