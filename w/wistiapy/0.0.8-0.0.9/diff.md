# Comparing `tmp/wistiapy-0.0.8.tar.gz` & `tmp/wistiapy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wistiapy-0.0.8.tar", last modified: Fri Oct  4 07:06:49 2019, max compression
+gzip compressed data, was "dist/wistiapy-0.0.9.tar", last modified: Tue Feb 14 07:17:24 2023, max compression
```

## Comparing `wistiapy-0.0.8.tar` & `wistiapy-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 07:06:49.000000 wistiapy-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (115)     2185 2019-10-04 07:06:49.000000 wistiapy-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     1209 2019-10-04 07:06:40.000000 wistiapy-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (115)       38 2019-10-04 07:06:49.000000 wistiapy-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)     1391 2019-10-04 07:06:40.000000 wistiapy-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 07:06:49.000000 wistiapy-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-10-04 07:06:40.000000 wistiapy-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     1267 2019-10-04 07:06:40.000000 wistiapy-0.0.8/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (115)      653 2019-10-04 07:06:40.000000 wistiapy-0.0.8/tests/test_media.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 07:06:49.000000 wistiapy-0.0.8/wistia/
--rw-r--r--   0 runner    (1001) docker     (115)      260 2019-10-04 07:06:40.000000 wistiapy-0.0.8/wistia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)       22 2019-10-04 07:06:40.000000 wistiapy-0.0.8/wistia/__version__.py
--rw-r--r--   0 runner    (1001) docker     (115)     1405 2019-10-04 07:06:40.000000 wistiapy-0.0.8/wistia/cli.py
--rw-r--r--   0 runner    (1001) docker     (115)     9381 2019-10-04 07:06:40.000000 wistiapy-0.0.8/wistia/client.py
--rw-r--r--   0 runner    (1001) docker     (115)     6880 2019-10-04 07:06:40.000000 wistiapy-0.0.8/wistia/dummy.py
--rw-r--r--   0 runner    (1001) docker     (115)     1097 2019-10-04 07:06:40.000000 wistiapy-0.0.8/wistia/helpers.py
--rw-r--r--   0 runner    (1001) docker     (115)     9945 2019-10-04 07:06:40.000000 wistiapy-0.0.8/wistia/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-10-04 07:06:49.000000 wistiapy-0.0.8/wistiapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)     2185 2019-10-04 07:06:49.000000 wistiapy-0.0.8/wistiapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)      394 2019-10-04 07:06:49.000000 wistiapy-0.0.8/wistiapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2019-10-04 07:06:49.000000 wistiapy-0.0.8/wistiapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)       44 2019-10-04 07:06:49.000000 wistiapy-0.0.8/wistiapy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (115)      105 2019-10-04 07:06:49.000000 wistiapy-0.0.8/wistiapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)       13 2019-10-04 07:06:49.000000 wistiapy-0.0.8/wistiapy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 07:17:24.000000 wistiapy-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-02-14 07:17:18.000000 wistiapy-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-02-14 07:17:24.000000 wistiapy-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-02-14 07:17:18.000000 wistiapy-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 07:17:24.000000 wistiapy-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-02-14 07:17:18.000000 wistiapy-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 07:17:24.000000 wistiapy-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 07:17:18.000000 wistiapy-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-02-14 07:17:18.000000 wistiapy-0.0.9/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-02-14 07:17:18.000000 wistiapy-0.0.9/tests/test_media.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 07:17:24.000000 wistiapy-0.0.9/wistia/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-14 07:17:18.000000 wistiapy-0.0.9/wistia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-14 07:17:18.000000 wistiapy-0.0.9/wistia/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-02-14 07:17:18.000000 wistiapy-0.0.9/wistia/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-02-14 07:17:18.000000 wistiapy-0.0.9/wistia/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-02-14 07:17:18.000000 wistiapy-0.0.9/wistia/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-02-14 07:17:18.000000 wistiapy-0.0.9/wistia/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-02-14 07:17:18.000000 wistiapy-0.0.9/wistia/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 07:17:24.000000 wistiapy-0.0.9/wistiapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-02-14 07:17:24.000000 wistiapy-0.0.9/wistiapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-02-14 07:17:24.000000 wistiapy-0.0.9/wistiapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 07:17:24.000000 wistiapy-0.0.9/wistiapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-14 07:17:24.000000 wistiapy-0.0.9/wistiapy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-14 07:17:24.000000 wistiapy-0.0.9/wistiapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-14 07:17:24.000000 wistiapy-0.0.9/wistiapy.egg-info/top_level.txt
```

### Comparing `wistiapy-0.0.8/PKG-INFO` & `wistiapy-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 Metadata-Version: 2.1
 Name: wistiapy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python client for the Wistia data API
 Home-page: https://github.com/Edrolo/wistiapy
 Author: Matt Fisher
 Author-email: matt@edrolo.com
 License: MIT
-Description: # Wistia Python client
-        
-        A Python client for the [Wistia Data API](https://wistia.com/support/developers/data-api)
-        
-        ![](https://github.com/Edrolo/wistiapy/workflows/Python%20Tests/badge.svg)
-        [![PyPI version](https://badge.fury.io/py/wistiapy.svg)](https://badge.fury.io/py/wistiapy)
-        
-        ## Installation
-        ```bash
-        pip install wistiapy
-        ```
-        
-        You'll need to create an access token [as documented](https://wistia.com/support/developers/data-api#creating-and-managing-access-tokens).
-        
-        ## Usage
-        
-        ```python
-        from wistia import WistiaClient
-        wistia = WistiaClient(api_password='YOUR_API_PASSWORD')
-        projects = wistia.list_projects()
-        ```
-        
-        Alternatively, you can set your password in an environment variable, or, if using Django, in a
-        setting called `WISTIA_API_PASSWORD`. Then use the factory function:
-        ```python
-        from wistia import get_wistia_client
-        wistia = get_wistia_client()
-        ```
-        
-        ## Dummy Client
-        Included is a mock version of the client for testing purposes. It will log any calls made to it,
-        and attempts to respond in the same manner as the live service. Currently a work-in-progress.
-        If using Django, including the setting `WISTIA_CLIENT_CLASS = 'WistiaDummyClient'` will make
-        `get_wistia_client` provide a dummy client.
-        
 Keywords: wistia api client
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# Wistia Python client
+
+A Python client for the [Wistia Data API](https://wistia.com/support/developers/data-api)
+
+![](https://github.com/Edrolo/wistiapy/workflows/Python%20Tests/badge.svg)
+[![PyPI version](https://badge.fury.io/py/wistiapy.svg)](https://badge.fury.io/py/wistiapy)
+
+## Installation
+```bash
+pip install wistiapy
+```
+
+You'll need to create an access token [as documented](https://wistia.com/support/developers/data-api#creating-and-managing-access-tokens).
+
+## Usage
+
+```python
+from wistia import WistiaClient
+wistia = WistiaClient(api_password='YOUR_API_PASSWORD')
+projects = wistia.list_projects()
+```
+
+Alternatively, you can set your password in an environment variable, or, if using Django, in a
+setting called `WISTIA_API_PASSWORD`. Then use the factory function:
+```python
+from wistia import get_wistia_client
+wistia = get_wistia_client()
+```
+
+## Dummy Client
+Included is a mock version of the client for testing purposes. It will log any calls made to it,
+and attempts to respond in the same manner as the live service. Currently a work-in-progress.
+If using Django, including the setting `WISTIA_CLIENT_CLASS = 'WistiaDummyClient'` will make
+`get_wistia_client` provide a dummy client.
```

### Comparing `wistiapy-0.0.8/README.md` & `wistiapy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `wistiapy-0.0.8/setup.py` & `wistiapy-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,20 +24,23 @@
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     keywords="wistia api client",
     include_package_data=False,
     install_requires=[
         "requests>=2.22.0,<3.0.0",
         "factory-boy>=2.7.0,<3.0.0",
-        "schematics<=2.1.0,<3.0.0",
+        "schematics>=2.1.1,<3.0.0",
     ],
     extras_require={"dev": ["black", "pytest", "responses"]},
     entry_points={"console_scripts": ["wistia = wistia.cli:main"]},
 )
```

### Comparing `wistiapy-0.0.8/tests/test_client.py` & `wistiapy-0.0.9/tests/test_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-import base64
-
 import responses
 import pytest
 
 from wistia.client import WistiaClient
 
 
-def generate_http_basic_auth_string(username, password):
-    encoded_string = base64.b64encode(f"{username}:{password}".encode("utf-8")).decode(
-        "ascii"
-    )
-    return f"Basic {encoded_string}"
+def generate_http_bearer_auth_string(password):
+    return f"Bearer {password}"
 
 
 @pytest.fixture
 def wistia_client():
     password = "letmein"
     return WistiaClient(api_password=password)
 
 
 @responses.activate
 def test_authentication_set_correctly_in_header(wistia_client):
     # Given
-    expected_url = f"https://api.wistia.com/v1/medias.json"
+    expected_url = 'https://api.wistia.com/v1/medias.json'
     responses.add(responses.GET, url=expected_url, json={}, status=200)
 
     # When
     wistia_client.list_medias()
 
     # Then
-    expected_auth_header = generate_http_basic_auth_string("api", "letmein")
+    expected_auth_header = generate_http_bearer_auth_string("letmein")
     assert expected_auth_header == responses.calls[0].request.headers["Authorization"]
 
 
 @responses.activate
 def test_purchase_captions_hits_correct_endpoint(wistia_client):
     media_hashed_id = "12345"
     expected_url = (
```

### Comparing `wistiapy-0.0.8/wistia/cli.py` & `wistiapy-0.0.9/wistia/cli.py`

 * *Files identical despite different names*

### Comparing `wistiapy-0.0.8/wistia/client.py` & `wistiapy-0.0.9/wistia/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 
 log = logging.getLogger("wistiapy")
 
 
 class WistiaClient:
     API_BASE_URL = "https://api.wistia.com/v1/"
 
-    def __init__(self, user="api", api_password=""):
+    def __init__(self, api_password=""):
         # https://wistia.com/support/developers/data-api#authentication
         self.session = requests.Session()
-        self.session.auth = (user, api_password)
+        self.session.headers = {
+            "Authorization": f"Bearer {api_password}",
+            **self.session.headers
+        }
 
     def request(self, method, rel_path, **kwargs):
         url = f"{self.API_BASE_URL}{rel_path}"
         response = self.session.request(method=method, url=url, **kwargs)
         response.raise_for_status()
-        response_data = response.json()
+        response_data = response.json() if response.text else {}
         return response_data
 
     def get(self, rel_path: str, params: dict = None):
         return self.request("GET", rel_path, params=params)
 
     def post(self, rel_path: str, **kwargs):
         return self.request("POST", rel_path, **kwargs)
@@ -65,16 +68,15 @@
             else:
                 return
 
     def show_project(self, project_hashed_id: str) -> Project:
         # https://wistia.com/support/developers/data-api#projects_show
         rel_path = f"projects/{project_hashed_id}.json"
         project_data = self.get(rel_path)
-        project = Project(project_data, strict=False)
-        return project
+        return Project(project_data, strict=False)
 
     # https://wistia.com/support/developers/data-api#projects_create
     # https://wistia.com/support/developers/data-api#projects_update
     # https://wistia.com/support/developers/data-api#projects_delete
     # https://wistia.com/support/developers/data-api#projects_copy
 
     # Project Sharings
@@ -131,16 +133,15 @@
     # https://wistia.com/support/developers/data-api#account
 
     # Customizations
 
     def show_media_customizations(self, wistia_hashed_id: str) -> dict:
         # https://wistia.com/support/developers/data-api#customizations_show
         rel_path = f"medias/{wistia_hashed_id}/customizations.json"
-        media_customizations_data = self.get(rel_path)
-        return media_customizations_data
+        return self.get(rel_path)
 
     # https://wistia.com/support/developers/data-api#customizations_create
     # https://wistia.com/support/developers/data-api#customizations_update
     # https://wistia.com/support/developers/data-api#customizations_delete
 
     # Captions
 
@@ -159,31 +160,29 @@
         caption_filename: str = "",
         caption_text: str = "",
     ) -> None:
         # https://wistia.com/support/developers/data-api#captions_create
         # Empty 200: OK; 400: already exist; 404: video DNE
         rel_path = f"medias/{wistia_hashed_id}/captions.json"
         if caption_text:
-            r = self.post(
+            self.post(
                 rel_path, data={"language": language_code, "caption_file": caption_text}
             )
         elif caption_filename:
             with open(caption_filename, "rb") as caption_file:
-                r = self.post(
+                self.post(
                     rel_path,
                     data={"language": language_code},
                     files={"caption_file": caption_file},
                 )
         else:
             raise ValueError(
                 "create_captions requires subtitle_filename or subtitle_text"
             )
 
-        r.raise_for_status()
-
     def show_captions(
         self, wistia_hashed_id, language_code: str = "eng"
     ) -> CaptionTrack:
         # https://wistia.com/support/developers/data-api#captions_show
         rel_path = f"medias/{wistia_hashed_id}/captions/{language_code}.json"
         return CaptionTrack(self.get(rel_path))
 
@@ -224,16 +223,15 @@
         # > If it is not null, that value will be set.
         rel_path = f"medias/{wistia_hashed_id}/customizations.json"
         if enabled:
             payload = {"plugin": {"captions-v1": {"onByDefault": False}}}
         else:
             payload = {"plugin": {"captions-v1": None}}
 
-        media_customizations_data = self.put(rel_path, json=payload)
-        return media_customizations_data
+        return self.put(rel_path, json=payload)
 
     def upload_subtitle_file_to_wistia_video(
         self,
         wistia_hashed_id: str,
         subtitle_file_name: str,
         replace=False,
         language_code: str = "eng",
```

### Comparing `wistiapy-0.0.8/wistia/dummy.py` & `wistiapy-0.0.9/wistia/dummy.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 
 class FakeResponse(NamedTuple):
     status_code: int
 
 
 class DummyWistiaClient(WistiaClient):
-    def __init__(self, user="api", api_password=""):
-        super().__init__(user, api_password)
+    def __init__(self, api_password=""):
+        super().__init__(api_password)
         self.session = (
             None
         )  # Make sure we don't hit the API in methods not yet overridden
 
         self.medias = {}
         self.captions = defaultdict(list)
         self.projects = {}
@@ -42,15 +42,15 @@
             f"WISTIA API CALL: list_projects("
             f"sort_by={sort_by!r}, sort_direction={sort_direction!r}, "
             f"page={page!r}, per_page={per_page!r})"
         )
         return self.projects.values()
 
     def list_all_projects(self) -> Iterable[Project]:
-        log.info(f"WISTIA API CALL: list_all_projects()")
+        log.info('WISTIA API CALL: list_all_projects()')
         yield from self.projects.values()
 
     def show_project(self, project_hashed_id: str) -> Project:
         log.info(f"WISTIA API CALL: show_project({project_hashed_id})")
         project = self.projects.get(project_hashed_id, None)
         if not project:
             raise requests.HTTPError(response=FakeResponse(status_code=404))
```

### Comparing `wistiapy-0.0.8/wistia/helpers.py` & `wistiapy-0.0.9/wistia/helpers.py`

 * *Files identical despite different names*

### Comparing `wistiapy-0.0.8/wistia/schema.py` & `wistiapy-0.0.9/wistia/schema.py`

 * *Files identical despite different names*

### Comparing `wistiapy-0.0.8/wistiapy.egg-info/PKG-INFO` & `wistiapy-0.0.9/wistiapy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 Metadata-Version: 2.1
 Name: wistiapy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python client for the Wistia data API
 Home-page: https://github.com/Edrolo/wistiapy
 Author: Matt Fisher
 Author-email: matt@edrolo.com
 License: MIT
-Description: # Wistia Python client
-        
-        A Python client for the [Wistia Data API](https://wistia.com/support/developers/data-api)
-        
-        ![](https://github.com/Edrolo/wistiapy/workflows/Python%20Tests/badge.svg)
-        [![PyPI version](https://badge.fury.io/py/wistiapy.svg)](https://badge.fury.io/py/wistiapy)
-        
-        ## Installation
-        ```bash
-        pip install wistiapy
-        ```
-        
-        You'll need to create an access token [as documented](https://wistia.com/support/developers/data-api#creating-and-managing-access-tokens).
-        
-        ## Usage
-        
-        ```python
-        from wistia import WistiaClient
-        wistia = WistiaClient(api_password='YOUR_API_PASSWORD')
-        projects = wistia.list_projects()
-        ```
-        
-        Alternatively, you can set your password in an environment variable, or, if using Django, in a
-        setting called `WISTIA_API_PASSWORD`. Then use the factory function:
-        ```python
-        from wistia import get_wistia_client
-        wistia = get_wistia_client()
-        ```
-        
-        ## Dummy Client
-        Included is a mock version of the client for testing purposes. It will log any calls made to it,
-        and attempts to respond in the same manner as the live service. Currently a work-in-progress.
-        If using Django, including the setting `WISTIA_CLIENT_CLASS = 'WistiaDummyClient'` will make
-        `get_wistia_client` provide a dummy client.
-        
 Keywords: wistia api client
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# Wistia Python client
+
+A Python client for the [Wistia Data API](https://wistia.com/support/developers/data-api)
+
+![](https://github.com/Edrolo/wistiapy/workflows/Python%20Tests/badge.svg)
+[![PyPI version](https://badge.fury.io/py/wistiapy.svg)](https://badge.fury.io/py/wistiapy)
+
+## Installation
+```bash
+pip install wistiapy
+```
+
+You'll need to create an access token [as documented](https://wistia.com/support/developers/data-api#creating-and-managing-access-tokens).
+
+## Usage
+
+```python
+from wistia import WistiaClient
+wistia = WistiaClient(api_password='YOUR_API_PASSWORD')
+projects = wistia.list_projects()
+```
+
+Alternatively, you can set your password in an environment variable, or, if using Django, in a
+setting called `WISTIA_API_PASSWORD`. Then use the factory function:
+```python
+from wistia import get_wistia_client
+wistia = get_wistia_client()
+```
+
+## Dummy Client
+Included is a mock version of the client for testing purposes. It will log any calls made to it,
+and attempts to respond in the same manner as the live service. Currently a work-in-progress.
+If using Django, including the setting `WISTIA_CLIENT_CLASS = 'WistiaDummyClient'` will make
+`get_wistia_client` provide a dummy client.
```

