# Comparing `tmp/dvc-gs-2.22.0.tar.gz` & `tmp/dvc-gs-2.22.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-gs-2.22.0.tar", last modified: Tue Feb 28 22:30:59 2023, max compression
+gzip compressed data, was "dvc-gs-2.22.1.tar", last modified: Tue May 23 06:41:52 2023, max compression
```

## Comparing `dvc-gs-2.22.0.tar` & `dvc-gs-2.22.1.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 22:30:59.721035 dvc-gs-2.22.0/
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-02-28 22:30:42.000000 dvc-gs-2.22.0/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 22:30:59.713034 dvc-gs-2.22.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 22:30:59.717034 dvc-gs-2.22.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-02-28 22:30:42.000000 dvc-gs-2.22.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1342 2023-02-28 22:30:42.000000 dvc-gs-2.22.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-02-28 22:30:42.000000 dvc-gs-2.22.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1827 2023-02-28 22:30:42.000000 dvc-gs-2.22.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-02-28 22:30:42.000000 dvc-gs-2.22.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-02-28 22:30:42.000000 dvc-gs-2.22.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-02-28 22:30:59.721035 dvc-gs-2.22.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-02-28 22:30:42.000000 dvc-gs-2.22.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 22:30:59.717034 dvc-gs-2.22.0/dvc_gs/
--rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-02-28 22:30:42.000000 dvc-gs-2.22.0/dvc_gs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-02-28 22:30:59.000000 dvc-gs-2.22.0/dvc_gs/_dvc_gs_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-02-28 22:30:42.000000 dvc-gs-2.22.0/dvc_gs/path.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 22:30:59.721035 dvc-gs-2.22.0/dvc_gs/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-28 22:30:42.000000 dvc-gs-2.22.0/dvc_gs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2691 2023-02-28 22:30:42.000000 dvc-gs-2.22.0/dvc_gs/tests/cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)      170 2023-02-28 22:30:42.000000 dvc-gs-2.22.0/dvc_gs/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-02-28 22:30:42.000000 dvc-gs-2.22.0/dvc_gs/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-02-28 22:30:42.000000 dvc-gs-2.22.0/dvc_gs/tests/test_dvc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 22:30:59.717034 dvc-gs-2.22.0/dvc_gs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-02-28 22:30:59.000000 dvc-gs-2.22.0/dvc_gs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-02-28 22:30:59.000000 dvc-gs-2.22.0/dvc_gs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-28 22:30:59.000000 dvc-gs-2.22.0/dvc_gs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-28 22:30:59.000000 dvc-gs-2.22.0/dvc_gs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      503 2023-02-28 22:30:59.000000 dvc-gs-2.22.0/dvc_gs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-02-28 22:30:59.000000 dvc-gs-2.22.0/dvc_gs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-02-28 22:30:42.000000 dvc-gs-2.22.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1536 2023-02-28 22:30:59.721035 dvc-gs-2.22.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-28 22:30:42.000000 dvc-gs-2.22.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 06:41:52.648548 dvc-gs-2.22.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-05-23 06:41:31.000000 dvc-gs-2.22.1/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 06:41:52.636548 dvc-gs-2.22.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 06:41:52.640548 dvc-gs-2.22.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2112 2023-05-23 06:41:31.000000 dvc-gs-2.22.1/.github/workflows/benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-05-23 06:41:31.000000 dvc-gs-2.22.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-05-23 06:41:31.000000 dvc-gs-2.22.1/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-05-23 06:41:31.000000 dvc-gs-2.22.1/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1827 2023-05-23 06:41:31.000000 dvc-gs-2.22.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-05-23 06:41:31.000000 dvc-gs-2.22.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-23 06:41:31.000000 dvc-gs-2.22.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-05-23 06:41:52.648548 dvc-gs-2.22.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-23 06:41:31.000000 dvc-gs-2.22.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 06:41:52.640548 dvc-gs-2.22.1/dvc_gs/
+-rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-05-23 06:41:31.000000 dvc-gs-2.22.1/dvc_gs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-05-23 06:41:52.000000 dvc-gs-2.22.1/dvc_gs/_dvc_gs_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-05-23 06:41:31.000000 dvc-gs-2.22.1/dvc_gs/path.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 06:41:52.648548 dvc-gs-2.22.1/dvc_gs/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 06:41:31.000000 dvc-gs-2.22.1/dvc_gs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-05-23 06:41:31.000000 dvc-gs-2.22.1/dvc_gs/tests/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2749 2023-05-23 06:41:31.000000 dvc-gs-2.22.1/dvc_gs/tests/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-05-23 06:41:31.000000 dvc-gs-2.22.1/dvc_gs/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1085 2023-05-23 06:41:31.000000 dvc-gs-2.22.1/dvc_gs/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-05-23 06:41:31.000000 dvc-gs-2.22.1/dvc_gs/tests/test_dvc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 06:41:52.648548 dvc-gs-2.22.1/dvc_gs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-05-23 06:41:52.000000 dvc-gs-2.22.1/dvc_gs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      619 2023-05-23 06:41:52.000000 dvc-gs-2.22.1/dvc_gs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 06:41:52.000000 dvc-gs-2.22.1/dvc_gs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 06:41:52.000000 dvc-gs-2.22.1/dvc_gs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-05-23 06:41:52.000000 dvc-gs-2.22.1/dvc_gs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-23 06:41:52.000000 dvc-gs-2.22.1/dvc_gs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-05-23 06:41:31.000000 dvc-gs-2.22.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1536 2023-05-23 06:41:52.652549 dvc-gs-2.22.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 06:41:31.000000 dvc-gs-2.22.1/setup.py
```

### Comparing `dvc-gs-2.22.0/.github/workflows/release.yaml` & `dvc-gs-2.22.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `dvc-gs-2.22.0/.github/workflows/tests.yaml` & `dvc-gs-2.22.1/.github/workflows/tests.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -44,16 +44,14 @@
 
     - name: lint
       timeout-minutes: 10
       uses: pre-commit/action@v3.0.0
 
     - name: run tests
       timeout-minutes: 40
-      env:
-        GS_CREDS: "${{ secrets.GS_CREDS }}"
       run: pytest -v -n=auto --cov-report=xml --cov-report=term
 
     - name: upload coverage report
       uses: codecov/codecov-action@v3
       with:
         file: ./coverage.xml
         fail_ci_if_error: false
```

### Comparing `dvc-gs-2.22.0/.github/workflows/update-template.yaml` & `dvc-gs-2.22.1/.github/workflows/update-template.yaml`

 * *Files identical despite different names*

### Comparing `dvc-gs-2.22.0/.gitignore` & `dvc-gs-2.22.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-gs-2.22.0/.pre-commit-config.yaml` & `dvc-gs-2.22.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-gs-2.22.0/LICENSE` & `dvc-gs-2.22.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-gs-2.22.0/PKG-INFO` & `dvc-gs-2.22.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-gs
-Version: 2.22.0
+Version: 2.22.1
 Summary: gs plugin for dvc
 Home-page: http://dvc.org
 Download-URL: https://github.com/iterative/dvc-gs
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Source, https://github.com/iterative/dvc-gs
 Keywords: dvc,gs
```

### Comparing `dvc-gs-2.22.0/dvc_gs/path.py` & `dvc-gs-2.22.1/dvc_gs/path.py`

 * *Files identical despite different names*

### Comparing `dvc-gs-2.22.0/dvc_gs/tests/cloud.py` & `dvc-gs-2.22.1/dvc_gs/tests/cloud.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
+import os
 import uuid
 
 from dvc.testing.cloud import Cloud
 from dvc.testing.path_info import CloudURLInfo
 
-GS_BUCKET = "dvc-temp"
-
 
 class GCP(Cloud, CloudURLInfo):
 
     IS_OBJECT_STORAGE = True
 
     def __init__(self, url, credentialpath):
         super().__init__(url)
@@ -17,23 +16,24 @@
     def __truediv__(self, key):
         ret = super().__truediv__(key)
         ret.credentialpath = self.credentialpath
         return ret
 
     @property
     def config(self):
-        # FIXME: we shouldn't need to set credentialpath if env var is set
-        return {
-            "url": self.url,
-            "credentialpath": self.credentialpath,
-        }
+        config = {"url": self.url}
+        if not os.environ.get("GOOGLE_APPLICATION_CREDENTIALS"):
+            config["credentialpath"] = self.credentialpath
+        return config
 
     @staticmethod
     def _get_storagepath():
-        return GS_BUCKET + "/" + str(uuid.uuid4())
+        bucket = os.environ.get("DVC_TEST_GS_BUCKET")
+        assert bucket
+        return bucket + "/" + str(uuid.uuid4())
 
     @staticmethod
     def get_url():
         return "gs://" + GCP._get_storagepath()
 
     @property
     def _gc(self):
```

### Comparing `dvc-gs-2.22.0/dvc_gs/tests/test_dvc.py` & `dvc-gs-2.22.1/dvc_gs/tests/test_dvc.py`

 * *Files identical despite different names*

### Comparing `dvc-gs-2.22.0/dvc_gs.egg-info/PKG-INFO` & `dvc-gs-2.22.1/dvc_gs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-gs
-Version: 2.22.0
+Version: 2.22.1
 Summary: gs plugin for dvc
 Home-page: http://dvc.org
 Download-URL: https://github.com/iterative/dvc-gs
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Source, https://github.com/iterative/dvc-gs
 Keywords: dvc,gs
```

### Comparing `dvc-gs-2.22.0/dvc_gs.egg-info/SOURCES.txt` & `dvc-gs-2.22.1/dvc_gs.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
+.github/workflows/benchmarks.yaml
 .github/workflows/release.yaml
 .github/workflows/tests.yaml
 .github/workflows/update-template.yaml
 dvc_gs/__init__.py
 dvc_gs/_dvc_gs_version.py
 dvc_gs/path.py
 dvc_gs.egg-info/PKG-INFO
 dvc_gs.egg-info/SOURCES.txt
 dvc_gs.egg-info/dependency_links.txt
 dvc_gs.egg-info/not-zip-safe
 dvc_gs.egg-info/requires.txt
 dvc_gs.egg-info/top_level.txt
 dvc_gs/tests/__init__.py
+dvc_gs/tests/benchmarks.py
 dvc_gs/tests/cloud.py
 dvc_gs/tests/conftest.py
 dvc_gs/tests/fixtures.py
 dvc_gs/tests/test_dvc.py
```

### Comparing `dvc-gs-2.22.0/pyproject.toml` & `dvc-gs-2.22.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-gs-2.22.0/setup.cfg` & `dvc-gs-2.22.1/setup.cfg`

 * *Files identical despite different names*

