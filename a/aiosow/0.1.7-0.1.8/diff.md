# Comparing `tmp/aiosow-0.1.7.tar.gz` & `tmp/aiosow-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosow-0.1.7.tar", last modified: Mon May 22 14:55:29 2023, max compression
+gzip compressed data, was "aiosow-0.1.8.tar", last modified: Tue May 23 12:02:49 2023, max compression
```

## Comparing `aiosow-0.1.7.tar` & `aiosow-0.1.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:55:29.705353 aiosow-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-22 14:55:29.705353 aiosow-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-22 14:55:15.000000 aiosow-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:55:29.701353 aiosow-0.1.7/aiosow/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 14:55:15.000000 aiosow-0.1.7/aiosow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-22 14:55:15.000000 aiosow-0.1.7/aiosow/autofill.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-22 14:55:15.000000 aiosow-0.1.7/aiosow/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-22 14:55:15.000000 aiosow-0.1.7/aiosow/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-22 14:55:15.000000 aiosow-0.1.7/aiosow/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-22 14:55:15.000000 aiosow-0.1.7/aiosow/perpetuate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-22 14:55:15.000000 aiosow-0.1.7/aiosow/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-22 14:55:15.000000 aiosow-0.1.7/aiosow/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:55:29.701353 aiosow-0.1.7/aiosow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-22 14:55:29.000000 aiosow-0.1.7/aiosow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-22 14:55:29.000000 aiosow-0.1.7/aiosow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:55:29.000000 aiosow-0.1.7/aiosow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-22 14:55:29.000000 aiosow-0.1.7/aiosow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-22 14:55:29.000000 aiosow-0.1.7/aiosow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 14:55:29.000000 aiosow-0.1.7/aiosow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:55:29.705353 aiosow-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-22 14:55:15.000000 aiosow-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:55:29.705353 aiosow-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-22 14:55:15.000000 aiosow-0.1.7/tests/test_autofill.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-22 14:55:15.000000 aiosow-0.1.7/tests/test_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:55:15.000000 aiosow-0.1.7/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-22 14:55:15.000000 aiosow-0.1.7/tests/test_perpetuate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-22 14:55:15.000000 aiosow-0.1.7/tests/test_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-22 14:55:15.000000 aiosow-0.1.7/tests/test_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:02:49.620287 aiosow-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-23 12:02:49.620287 aiosow-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-23 12:02:34.000000 aiosow-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:02:49.616287 aiosow-0.1.8/aiosow/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-23 12:02:34.000000 aiosow-0.1.8/aiosow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-23 12:02:34.000000 aiosow-0.1.8/aiosow/autofill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-23 12:02:34.000000 aiosow-0.1.8/aiosow/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-23 12:02:34.000000 aiosow-0.1.8/aiosow/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-23 12:02:34.000000 aiosow-0.1.8/aiosow/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-23 12:02:34.000000 aiosow-0.1.8/aiosow/perpetuate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-23 12:02:34.000000 aiosow-0.1.8/aiosow/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-23 12:02:34.000000 aiosow-0.1.8/aiosow/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:02:49.616287 aiosow-0.1.8/aiosow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-23 12:02:49.000000 aiosow-0.1.8/aiosow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-23 12:02:49.000000 aiosow-0.1.8/aiosow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:02:49.000000 aiosow-0.1.8/aiosow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 12:02:49.000000 aiosow-0.1.8/aiosow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 12:02:49.000000 aiosow-0.1.8/aiosow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 12:02:49.000000 aiosow-0.1.8/aiosow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 12:02:49.620287 aiosow-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-23 12:02:34.000000 aiosow-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:02:49.620287 aiosow-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-23 12:02:34.000000 aiosow-0.1.8/tests/test_autofill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-23 12:02:34.000000 aiosow-0.1.8/tests/test_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 12:02:34.000000 aiosow-0.1.8/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-23 12:02:34.000000 aiosow-0.1.8/tests/test_perpetuate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-23 12:02:34.000000 aiosow-0.1.8/tests/test_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-23 12:02:34.000000 aiosow-0.1.8/tests/test_setup.py
```

### Comparing `aiosow-0.1.7/PKG-INFO` & `aiosow-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosow
-Version: 0.1.7
+Version: 0.1.8
 Summary: An event-based framework
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 
 [![Pypi](https://img.shields.io/pypi/v/aiosow?color=white&style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/aiosow/)
```

### Comparing `aiosow-0.1.7/README.md` & `aiosow-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.7/aiosow/autofill.py` & `aiosow-0.1.8/aiosow/autofill.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.7/aiosow/bindings.py` & `aiosow-0.1.8/aiosow/bindings.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.7/aiosow/command.py` & `aiosow-0.1.8/aiosow/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! env python3.11
 
 import logging, asyncio, importlib, argparse, sys
-from aiosow.setup import initialize, TRIGGER_ROUTINES
+from aiosow.setup import initialize, should_trigger_routines
 from aiosow.options import options, commands
 from aiosow.routines import spawn_routine_consumer
 
 
 def load_composition(composition=None, **kwargs):
     debug = (
         "-d" in sys.argv
@@ -81,22 +81,20 @@
 def run(composition=None, **kwargs):
     memory = load_composition(composition=composition, **kwargs)
     logging.debug(memory)
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
     tasks = loop.run_until_complete(initialize(memory))
     memory["running"] = True
-    if TRIGGER_ROUTINES:
+    if should_trigger_routines():
         consumer = loop.run_until_complete(spawn_routine_consumer(memory))
         if consumer:
             tasks = tasks + [consumer]
-    # setups can return a task which is ran here
-    # this allows setups to start tasks and still have them complete
     loop.run_until_complete(asyncio.gather(*tasks))
-    if memory["run_forever"]:
+    if memory.get("run_forever", False):
         loop.run_forever()
 
 
 if __name__ == "__main__":
     run()
 
 __all__ = []
```

### Comparing `aiosow-0.1.7/aiosow/options.py` & `aiosow-0.1.8/aiosow/options.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.7/aiosow/perpetuate.py` & `aiosow-0.1.8/aiosow/perpetuate.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.7/aiosow/routines.py` & `aiosow-0.1.8/aiosow/routines.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.7/aiosow/setup.py` & `aiosow-0.1.8/aiosow/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 
 
 def trigger_routines():
     global TRIGGER_ROUTINES
     TRIGGER_ROUTINES = True
 
 
+def should_trigger_routines() -> bool:  # pragma: no cover
+    global TRIGGER_ROUTINES
+    return TRIGGER_ROUTINES
+
+
 def clear_setups():  # pragma: no cover
     global SETUP_FUNCTIONS
     SETUP_FUNCTIONS = []
 
 
 def get_setups():  # pragma: no cover
     global SETUP_FUNCTIONS
@@ -28,30 +33,34 @@
     **Args**:
     - func (Callable): Function to add to the list of initialization functions.
 
     **Returns**:
     - func (Callable): The same function, unchanged.
     """
     if func in SETUP_FUNCTIONS:
-        logging.debug("duplicate setup declaration of %s is ignored", func.__name__)
+        logging.debug(
+            "duplicate setup declaration of %s is ignored", func.__name__
+        )
     else:
         logging.info("+ setup %s", func.__name__)
         SETUP_FUNCTIONS.append(func)
     return func
 
 
 async def initialize(memory: Dict) -> List[asyncio.Task]:
     """
     Function that runs all initialization functions added to the list.
 
     Args:
         - app (web.Application): The aiohttp application.
         - mem (Dict): The mem dictionary.
     """
-    logging.debug("initialize with %s", [f"{fn.__name__}" for fn in SETUP_FUNCTIONS])
+    logging.debug(
+        "initialize with %s", [f"{fn.__name__}" for fn in SETUP_FUNCTIONS]
+    )
     tasks = []
     for setup_func in SETUP_FUNCTIONS:
         logging.debug("setup(%s)", setup_func.__name__)
         result = await perpetuate(setup_func, memory=memory)
         logging.debug("%s() => %s", setup_func.__name__, result)
         if asyncio.iscoroutine(result):
             tasks.append(result)
```

### Comparing `aiosow-0.1.7/aiosow.egg-info/PKG-INFO` & `aiosow-0.1.8/aiosow.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosow
-Version: 0.1.7
+Version: 0.1.8
 Summary: An event-based framework
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 
 [![Pypi](https://img.shields.io/pypi/v/aiosow?color=white&style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/aiosow/)
```

### Comparing `aiosow-0.1.7/setup.py` & `aiosow-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="aiosow",
-    version="0.1.7",
+    version="0.1.8",
     packages=find_packages(include=["aiosow"]),
     description="An event-based framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     entry_points={
         "console_scripts": [
```

### Comparing `aiosow-0.1.7/tests/test_autofill.py` & `aiosow-0.1.8/tests/test_autofill.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.7/tests/test_bindings.py` & `aiosow-0.1.8/tests/test_bindings.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.7/tests/test_perpetuate.py` & `aiosow-0.1.8/tests/test_perpetuate.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.7/tests/test_routines.py` & `aiosow-0.1.8/tests/test_routines.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.7/tests/test_setup.py` & `aiosow-0.1.8/tests/test_setup.py`

 * *Files identical despite different names*

