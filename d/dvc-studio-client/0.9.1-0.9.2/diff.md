# Comparing `tmp/dvc-studio-client-0.9.1.tar.gz` & `tmp/dvc-studio-client-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-studio-client-0.9.1.tar", last modified: Mon May 15 19:13:15 2023, max compression
+gzip compressed data, was "dvc-studio-client-0.9.2.tar", last modified: Tue May 16 00:02:41 2023, max compression
```

## Comparing `dvc-studio-client-0.9.1.tar` & `dvc-studio-client-0.9.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:15.389715 dvc-studio-client-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:15.385715 dvc-studio-client-0.9.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:15.385715 dvc-studio-client-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.github/workflows/leaked-secrets-scan.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:15.385715 dvc-studio-client-0.9.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-15 19:13:15.389715 dvc-studio-client-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:15.385715 dvc-studio-client-0.9.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:15.389715 dvc-studio-client-0.9.1/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/docs/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-15 19:13:15.389715 dvc-studio-client-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:15.385715 dvc-studio-client-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:15.389715 dvc-studio-client-0.9.1/src/dvc_studio_client/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/src/dvc_studio_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/src/dvc_studio_client/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/src/dvc_studio_client/post_live_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/src/dvc_studio_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/src/dvc_studio_client/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:15.389715 dvc-studio-client-0.9.1/src/dvc_studio_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-15 19:13:15.000000 dvc-studio-client-0.9.1/src/dvc_studio_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-15 19:13:15.000000 dvc-studio-client-0.9.1/src/dvc_studio_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:13:15.000000 dvc-studio-client-0.9.1/src/dvc_studio_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:13:15.000000 dvc-studio-client-0.9.1/src/dvc_studio_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-15 19:13:15.000000 dvc-studio-client-0.9.1/src/dvc_studio_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 19:13:15.000000 dvc-studio-client-0.9.1/src/dvc_studio_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:13:15.389715 dvc-studio-client-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15587 2023-05-15 19:13:03.000000 dvc-studio-client-0.9.1/tests/test_post_live_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:41.357737 dvc-studio-client-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:41.357737 dvc-studio-client-0.9.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:41.357737 dvc-studio-client-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/.github/workflows/leaked-secrets-scan.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:41.357737 dvc-studio-client-0.9.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-16 00:02:41.357737 dvc-studio-client-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:41.357737 dvc-studio-client-0.9.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:41.357737 dvc-studio-client-0.9.2/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-16 00:02:41.361738 dvc-studio-client-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:41.353737 dvc-studio-client-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:41.357737 dvc-studio-client-0.9.2/src/dvc_studio_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/src/dvc_studio_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/src/dvc_studio_client/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/src/dvc_studio_client/post_live_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/src/dvc_studio_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/src/dvc_studio_client/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:41.357737 dvc-studio-client-0.9.2/src/dvc_studio_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-16 00:02:41.000000 dvc-studio-client-0.9.2/src/dvc_studio_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-16 00:02:41.000000 dvc-studio-client-0.9.2/src/dvc_studio_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:02:41.000000 dvc-studio-client-0.9.2/src/dvc_studio_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:02:41.000000 dvc-studio-client-0.9.2/src/dvc_studio_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-16 00:02:41.000000 dvc-studio-client-0.9.2/src/dvc_studio_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 00:02:41.000000 dvc-studio-client-0.9.2/src/dvc_studio_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:41.357737 dvc-studio-client-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-05-16 00:02:27.000000 dvc-studio-client-0.9.2/tests/test_post_live_metrics.py
```

### Comparing `dvc-studio-client-0.9.1/.cruft.json` & `dvc-studio-client-0.9.2/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.1/.github/dependabot.yml` & `dvc-studio-client-0.9.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.1/.github/workflows/docs.yml` & `dvc-studio-client-0.9.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.1/.github/workflows/leaked-secrets-scan.yaml` & `dvc-studio-client-0.9.2/.github/workflows/leaked-secrets-scan.yaml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.1/.github/workflows/pre-commit.yml` & `dvc-studio-client-0.9.2/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.1/.github/workflows/release.yml` & `dvc-studio-client-0.9.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.1/.github/workflows/tests.yml` & `dvc-studio-client-0.9.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.1/.gitignore` & `dvc-studio-client-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.1/.pre-commit-config.yaml` & `dvc-studio-client-0.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.1/CODE_OF_CONDUCT.rst` & `dvc-studio-client-0.9.2/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.1/CONTRIBUTING.rst` & `dvc-studio-client-0.9.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.1/LICENSE` & `dvc-studio-client-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.1/PKG-INFO` & `dvc-studio-client-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-studio-client
-Version: 0.9.1
+Version: 0.9.2
 Summary: Small library to post data from DVC/DVCLive to Iterative Studio
 Home-page: https://github.com/iterative/dvc-studio-client
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-studio-client-0.9.1/README.rst` & `dvc-studio-client-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.1/docs/assets/logo.svg` & `dvc-studio-client-0.9.2/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.1/docs/gen_ref_pages.py` & `dvc-studio-client-0.9.2/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.1/mkdocs.yml` & `dvc-studio-client-0.9.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.1/pyproject.toml` & `dvc-studio-client-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.1/setup.cfg` & `dvc-studio-client-0.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.1/src/dvc_studio_client/post_live_metrics.py` & `dvc-studio-client-0.9.2/src/dvc_studio_client/post_live_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 def get_studio_token_and_repo_url(studio_token=None, studio_repo_url=None):
     studio_token = studio_token or getenv(DVC_STUDIO_TOKEN) or getenv(STUDIO_TOKEN)
     """Get studio token and repo_url. Kept for backwards compatibility."""
     config = get_studio_config(
         studio_token=studio_token, studio_repo_url=studio_repo_url
     )
-    return config["token"], config["repo_url"]
+    return config.get("token"), config.get("repo_url")
 
 
 def get_studio_config(
     dvc_studio_config: Optional[Dict[str, Any]] = None,
     offline: bool = False,
     studio_token: Optional[str] = None,
     studio_repo_url: Optional[str] = None,
```

### Comparing `dvc-studio-client-0.9.1/src/dvc_studio_client/schema.py` & `dvc-studio-client-0.9.2/src/dvc_studio_client/schema.py`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.1/src/dvc_studio_client.egg-info/PKG-INFO` & `dvc-studio-client-0.9.2/src/dvc_studio_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-studio-client
-Version: 0.9.1
+Version: 0.9.2
 Summary: Small library to post data from DVC/DVCLive to Iterative Studio
 Home-page: https://github.com/iterative/dvc-studio-client
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-studio-client-0.9.1/src/dvc_studio_client.egg-info/SOURCES.txt` & `dvc-studio-client-0.9.2/src/dvc_studio_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-studio-client-0.9.1/tests/test_post_live_metrics.py` & `dvc-studio-client-0.9.2/tests/test_post_live_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     STUDIO_REPO_URL,
     STUDIO_TOKEN,
 )
 from dvc_studio_client.post_live_metrics import (
     STUDIO_URL,
     _get_remote_url,
     get_studio_config,
+    get_studio_token_and_repo_url,
     post_live_metrics,
 )
 
 
 def test_get_url(monkeypatch, tmp_path_factory):
     source = os.fspath(tmp_path_factory.mktemp("source"))
     target = os.fspath(tmp_path_factory.mktemp("target"))
@@ -538,7 +539,21 @@
         },
         headers={
             "Authorization": "token FOO_TOKEN",
             "Content-type": "application/json",
         },
         timeout=5,
     )
+
+
+@pytest.mark.parametrize("var", [DVC_STUDIO_TOKEN, STUDIO_TOKEN])
+def test_studio_token_envvar(monkeypatch, var):
+    monkeypatch.setenv(var, "FOO_TOKEN")
+    monkeypatch.setenv(STUDIO_REPO_URL, "FOO_REPO_URL")
+    assert get_studio_token_and_repo_url() == ("FOO_TOKEN", "FOO_REPO_URL")
+
+
+def test_get_studio_token_and_repo_url_skip_repo_url(monkeypatch):
+    monkeypatch.setenv(STUDIO_REPO_URL, "FOO_REPO_URL")
+    token, repo_url = get_studio_token_and_repo_url()
+    assert token is None
+    assert repo_url is None  # Skipped call to get_repo_url
```

