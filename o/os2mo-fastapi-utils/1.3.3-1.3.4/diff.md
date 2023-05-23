# Comparing `tmp/os2mo_fastapi_utils-1.3.3.tar.gz` & `tmp/os2mo_fastapi_utils-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os2mo_fastapi_utils-1.3.3.tar", max compression
+gzip compressed data, was "os2mo_fastapi_utils-1.3.4.tar", max compression
```

## Comparing `os2mo_fastapi_utils-1.3.3.tar` & `os2mo_fastapi_utils-1.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0        0        0        0 2023-05-23 15:28:30.077868 os2mo_fastapi_utils-1.3.3/LICENSES/
--rw-r--r--   0        0        0    16725 2023-05-23 15:28:30.077868 os2mo_fastapi_utils-1.3.3/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0     1426 2023-05-23 15:28:30.077868 os2mo_fastapi_utils-1.3.3/README.md
--rw-r--r--   0        0        0       75 2023-05-23 15:28:30.077868 os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 15:28:30.139873 os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/auth/__init__.py
--rw-r--r--   0        0        0     1064 2023-05-23 15:28:30.077868 os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/auth/exceptions.py
--rw-r--r--   0        0        0      537 2023-05-23 15:28:30.078868 os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/auth/models.py
--rw-r--r--   0        0        0     4937 2023-05-23 15:28:30.078868 os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/auth/oidc.py
--rw-r--r--   0        0        0     2203 2023-05-23 15:28:30.078868 os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/auth/test_helper.py
--rw-r--r--   0        0        0        0 2023-05-23 15:28:30.141873 os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/py.typed
--rw-r--r--   0        0        0     2396 2023-05-23 15:28:30.078868 os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/pydantic_types.py
--rw-r--r--   0        0        0     4678 2023-05-23 15:28:30.078868 os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/tracing.py
--rw-r--r--   0        0        0     1332 2023-05-23 15:28:30.809929 os2mo_fastapi_utils-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     2761 1970-01-01 00:00:00.000000 os2mo_fastapi_utils-1.3.3/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-05-23 16:14:50.734984 os2mo_fastapi_utils-1.3.4/LICENSES/
+-rw-r--r--   0        0        0    16725 2023-05-23 16:14:50.735983 os2mo_fastapi_utils-1.3.4/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0     1426 2023-05-23 16:14:50.735983 os2mo_fastapi_utils-1.3.4/README.md
+-rw-r--r--   0        0        0       75 2023-05-23 16:14:50.735983 os2mo_fastapi_utils-1.3.4/os2mo_fastapi_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 16:14:50.779987 os2mo_fastapi_utils-1.3.4/os2mo_fastapi_utils/auth/__init__.py
+-rw-r--r--   0        0        0     1064 2023-05-23 16:14:50.735983 os2mo_fastapi_utils-1.3.4/os2mo_fastapi_utils/auth/exceptions.py
+-rw-r--r--   0        0        0      537 2023-05-23 16:14:50.735983 os2mo_fastapi_utils-1.3.4/os2mo_fastapi_utils/auth/models.py
+-rw-r--r--   0        0        0     4937 2023-05-23 16:14:50.736984 os2mo_fastapi_utils-1.3.4/os2mo_fastapi_utils/auth/oidc.py
+-rw-r--r--   0        0        0     2203 2023-05-23 16:14:50.736984 os2mo_fastapi_utils-1.3.4/os2mo_fastapi_utils/auth/test_helper.py
+-rw-r--r--   0        0        0        0 2023-05-23 16:14:50.779987 os2mo_fastapi_utils-1.3.4/os2mo_fastapi_utils/py.typed
+-rw-r--r--   0        0        0     2396 2023-05-23 16:14:50.736984 os2mo_fastapi_utils-1.3.4/os2mo_fastapi_utils/pydantic_types.py
+-rw-r--r--   0        0        0     4678 2023-05-23 16:14:50.736984 os2mo_fastapi_utils-1.3.4/os2mo_fastapi_utils/tracing.py
+-rw-r--r--   0        0        0     1373 2023-05-23 16:14:51.892081 os2mo_fastapi_utils-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 os2mo_fastapi_utils-1.3.4/PKG-INFO
```

### Comparing `os2mo_fastapi_utils-1.3.3/LICENSES/MPL-2.0.txt` & `os2mo_fastapi_utils-1.3.4/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `os2mo_fastapi_utils-1.3.3/README.md` & `os2mo_fastapi_utils-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/auth/exceptions.py` & `os2mo_fastapi_utils-1.3.4/os2mo_fastapi_utils/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/auth/models.py` & `os2mo_fastapi_utils-1.3.4/os2mo_fastapi_utils/auth/models.py`

 * *Files identical despite different names*

### Comparing `os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/auth/oidc.py` & `os2mo_fastapi_utils-1.3.4/os2mo_fastapi_utils/auth/oidc.py`

 * *Files identical despite different names*

### Comparing `os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/auth/test_helper.py` & `os2mo_fastapi_utils-1.3.4/os2mo_fastapi_utils/auth/test_helper.py`

 * *Files identical despite different names*

### Comparing `os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/pydantic_types.py` & `os2mo_fastapi_utils-1.3.4/os2mo_fastapi_utils/pydantic_types.py`

 * *Files identical despite different names*

### Comparing `os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/tracing.py` & `os2mo_fastapi_utils-1.3.4/os2mo_fastapi_utils/tracing.py`

 * *Files identical despite different names*

### Comparing `os2mo_fastapi_utils-1.3.3/pyproject.toml` & `os2mo_fastapi_utils-1.3.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # SPDX-FileCopyrightText: Magenta ApS
 #
 # SPDX-License-Identifier: MPL-2.0
 
 [tool.poetry]
 name = "os2mo-fastapi-utils"
-version = "1.3.3"
+version = "1.3.4"
 description = "FastAPI utils for os2mo"
 authors = ["Magenta <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/os2mo-fastapi-utils"
 keywords = ["os2mo-fastapi-utils", "os2mo", "fastapi", "utils"]
 include = ["os2mo_fastapi_utils/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-fastapi = "^0.95.2"
-httpx = "^0.24.1"
-pydantic = {extras = ["email"], version = "^1.10.7"}
-opentelemetry-api = "^1.18.0"
-opentelemetry-sdk = "^1.18.0"
-opentelemetry-exporter-jaeger = "^1.18.0"
-opentelemetry-instrumentation-aiohttp-client = "^0.39b0"
-opentelemetry-instrumentation-requests = "^0.39b0"
-opentelemetry-instrumentation-fastapi = "^0.39b0"
-opentelemetry-instrumentation-httpx = "^0.39b0"
-pyjwt = {extras = ["crypto"], version = "^2.7.0"}
-structlog = "^23.1.0"
-requests = "^2.31.0"
-aiohttp = "^3.8.4"
+fastapi = ">=0.85, <1"
+httpx = ">=0.19, <1"
+pydantic = {extras = ["email"], version = ">=1.10, <2"}
+opentelemetry-api = ">=1.18, <2"
+opentelemetry-sdk = ">=1.18, <2"
+opentelemetry-exporter-jaeger = ">=1.18, <2"
+opentelemetry-instrumentation-aiohttp-client = ">=0.39b0, <1"
+opentelemetry-instrumentation-requests = ">=0.39b0, <1"
+opentelemetry-instrumentation-fastapi = ">=0.39b0, <1"
+opentelemetry-instrumentation-httpx = ">=0.39b0, <1"
+pyjwt = {extras = ["crypto"], version = ">=2.7, <3"}
+structlog = ">=22.1"
+requests = ">=2, <3"
+aiohttp = ">=3, <4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 pytest-split = "^0.8.1"
 pre-commit = "^3.3.2"
```

### Comparing `os2mo_fastapi_utils-1.3.3/PKG-INFO` & `os2mo_fastapi_utils-1.3.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: os2mo-fastapi-utils
-Version: 1.3.3
+Version: 1.3.4
 Summary: FastAPI utils for os2mo
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo-fastapi-utils,os2mo,fastapi,utils
 Author: Magenta
 Author-email: info@magenta.dk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: fastapi (>=0.95.2,<0.96.0)
-Requires-Dist: httpx (>=0.24.1,<0.25.0)
-Requires-Dist: opentelemetry-api (>=1.18.0,<2.0.0)
-Requires-Dist: opentelemetry-exporter-jaeger (>=1.18.0,<2.0.0)
-Requires-Dist: opentelemetry-instrumentation-aiohttp-client (>=0.39b0,<0.40)
-Requires-Dist: opentelemetry-instrumentation-fastapi (>=0.39b0,<0.40)
-Requires-Dist: opentelemetry-instrumentation-httpx (>=0.39b0,<0.40)
-Requires-Dist: opentelemetry-instrumentation-requests (>=0.39b0,<0.40)
-Requires-Dist: opentelemetry-sdk (>=1.18.0,<2.0.0)
-Requires-Dist: pydantic[email] (>=1.10.7,<2.0.0)
-Requires-Dist: pyjwt[crypto] (>=2.7.0,<3.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: structlog (>=23.1.0,<24.0.0)
+Requires-Dist: aiohttp (>=3,<4)
+Requires-Dist: fastapi (>=0.85,<1)
+Requires-Dist: httpx (>=0.19,<1)
+Requires-Dist: opentelemetry-api (>=1.18,<2)
+Requires-Dist: opentelemetry-exporter-jaeger (>=1.18,<2)
+Requires-Dist: opentelemetry-instrumentation-aiohttp-client (>=0.39b0,<1)
+Requires-Dist: opentelemetry-instrumentation-fastapi (>=0.39b0,<1)
+Requires-Dist: opentelemetry-instrumentation-httpx (>=0.39b0,<1)
+Requires-Dist: opentelemetry-instrumentation-requests (>=0.39b0,<1)
+Requires-Dist: opentelemetry-sdk (>=1.18,<2)
+Requires-Dist: pydantic[email] (>=1.10,<2)
+Requires-Dist: pyjwt[crypto] (>=2.7,<3)
+Requires-Dist: requests (>=2,<3)
+Requires-Dist: structlog (>=22.1)
 Project-URL: Repository, https://git.magenta.dk/rammearkitektur/os2mo-fastapi-utils
 Description-Content-Type: text/markdown
 
 <!--
 SPDX-FileCopyrightText: Magenta ApS
 
 SPDX-License-Identifier: MPL-2.0
```

