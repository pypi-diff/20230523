# Comparing `tmp/pycocotools_stubs-0.0.4.tar.gz` & `tmp/pycocotools_stubs-0.1.0.tar.gz`

## Comparing `pycocotools_stubs-0.0.4.tar` & `pycocotools_stubs-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/requirements/README.md
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/requirements/requirements-build.txt
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/requirements/requirements-dev.txt
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/requirements/requirements.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/src/pycocotools-stubs/__init__.pyi
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/src/pycocotools-stubs/coco.pyi
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/src/pycocotools-stubs/coco_types.pyi
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/src/pycocotools-stubs/cocoeval.pyi
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/src/pycocotools-stubs/mask.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/src/pycocotools-stubs/py.typed
--rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/LICENSE
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/README.md
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pycocotools_stubs-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pycocotools_stubs-0.1.0/requirements/README.md
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 pycocotools_stubs-0.1.0/requirements/requirements-build.txt
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 pycocotools_stubs-0.1.0/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 pycocotools_stubs-0.1.0/requirements/requirements.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pycocotools_stubs-0.1.0/src/pycocotools-stubs/__init__.pyi
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 pycocotools_stubs-0.1.0/src/pycocotools-stubs/coco.pyi
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 pycocotools_stubs-0.1.0/src/pycocotools-stubs/coco_types.pyi
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 pycocotools_stubs-0.1.0/src/pycocotools-stubs/cocoeval.pyi
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pycocotools_stubs-0.1.0/src/pycocotools-stubs/mask.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pycocotools_stubs-0.1.0/src/pycocotools-stubs/py.typed
+-rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 pycocotools_stubs-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pycocotools_stubs-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 pycocotools_stubs-0.1.0/README.md
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 pycocotools_stubs-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 pycocotools_stubs-0.1.0/PKG-INFO
```

### Comparing `pycocotools_stubs-0.0.4/.pre-commit-config.yaml` & `pycocotools_stubs-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pycocotools_stubs-0.0.4/requirements/requirements-build.txt` & `pycocotools_stubs-0.1.0/requirements/requirements-build.txt`

 * *Files identical despite different names*

### Comparing `pycocotools_stubs-0.0.4/requirements/requirements-dev.txt` & `pycocotools_stubs-0.1.0/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `pycocotools_stubs-0.0.4/requirements/requirements.txt` & `pycocotools_stubs-0.1.0/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `pycocotools_stubs-0.0.4/src/pycocotools-stubs/coco.pyi` & `pycocotools_stubs-0.1.0/src/pycocotools-stubs/coco.pyi`

 * *Files identical despite different names*

### Comparing `pycocotools_stubs-0.0.4/src/pycocotools-stubs/coco_types.pyi` & `pycocotools_stubs-0.1.0/src/pycocotools-stubs/coco_types.pyi`

 * *Files identical despite different names*

### Comparing `pycocotools_stubs-0.0.4/src/pycocotools-stubs/cocoeval.pyi` & `pycocotools_stubs-0.1.0/src/pycocotools-stubs/cocoeval.pyi`

 * *Files identical despite different names*

### Comparing `pycocotools_stubs-0.0.4/src/pycocotools-stubs/mask.pyi` & `pycocotools_stubs-0.1.0/src/pycocotools-stubs/mask.pyi`

 * *Files identical despite different names*

### Comparing `pycocotools_stubs-0.0.4/LICENSE` & `pycocotools_stubs-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycocotools_stubs-0.0.4/README.md` & `pycocotools_stubs-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pycocotools_stubs-0.0.4/pyproject.toml` & `pycocotools_stubs-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycocotools_stubs-0.0.4/PKG-INFO` & `pycocotools_stubs-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycocotools-stubs
-Version: 0.0.4
+Version: 0.1.0
 Summary: Unofficial stubs for the pycocotools package.
 Project-URL: Homepage, https://github.com/hoel-bagard/pycocotools-stubs
 Project-URL: Bug Tracker, https://github.com/hoel-bagard/pycocotools-stubs/issues
 Author: Bagard Hoel
 License: MIT
 License-File: LICENSE
 Keywords: pycocotools,stubs
```

