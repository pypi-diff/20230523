# Comparing `tmp/changedetector-0.6.2.tar.gz` & `tmp/changedetector-0.6.3.tar.gz`

## Comparing `changedetector-0.6.2.tar` & `changedetector-0.6.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/__init__.py
--rw-r--r--   0        0        0    17819 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/detectchange.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/gobals_variables.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/makeParser.py
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/menu.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/versionControl.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/wrapperComponents.py
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/wrm.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/wro.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/wrs.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/wtch.py
--rwxr-xr-x   0        0        0     1558 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/scripts/detectchange.fish
--rwxr-xr-x   0        0        0     1555 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/scripts/detectchange.sh
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 changedetector-0.6.2/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 changedetector-0.6.2/LICENCE
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 changedetector-0.6.2/README.md
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 changedetector-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 changedetector-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/__init__.py
+-rw-r--r--   0        0        0    17823 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/detectchange.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/gobals_variables.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/makeParser.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/menu.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/versionControl.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/wrapperComponents.py
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/wrm.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/wro.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/wrs.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/wtch.py
+-rwxr-xr-x   0        0        0     1558 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/scripts/detectchange.fish
+-rwxr-xr-x   0        0        0     1555 2020-02-02 00:00:00.000000 changedetector-0.6.3/changedetector/scripts/detectchange.sh
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 changedetector-0.6.3/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 changedetector-0.6.3/LICENCE
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 changedetector-0.6.3/README.md
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 changedetector-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 changedetector-0.6.3/PKG-INFO
```

### Comparing `changedetector-0.6.2/changedetector/__init__.py` & `changedetector-0.6.3/changedetector/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 :license: MIT, see LICENSE for more details.
 """
 
 __title__ = "changedetector"
 __author__ = "LuxLuth"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) 2023 LuxLuth"
-__version__ = "0.6.2"
+__version__ = "0.6.3"
```

### Comparing `changedetector-0.6.2/changedetector/detectchange.py` & `changedetector-0.6.3/changedetector/detectchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 """
 detectchange CLI module
 ===
 """
+
+import time
+import os
+
+from rich import print as rprint
+from rich.console import Console
+import typer
+
+from watchdog.observers import Observer
+from pyfiglet import Figlet
+import tomli
+
+import sys
+
+sys.path.append(os.path.dirname(os.path.realpath(__file__)))
+
 from menu import menu
 from wrapperComponents import WrapperComponents as wp
 from makeParser import Parser
 
 # handlers
 from wrs import WrsHandler
 from wro import WroHandler
 from wtch import WatchForHandler
 from wrm import WrmHandler
 
 # Version Control
 from versionControl import VersionControl
 from gobals_variables import VARS as v
 
-import time
-import os
-
-import sys
-from rich import print as rprint
-from rich.console import Console
-import typer
-
-from watchdog.observers import Observer
-from pyfiglet import Figlet
-import tomli
 
-sys.path.append(os.path.dirname(os.path.realpath(__file__)))
 
 class Entries:
     """
     Save all the data values
     """
     def __init__(self, is_empty=False):
         self.entries = {}
```

### Comparing `changedetector-0.6.2/changedetector/makeParser.py` & `changedetector-0.6.3/changedetector/makeParser.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.2/changedetector/menu.py` & `changedetector-0.6.3/changedetector/menu.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.2/changedetector/versionControl.py` & `changedetector-0.6.3/changedetector/versionControl.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.2/changedetector/wrapperComponents.py` & `changedetector-0.6.3/changedetector/wrapperComponents.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.2/changedetector/wrm.py` & `changedetector-0.6.3/changedetector/wrm.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.2/changedetector/wro.py` & `changedetector-0.6.3/changedetector/wro.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.2/changedetector/wrs.py` & `changedetector-0.6.3/changedetector/wrs.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.2/changedetector/wtch.py` & `changedetector-0.6.3/changedetector/wtch.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.2/changedetector/scripts/detectchange.fish` & `changedetector-0.6.3/changedetector/scripts/detectchange.fish`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.2/changedetector/scripts/detectchange.sh` & `changedetector-0.6.3/changedetector/scripts/detectchange.sh`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.2/LICENCE` & `changedetector-0.6.3/LICENCE`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.2/README.md` & `changedetector-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.2/pyproject.toml` & `changedetector-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.2/PKG-INFO` & `changedetector-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changedetector
-Version: 0.6.2
+Version: 0.6.3
 Summary: A basic change detector for the Python, Ruby and C++.
 Project-URL: Bug Tracker, https://github.com/luxluth/changedetector/issues
 Project-URL: Homepage, https://github.com/luxluth/changedetector
 Author-email: Lux Luth <luxusluth@gmail.com>
 License-Expression: MIT
 License-File: LICENCE
 Classifier: Development Status :: 5 - Production/Stable
```

