# Comparing `tmp/sag-py-fastapi-health-0.1.2.tar.gz` & `tmp/sag-py-fastapi-health-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-fastapi-health-0.1.2.tar", last modified: Tue May 23 16:57:59 2023, max compression
+gzip compressed data, was "sag-py-fastapi-health-0.1.3.tar", last modified: Tue May 23 17:25:31 2023, max compression
```

## Comparing `sag-py-fastapi-health-0.1.2.tar` & `sag-py-fastapi-health-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:57:59.155921 sag-py-fastapi-health-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-23 16:57:59.155921 sag-py-fastapi-health-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:57:59.147921 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:57:59.151921 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/checks/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/checks/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:57:59.151921 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-23 16:57:59.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-23 16:57:59.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:57:59.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-23 16:57:59.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 16:57:59.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-23 16:57:59.155921 sag-py-fastapi-health-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:57:59.151921 sag-py-fastapi-health-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/tests/test_checks_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/tests/test_checks_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/tests/test_json_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/tests/test_prtg_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/tests/test_router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:25:31.247773 sag-py-fastapi-health-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-23 17:25:31.247773 sag-py-fastapi-health-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:25:31.247773 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:25:31.247773 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/checks/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/checks/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:25:31.247773 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-23 17:25:31.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-23 17:25:31.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:25:31.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-23 17:25:31.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 17:25:31.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-23 17:25:31.247773 sag-py-fastapi-health-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:25:31.247773 sag-py-fastapi-health-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/tests/test_checks_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/tests/test_checks_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/tests/test_json_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/tests/test_prtg_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/tests/test_router.py
```

### Comparing `sag-py-fastapi-health-0.1.2/LICENSE.txt` & `sag-py-fastapi-health-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.2/PKG-INFO` & `sag-py-fastapi-health-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-fastapi-health
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library for fastapi health checks
 Home-page: https://github.com/SamhammerAG/sag_py_fastapi_health
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_fastapi_health
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_fastapi_health/issues
```

### Comparing `sag-py-fastapi-health-0.1.2/README.md` & `sag-py-fastapi-health-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/checks/http.py` & `sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/checks/http.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/checks/storage.py` & `sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/checks/storage.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/formatter.py` & `sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/formatter.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/models.py` & `sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import re
 from abc import ABC, abstractmethod
-from typing import Iterable, List, Literal, NamedTuple, Optional, Type
+from typing import Iterable, List, NamedTuple, Optional, Type
 
 from fastapi import Response
 from pydantic import BaseModel
+from typing_extensions import Literal
 
 
 class CheckResult(BaseModel):
     name: str
-    status: Literal["Healthy", "Unhealthy", "Degraded"] = "Unhealthy"
+    status: Literal["Healthy", "Unhealthy", "Degraded"]
     duration: float = 0
     description: Optional[str] = None
 
 
 class Check(ABC):
     @abstractmethod
     async def __call__(self) -> CheckResult:
         ...  # pragma: no cover
 
 
 class HealthcheckReport(BaseModel):
-    status: Literal["Healthy", "Unhealthy", "Degraded"] = "Unhealthy"
+    status: Literal["Healthy", "Unhealthy", "Degraded"]
     total_duration: float
     entries: List[CheckResult]
 
 
 class HealthResponseFormatter:
     @abstractmethod
     def get_response_type(self) -> Type[BaseModel]:
```

### Comparing `sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/router.py` & `sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/router.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.2/sag_py_fastapi_health.egg-info/PKG-INFO` & `sag-py-fastapi-health-0.1.3/sag_py_fastapi_health.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-fastapi-health
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library for fastapi health checks
 Home-page: https://github.com/SamhammerAG/sag_py_fastapi_health
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_fastapi_health
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_fastapi_health/issues
```

### Comparing `sag-py-fastapi-health-0.1.2/sag_py_fastapi_health.egg-info/SOURCES.txt` & `sag-py-fastapi-health-0.1.3/sag_py_fastapi_health.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.2/setup.py` & `sag-py-fastapi-health-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     REQS = fin.read().splitlines()
 
 with open("requirements-dev.txt", "r") as fin:
     REQS_DEV = [item for item in fin.read().splitlines() if not item.endswith(".txt")]
 
 setuptools.setup(
     name="sag-py-fastapi-health",
-    version="0.1.2",
+    version="0.1.3",
     description="A library for fastapi health checks",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_fastapi_health",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
```

### Comparing `sag-py-fastapi-health-0.1.2/tests/test_checks_http.py` & `sag-py-fastapi-health-0.1.3/tests/test_checks_http.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.2/tests/test_checks_storage.py` & `sag-py-fastapi-health-0.1.3/tests/test_checks_storage.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.2/tests/test_json_formatter.py` & `sag-py-fastapi-health-0.1.3/tests/test_json_formatter.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.2/tests/test_prtg_formatter.py` & `sag-py-fastapi-health-0.1.3/tests/test_prtg_formatter.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.2/tests/test_router.py` & `sag-py-fastapi-health-0.1.3/tests/test_router.py`

 * *Files identical despite different names*

