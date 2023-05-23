# Comparing `tmp/sag-py-fastapi-health-0.1.1.tar.gz` & `tmp/sag-py-fastapi-health-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-fastapi-health-0.1.1.tar", last modified: Thu Apr 20 08:46:10 2023, max compression
+gzip compressed data, was "sag-py-fastapi-health-0.1.2.tar", last modified: Tue May 23 16:57:59 2023, max compression
```

## Comparing `sag-py-fastapi-health-0.1.1.tar` & `sag-py-fastapi-health-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:46:10.128703 sag-py-fastapi-health-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-04-20 08:46:10.128703 sag-py-fastapi-health-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:46:10.128703 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:46:10.128703 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/checks/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/checks/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:46:10.128703 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-04-20 08:46:10.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-20 08:46:10.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 08:46:10.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-20 08:46:10.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 08:46:10.000000 sag-py-fastapi-health-0.1.1/sag_py_fastapi_health.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-20 08:46:10.128703 sag-py-fastapi-health-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:46:10.128703 sag-py-fastapi-health-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/tests/test_checks_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/tests/test_checks_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/tests/test_json_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/tests/test_prtg_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-20 08:45:52.000000 sag-py-fastapi-health-0.1.1/tests/test_router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:57:59.155921 sag-py-fastapi-health-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-23 16:57:59.155921 sag-py-fastapi-health-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:57:59.147921 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:57:59.151921 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/checks/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/checks/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:57:59.151921 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-23 16:57:59.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-23 16:57:59.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:57:59.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-23 16:57:59.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 16:57:59.000000 sag-py-fastapi-health-0.1.2/sag_py_fastapi_health.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-23 16:57:59.155921 sag-py-fastapi-health-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:57:59.151921 sag-py-fastapi-health-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/tests/test_checks_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/tests/test_checks_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/tests/test_json_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/tests/test_prtg_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-23 16:57:49.000000 sag-py-fastapi-health-0.1.2/tests/test_router.py
```

### Comparing `sag-py-fastapi-health-0.1.1/LICENSE.txt` & `sag-py-fastapi-health-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.1/PKG-INFO` & `sag-py-fastapi-health-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-fastapi-health
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for fastapi health checks
 Home-page: https://github.com/SamhammerAG/sag_py_fastapi_health
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_fastapi_health
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_fastapi_health/issues
```

### Comparing `sag-py-fastapi-health-0.1.1/README.md` & `sag-py-fastapi-health-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/checks/http.py` & `sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/checks/http.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/checks/storage.py` & `sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/checks/storage.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/formatter.py` & `sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/formatter.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/models.py` & `sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 from fastapi import Response
 from pydantic import BaseModel
 
 
 class CheckResult(BaseModel):
     name: str
-    status: Literal["Healthy", "Unhealthy", "Degraded"]
+    status: Literal["Healthy", "Unhealthy", "Degraded"] = "Unhealthy"
     duration: float = 0
     description: Optional[str] = None
 
 
 class Check(ABC):
     @abstractmethod
     async def __call__(self) -> CheckResult:
         ...  # pragma: no cover
 
 
 class HealthcheckReport(BaseModel):
-    status: Literal["Healthy", "Unhealthy", "Degraded"]
+    status: Literal["Healthy", "Unhealthy", "Degraded"] = "Unhealthy"
     total_duration: float
     entries: List[CheckResult]
 
 
 class HealthResponseFormatter:
     @abstractmethod
     def get_response_type(self) -> Type[BaseModel]:
```

### Comparing `sag-py-fastapi-health-0.1.1/sag_py_fastapi_health/router.py` & `sag-py-fastapi-health-0.1.2/sag_py_fastapi_health/router.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.1/sag_py_fastapi_health.egg-info/PKG-INFO` & `sag-py-fastapi-health-0.1.2/sag_py_fastapi_health.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-fastapi-health
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for fastapi health checks
 Home-page: https://github.com/SamhammerAG/sag_py_fastapi_health
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_fastapi_health
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_fastapi_health/issues
```

### Comparing `sag-py-fastapi-health-0.1.1/sag_py_fastapi_health.egg-info/SOURCES.txt` & `sag-py-fastapi-health-0.1.2/sag_py_fastapi_health.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.1/setup.py` & `sag-py-fastapi-health-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     REQS = fin.read().splitlines()
 
 with open("requirements-dev.txt", "r") as fin:
     REQS_DEV = [item for item in fin.read().splitlines() if not item.endswith(".txt")]
 
 setuptools.setup(
     name="sag-py-fastapi-health",
-    version="0.1.1",
+    version="0.1.2",
     description="A library for fastapi health checks",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_fastapi_health",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
```

### Comparing `sag-py-fastapi-health-0.1.1/tests/test_checks_http.py` & `sag-py-fastapi-health-0.1.2/tests/test_checks_http.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.1/tests/test_checks_storage.py` & `sag-py-fastapi-health-0.1.2/tests/test_checks_storage.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.1/tests/test_json_formatter.py` & `sag-py-fastapi-health-0.1.2/tests/test_json_formatter.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.1/tests/test_prtg_formatter.py` & `sag-py-fastapi-health-0.1.2/tests/test_prtg_formatter.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.1/tests/test_router.py` & `sag-py-fastapi-health-0.1.2/tests/test_router.py`

 * *Files identical despite different names*

