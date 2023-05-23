# Comparing `tmp/owlml-0.1.1.dev1682711592.tar.gz` & `tmp/owlml-0.1.1.dev1682711660.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owlml-0.1.1.dev1682711592.tar", last modified: Fri Apr 28 19:53:24 2023, max compression
+gzip compressed data, was "owlml-0.1.1.dev1682711660.tar", last modified: Fri Apr 28 19:54:31 2023, max compression
```

## Comparing `owlml-0.1.1.dev1682711592.tar` & `owlml-0.1.1.dev1682711660.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:53:24.099003 owlml-0.1.1.dev1682711592/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 19:52:35.000000 owlml-0.1.1.dev1682711592/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-28 19:53:24.099003 owlml-0.1.1.dev1682711592/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-28 19:52:35.000000 owlml-0.1.1.dev1682711592/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:53:24.099003 owlml-0.1.1.dev1682711592/owlml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:52:35.000000 owlml-0.1.1.dev1682711592/owlml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 19:52:35.000000 owlml-0.1.1.dev1682711592/owlml/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:53:24.099003 owlml-0.1.1.dev1682711592/owlml/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 19:52:35.000000 owlml-0.1.1.dev1682711592/owlml/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-28 19:52:35.000000 owlml-0.1.1.dev1682711592/owlml/auth/cvat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-28 19:52:35.000000 owlml-0.1.1.dev1682711592/owlml/upload_images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:53:24.099003 owlml-0.1.1.dev1682711592/owlml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-28 19:53:24.000000 owlml-0.1.1.dev1682711592/owlml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-28 19:53:24.000000 owlml-0.1.1.dev1682711592/owlml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:53:24.000000 owlml-0.1.1.dev1682711592/owlml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-28 19:53:24.000000 owlml-0.1.1.dev1682711592/owlml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-28 19:53:24.000000 owlml-0.1.1.dev1682711592/owlml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 19:53:24.000000 owlml-0.1.1.dev1682711592/owlml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-28 19:53:24.103003 owlml-0.1.1.dev1682711592/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 19:52:35.000000 owlml-0.1.1.dev1682711592/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:54:31.787165 owlml-0.1.1.dev1682711660/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 19:53:42.000000 owlml-0.1.1.dev1682711660/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-28 19:54:31.787165 owlml-0.1.1.dev1682711660/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-28 19:53:42.000000 owlml-0.1.1.dev1682711660/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:54:31.783166 owlml-0.1.1.dev1682711660/owlml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:53:42.000000 owlml-0.1.1.dev1682711660/owlml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 19:53:42.000000 owlml-0.1.1.dev1682711660/owlml/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:54:31.787165 owlml-0.1.1.dev1682711660/owlml/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 19:53:42.000000 owlml-0.1.1.dev1682711660/owlml/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-28 19:53:42.000000 owlml-0.1.1.dev1682711660/owlml/auth/cvat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-28 19:53:42.000000 owlml-0.1.1.dev1682711660/owlml/upload_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:54:31.787165 owlml-0.1.1.dev1682711660/owlml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-28 19:54:31.000000 owlml-0.1.1.dev1682711660/owlml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-28 19:54:31.000000 owlml-0.1.1.dev1682711660/owlml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:54:31.000000 owlml-0.1.1.dev1682711660/owlml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-28 19:54:31.000000 owlml-0.1.1.dev1682711660/owlml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-28 19:54:31.000000 owlml-0.1.1.dev1682711660/owlml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 19:54:31.000000 owlml-0.1.1.dev1682711660/owlml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-28 19:54:31.787165 owlml-0.1.1.dev1682711660/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 19:53:42.000000 owlml-0.1.1.dev1682711660/setup.py
```

### Comparing `owlml-0.1.1.dev1682711592/LICENSE` & `owlml-0.1.1.dev1682711660/LICENSE`

 * *Files identical despite different names*

### Comparing `owlml-0.1.1.dev1682711592/README.md` & `owlml-0.1.1.dev1682711660/README.md`

 * *Files identical despite different names*

### Comparing `owlml-0.1.1.dev1682711592/owlml/auth/cvat.py` & `owlml-0.1.1.dev1682711660/owlml/auth/cvat.py`

 * *Files identical despite different names*

### Comparing `owlml-0.1.1.dev1682711592/owlml/upload_images.py` & `owlml-0.1.1.dev1682711660/owlml/upload_images.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,8 +45,8 @@
     task = create_task(task_name, project_id, segment_size)
     task_id = task["id"]
     image_directory = Path(image_directory)
     images = []
     for extension in VALID_IMAGE_FORMATS:
         images.extend(image_directory.glob(f"*{extension}"))
     upload_image_list(task_id, sorted(images))
-    print(f"Uploaded {len(images)} images to task {task_id}")
+    print(f"Uploaded {len(images)} images to task {task_name}")
```

