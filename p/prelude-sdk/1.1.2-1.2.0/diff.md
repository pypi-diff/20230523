# Comparing `tmp/prelude-sdk-1.1.2.tar.gz` & `tmp/prelude-sdk-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-sdk-1.1.2.tar", last modified: Tue May 16 20:31:57 2023, max compression
+gzip compressed data, was "prelude-sdk-1.2.0.tar", last modified: Tue May 23 20:18:24 2023, max compression
```

## Comparing `prelude-sdk-1.1.2.tar` & `prelude-sdk-1.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-16 20:31:57.516418 prelude-sdk-1.1.2/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.1.2/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-16 20:31:57.516488 prelude-sdk-1.1.2/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.1.2/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-16 20:31:57.512205 prelude-sdk-1.1.2/prelude_sdk/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.1.2/prelude_sdk/__init__.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-16 20:31:57.514202 prelude-sdk-1.1.2/prelude_sdk/controllers/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.1.2/prelude_sdk/controllers/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2230 2023-05-07 12:16:47.000000 prelude-sdk-1.1.2/prelude_sdk/controllers/build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     4115 2023-05-12 13:56:19.000000 prelude-sdk-1.1.2/prelude_sdk/controllers/detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3266 2023-05-12 13:56:19.000000 prelude-sdk-1.1.2/prelude_sdk/controllers/iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     2046 2023-05-03 13:30:52.000000 prelude-sdk-1.1.2/prelude_sdk/controllers/partner_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      443 2023-05-03 13:30:52.000000 prelude-sdk-1.1.2/prelude_sdk/controllers/probe_controller.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-16 20:31:57.514735 prelude-sdk-1.1.2/prelude_sdk/models/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.1.2/prelude_sdk/models/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2816 2023-04-07 19:23:14.000000 prelude-sdk-1.1.2/prelude_sdk/models/account.py
--rw-r--r--   0 pack       (501) staff       (20)     2698 2023-05-09 16:39:45.000000 prelude-sdk-1.1.2/prelude_sdk/models/codes.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-16 20:31:57.512780 prelude-sdk-1.1.2/prelude_sdk.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-16 20:31:57.000000 prelude-sdk-1.1.2/prelude_sdk.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      806 2023-05-16 20:31:57.000000 prelude-sdk-1.1.2/prelude_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-05-16 20:31:57.000000 prelude-sdk-1.1.2/prelude_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)        9 2023-05-16 20:31:57.000000 prelude-sdk-1.1.2/prelude_sdk.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       18 2023-05-16 20:31:57.000000 prelude-sdk-1.1.2/prelude_sdk.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.1.2/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      532 2023-05-16 20:31:57.516719 prelude-sdk-1.1.2/setup.cfg
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-16 20:31:57.516105 prelude-sdk-1.1.2/tests/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.1.2/tests/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1101 2023-04-11 22:16:02.000000 prelude-sdk-1.1.2/tests/conftest.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-16 20:31:57.516317 prelude-sdk-1.1.2/tests/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.1.2/tests/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2188 2023-05-07 12:16:47.000000 prelude-sdk-1.1.2/tests/test_build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3734 2023-05-03 13:30:52.000000 prelude-sdk-1.1.2/tests/test_detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3359 2023-05-12 13:56:19.000000 prelude-sdk-1.1.2/tests/test_iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      785 2023-05-02 14:19:17.000000 prelude-sdk-1.1.2/tests/test_partner_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-1.1.2/tests/test_probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 20:18:24.407507 prelude-sdk-1.2.0/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.2.0/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-23 20:18:24.407564 prelude-sdk-1.2.0/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.2.0/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 20:18:24.403297 prelude-sdk-1.2.0/prelude_sdk/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.0/prelude_sdk/__init__.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 20:18:24.405130 prelude-sdk-1.2.0/prelude_sdk/controllers/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.0/prelude_sdk/controllers/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1479 2023-05-18 20:31:39.000000 prelude-sdk-1.2.0/prelude_sdk/controllers/build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     4923 2023-05-22 15:57:51.000000 prelude-sdk-1.2.0/prelude_sdk/controllers/detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3266 2023-05-12 13:56:19.000000 prelude-sdk-1.2.0/prelude_sdk/controllers/iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     2079 2023-05-22 15:57:51.000000 prelude-sdk-1.2.0/prelude_sdk/controllers/partner_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      443 2023-05-03 13:30:52.000000 prelude-sdk-1.2.0/prelude_sdk/controllers/probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 20:18:24.405773 prelude-sdk-1.2.0/prelude_sdk/models/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.0/prelude_sdk/models/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2816 2023-04-07 19:23:14.000000 prelude-sdk-1.2.0/prelude_sdk/models/account.py
+-rw-r--r--   0 pack       (501) staff       (20)     2555 2023-05-22 15:57:51.000000 prelude-sdk-1.2.0/prelude_sdk/models/codes.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 20:18:24.403808 prelude-sdk-1.2.0/prelude_sdk.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-23 20:18:24.000000 prelude-sdk-1.2.0/prelude_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      806 2023-05-23 20:18:24.000000 prelude-sdk-1.2.0/prelude_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-05-23 20:18:24.000000 prelude-sdk-1.2.0/prelude_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)        9 2023-05-23 20:18:24.000000 prelude-sdk-1.2.0/prelude_sdk.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       18 2023-05-23 20:18:24.000000 prelude-sdk-1.2.0/prelude_sdk.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.2.0/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      532 2023-05-23 20:18:24.407761 prelude-sdk-1.2.0/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 20:18:24.407223 prelude-sdk-1.2.0/tests/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.2.0/tests/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1097 2023-05-17 16:29:25.000000 prelude-sdk-1.2.0/tests/conftest.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 20:18:24.407425 prelude-sdk-1.2.0/tests/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.2.0/tests/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1622 2023-05-22 15:57:51.000000 prelude-sdk-1.2.0/tests/test_build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     4483 2023-05-22 15:57:51.000000 prelude-sdk-1.2.0/tests/test_detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3353 2023-05-22 18:28:42.000000 prelude-sdk-1.2.0/tests/test_iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      619 2023-05-22 15:57:51.000000 prelude-sdk-1.2.0/tests/test_partner_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-1.2.0/tests/test_probe_controller.py
```

### Comparing `prelude-sdk-1.1.2/LICENSE` & `prelude-sdk-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.1.2/PKG-INFO` & `prelude-sdk-1.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.1.2
+Version: 1.2.0
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.1.2/README.md` & `prelude-sdk-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.1.2/prelude_sdk/controllers/build_controller.py` & `prelude-sdk-1.2.0/prelude_sdk/controllers/build_controller.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 
 class BuildController:
 
     def __init__(self, account):
         self.account = account
 
     @verify_credentials
-    def create_test(self, test_id, name, unit, alert=None):
+    def create_test(self, test_id, name, unit, advisory=None):
         """ Create or update a test """
         body = dict(name=name, unit=unit)
-        if alert is not None:
-            body['alert'] = alert
+        if advisory:
+            body['advisory'] = advisory
+
         res = requests.post(
             f'{self.account.hq}/build/tests/{test_id}',
             json=body,
             headers=self.account.headers,
             timeout=10
         )
         if not res.status_code == 200:
@@ -31,38 +32,14 @@
             headers=self.account.headers,
             timeout=10
         )
         if not res.status_code == 200:
             raise Exception(res.text)
 
     @verify_credentials
-    def get_test(self, test_id):
-        """ Get properties of an existing test """
-        res = requests.get(
-            f'{self.account.hq}/build/tests/{test_id}',
-            headers=self.account.headers,
-            timeout=10
-        )
-        if res.status_code == 200:
-            return res.json()
-        raise Exception(res.text)
-
-    @verify_credentials
-    def download(self, test_id, filename):
-        """ Clone a test file or attachment"""
-        res = requests.get(
-            f'{self.account.hq}/build/tests/{test_id}/{filename}',
-            headers=self.account.headers,
-            timeout=10
-        )
-        if res.status_code == 200:
-            return res.content
-        raise Exception(res.text)
-
-    @verify_credentials
     def upload(self, test_id, filename, data, binary=False):
         """ Upload a test or attachment """
         h = self.account.headers | ({'Content-Type': 'application/octet-stream'} if binary else {})
         res = requests.post(
             f'{self.account.hq}/build/tests/{test_id}/{filename}',
             data=data,
             headers=h,
```

### Comparing `prelude-sdk-1.1.2/prelude_sdk/controllers/detect_controller.py` & `prelude-sdk-1.2.0/prelude_sdk/controllers/detect_controller.py`

 * *Files 15% similar despite different names*

```diff
@@ -47,53 +47,78 @@
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
+    def list_advisories(self, year: int = None):
+        """ List advisories """
+        params = dict(year=year) if year else {}
+        res = requests.get(
+            f'{self.account.hq}/detect/advisories',
+            headers=self.account.headers,
+            params=params,
+            timeout=10
+        )
+        if res.status_code == 200:
+            return res.json()
+        raise Exception(res.text)
+
+    @verify_credentials
     def describe_activity(self, filters: dict, view: str = 'logs'):
         """ Get report for an Account """
         params = dict(view=view, **filters)
         res = requests.get(
             f'{self.account.hq}/detect/activity',
             headers=self.account.headers,
             params=params,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
-    def list_queue(self):
-        """ List all tests in the queue """
+    def list_tests(self):
+        """ List all tests available to an account """
         res = requests.get(
-            f'{self.account.hq}/iam/account',
+            f'{self.account.hq}/detect/tests',
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
-            account = res.json()
-            return account['queue']
+            return res.json()
         raise Exception(res.text)
 
     @verify_credentials
-    def list_tests(self):
-        """ List all tests available to an account """
+    def get_test(self, test_id):
+        """ Get properties of an existing test """
         res = requests.get(
-            f'{self.account.hq}/detect/tests',
+            f'{self.account.hq}/detect/tests/{test_id}',
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
+    def download(self, test_id, filename):
+        """ Clone a test file or attachment"""
+        res = requests.get(
+            f'{self.account.hq}/detect/tests/{test_id}/{filename}',
+            headers=self.account.headers,
+            timeout=10
+        )
+        if res.status_code == 200:
+            return res.content
+        raise Exception(res.text)
+
+    @verify_credentials
     def enable_test(self, ident: str, run_code: int, tags: str):
         """ Enable a test so endpoints will start running it """
         res = requests.post(
             url=f'{self.account.hq}/detect/queue/{ident}',
             headers=self.account.headers,
             json=dict(code=run_code, tags=tags),
             timeout=10
```

### Comparing `prelude-sdk-1.1.2/prelude_sdk/controllers/iam_controller.py` & `prelude-sdk-1.2.0/prelude_sdk/controllers/iam_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.1.2/prelude_sdk/controllers/partner_controller.py` & `prelude-sdk-1.2.0/prelude_sdk/controllers/partner_controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         res = requests.post(
             f'{self.account.hq}/partner/{name}',
             headers=self.account.headers,
             json=params,
             timeout=10
         )
         if res.status_code == 200:
-            return res.text
+            return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def detach(self, name: str):
         """ Detach a partner from your Detect account """
         res = requests.delete(
             f'{self.account.hq}/partner/{name}',
@@ -31,17 +31,17 @@
             timeout=10
         )
         if res.status_code == 200:
             return res.text
         raise Exception(res.text)
         
     @verify_credentials
-    def endpoints(self, partner_name: str, platform: str, hostname: str = '', offset: int = 0):
+    def endpoints(self, partner_name: str, platform: str, hostname: str = '', offset: int = 0, count: int = 100):
         """ Get a list of endpoints from all partners """
-        params = dict(platform=platform, hostname=hostname, offset=offset)
+        params = dict(platform=platform, hostname=hostname, offset=offset, count=count)
         res = requests.get(
             f'{self.account.hq}/partner/endpoints/{partner_name}',
             headers=self.account.headers,
             params=params,
             timeout=30
         )
         if res.status_code == 200:
```

### Comparing `prelude-sdk-1.1.2/prelude_sdk/models/account.py` & `prelude-sdk-1.2.0/prelude_sdk/models/account.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.1.2/prelude_sdk/models/codes.py` & `prelude-sdk-1.2.0/prelude_sdk/models/codes.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,23 +97,14 @@
                 ExitCode.MALFORMED_VST,
                 ExitCode.TIMEOUT,
                 ExitCode.UNEXPECTED
             ]
         }
 
 
-class Decision(Enum):
-    NONE = 0
-    APPROVE = 1
-    DENY = 2
-
-    @classmethod
-    def _missing_(cls, value):
-        return Decision.NONE
-
 class DOS(Enum):
     none = 'none'
     arm64 = 'arm64'
     x86_64 = 'x86_64'
     aarch64 = 'arm64'
     amd64 = 'x86_64'
     x86 = 'x86_64'
```

### Comparing `prelude-sdk-1.1.2/prelude_sdk.egg-info/PKG-INFO` & `prelude-sdk-1.2.0/prelude_sdk.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.1.2
+Version: 1.2.0
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.1.2/prelude_sdk.egg-info/SOURCES.txt` & `prelude-sdk-1.2.0/prelude_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.1.2/setup.cfg` & `prelude-sdk-1.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-sdk
-version = 1.1.2
+version = 1.2.0
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers =
```

### Comparing `prelude-sdk-1.1.2/tests/conftest.py` & `prelude-sdk-1.2.0/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         def __exit__(self, _1, _2, _3):
             self.capture.resume_global_capture()
 
     yield suspend()
 
 
 def pytest_addoption(parser):
-    parser.addoption("--api", default='https://api.staging.preludesecurity.com', action='store', help='API target for tests')
+    parser.addoption("--api", default='https://api.us2.preludesecurity.com', action='store', help='API target for tests')
     parser.addoption('--email', default='test@auto-accept.developer.preludesecurity.com', action='store', help='Email address to use for testing')
 
 
 @pytest.fixture(scope='session')
 def api(pytestconfig):
     return pytestconfig.getoption('api')
```

### Comparing `prelude-sdk-1.1.2/tests/test_detect_controller.py` & `prelude-sdk-1.2.0/tests/test_detect_controller.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 from datetime import datetime, timedelta, time
 
 import pytest
 import subprocess
 
-from prelude_sdk.models.codes import Decision, RunCode
+from prelude_sdk.models.codes import RunCode
+from prelude_sdk.controllers.iam_controller import IAMController
 from prelude_sdk.controllers.detect_controller import DetectController
 
 
 @pytest.mark.order(after='test_probe_controller.py::TestProbeController::test_download')
 class TestDetectController:
 
     def setup_class(self):
@@ -16,14 +17,45 @@
         self.host = 'test_host'
         self.serial = 'test_serial'
         self.edr_id = 'test_edr_id'
         self.tags = 'test_tag'
         self.health_check = '39de298a-911d-4a3b-aed4-1e8281010a9a'
         self.recommendation = 'Test'
         self.detect = DetectController(pytest.account)
+        self.iam = IAMController(pytest.account)
+
+    def test_list_advisories(self, unwrap):
+        """Test list_advisories method"""
+        res = unwrap(self.detect.list_advisories)(self.detect)
+        assert len(res) > 0
+        assert 'id' in res[0]
+        assert 'name' in res[0]
+        assert 'source' in res[0]
+        assert 'published' in res[0]
+
+    def test_list_tests(self, unwrap):
+        """Test list_tests method"""
+        res = unwrap(self.detect.list_tests)(self.detect)
+        assert len(res) > 0
+        tests = [test for test in res if test['id'] != self.health_check]
+        pytest.test_id = tests[0]['id']
+
+    def test_get_test(self, unwrap):
+        """Test get_test method"""
+        res = unwrap(self.detect.get_test)(self.detect, test_id=pytest.test_id)
+        assert res['id'] == pytest.test_id
+
+    def test_download(self, unwrap):
+        """Test download method"""
+        res = unwrap(self.detect.download)(self.detect, test_id=pytest.test_id, filename=f'{pytest.test_id}.go')
+        assert res is not None
+        with open(f'{pytest.test_id}.go', 'wb') as f:
+            f.write(res)
+        assert os.path.isfile(f'{pytest.test_id}.go')
+        os.remove(f'{pytest.test_id}.go')
 
     def test_register_endpoint(self, unwrap):
         """Test register_endpoint method"""
         res = unwrap(self.detect.register_endpoint)(self.detect, host=self.host, serial_num=self.serial, edr_id=self.edr_id, tags=self.tags)
         assert len(res) == 32
         pytest.endpoint_token = res
 
@@ -33,33 +65,19 @@
         assert len(res) > 0
         assert self.host == res[0]['host']
         assert self.serial == res[0]['serial_num']
         assert self.edr_id == res[0]['edr_id']
         assert self.tags in res[0]['tags']
         pytest.endpoint_id = res[0]['endpoint_id']
 
-    def test_list_tests(self, unwrap):
-        """Test list_tests method"""
-        res = unwrap(self.detect.list_tests)(self.detect)
-        assert len(res) > 0
-        tests = [test for test in res if test['id'] != self.health_check]
-        pytest.test_id = tests[0]['id']
-
-    def test_list_queue(self, unwrap):
-        """Test list_queue method"""
-        res = unwrap(self.detect.list_queue)(self.detect)
-        assert len(res) > 0
-        assert self.health_check == res[0]['test']
-        assert RunCode.DAILY.value == res[0]['run_code']
-
     def test_enable_test(self, unwrap):
         """Test enable_test method"""
         unwrap(self.detect.enable_test)(self.detect, ident=pytest.test_id, run_code=RunCode.DEBUG.value, tags=self.tags)
-        res = unwrap(self.detect.list_queue)(self.detect)
-        assert len([test for test in res if test['test'] == pytest.test_id]) == 1
+        queue = unwrap(self.iam.get_account)(self.iam)['queue']
+        assert len([test for test in queue if test['test'] == pytest.test_id]) == 1
 
     def test_describe_activity(self, unwrap):
         """Test describe_activity method"""
         try:
             subprocess.run([pytest.probe], capture_output=True, env={'PRELUDE_TOKEN': pytest.endpoint_token}, timeout=20)
         except subprocess.TimeoutExpired:
             filters = dict(
@@ -70,20 +88,21 @@
             assert len(describe_activity) == 2
         finally:
             os.remove(pytest.probe)
 
     def test_disable_test(self, unwrap):
         """Test disable_test method"""
         unwrap(self.detect.disable_test)(self.detect, ident=pytest.test_id, tags=self.tags)
-        res = unwrap(self.detect.list_queue)(self.detect)
-        assert len([test for test in res if test['test'] == pytest.test_id]) == 0
+        queue = unwrap(self.iam.get_account)(self.iam)['queue']
+        assert len([test for test in queue if test['test'] == pytest.test_id]) == 0
 
     def test_social_stats(self, unwrap):
         """Test social_stats method"""
         res = unwrap(self.detect.social_stats)(self.detect, ident=pytest.test_id)
         assert len(res.values()) >= 1
 
     def test_delete_endpoint(self, unwrap):
         """Test delete_endpoint method"""
         unwrap(self.detect.delete_endpoint)(self.detect, ident=pytest.endpoint_id)
         res = unwrap(self.detect.list_endpoints)(self.detect)
         assert len(res) == 0
+
```

### Comparing `prelude-sdk-1.1.2/tests/test_iam_controller.py` & `prelude-sdk-1.2.0/tests/test_iam_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         res = unwrap(iam.get_account)(iam)
         assert len([user for user in res['users'] if user['handle'] == 'registration']) == 1
 
     @pytest.mark.order(4)
     def test_delete_user(self, unwrap):
         """Test delete_user method"""
         iam = IAMController(pytest.account)
-        res = unwrap(iam.delete_user)(iam, handle='registration')
+        unwrap(iam.delete_user)(iam, handle='registration')
         res = unwrap(iam.get_account)(iam)
         assert len([user for user in res['users'] if user['handle'] == 'registration']) == 0
 
     @pytest.mark.order(after='test_detect_controller.py::TestDetectController::test_describe_activity')
     def test_update_account(self, unwrap):
         """Test update_account method"""
         iam = IAMController(pytest.account)
```

### Comparing `prelude-sdk-1.1.2/tests/test_probe_controller.py` & `prelude-sdk-1.2.0/tests/test_probe_controller.py`

 * *Files identical despite different names*

