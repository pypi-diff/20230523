# Comparing `tmp/print_torch-1.1.tar.gz` & `tmp/print_torch-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "print_torch-1.1.tar", last modified: Mon May 22 18:19:42 2023, max compression
+gzip compressed data, was "print_torch-1.2.tar", last modified: Mon May 22 18:25:18 2023, max compression
```

## Comparing `print_torch-1.1.tar` & `print_torch-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:19:40.000000 print_torch-1.1/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-05-22 18:15:47.000000 print_torch-1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1516 2023-05-22 18:19:42.000000 print_torch-1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      985 2023-05-22 18:17:49.000000 print_torch-1.1/README.md
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-22 18:15:47.000000 print_torch-1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      700 2023-05-22 18:19:42.000000 print_torch-1.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:19:40.000000 print_torch-1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:19:40.000000 print_torch-1.1/src/print_torch/
--rw-r--r--   0 root         (0) root         (0)     5442 2023-05-22 18:15:47.000000 print_torch-1.1/src/print_torch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:19:40.000000 print_torch-1.1/src/print_torch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1516 2023-05-22 18:19:40.000000 print_torch-1.1/src/print_torch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      264 2023-05-22 18:19:40.000000 print_torch-1.1/src/print_torch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 18:19:40.000000 print_torch-1.1/src/print_torch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-22 18:19:40.000000 print_torch-1.1/src/print_torch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-22 18:19:40.000000 print_torch-1.1/src/print_torch.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:25:16.000000 print_torch-1.2/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-22 18:15:47.000000 print_torch-1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-05-22 18:25:18.000000 print_torch-1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      985 2023-05-22 18:17:49.000000 print_torch-1.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-22 18:15:47.000000 print_torch-1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-22 18:25:18.000000 print_torch-1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:25:16.000000 print_torch-1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:25:16.000000 print_torch-1.2/src/print_torch/
+-rw-r--r--   0 root         (0) root         (0)     5423 2023-05-22 18:24:47.000000 print_torch-1.2/src/print_torch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:25:17.000000 print_torch-1.2/src/print_torch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-05-22 18:25:16.000000 print_torch-1.2/src/print_torch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      264 2023-05-22 18:25:16.000000 print_torch-1.2/src/print_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 18:25:16.000000 print_torch-1.2/src/print_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-22 18:25:16.000000 print_torch-1.2/src/print_torch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-22 18:25:16.000000 print_torch-1.2/src/print_torch.egg-info/top_level.txt
```

### Comparing `print_torch-1.1/LICENSE` & `print_torch-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `print_torch-1.1/PKG-INFO` & `print_torch-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: print_torch
-Version: 1.1
+Version: 1.2
 Summary: print pytorch tensors and numpy arrays concisely.
-Home-page: https://github.com/tjyuyao/neurlinkprint_torch
+Home-page: https://github.com/tjyuyao/print_torch
 Author: Yuyao Huang
 Author-email: huangyuyao@outlook.com
 Project-URL: Bug Tracker, https://github.com/tjyuyao/print_torch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `print_torch-1.1/README.md` & `print_torch-1.2/README.md`

 * *Files identical despite different names*

### Comparing `print_torch-1.1/setup.cfg` & `print_torch-1.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = print_torch
-version = 1.1
+version = 1.2
 author = Yuyao Huang
 author_email = huangyuyao@outlook.com
 description = print pytorch tensors and numpy arrays concisely.
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/tjyuyao/neurlinkprint_torch
+url = https://github.com/tjyuyao/print_torch
 project_urls = 
 	Bug Tracker = https://github.com/tjyuyao/print_torch/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
```

### Comparing `print_torch-1.1/src/print_torch/__init__.py` & `print_torch-1.2/src/print_torch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,8 +168,7 @@
     if uri != "" and not uri.endswith(": "):
         uri = uri + ": "
     tqdm.write(f"{prefix}{uri}{brief}\n", end="")
 
 pt = print_torch
 
 __all__ = ['print_torch', 'pt']
-__version__ = "1.1"
```

### Comparing `print_torch-1.1/src/print_torch.egg-info/PKG-INFO` & `print_torch-1.2/src/print_torch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: print-torch
-Version: 1.1
+Version: 1.2
 Summary: print pytorch tensors and numpy arrays concisely.
-Home-page: https://github.com/tjyuyao/neurlinkprint_torch
+Home-page: https://github.com/tjyuyao/print_torch
 Author: Yuyao Huang
 Author-email: huangyuyao@outlook.com
 Project-URL: Bug Tracker, https://github.com/tjyuyao/print_torch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

