# Comparing `tmp/pyterrain-0.0.1.tar.gz` & `tmp/pyterrain-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyterrain-0.0.1.tar", last modified: Tue Jan 24 13:27:15 2023, max compression
+gzip compressed data, was "pyterrain-0.0.2.tar", last modified: Tue May 23 13:11:11 2023, max compression
```

## Comparing `pyterrain-0.0.1.tar` & `pyterrain-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:27:15.367700 pyterrain-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-24 13:26:59.000000 pyterrain-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-01-24 13:26:59.000000 pyterrain-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-24 13:27:15.367700 pyterrain-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-01-24 13:26:59.000000 pyterrain-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:27:15.367700 pyterrain-0.0.1/pyterrain/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-24 13:26:59.000000 pyterrain-0.0.1/pyterrain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-01-24 13:26:59.000000 pyterrain-0.0.1/pyterrain/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:27:15.367700 pyterrain-0.0.1/pyterrain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-24 13:27:15.000000 pyterrain-0.0.1/pyterrain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-01-24 13:27:15.000000 pyterrain-0.0.1/pyterrain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 13:27:15.000000 pyterrain-0.0.1/pyterrain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-24 13:27:15.000000 pyterrain-0.0.1/pyterrain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-24 13:27:15.000000 pyterrain-0.0.1/pyterrain.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:27:15.367700 pyterrain-0.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-24 13:26:59.000000 pyterrain-0.0.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-01-24 13:26:59.000000 pyterrain-0.0.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 13:27:15.367700 pyterrain-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-01-24 13:26:59.000000 pyterrain-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:11:11.230124 pyterrain-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 13:10:56.000000 pyterrain-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-23 13:10:56.000000 pyterrain-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-23 13:11:11.230124 pyterrain-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-23 13:10:56.000000 pyterrain-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:11:11.230124 pyterrain-0.0.2/pyterrain/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-23 13:10:56.000000 pyterrain-0.0.2/pyterrain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-05-23 13:10:56.000000 pyterrain-0.0.2/pyterrain/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:11:11.230124 pyterrain-0.0.2/pyterrain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-23 13:11:11.000000 pyterrain-0.0.2/pyterrain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-23 13:11:11.000000 pyterrain-0.0.2/pyterrain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:11:11.000000 pyterrain-0.0.2/pyterrain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-23 13:11:11.000000 pyterrain-0.0.2/pyterrain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 13:11:11.000000 pyterrain-0.0.2/pyterrain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:11:11.230124 pyterrain-0.0.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-23 13:10:56.000000 pyterrain-0.0.2/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-23 13:10:56.000000 pyterrain-0.0.2/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:11:11.230124 pyterrain-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-23 13:10:56.000000 pyterrain-0.0.2/setup.py
```

### Comparing `pyterrain-0.0.1/LICENSE` & `pyterrain-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyterrain-0.0.1/PKG-INFO` & `pyterrain-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyterrain
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package to fetch terrain data easily.
 Home-page: https://github.com/Clarmy/pyterrain
 Author: Wentao Li
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -15,20 +15,20 @@
 
 # Installation
 You can install by pip `$ pip install pyterrain`
 
 # Usage
 
 ## Register API Key
-Pyterrain don't offer terrain data itself, it fetches data from another website. Before downloading data, you should sign up an API key from [nextzen.org](https://developers.nextzen.org/). The key's pattern is like `Dto0r88DQuaQizoxcQSxxx`
+Pyterrain doesn't offer terrain data by itself, it fetches data from another website. Before downloading data, you should sign up an API key from [nextzen.org](https://developers.nextzen.org/). The key's pattern is like `Dto0r88DQuaQizoxcQSxxx`
 
 ## Fetch DEM by bound box
 When API key is reday, you can download DEM data like this:
 
 ```python
 bbox = 108.444319, 20.161757, 111.318897, 18.05883  # Hainan province of China
 
 terrain = Terrain("Dto0r88DQuaQizoxcQSxxx")  # Pass API key
 xs, ys, elevation = terrain.fetch(bbox=bbox, quiet=False, coord="lonlat", zoom=10)
 ```
 
-If download is not complete because of connection, retry it.
+If download is not completed because of connection, retry it.
```

### Comparing `pyterrain-0.0.1/pyterrain/core.py` & `pyterrain-0.0.2/pyterrain/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,32 +3,37 @@
 from typing import List
 from multiprocessing.dummy import Pool
 
 import requests
 import mercantile
 import numpy as np
 import pyproj
+from loguru import logger
 
 import matplotlib.pyplot as plt
 from tqdm import tqdm
 from retrying import retry
 
 
 @retry
 def single_download(arg):
     url, tmpfp, timeout = arg
     resp = requests.get(url, timeout=timeout, stream=True)
     if resp.ok:
         content = resp.content
+    else:
+        logger.debug(f"{resp}: {resp.url}")
+        return False
     os.makedirs(os.path.dirname(tmpfp), exist_ok=True)
     try:
         with open(tmpfp, "wb") as f:
             f.write(content)
-    except Exception:
+    except Exception as err:
         os.remove(tmpfp)
+        logger.exception(err)
         return False
     else:
         return True
 
 
 class Terrain:
     API_URL_PATTERN = "https://tile.nextzen.org/tilezen/terrain/v1/256/terrarium/{z}/{x}/{y}.png?api_key={api_key}"
@@ -171,15 +176,22 @@
         for (nx, ny), (x, y), url in tqdm(
             urls, disable=not progress_bar, desc="mosaicing"
         ):
             tmpfp = os.path.join(cache_path, f"{zoom}/{x}/{y}.bin")
             with open(tmpfp, "rb") as f:
                 img = (plt.imread(f) * 255).astype(int)
 
-            canvas[ny * 256 : ny * 256 + 256, nx * 256 : nx * 256 + 256] = img  # noqa
+            if img.shape[-1] == 4:
+                canvas[
+                    ny * 256 : ny * 256 + 256, nx * 256 : nx * 256 + 256
+                ] = img  # noqa
+            elif img.shape[-1] == 3:
+                canvas[
+                    ny * 256 : ny * 256 + 256, nx * 256 : nx * 256 + 256, :3
+                ] = img  # noqa
 
         red = canvas[..., 0]
         green = canvas[..., 1]
         blue = canvas[..., 2]
         elevation = ((red * 256 + green + blue / 256) - 32768).astype(int)[idx]
 
         if not quiet:
```

### Comparing `pyterrain-0.0.1/pyterrain.egg-info/PKG-INFO` & `pyterrain-0.0.2/pyterrain.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyterrain
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package to fetch terrain data easily.
 Home-page: https://github.com/Clarmy/pyterrain
 Author: Wentao Li
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -15,20 +15,20 @@
 
 # Installation
 You can install by pip `$ pip install pyterrain`
 
 # Usage
 
 ## Register API Key
-Pyterrain don't offer terrain data itself, it fetches data from another website. Before downloading data, you should sign up an API key from [nextzen.org](https://developers.nextzen.org/). The key's pattern is like `Dto0r88DQuaQizoxcQSxxx`
+Pyterrain doesn't offer terrain data by itself, it fetches data from another website. Before downloading data, you should sign up an API key from [nextzen.org](https://developers.nextzen.org/). The key's pattern is like `Dto0r88DQuaQizoxcQSxxx`
 
 ## Fetch DEM by bound box
 When API key is reday, you can download DEM data like this:
 
 ```python
 bbox = 108.444319, 20.161757, 111.318897, 18.05883  # Hainan province of China
 
 terrain = Terrain("Dto0r88DQuaQizoxcQSxxx")  # Pass API key
 xs, ys, elevation = terrain.fetch(bbox=bbox, quiet=False, coord="lonlat", zoom=10)
 ```
 
-If download is not complete because of connection, retry it.
+If download is not completed because of connection, retry it.
```

### Comparing `pyterrain-0.0.1/setup.py` & `pyterrain-0.0.2/setup.py`

 * *Files identical despite different names*

