# Comparing `tmp/pollination-annual-daylight-0.9.8.tar.gz` & `tmp/pollination-annual-daylight-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-annual-daylight-0.9.8.tar", last modified: Wed Feb  1 11:33:06 2023, max compression
+gzip compressed data, was "dist/pollination-annual-daylight-0.9.9.tar", last modified: Fri Feb  3 13:15:22 2023, max compression
```

## Comparing `pollination-annual-daylight-0.9.8.tar` & `pollination-annual-daylight-0.9.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 11:33:06.000000 pollination-annual-daylight-0.9.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 11:33:06.000000 pollination-annual-daylight-0.9.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-02-01 11:31:52.000000 pollination-annual-daylight-0.9.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 11:33:06.000000 pollination-annual-daylight-0.9.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-02-01 11:31:52.000000 pollination-annual-daylight-0.9.8/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-02-01 11:31:52.000000 pollination-annual-daylight-0.9.8/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-01 11:31:52.000000 pollination-annual-daylight-0.9.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-01 11:31:52.000000 pollination-annual-daylight-0.9.8/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-02-01 11:31:52.000000 pollination-annual-daylight-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-01 11:33:06.000000 pollination-annual-daylight-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-02-01 11:31:52.000000 pollination-annual-daylight-0.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-01 11:31:52.000000 pollination-annual-daylight-0.9.8/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-01 11:31:52.000000 pollination-annual-daylight-0.9.8/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-01 11:31:52.000000 pollination-annual-daylight-0.9.8/extras-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 11:33:06.000000 pollination-annual-daylight-0.9.8/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 11:33:06.000000 pollination-annual-daylight-0.9.8/pollination/annual_daylight/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-01 11:31:52.000000 pollination-annual-daylight-0.9.8/pollination/annual_daylight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-02-01 11:31:52.000000 pollination-annual-daylight-0.9.8/pollination/annual_daylight/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 11:33:06.000000 pollination-annual-daylight-0.9.8/pollination_annual_daylight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-01 11:33:06.000000 pollination-annual-daylight-0.9.8/pollination_annual_daylight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-02-01 11:33:06.000000 pollination-annual-daylight-0.9.8/pollination_annual_daylight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 11:33:06.000000 pollination-annual-daylight-0.9.8/pollination_annual_daylight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 11:32:18.000000 pollination-annual-daylight-0.9.8/pollination_annual_daylight.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-01 11:33:06.000000 pollination-annual-daylight-0.9.8/pollination_annual_daylight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-01 11:33:06.000000 pollination-annual-daylight-0.9.8/pollination_annual_daylight.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-01 11:31:52.000000 pollination-annual-daylight-0.9.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-01 11:33:06.000000 pollination-annual-daylight-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-02-01 11:31:52.000000 pollination-annual-daylight-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 11:33:06.000000 pollination-annual-daylight-0.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 11:31:52.000000 pollination-annual-daylight-0.9.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-02-01 11:31:52.000000 pollination-annual-daylight-0.9.8/tests/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:15:22.000000 pollination-annual-daylight-0.9.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:15:22.000000 pollination-annual-daylight-0.9.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-02-03 13:14:26.000000 pollination-annual-daylight-0.9.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:15:22.000000 pollination-annual-daylight-0.9.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-02-03 13:14:26.000000 pollination-annual-daylight-0.9.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-02-03 13:14:26.000000 pollination-annual-daylight-0.9.9/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-03 13:14:26.000000 pollination-annual-daylight-0.9.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-03 13:14:26.000000 pollination-annual-daylight-0.9.9/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-02-03 13:14:26.000000 pollination-annual-daylight-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-03 13:15:22.000000 pollination-annual-daylight-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-02-03 13:14:26.000000 pollination-annual-daylight-0.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-03 13:14:26.000000 pollination-annual-daylight-0.9.9/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-03 13:14:26.000000 pollination-annual-daylight-0.9.9/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-03 13:14:26.000000 pollination-annual-daylight-0.9.9/extras-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:15:22.000000 pollination-annual-daylight-0.9.9/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:15:22.000000 pollination-annual-daylight-0.9.9/pollination/annual_daylight/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-03 13:14:26.000000 pollination-annual-daylight-0.9.9/pollination/annual_daylight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-02-03 13:14:26.000000 pollination-annual-daylight-0.9.9/pollination/annual_daylight/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:15:22.000000 pollination-annual-daylight-0.9.9/pollination_annual_daylight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-03 13:15:22.000000 pollination-annual-daylight-0.9.9/pollination_annual_daylight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-02-03 13:15:22.000000 pollination-annual-daylight-0.9.9/pollination_annual_daylight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 13:15:22.000000 pollination-annual-daylight-0.9.9/pollination_annual_daylight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 13:14:47.000000 pollination-annual-daylight-0.9.9/pollination_annual_daylight.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-03 13:15:22.000000 pollination-annual-daylight-0.9.9/pollination_annual_daylight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-03 13:15:22.000000 pollination-annual-daylight-0.9.9/pollination_annual_daylight.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-03 13:14:26.000000 pollination-annual-daylight-0.9.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-03 13:15:22.000000 pollination-annual-daylight-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-02-03 13:14:26.000000 pollination-annual-daylight-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:15:22.000000 pollination-annual-daylight-0.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 13:14:26.000000 pollination-annual-daylight-0.9.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-02-03 13:14:26.000000 pollination-annual-daylight-0.9.9/tests/validation_test.py
```

### Comparing `pollination-annual-daylight-0.9.8/.github/workflows/ci.yaml` & `pollination-annual-daylight-0.9.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-0.9.8/.github/workflows/tests.yaml` & `pollination-annual-daylight-0.9.9/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-0.9.8/LICENSE` & `pollination-annual-daylight-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-0.9.8/PKG-INFO` & `pollination-annual-daylight-0.9.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-daylight
-Version: 0.9.8
+Version: 0.9.9
 Summary: Annual daylight recipe for Pollination.
 Home-page: https://github.com/pollination/annual-daylight
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-annual-daylight-0.9.8/pollination/annual_daylight/entry.py` & `pollination-annual-daylight-0.9.9/pollination/annual_daylight/entry.py`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-0.9.8/pollination_annual_daylight.egg-info/PKG-INFO` & `pollination-annual-daylight-0.9.9/pollination_annual_daylight.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-daylight
-Version: 0.9.8
+Version: 0.9.9
 Summary: Annual daylight recipe for Pollination.
 Home-page: https://github.com/pollination/annual-daylight
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-annual-daylight-0.9.8/pollination_annual_daylight.egg-info/SOURCES.txt` & `pollination-annual-daylight-0.9.9/pollination_annual_daylight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-0.9.8/setup.py` & `pollination-annual-daylight-0.9.9/setup.py`

 * *Files identical despite different names*

