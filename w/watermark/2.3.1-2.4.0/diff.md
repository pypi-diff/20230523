# Comparing `tmp/watermark-2.3.1.tar.gz` & `tmp/watermark-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watermark-2.3.1.tar", last modified: Fri May 27 13:55:16 2022, max compression
+gzip compressed data, was "watermark-2.4.0.tar", last modified: Tue May 23 15:50:08 2023, max compression
```

## Comparing `watermark-2.3.1.tar` & `watermark-2.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2022-05-27 13:55:16.059638 watermark-2.3.1/
--rw-r--r--   0 sebastian   (501) staff       (20)     1507 2022-01-04 01:54:42.000000 watermark-2.3.1/LICENSE
--rw-r--r--   0 sebastian   (501) staff       (20)       34 2022-01-04 01:25:16.000000 watermark-2.3.1/MANIFEST.in
--rw-r--r--   0 sebastian   (501) staff       (20)     1224 2022-05-27 13:55:16.059700 watermark-2.3.1/PKG-INFO
--rw-r--r--   0 sebastian   (501) staff       (20)    10753 2022-05-27 13:53:24.000000 watermark-2.3.1/README.md
--rw-r--r--   0 sebastian   (501) staff       (20)      512 2022-05-27 13:55:16.059921 watermark-2.3.1/setup.cfg
--rw-r--r--   0 sebastian   (501) staff       (20)     1292 2022-05-27 13:51:08.000000 watermark-2.3.1/setup.py
-drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2022-05-27 13:55:16.059021 watermark-2.3.1/watermark/
--rw-r--r--   0 sebastian   (501) staff       (20)      373 2022-01-04 01:25:16.000000 watermark-2.3.1/watermark/__init__.py
--rw-r--r--   0 sebastian   (501) staff       (20)     3682 2022-01-04 01:54:42.000000 watermark-2.3.1/watermark/magic.py
--rw-r--r--   0 sebastian   (501) staff       (20)      291 2022-01-04 01:25:16.000000 watermark-2.3.1/watermark/version.py
--rw-r--r--   0 sebastian   (501) staff       (20)     9056 2022-01-04 01:25:26.000000 watermark-2.3.1/watermark/watermark.py
-drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2022-05-27 13:55:16.059545 watermark-2.3.1/watermark.egg-info/
--rw-r--r--   0 sebastian   (501) staff       (20)     1224 2022-05-27 13:55:16.000000 watermark-2.3.1/watermark.egg-info/PKG-INFO
--rw-r--r--   0 sebastian   (501) staff       (20)      297 2022-05-27 13:55:16.000000 watermark-2.3.1/watermark.egg-info/SOURCES.txt
--rw-r--r--   0 sebastian   (501) staff       (20)        1 2022-05-27 13:55:16.000000 watermark-2.3.1/watermark.egg-info/dependency_links.txt
--rw-r--r--   0 sebastian   (501) staff       (20)       59 2022-05-27 13:55:16.000000 watermark-2.3.1/watermark.egg-info/requires.txt
--rw-r--r--   0 sebastian   (501) staff       (20)       10 2022-05-27 13:55:16.000000 watermark-2.3.1/watermark.egg-info/top_level.txt
+drwxr-xr-x   0 sebastianraschka   (501) staff       (20)        0 2023-05-23 15:50:08.992339 watermark-2.4.0/
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)     1507 2023-05-23 15:48:12.000000 watermark-2.4.0/LICENSE
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)       34 2023-05-23 15:48:12.000000 watermark-2.4.0/MANIFEST.in
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)     1205 2023-05-23 15:50:08.992422 watermark-2.4.0/PKG-INFO
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)    11591 2023-05-23 15:48:12.000000 watermark-2.4.0/README.md
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)      512 2023-05-23 15:50:08.992696 watermark-2.4.0/setup.cfg
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)     1476 2023-05-23 15:48:12.000000 watermark-2.4.0/setup.py
+drwxr-xr-x   0 sebastianraschka   (501) staff       (20)        0 2023-05-23 15:50:08.991489 watermark-2.4.0/watermark/
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)      373 2023-05-23 15:48:12.000000 watermark-2.4.0/watermark/__init__.py
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)     3842 2023-05-23 15:48:12.000000 watermark-2.4.0/watermark/magic.py
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)      291 2023-05-23 15:48:12.000000 watermark-2.4.0/watermark/version.py
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)    10070 2023-05-23 15:48:12.000000 watermark-2.4.0/watermark/watermark.py
+drwxr-xr-x   0 sebastianraschka   (501) staff       (20)        0 2023-05-23 15:50:08.992219 watermark-2.4.0/watermark.egg-info/
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)     1205 2023-05-23 15:50:08.000000 watermark-2.4.0/watermark.egg-info/PKG-INFO
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)      297 2023-05-23 15:50:08.000000 watermark-2.4.0/watermark.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)        1 2023-05-23 15:50:08.000000 watermark-2.4.0/watermark.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)       61 2023-05-23 15:50:08.000000 watermark-2.4.0/watermark.egg-info/requires.txt
+-rw-r--r--   0 sebastianraschka   (501) staff       (20)       10 2023-05-23 15:50:08.000000 watermark-2.4.0/watermark.egg-info/top_level.txt
```

### Comparing `watermark-2.3.1/LICENSE` & `watermark-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `watermark-2.3.1/PKG-INFO` & `watermark-2.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: watermark
-Version: 2.3.1
+Version: 2.4.0
 Summary: IPython magic function to print date/time stamps and various system information.
 Home-page: https://github.com/rasbt/watermark
 Author: Sebastian Raschka
 Author-email: mail@sebastianraschka.com
 License: newBSD
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -29,8 +28,7 @@
 please feel free to contact me via
 email: mail@sebastianraschka.com
 
 This project is hosted at https://github.com/rasbt/watermark
 
 The documentation can be found at
 https://github.com/rasbt/watermark/blob/master/README.md
-
```

### Comparing `watermark-2.3.1/README.md` & `watermark-2.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,25 +18,68 @@
 
 <br>
 
 ## Examples
 
 [[top](#sections)]
 
+### Using watermark in  Jupyter notebooks and IPython sessions
+
+
+
 ![](docs/images/ex1.png)
 
 ![](docs/images/ex2.png)
 
-
 **More examples can be found in this [Jupyter notebook](docs/watermark.ipynb).**
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/rasbt/watermark/master?filepath=docs%2Fwatermark.ipynb)
 
 <br>
 
+
+### Using watermark as a module
+
+
+```python
+from watermark import watermark
+print(watermark())
+```
+
+```
+Last updated: 2022-09-13T16:28:56.177487-05:00
+
+Python implementation: CPython
+Python version       : 3.9.13
+IPython version      : 8.4.0
+
+Compiler    : Clang 13.0.1 
+OS          : Darwin
+Release     : 21.6.0
+Machine     : arm64
+Processor   : arm
+CPU cores   : 10
+Architecture: 64bit
+```
+
+```python
+print(watermark(packages="numpy,scipy"))
+```
+
+```
+numpy: 1.23.2
+scipy: 1.9.1
+```
+
+
+
+See `help(watermark)` for more options.
+
+
+
 ## Installation and updating
 
 [[top](#sections)]
 
 The watermark line magic can be installed by executing
 
 ```bash
@@ -129,14 +172,17 @@
 
 <br>
 
 ## Changelog
 
 [[top](#sections)]
 
+#### v. 2.4.0 (May 23, 2023)
+
+- Adds a new `--gpu` flag to print out GPU information (currently limited to NVIDIA devices) ([#90](https://github.com/rasbt/watermark/pull/63), via contribution by [907Resident](https://github.com/907Resident))
 
 
 #### v. 2.3.1 (May 27, 2022)
 
 - Upper limit on importlib-metadata caused trouble installing on Python 3.7.
   Instead pin to minimum version with Python 3.8 functionality according to https://github.com/python/importlib_metadata#compatibility  ([#86](https://github.com/rasbt/watermark/pull/63), via contribution by [James Myatt](https://github.com/jamesmyatt))
```

### Comparing `watermark-2.3.1/setup.cfg` & `watermark-2.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 2.3.1
+version = 2.4.0
 license_file = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: IPython
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
```

### Comparing `watermark-2.3.1/setup.py` & `watermark-2.4.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 # Sebastian Raschka 2014-2022
 # IPython magic function to print date/time stamps and
 # various system information.
 # Author: Sebastian Raschka <sebastianraschka.com>
 #
 # License: BSD 3 clause
 
+from os.path import dirname, join, realpath
 from textwrap import dedent
 
 from setuptools import find_packages, setup
 
+
+PROJECT_ROOT = dirname(realpath(__file__))
+REQUIREMENTS_FILE = join(PROJECT_ROOT, "requirements.txt")
+
+with open(REQUIREMENTS_FILE) as f:
+    install_reqs = f.read().splitlines()
+
+install_reqs.append("setuptools")
+
 # Also see settings in setup.cfg
 setup(
     name="watermark",
     license="newBSD",
     description=(
         "IPython magic function to print date/time stamps and "
         "various system information."
     ),
     author="Sebastian Raschka",
     author_email="mail@sebastianraschka.com",
     url="https://github.com/rasbt/watermark",
     packages=find_packages(exclude=[]),
-    install_requires=[
-        "ipython",
-        'importlib-metadata >= 1.4 ; python_version < "3.8"',
-    ],
+    install_requires=install_reqs,
     long_description=dedent(
         """\
         An IPython magic extension for printing date and time stamps, version
         numbers, and hardware information.
 
         Contact
         =============
```

### Comparing `watermark-2.3.1/watermark/magic.py` & `watermark-2.4.0/watermark/magic.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,14 +66,17 @@
               help='prints current Git remote address')
     @argument('-b', '--gitbranch', action='store_true',
               help='prints current Git branch')
     @argument('-w', '--watermark', action='store_true',
               help='prints the current version of watermark')
     @argument('-iv', '--iversions', action='store_true',
               help='prints the name/version of all imported modules')
+    @argument('--gpu', action='store_true',
+              help='prints GPU information (currently limited to NVIDIA GPUs),'
+                   ' if available')
     @line_magic
     def watermark(self, line):
         """
         IPython magic function to print date/time stamps
         and various system information.
         """
         args = vars(parse_argstring(self.watermark, line))
```

### Comparing `watermark-2.3.1/watermark/watermark.py` & `watermark-2.4.0/watermark/watermark.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,34 +14,54 @@
 import os
 import platform
 import subprocess
 import time
 import types
 from multiprocessing import cpu_count
 from socket import gethostname
+import platform
+from py3nvml import py3nvml
 
 try:
     import importlib.metadata as importlib_metadata
 except ImportError:
     # Running on pre-3.8 Python; use importlib-metadata package
     import importlib_metadata
 
 import IPython
 
 from .version import __version__
 
 
-def watermark(author=None, email=None, github_username=None,
-              website=None, current_date=False, datename=False,
-              current_time=False, iso8601=False, timezone=False,
-              updated=False, custom_time=None, python=False,
-              packages=None, conda=False, hostname=False, machine=False,
-              githash=False, gitrepo=False, gitbranch=False,
-              watermark=False, iversions=False, watermark_self=None,
-              globals_=None):
+def watermark(
+        author=None, 
+        email=None, 
+        github_username=None,
+        website=None, 
+        current_date=False, 
+        datename=False,
+        current_time=False, 
+        iso8601=False, 
+        timezone=False,
+        updated=False, 
+        custom_time=None, 
+        python=False,
+        packages=None, 
+        conda=False, 
+        hostname=False, 
+        machine=False,
+        githash=False, 
+        gitrepo=False, 
+        gitbranch=False,
+        watermark=False, 
+        iversions=False, 
+        gpu=False,
+        watermark_self=None,
+        globals_=None
+):
 
     '''Function to print date/time stamps and various system information.
 
     Parameters:
     ===========
 
     author :
@@ -103,14 +123,17 @@
         prints current Git branch
 
     watermark :
         prints the current version of watermark
 
     iversions :
         prints the name/version of all imported modules
+    
+    gpu :
+        prints GPU information (currently limited to NVIDIA GPUs), if available
 
     watermark_self :
         instance of the watermark magics class, which is required
         for iversions.
 
     '''
     output = []
@@ -178,14 +201,16 @@
                 ns = globals_
             else:
                 raise RuntimeError(
                     "Either `watermark_self` or `globals_` must be provided "
                     "to show imported package versions."
                 )
             output.append(_get_all_import_versions(ns))
+        if args['gpu']:
+            output.append(_get_gpu_info())
         if args['watermark']:
             output.append({"Watermark": __version__})
 
     return _generate_formatted_text(output)
 
 
 def _generate_formatted_text(list_of_dicts):
@@ -302,7 +327,27 @@
             to_print[pkg_name] = pkg_version
     return to_print
 
 
 def _get_conda_env():
     name = os.getenv('CONDA_DEFAULT_ENV', 'n/a')
     return {"conda environment": name}
+
+
+def _get_gpu_info():
+    try:
+        gpu_info = [""]
+        py3nvml.nvmlInit()
+        num_gpus = py3nvml.nvmlDeviceGetCount()
+        for i in range(num_gpus):
+            handle = py3nvml.nvmlDeviceGetHandleByIndex(i)
+            gpu_name = py3nvml.nvmlDeviceGetName(handle)
+            gpu_info.append(f"GPU {i}: {gpu_name}")
+        py3nvml.nvmlShutdown()
+        return {"GPU Info": "\n  ".join(gpu_info)}
+
+    except py3nvml.NVMLError_LibraryNotFound:
+        return {"GPU Info": "NVIDIA drivers do not appear "
+                "to be installed on this machine."}
+    except:
+        return {"GPU Info": "GPU information is not "
+                "available for this machine."}
```

### Comparing `watermark-2.3.1/watermark.egg-info/PKG-INFO` & `watermark-2.4.0/watermark.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: watermark
-Version: 2.3.1
+Version: 2.4.0
 Summary: IPython magic function to print date/time stamps and various system information.
 Home-page: https://github.com/rasbt/watermark
 Author: Sebastian Raschka
 Author-email: mail@sebastianraschka.com
 License: newBSD
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -29,8 +28,7 @@
 please feel free to contact me via
 email: mail@sebastianraschka.com
 
 This project is hosted at https://github.com/rasbt/watermark
 
 The documentation can be found at
 https://github.com/rasbt/watermark/blob/master/README.md
-
```

