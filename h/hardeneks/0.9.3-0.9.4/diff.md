# Comparing `tmp/hardeneks-0.9.3.tar.gz` & `tmp/hardeneks-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hardeneks-0.9.3.tar", max compression
+gzip compressed data, was "hardeneks-0.9.4.tar", max compression
```

## Comparing `hardeneks-0.9.3.tar` & `hardeneks-0.9.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      927 2023-05-15 15:09:20.321742 hardeneks-0.9.3/LICENSE
--rw-r--r--   0        0        0     6610 2023-05-15 15:09:20.321742 hardeneks-0.9.3/README.md
--rw-r--r--   0        0        0     7046 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/cluster_wide/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/cluster_wide/cluster_autoscaling/__init__.py
--rw-r--r--   0        0        0     9687 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/cluster_wide/cluster_autoscaling/cluster_autoscaler.py
--rw-r--r--   0        0        0        0 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/cluster_wide/reliability/__init__.py
--rw-r--r--   0        0        0     1525 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/cluster_wide/reliability/applications.py
--rw-r--r--   0        0        0        0 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/cluster_wide/scalability/__init__.py
--rw-r--r--   0        0        0     2112 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/cluster_wide/scalability/control_plane.py
--rw-r--r--   0        0        0      551 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/cluster_wide/scalability/skipped.json
--rw-r--r--   0        0        0        0 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/cluster_wide/security/__init__.py
--rw-r--r--   0        0        0      874 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/cluster_wide/security/detective_controls.py
--rw-r--r--   0        0        0     3161 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/cluster_wide/security/encryption_secrets.py
--rw-r--r--   0        0        0     5814 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/cluster_wide/security/iam.py
--rw-r--r--   0        0        0     1009 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/cluster_wide/security/image_security.py
--rw-r--r--   0        0        0     2374 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/cluster_wide/security/infrastructure_security.py
--rw-r--r--   0        0        0      760 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/cluster_wide/security/multi_tenancy.py
--rw-r--r--   0        0        0     2558 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/cluster_wide/security/network_security.py
--rw-r--r--   0        0        0     1222 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/cluster_wide/security/pod_security.py
--rw-r--r--   0        0        0     2731 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/config.yaml
--rw-r--r--   0        0        0      728 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/harden.py
--rw-r--r--   0        0        0      544 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/helpers.py
--rw-r--r--   0        0        0        0 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/namespace_based/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/namespace_based/reliability/__init__.py
--rw-r--r--   0        0        0     5859 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/namespace_based/reliability/applications.py
--rw-r--r--   0        0        0        0 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/namespace_based/security/__init__.py
--rw-r--r--   0        0        0     1305 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/namespace_based/security/encryption_secrets.py
--rw-r--r--   0        0        0     8011 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/namespace_based/security/iam.py
--rw-r--r--   0        0        0     1370 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/namespace_based/security/network_security.py
--rw-r--r--   0        0        0     5259 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/namespace_based/security/pod_security.py
--rw-r--r--   0        0        0     1685 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/namespace_based/security/runtime_security.py
--rw-r--r--   0        0        0     2289 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/resources.py
--rw-r--r--   0        0        0     1412 2023-05-15 15:09:20.333742 hardeneks-0.9.3/hardeneks/rules.py
--rw-r--r--   0        0        0     1005 2023-05-15 15:09:20.333742 hardeneks-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     7081 1970-01-01 00:00:00.000000 hardeneks-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0      927 2023-05-23 17:48:48.914389 hardeneks-0.9.4/LICENSE
+-rw-r--r--   0        0        0     6610 2023-05-23 17:48:48.914389 hardeneks-0.9.4/README.md
+-rw-r--r--   0        0        0     7046 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/cluster_wide/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/cluster_wide/cluster_autoscaling/__init__.py
+-rw-r--r--   0        0        0     9687 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/cluster_wide/cluster_autoscaling/cluster_autoscaler.py
+-rw-r--r--   0        0        0        0 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/cluster_wide/reliability/__init__.py
+-rw-r--r--   0        0        0     1525 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/cluster_wide/reliability/applications.py
+-rw-r--r--   0        0        0        0 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/cluster_wide/scalability/__init__.py
+-rw-r--r--   0        0        0     2112 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/cluster_wide/scalability/control_plane.py
+-rw-r--r--   0        0        0      551 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/cluster_wide/scalability/skipped.json
+-rw-r--r--   0        0        0        0 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/cluster_wide/security/__init__.py
+-rw-r--r--   0        0        0      874 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/cluster_wide/security/detective_controls.py
+-rw-r--r--   0        0        0     3161 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/cluster_wide/security/encryption_secrets.py
+-rw-r--r--   0        0        0     5814 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/cluster_wide/security/iam.py
+-rw-r--r--   0        0        0     1009 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/cluster_wide/security/image_security.py
+-rw-r--r--   0        0        0     2374 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/cluster_wide/security/infrastructure_security.py
+-rw-r--r--   0        0        0      760 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/cluster_wide/security/multi_tenancy.py
+-rw-r--r--   0        0        0     2558 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/cluster_wide/security/network_security.py
+-rw-r--r--   0        0        0     1222 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/cluster_wide/security/pod_security.py
+-rw-r--r--   0        0        0     2731 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/config.yaml
+-rw-r--r--   0        0        0      728 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/harden.py
+-rw-r--r--   0        0        0      544 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/helpers.py
+-rw-r--r--   0        0        0        0 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/namespace_based/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/namespace_based/reliability/__init__.py
+-rw-r--r--   0        0        0     5859 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/namespace_based/reliability/applications.py
+-rw-r--r--   0        0        0        0 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/namespace_based/security/__init__.py
+-rw-r--r--   0        0        0     1305 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/namespace_based/security/encryption_secrets.py
+-rw-r--r--   0        0        0     8011 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/namespace_based/security/iam.py
+-rw-r--r--   0        0        0     1370 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/namespace_based/security/network_security.py
+-rw-r--r--   0        0        0     5259 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/namespace_based/security/pod_security.py
+-rw-r--r--   0        0        0     1685 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/namespace_based/security/runtime_security.py
+-rw-r--r--   0        0        0     2289 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/resources.py
+-rw-r--r--   0        0        0     1412 2023-05-23 17:48:48.926389 hardeneks-0.9.4/hardeneks/rules.py
+-rw-r--r--   0        0        0     1005 2023-05-23 17:48:48.926389 hardeneks-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     7081 1970-01-01 00:00:00.000000 hardeneks-0.9.4/PKG-INFO
```

### Comparing `hardeneks-0.9.3/LICENSE` & `hardeneks-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/README.md` & `hardeneks-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/__init__.py` & `hardeneks-0.9.4/hardeneks/__init__.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/cluster_wide/cluster_autoscaling/cluster_autoscaler.py` & `hardeneks-0.9.4/hardeneks/cluster_wide/cluster_autoscaling/cluster_autoscaler.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/cluster_wide/reliability/applications.py` & `hardeneks-0.9.4/hardeneks/cluster_wide/reliability/applications.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/cluster_wide/scalability/control_plane.py` & `hardeneks-0.9.4/hardeneks/cluster_wide/scalability/control_plane.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/cluster_wide/scalability/skipped.json` & `hardeneks-0.9.4/hardeneks/cluster_wide/scalability/skipped.json`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/cluster_wide/security/detective_controls.py` & `hardeneks-0.9.4/hardeneks/cluster_wide/security/detective_controls.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/cluster_wide/security/encryption_secrets.py` & `hardeneks-0.9.4/hardeneks/cluster_wide/security/encryption_secrets.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/cluster_wide/security/iam.py` & `hardeneks-0.9.4/hardeneks/cluster_wide/security/iam.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/cluster_wide/security/image_security.py` & `hardeneks-0.9.4/hardeneks/cluster_wide/security/image_security.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/cluster_wide/security/infrastructure_security.py` & `hardeneks-0.9.4/hardeneks/cluster_wide/security/infrastructure_security.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/cluster_wide/security/multi_tenancy.py` & `hardeneks-0.9.4/hardeneks/cluster_wide/security/multi_tenancy.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/cluster_wide/security/network_security.py` & `hardeneks-0.9.4/hardeneks/cluster_wide/security/network_security.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/cluster_wide/security/pod_security.py` & `hardeneks-0.9.4/hardeneks/cluster_wide/security/pod_security.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/config.yaml` & `hardeneks-0.9.4/hardeneks/config.yaml`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/harden.py` & `hardeneks-0.9.4/hardeneks/harden.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/helpers.py` & `hardeneks-0.9.4/hardeneks/helpers.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/namespace_based/reliability/applications.py` & `hardeneks-0.9.4/hardeneks/namespace_based/reliability/applications.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/namespace_based/security/encryption_secrets.py` & `hardeneks-0.9.4/hardeneks/namespace_based/security/encryption_secrets.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/namespace_based/security/iam.py` & `hardeneks-0.9.4/hardeneks/namespace_based/security/iam.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/namespace_based/security/network_security.py` & `hardeneks-0.9.4/hardeneks/namespace_based/security/network_security.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/namespace_based/security/pod_security.py` & `hardeneks-0.9.4/hardeneks/namespace_based/security/pod_security.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/namespace_based/security/runtime_security.py` & `hardeneks-0.9.4/hardeneks/namespace_based/security/runtime_security.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/resources.py` & `hardeneks-0.9.4/hardeneks/resources.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/hardeneks/rules.py` & `hardeneks-0.9.4/hardeneks/rules.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.3/pyproject.toml` & `hardeneks-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hardeneks"
-version = "0.9.3"
+version = "0.9.4"
 description = ""
 authors = ["Doruk Ozturk <dozturk@amazon.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 typer = {extras = ["all"], version = "^0.6.1"}
@@ -37,15 +37,15 @@
   | build
   | dist
 )/
 '''
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.9.3"
+version = "0.9.4"
 version_files = [
   "pyproject.toml:[tool.commitizen]\nversion",
   "pyproject.toml:[tool.poetry]\nname = \"commitizen\"\nversion",
   "pyproject.toml:^version"
 ]
 tag_format = "v$version"
 [build-system]
```

### Comparing `hardeneks-0.9.3/PKG-INFO` & `hardeneks-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hardeneks
-Version: 0.9.3
+Version: 0.9.4
 Summary: 
 Author: Doruk Ozturk
 Author-email: dozturk@amazon.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

