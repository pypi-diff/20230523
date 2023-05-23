# Comparing `tmp/vital-1.3.7.tar.gz` & `tmp/vital-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vital-1.3.7.tar", max compression
+gzip compressed data, was "vital-1.3.9.tar", max compression
```

## Comparing `vital-1.3.7.tar` & `vital-1.3.9.tar`

### file list

```diff
@@ -1,27 +1,30 @@
--rw-r--r--   0        0        0      388 2023-01-25 13:43:37.341533 vital-1.3.7/README.md
--rw-r--r--   0        0        0     1102 2023-01-25 13:43:37.345533 vital-1.3.7/pyproject.toml
--rw-r--r--   0        0        0      107 2023-01-25 13:43:37.345533 vital-1.3.7/vital/__init__.py
--rw-r--r--   0        0        0      621 2023-01-25 13:43:37.345533 vital-1.3.7/vital/api/__init__.py
--rw-r--r--   0        0        0     1531 2023-01-25 13:43:37.345533 vital-1.3.7/vital/api/activity.py
--rw-r--r--   0        0        0      142 2023-01-25 13:43:37.345533 vital-1.3.7/vital/api/api.py
--rw-r--r--   0        0        0     1515 2023-01-25 13:43:37.345533 vital-1.3.7/vital/api/body.py
--rw-r--r--   0        0        0      598 2023-01-25 13:43:37.345533 vital-1.3.7/vital/api/devices.py
--rw-r--r--   0        0        0     2101 2023-01-25 13:43:37.345533 vital-1.3.7/vital/api/labtests.py
--rw-r--r--   0        0        0     3093 2023-01-25 13:43:37.345533 vital-1.3.7/vital/api/link.py
--rw-r--r--   0        0        0      823 2023-01-25 13:43:37.345533 vital-1.3.7/vital/api/meals.py
--rw-r--r--   0        0        0      820 2023-01-25 13:43:37.345533 vital-1.3.7/vital/api/profile.py
--rw-r--r--   0        0        0     2259 2023-01-25 13:43:37.345533 vital-1.3.7/vital/api/sleep.py
--rw-r--r--   0        0        0     2287 2023-01-25 13:43:37.345533 vital-1.3.7/vital/api/user.py
--rw-r--r--   0        0        0     3866 2023-01-25 13:43:37.345533 vital-1.3.7/vital/api/vitals.py
--rw-r--r--   0        0        0      632 2023-01-25 13:43:37.345533 vital-1.3.7/vital/api/webhooks.py
--rw-r--r--   0        0        0     1318 2023-01-25 13:43:37.345533 vital-1.3.7/vital/api/workouts.py
--rw-r--r--   0        0        0     4981 2023-01-25 13:43:37.345533 vital-1.3.7/vital/client.py
--rw-r--r--   0        0        0     3118 2023-01-25 13:43:37.345533 vital-1.3.7/vital/errors.py
--rw-r--r--   0        0        0        0 2023-01-25 13:43:37.345533 vital-1.3.7/vital/internal/__init__.py
--rw-r--r--   0        0        0     2299 2023-01-25 13:43:37.345533 vital-1.3.7/vital/internal/requester.py
--rw-r--r--   0        0        0       80 2023-01-25 13:43:37.345533 vital-1.3.7/vital/internal/utils.py
--rw-r--r--   0        0        0     2762 2023-01-25 13:43:37.345533 vital-1.3.7/vital/internal/webhook.py
--rw-r--r--   0        0        0      359 2023-01-25 13:43:37.345533 vital-1.3.7/vital/types.py
--rw-r--r--   0        0        0      239 2023-01-25 13:43:37.345533 vital-1.3.7/vital/version.py
--rw-r--r--   0        0        0     1166 1970-01-01 00:00:00.000000 vital-1.3.7/setup.py
--rw-r--r--   0        0        0     1387 1970-01-01 00:00:00.000000 vital-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0      388 2023-05-23 08:44:09.363236 vital-1.3.9/README.md
+-rw-r--r--   0        0        0     1123 2023-05-23 08:44:09.363236 vital-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-05-23 08:44:09.363236 vital-1.3.9/vital/__init__.py
+-rw-r--r--   0        0        0      702 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/__init__.py
+-rw-r--r--   0        0        0     1531 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/activity.py
+-rw-r--r--   0        0        0      142 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/api.py
+-rw-r--r--   0        0        0     2904 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/athome_phlebotomy.py
+-rw-r--r--   0        0        0     1515 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/body.py
+-rw-r--r--   0        0        0      598 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/devices.py
+-rw-r--r--   0        0        0     2656 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/labtests.py
+-rw-r--r--   0        0        0     3093 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/link.py
+-rw-r--r--   0        0        0      823 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/meals.py
+-rw-r--r--   0        0        0      820 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/profile.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/schema/__init__.py
+-rw-r--r--   0        0        0     1719 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/schema/athome_phlebotomy.py
+-rw-r--r--   0        0        0     2259 2023-05-23 08:44:09.363236 vital-1.3.9/vital/api/sleep.py
+-rw-r--r--   0        0        0     2287 2023-05-23 08:44:09.367236 vital-1.3.9/vital/api/user.py
+-rw-r--r--   0        0        0     3866 2023-05-23 08:44:09.367236 vital-1.3.9/vital/api/vitals.py
+-rw-r--r--   0        0        0      632 2023-05-23 08:44:09.367236 vital-1.3.9/vital/api/webhooks.py
+-rw-r--r--   0        0        0     1318 2023-05-23 08:44:09.367236 vital-1.3.9/vital/api/workouts.py
+-rw-r--r--   0        0        0     5888 2023-05-23 08:44:09.367236 vital-1.3.9/vital/client.py
+-rw-r--r--   0        0        0     3118 2023-05-23 08:44:09.367236 vital-1.3.9/vital/errors.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:44:09.367236 vital-1.3.9/vital/internal/__init__.py
+-rw-r--r--   0        0        0     2363 2023-05-23 08:44:09.367236 vital-1.3.9/vital/internal/requester.py
+-rw-r--r--   0        0        0       80 2023-05-23 08:44:09.367236 vital-1.3.9/vital/internal/utils.py
+-rw-r--r--   0        0        0     2762 2023-05-23 08:44:09.367236 vital-1.3.9/vital/internal/webhook.py
+-rw-r--r--   0        0        0      359 2023-05-23 08:44:09.367236 vital-1.3.9/vital/types.py
+-rw-r--r--   0        0        0      239 2023-05-23 08:44:09.367236 vital-1.3.9/vital/version.py
+-rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 vital-1.3.9/setup.py
+-rw-r--r--   0        0        0     1429 1970-01-01 00:00:00.000000 vital-1.3.9/PKG-INFO
```

### Comparing `vital-1.3.7/pyproject.toml` & `vital-1.3.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vital"
-version = "1.3.7"
+version = "1.3.9"
 description = ""
 authors = ["maitham <maitham@tryvital.io>"]
 license = "GNU"
 readme = "README.md"
 homepage = "https://github.com/adeptlabs/vital-python"
 repository = "https://github.com/adeptlabs/vital-python"
 keywords = ["vital", "tryvital", "python"]
@@ -21,14 +21,15 @@
 python = "^3.8"
 PyJWT = "^2.0.1"
 arrow = "*"
 requests = "*"
 importlib-metadata = "^3.7.3"
 svix = "^0.41.2"
 typed-ast="^1.5.4"
+pydantic = "^1.10.7"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.2"
 isort = "^5.8.0"
 flake8 = "^3.9.0"
 mypy = "^0.990"
 black =  "^22.6.0"
```

### Comparing `vital-1.3.7/vital/api/__init__.py` & `vital-1.3.9/vital/api/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from vital.api.activity import Activity
+from vital.api.athome_phlebotomy import AtHomePhlebotomy
 from vital.api.body import Body
 from vital.api.devices import Devices
 from vital.api.labtests import LabTests
 from vital.api.link import Link
 from vital.api.meals import Meals
 from vital.api.profile import Profile
 from vital.api.sleep import Sleep
 from vital.api.user import User
 from vital.api.vitals import Vitals
 from vital.api.webhooks import Webhooks
 from vital.api.workouts import Workouts
 
 __all__ = [
-    "Link",
-    "Body",
     "Activity",
+    "AtHomePhlebotomy",
+    "Body",
+    "Devices",
+    "LabTests",
+    "Link",
+    "Meals",
+    "Profile",
     "Sleep",
     "User",
-    "Workouts",
-    "Webhooks",
     "Vitals",
-    "LabTests",
-    "Devices",
-    "Profile",
-    "Meals",
+    "Webhooks",
+    "Workouts",
 ]
```

### Comparing `vital-1.3.7/vital/api/activity.py` & `vital-1.3.9/vital/api/activity.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.7/vital/api/body.py` & `vital-1.3.9/vital/api/body.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.7/vital/api/devices.py` & `vital-1.3.9/vital/api/devices.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.7/vital/api/labtests.py` & `vital-1.3.9/vital/api/labtests.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,26 +9,34 @@
     def create_order(
         self,
         user_id: str,
         patient_details: Dict,
         patient_address: Dict,
         lab_test_id: str,
         physician: Optional[Dict],
+        health_insurance: Optional[Dict] = None,
     ) -> Mapping[str, str]:
         """Create new order"""
-
-        return self.client.post(
-            "/order",
-            {
-                "user_id": user_id,
-                "patient_details": patient_details,
-                "patient_address": patient_address,
-                "lab_test_id": lab_test_id,
-                "physician": physician,
-            },
+        params = {
+            "user_id": user_id,
+            "patient_details": patient_details,
+            "patient_address": patient_address,
+            "lab_test_id": lab_test_id,
+            "physician": physician,
+        }
+        if health_insurance:
+            params["health_insurance"] = health_insurance
+
+        return self.client.post("/order", params, api_version="v3")
+
+    def get_orders(self, page: int = 1, size: int = 50) -> Mapping[str, str]:
+        """Get all orders"""
+        return self.client.get(
+            "/orders",
+            {"page": page, "size": size},
             api_version="v3",
         )
 
     def get_order(self, order_id: str) -> Mapping[str, str]:
         """
         Get order status.
         :param str user_id: The order_id.
@@ -62,7 +70,13 @@
 
     def get_results_metadata(self, order_id: str) -> Mapping[str, str]:
         """
         GET metadata related to order results, such as
         lab metadata, provider and sample dates.
         """
         return self.client.get(f"/order/{order_id}/result/metadata", api_version="v3")
+
+    def get_area_info(self, zip_code: str) -> Mapping[str, str]:
+        """
+        GET area info for a given zip code.
+        """
+        return self.client.get("/area/info", {"zip_code": zip_code}, api_version="v3")
```

### Comparing `vital-1.3.7/vital/api/link.py` & `vital-1.3.9/vital/api/link.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.7/vital/api/meals.py` & `vital-1.3.9/vital/api/meals.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.7/vital/api/profile.py` & `vital-1.3.9/vital/api/profile.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.7/vital/api/sleep.py` & `vital-1.3.9/vital/api/sleep.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.7/vital/api/user.py` & `vital-1.3.9/vital/api/user.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.7/vital/api/vitals.py` & `vital-1.3.9/vital/api/vitals.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.7/vital/api/webhooks.py` & `vital-1.3.9/vital/api/webhooks.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.7/vital/api/workouts.py` & `vital-1.3.9/vital/api/workouts.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.7/vital/client.py` & `vital-1.3.9/vital/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 
 from vital.api import (
     Activity,
+    AtHomePhlebotomy,
     Body,
     Devices,
     LabTests,
     Link,
     Meals,
     Profile,
     Sleep,
@@ -15,14 +16,15 @@
     Workouts,
 )
 from vital.internal.requester import (
     DEFAULT_TIMEOUT,
     delete_request,
     get_request,
     post_request,
+    patch_request,
 )
 from vital.internal.utils import urljoin
 
 base_urls = {
     "eu": {
         "prod": "https://api.eu.tryvital.io",
         "production": "https://api.eu.tryvital.io",
@@ -90,25 +92,34 @@
         self.Activity = Activity(self)
         self.Sleep = Sleep(self)
         self.User = User(self)
         self.Workouts = Workouts(self)
         self.Webhooks = Webhooks(self)
         self.Vitals = Vitals(self)
         self.LabTests = LabTests(self)
+        self.AtHomePhlebotomy = AtHomePhlebotomy(self)
         self.Devices = Devices(self)
         self.Meals = Meals(self)
 
     def post(
         self, path, data=None, is_json=True, params={}, headers={}, api_version=None
     ):
         """Make a post request."""
         return self._post(
             path, data, is_json, params, self.session, headers, api_version
         )
 
+    def patch(
+        self, path, data=None, is_json=True, params={}, headers={}, api_version=None
+    ):
+        """Make a PATCH request."""
+        return self._patch(
+            path, data, is_json, params, self.session, headers, api_version
+        )
+
     def get(self, path, params={}, headers={}, api_version=None):
         """Make a get request."""
         return self._get(path, params, self.session, headers, api_version)
 
     def delete(self, path, params={}, api_version=None):
         """Make a delete request."""
         return self._delete(path, params, self.session, api_version)
@@ -128,14 +139,34 @@
             urljoin(
                 self.base_url,
                 f"{self.api_version if not api_version else api_version}{path}",
             ),
             data=data,
             timeout=self.timeout,
             is_json=is_json,
+            headers=headers,
+            params=params,
+            session=session,
+        )
+
+    def _patch(
+        self, path, data, is_json, params={}, session=None, headers={}, api_version=None
+    ):
+        headers = {
+            **self.headers,
+            **headers,
+        }
+        return patch_request(
+            urljoin(
+                self.base_url,
+                f"{self.api_version if not api_version else api_version}{path}",
+            ),
+            data=data,
+            timeout=self.timeout,
+            is_json=is_json,
             headers=headers,
             params=params,
             session=session,
         )
 
     def _get(self, path, params={}, session=None, headers={}, api_version=None):
         headers = {
```

### Comparing `vital-1.3.7/vital/errors.py` & `vital-1.3.9/vital/errors.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.7/vital/internal/requester.py` & `vital-1.3.9/vital/internal/requester.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any, Dict, Mapping, Optional
 
 import requests
 
 from vital.errors import VitalError
 from vital.version import __version__
 
-ALLOWED_METHODS = {"post", "get", "delete"}
+ALLOWED_METHODS = {"post", "patch", "get", "delete"}
 DEFAULT_TIMEOUT = 600  # 10 minutes
 
 
 def _requests_http_request(
     url: str,
     method: str,
     data: Optional[Mapping],
@@ -66,9 +66,10 @@
             return response_body
     else:
         return response.content
 
 
 # helpers to simplify partial function application
 post_request = partial(_http_request, method="POST")
+patch_request = partial(_http_request, method="PATCH")
 get_request = partial(_http_request, method="GET", data=None)
 delete_request = partial(_http_request, method="DELETE", data=None)
```

### Comparing `vital-1.3.7/vital/internal/webhook.py` & `vital-1.3.9/vital/internal/webhook.py`

 * *Files identical despite different names*

### Comparing `vital-1.3.7/setup.py` & `vital-1.3.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['vital', 'vital.api', 'vital.internal']
+['vital', 'vital.api', 'vital.api.schema', 'vital.internal']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyJWT>=2.0.1,<3.0.0',
  'arrow',
  'importlib-metadata>=3.7.3,<4.0.0',
+ 'pydantic>=1.10.7,<2.0.0',
  'requests',
  'svix>=0.41.2,<0.42.0',
  'typed-ast>=1.5.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'vital',
-    'version': '1.3.7',
+    'version': '1.3.9',
     'description': '',
     'long_description': "# vital-python\n\nThe official Python Library for [Vital API](https://docs.tryvital.io)\n\n# Install\n\n```\npip install vital\n```\n\n# Installing locally\n\n```\npoetry build --format sdist\ntar -xvf dist/*-`poetry version -s`.tar.gz -O '*/setup.py' > setup.py\n```\n\n## Documentation\n\nPlease refer to the official [Vital docs](https://docs.tryvital.io) provide a full reference on using this library.\n",
     'author': 'maitham',
     'author_email': 'maitham@tryvital.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/adeptlabs/vital-python',
```

### Comparing `vital-1.3.7/PKG-INFO` & `vital-1.3.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vital
-Version: 1.3.7
+Version: 1.3.9
 Summary: 
 Home-page: https://github.com/adeptlabs/vital-python
 License: GNU
 Keywords: vital,tryvital,python
 Author: maitham
 Author-email: maitham@tryvital.io
 Requires-Python: >=3.8,<4.0
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Documentation
 Requires-Dist: PyJWT (>=2.0.1,<3.0.0)
 Requires-Dist: arrow
 Requires-Dist: importlib-metadata (>=3.7.3,<4.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: requests
 Requires-Dist: svix (>=0.41.2,<0.42.0)
 Requires-Dist: typed-ast (>=1.5.4,<2.0.0)
 Project-URL: Repository, https://github.com/adeptlabs/vital-python
 Description-Content-Type: text/markdown
 
 # vital-python
```

