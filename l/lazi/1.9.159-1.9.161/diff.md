# Comparing `tmp/lazi-1.9.159.tar.gz` & `tmp/lazi-1.9.161.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazi-1.9.159.tar", max compression
+gzip compressed data, was "lazi-1.9.161.tar", max compression
```

## Comparing `lazi-1.9.159.tar` & `lazi-1.9.161.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      150 2023-05-17 23:57:14.424788 lazi-1.9.159/lazi/auto.py
--rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.9.159/lazi/conf/auto.py
--rw-r--r--   0        0        0     2889 2023-05-21 03:45:32.024218 lazi-1.9.159/lazi/conf/base.py
--rw-r--r--   0        0        0     4708 2023-05-18 02:24:12.623535 lazi-1.9.159/lazi/conf/conf.py
--rw-r--r--   0        0        0     1330 2023-05-18 02:20:03.676308 lazi-1.9.159/lazi/conf/envs.py
--rw-r--r--   0        0        0      636 2023-05-21 03:44:00.843059 lazi-1.9.159/lazi/conf/lazy.py
--rw-r--r--   0        0        0      289 2023-05-20 16:53:17.056017 lazi-1.9.159/lazi/core/__init__.py
--rw-r--r--   0        0        0     4902 2023-05-21 03:21:48.078178 lazi-1.9.159/lazi/core/finder.py
--rw-r--r--   0        0        0     6755 2023-05-21 03:23:16.099290 lazi-1.9.159/lazi/core/loader.py
--rw-r--r--   0        0        0     4461 2023-05-21 03:44:53.939734 lazi-1.9.159/lazi/core/module.py
--rw-r--r--   0        0        0     3355 2023-05-21 03:13:04.587587 lazi-1.9.159/lazi/core/spec.py
--rw-r--r--   0        0        0     3571 2023-05-17 06:13:14.860256 lazi-1.9.159/lazi/core/stat.py
--rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.9.159/lazi/util/__init__.py
--rw-r--r--   0        0        0      873 2023-05-18 05:48:25.043176 lazi-1.9.159/lazi/util/debug.py
--rw-r--r--   0        0        0      146 2023-05-18 08:04:01.089875 lazi-1.9.159/lazi/util/functional.py
--rw-r--r--   0        0        0       73 2023-05-18 08:06:11.639587 lazi-1.9.159/lazi/util/util.py
--rw-r--r--   0        0        0     2077 2023-05-21 03:46:47.089172 lazi-1.9.159/pyproject.toml
--rw-r--r--   0        0        0     8937 2023-05-18 16:04:24.075835 lazi-1.9.159/readme.md
--rw-r--r--   0        0        0        0 2023-05-17 06:10:55.650459 lazi-1.9.159/tests/__init__.py
--rw-r--r--   0        0        0      203 2023-05-15 22:42:51.727662 lazi-1.9.159/tests/standalone/sa_array.py
--rw-r--r--   0        0        0      922 2023-05-18 00:51:41.543400 lazi-1.9.159/tests/standalone/sa_nested.py
--rw-r--r--   0        0        0       43 2023-05-18 04:25:44.850316 lazi-1.9.159/tests/standalone/sa_pandas.py
--rw-r--r--   0        0        0      273 2023-05-15 22:42:51.727662 lazi-1.9.159/tests/standalone/sa_pygments.py
--rw-r--r--   0        0        0      524 2023-05-20 17:57:16.350542 lazi-1.9.159/tests/test_array.py
--rw-r--r--   0        0        0      408 2023-05-20 17:46:16.661789 lazi-1.9.159/tests/test_asyncio.py
--rw-r--r--   0        0        0     1291 2023-05-20 17:46:16.661789 lazi-1.9.159/tests/test_django.py
--rw-r--r--   0        0        0     1285 2023-05-18 22:58:43.789962 lazi-1.9.159/tests/test_importlib.py
--rw-r--r--   0        0        0      263 2023-05-20 17:46:16.673789 lazi-1.9.159/tests/test_lazy.py
--rw-r--r--   0        0        0      337 2023-05-20 17:46:16.673789 lazi-1.9.159/tests/test_pygments.py
--rw-r--r--   0        0        0      862 2023-05-20 17:46:16.669789 lazi-1.9.159/tests/test_requests.py
--rw-r--r--   0        0        0     1046 2023-05-20 17:46:16.665789 lazi-1.9.159/tests/test_rich.py
--rw-r--r--   0        0        0     1259 2023-05-20 18:00:58.413489 lazi-1.9.159/tests/test_stat.py
--rw-r--r--   0        0        0     9934 1970-01-01 00:00:00.000000 lazi-1.9.159/PKG-INFO
+-rw-r--r--   0        0        0      150 2023-05-17 23:57:14.424788 lazi-1.9.161/lazi/auto.py
+-rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.9.161/lazi/conf/auto.py
+-rw-r--r--   0        0        0     2889 2023-05-21 03:45:32.024218 lazi-1.9.161/lazi/conf/base.py
+-rw-r--r--   0        0        0     4708 2023-05-18 02:24:12.623535 lazi-1.9.161/lazi/conf/conf.py
+-rw-r--r--   0        0        0     1330 2023-05-18 02:20:03.676308 lazi-1.9.161/lazi/conf/envs.py
+-rw-r--r--   0        0        0      636 2023-05-21 03:44:00.843059 lazi-1.9.161/lazi/conf/lazy.py
+-rw-r--r--   0        0        0      289 2023-05-20 16:53:17.056017 lazi-1.9.161/lazi/core/__init__.py
+-rw-r--r--   0        0        0     4877 2023-05-23 00:27:38.458660 lazi-1.9.161/lazi/core/finder.py
+-rw-r--r--   0        0        0     6755 2023-05-21 03:23:16.099290 lazi-1.9.161/lazi/core/loader.py
+-rw-r--r--   0        0        0     4461 2023-05-21 03:44:53.939734 lazi-1.9.161/lazi/core/module.py
+-rw-r--r--   0        0        0     3355 2023-05-21 03:13:04.587587 lazi-1.9.161/lazi/core/spec.py
+-rw-r--r--   0        0        0     3571 2023-05-17 06:13:14.860256 lazi-1.9.161/lazi/core/stat.py
+-rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.9.161/lazi/util/__init__.py
+-rw-r--r--   0        0        0      873 2023-05-18 05:48:25.043176 lazi-1.9.161/lazi/util/debug.py
+-rw-r--r--   0        0        0      146 2023-05-18 08:04:01.089875 lazi-1.9.161/lazi/util/functional.py
+-rw-r--r--   0        0        0       73 2023-05-18 08:06:11.639587 lazi-1.9.161/lazi/util/util.py
+-rw-r--r--   0        0        0     1904 2023-05-23 00:38:31.447092 lazi-1.9.161/pyproject.toml
+-rw-r--r--   0        0        0     9025 2023-05-23 00:35:42.076886 lazi-1.9.161/readme.md
+-rw-r--r--   0        0        0        0 2023-05-17 06:10:55.650459 lazi-1.9.161/tests/__init__.py
+-rw-r--r--   0        0        0      203 2023-05-15 22:42:51.727662 lazi-1.9.161/tests/standalone/sa_array.py
+-rw-r--r--   0        0        0      922 2023-05-18 00:51:41.543400 lazi-1.9.161/tests/standalone/sa_nested.py
+-rw-r--r--   0        0        0       43 2023-05-18 04:25:44.850316 lazi-1.9.161/tests/standalone/sa_pandas.py
+-rw-r--r--   0        0        0      273 2023-05-15 22:42:51.727662 lazi-1.9.161/tests/standalone/sa_pygments.py
+-rw-r--r--   0        0        0      524 2023-05-20 17:57:16.350542 lazi-1.9.161/tests/test_array.py
+-rw-r--r--   0        0        0      408 2023-05-20 17:46:16.661789 lazi-1.9.161/tests/test_asyncio.py
+-rw-r--r--   0        0        0     1291 2023-05-20 17:46:16.661789 lazi-1.9.161/tests/test_django.py
+-rw-r--r--   0        0        0     1285 2023-05-18 22:58:43.789962 lazi-1.9.161/tests/test_importlib.py
+-rw-r--r--   0        0        0      263 2023-05-20 17:46:16.673789 lazi-1.9.161/tests/test_lazy.py
+-rw-r--r--   0        0        0      337 2023-05-20 17:46:16.673789 lazi-1.9.161/tests/test_pygments.py
+-rw-r--r--   0        0        0      955 2023-05-23 00:30:25.892775 lazi-1.9.161/tests/test_requests.py
+-rw-r--r--   0        0        0     1046 2023-05-20 17:46:16.665789 lazi-1.9.161/tests/test_rich.py
+-rw-r--r--   0        0        0     1375 2023-05-23 00:31:14.009382 lazi-1.9.161/tests/test_stat.py
+-rw-r--r--   0        0        0    10022 1970-01-01 00:00:00.000000 lazi-1.9.161/PKG-INFO
```

### Comparing `lazi-1.9.159/lazi/conf/base.py` & `lazi-1.9.161/lazi/conf/base.py`

 * *Files identical despite different names*

### Comparing `lazi-1.9.159/lazi/conf/conf.py` & `lazi-1.9.161/lazi/conf/conf.py`

 * *Files identical despite different names*

### Comparing `lazi-1.9.159/lazi/conf/envs.py` & `lazi-1.9.161/lazi/conf/envs.py`

 * *Files identical despite different names*

### Comparing `lazi-1.9.159/lazi/conf/lazy.py` & `lazi-1.9.161/lazi/conf/lazy.py`

 * *Files identical despite different names*

### Comparing `lazi-1.9.159/lazi/core/finder.py` & `lazi-1.9.161/lazi/core/finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 import sys
 import atexit
 from types import ModuleType
 from importlib.abc import MetaPathFinder
 from importlib.machinery import ModuleSpec
 from importlib import import_module
-from pathlib import Path
 import re
 
 from lazi.conf import conf
 from lazi.util import classproperty, debug, oid
 
 from .spec import Spec
 from .loader import Loader
```

### Comparing `lazi-1.9.159/lazi/core/loader.py` & `lazi-1.9.161/lazi/core/loader.py`

 * *Files identical despite different names*

### Comparing `lazi-1.9.159/lazi/core/module.py` & `lazi-1.9.161/lazi/core/module.py`

 * *Files identical despite different names*

### Comparing `lazi-1.9.159/lazi/core/spec.py` & `lazi-1.9.161/lazi/core/spec.py`

 * *Files identical despite different names*

### Comparing `lazi-1.9.159/lazi/core/stat.py` & `lazi-1.9.161/lazi/core/stat.py`

 * *Files identical despite different names*

### Comparing `lazi-1.9.159/lazi/util/debug.py` & `lazi-1.9.161/lazi/util/debug.py`

 * *Files identical despite different names*

### Comparing `lazi-1.9.159/pyproject.toml` & `lazi-1.9.161/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazi"
-version = "1.9.159"
+version = "1.9.161"
 description = "A lightweight and extensible way to implement lazy imports globally."
 authors = ["Phillip Sitbon <phillip.sitbon@gmail.com>"]
 readme = "readme.md"
 license = "AGPLv3"
 repository = "https://github.com/sitbon/lazi"
 classifiers= [
     "Environment :: Web Environment",
@@ -43,35 +43,28 @@
 build.sequence = [
     { ref = "commit-info" },
     { cmd = "poetry build" },
     { shell = "sha512sum dist/lazi-$(poetry version -s).tar.gz" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 
 
 [tool.poetry.group.dev.dependencies]
 django = "^4"
 requests = "^2"
 toolz = "^0"
 rich = "^13"
 setuptools = "^67"
 pandas = "^2"
 pytest = "^7"
 wagtail = "^5.0"
-presto-requests = "^1.3.6"
 poethepoet = "^0.20.0"
 
-[tool.poetry.group.direct]
-optional = true
-[tool.poetry.group.direct.dependencies]
-presto-requests = {git = "https://github.com/sitbon/presto"}
-
-
 [tool.pytest.ini_options]
 addopts = "-v --no-header -rA"
 cache_dir = ".cache/pytest"
 # log_cli = true
 log_cli_level = "DEBUG"
 log_cli_format = "%(message)s"
 log_format = "%(message)s"
```

### Comparing `lazi-1.9.159/readme.md` & `lazi-1.9.161/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Lazi: Lazy Imports Everywhere
 
 An easy way to implement and track lazy imports globally.
 
 No external dependencies.
 
-**Requres Python 3.11.**
+**Requires Python >= 3.10, and 3.11 is HIGHLY Recommended.**
 
 ## Usage:
 
 ```shell
 poetry add lazi
 ```
 ```shell
@@ -30,25 +30,25 @@
 And with `TRACE=3`:
 
 ```pycon
 >>> import lazi.auto
 [7F4C28B37350] HOOK Finder refs:0 inst:0 sys:5 
 >>> import django
 [7F4C28B37350] FIND pyc  django *
-[7F4C289BD5D0] CREA LAZY [7F4C28C4A160] django ....  # This is where the lazy module is set up.
+[7F4C289BD5D0] CREA LAZY [7F4C28C4A160] django ....  # This is where the a module is set up.
 >>> django.VERSION
 [7F4C289BD5D0] LAZY >>>> [7F4C28C4A160] django VERSION
 [7F4C289BD5D0] LAZY EXEC [7F4C28C4A160] django >>>> 
 [7F4C28B37350] FIND pyc  django.utils 
 [7F4C289BD080] CREA LAZY [7F4C289BD0D0] django.utils .... 
 [7F4C28B37350] FIND pyc  django.utils|version 
 [7F4C289BD800] CREA LAZY [7F4C289BD490] django.utils|version .... 
 [7F4C289BD080] LAZY >>>> [7F4C289BD0D0] django.utils version = [7F4C289BD800]
 [7F4C289BD080] LAZY EXEC [7F4C289BD0D0] django.utils >>>> 
-[7F4C289BD080] EXEC LOAD [7F4C289BD0D0] django.utils ++++  # This is where the lazy module is fully loaded. 
+[7F4C289BD080] EXEC LOAD [7F4C289BD0D0] django.utils ++++ 
 [7F4C289BD800] LAZY >>>> [7F4C289BD490] django.utils|version get_version
 [7F4C289BD800] LAZY EXEC [7F4C289BD490] django.utils|version >>>> 
 [7F4C28B37350] FIND pycS datetime *  # "S" means it's a stdlib module. "B" means it's a builtin module.
 [7F4C289BDF30] CREA LAZY [7F4C289BDF80] datetime .... 
 [7F4C28B37350] FIND pycS subprocess *
 [7F4C289BE020] CREA LAZY [7F4C289BE070] subprocess .... 
 [7F4C28B37350] FIND pyc  django.utils|regex_helper 
@@ -60,15 +60,15 @@
 [7F4C289BE4D0] LAZY >>>> [7F4C289BE3E0] django.utils|functional SimpleLazyObject
 [7F4C289BE4D0] LAZY EXEC [7F4C289BE3E0] django.utils|functional >>>> 
 [7F4C28B37350] FIND pycS copy *
 [7F4C289BF830] CREA LAZY [7F4C289BF380] copy .... 
 [7F4C289BE4D0] EXEC LOAD [7F4C289BE3E0] django.utils|functional ++++ 
 [7F4C289BE0C0] EXEC LOAD [7F4C289BDFD0] django.utils|regex_helper ++++ 
 [7F4C289BD800] EXEC LOAD [7F4C289BD490] django.utils|version ++++ 
-[7F4C289BD5D0] EXEC LOAD [7F4C28C4A160] django ++++ 
+[7F4C289BD5D0] EXEC LOAD [7F4C28C4A160] django ++++  # This is where a lazy module is fully loaded. 
 (4, 2, 1, 'final', 0)
 >>> exit()
 [7F4C289BF830] LAZY DEAD [7F4C289BF380] copy
 [7F4C289BE4D0] LOAD DEAD [7F4C289BE3E0] django.utils|functional
 [7F4C289BE0C0] LOAD DEAD [7F4C289BDFD0] django.utils|regex_helper
 [7F4C289BE020] LAZY DEAD [7F4C289BE070] subprocess
 [7F4C289BDF30] LAZY DEAD [7F4C289BDF80] datetime
@@ -176,15 +176,16 @@
 lazi.core.loader.Loader.Error: [7F899C139260] EXEC DEAD [7F899C1382C0] pandas.core|nanops !!!! OptionError
 >>> _
 ```
 
 _Unforunately_... This isn't something that can be worked around without outer dependency tracking, which
 generally results in entire packages getting loaded anyway.
 
-If you're more interested in just tracking imports with Lazi, use the `NO_HOOK` config variable (see below).
+If you're more interested in just tracking imports with Lazi, use the `NO_HOOK`
+or `NO_LAZY` config variables (see below and [lazi/conf/base.py](lazi/conf/base.py)).
 
 ## Configuration
 
 The `lazi.conf` namespace package contains configuration modules
 that get autoloaded (in import order) by `lazi.conf.conf`.
 It is fully decoupled from the rest of the codebase.
```

### Comparing `lazi-1.9.159/tests/standalone/sa_nested.py` & `lazi-1.9.161/tests/standalone/sa_nested.py`

 * *Files identical despite different names*

### Comparing `lazi-1.9.159/tests/test_array.py` & `lazi-1.9.161/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `lazi-1.9.159/tests/test_django.py` & `lazi-1.9.161/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `lazi-1.9.159/tests/test_importlib.py` & `lazi-1.9.161/tests/test_importlib.py`

 * *Files identical despite different names*

### Comparing `lazi-1.9.159/tests/test_requests.py` & `lazi-1.9.161/tests/test_requests.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+import pytest
 
 
 def test_requests_parse_dict_header():
     from lazi.util import debug
     from lazi.core.finder import Finder
 
     with Finder() as finder:
         debug.trace("-> from requests.utils import parse_dict_header ->")
         from requests.utils import parse_dict_header
         debug.trace("^- from requests.utils import parse_dict_header -^")
 
     finder.invalidate_caches()
 
 
+@pytest.mark.skip(reason="Not using presto to remove Python 3.11 dependency.")
 def test_requests_presto_import():
     from lazi.util import debug
     from lazi.core.finder import Finder
 
     with Finder() as finder:
         debug.trace("-> from presto import Presto ->")
         from presto import Presto
```

### Comparing `lazi-1.9.159/tests/test_rich.py` & `lazi-1.9.161/tests/test_rich.py`

 * *Files identical despite different names*

### Comparing `lazi-1.9.159/tests/test_stat.py` & `lazi-1.9.161/tests/test_stat.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         with track("TestCase = dt.TestCase"):
             TestCase = dt.TestCase
             info(Stat())
 
     lazi.invalidate_caches()
 
 
-# @pytest.mark.skip(reason="not working")
+@pytest.mark.skip(reason="Not using presto to remove Python 3.11 dependency.")
 def test_stat_presto():
     from lazi.util.debug import track, info
 
     from lazi.core.stat import Stat
     from lazi.core import lazi
 
     with lazi:
@@ -37,14 +37,15 @@
         with track("p = presto.Presto('https://httpbin.org')"):
             p = presto.Presto("https://httpbin.org")
             info(Stat())
 
     lazi.invalidate_caches()
 
 
+@pytest.mark.skip(reason="Not using presto to remove Python 3.11 dependency.")
 def test_stat_nolazi_presto():
     from lazi.util.debug import track, info
 
     from lazi.core.stat import Stat
 
     with track("import presto"):
         info(Stat())
```

### Comparing `lazi-1.9.159/PKG-INFO` & `lazi-1.9.161/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: lazi
-Version: 1.9.159
+Version: 1.9.161
 Summary: A lightweight and extensible way to implement lazy imports globally.
 Home-page: https://github.com/sitbon/lazi
 License: AGPLv3
 Author: Phillip Sitbon
 Author-email: phillip.sitbon@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Project-URL: Repository, https://github.com/sitbon/lazi
 Description-Content-Type: text/markdown
 
 # Lazi: Lazy Imports Everywhere
 
 An easy way to implement and track lazy imports globally.
 
 No external dependencies.
 
-**Requres Python 3.11.**
+**Requires Python >= 3.10, and 3.11 is HIGHLY Recommended.**
 
 ## Usage:
 
 ```shell
 poetry add lazi
 ```
 ```shell
@@ -54,25 +54,25 @@
 And with `TRACE=3`:
 
 ```pycon
 >>> import lazi.auto
 [7F4C28B37350] HOOK Finder refs:0 inst:0 sys:5 
 >>> import django
 [7F4C28B37350] FIND pyc  django *
-[7F4C289BD5D0] CREA LAZY [7F4C28C4A160] django ....  # This is where the lazy module is set up.
+[7F4C289BD5D0] CREA LAZY [7F4C28C4A160] django ....  # This is where the a module is set up.
 >>> django.VERSION
 [7F4C289BD5D0] LAZY >>>> [7F4C28C4A160] django VERSION
 [7F4C289BD5D0] LAZY EXEC [7F4C28C4A160] django >>>> 
 [7F4C28B37350] FIND pyc  django.utils 
 [7F4C289BD080] CREA LAZY [7F4C289BD0D0] django.utils .... 
 [7F4C28B37350] FIND pyc  django.utils|version 
 [7F4C289BD800] CREA LAZY [7F4C289BD490] django.utils|version .... 
 [7F4C289BD080] LAZY >>>> [7F4C289BD0D0] django.utils version = [7F4C289BD800]
 [7F4C289BD080] LAZY EXEC [7F4C289BD0D0] django.utils >>>> 
-[7F4C289BD080] EXEC LOAD [7F4C289BD0D0] django.utils ++++  # This is where the lazy module is fully loaded. 
+[7F4C289BD080] EXEC LOAD [7F4C289BD0D0] django.utils ++++ 
 [7F4C289BD800] LAZY >>>> [7F4C289BD490] django.utils|version get_version
 [7F4C289BD800] LAZY EXEC [7F4C289BD490] django.utils|version >>>> 
 [7F4C28B37350] FIND pycS datetime *  # "S" means it's a stdlib module. "B" means it's a builtin module.
 [7F4C289BDF30] CREA LAZY [7F4C289BDF80] datetime .... 
 [7F4C28B37350] FIND pycS subprocess *
 [7F4C289BE020] CREA LAZY [7F4C289BE070] subprocess .... 
 [7F4C28B37350] FIND pyc  django.utils|regex_helper 
@@ -84,15 +84,15 @@
 [7F4C289BE4D0] LAZY >>>> [7F4C289BE3E0] django.utils|functional SimpleLazyObject
 [7F4C289BE4D0] LAZY EXEC [7F4C289BE3E0] django.utils|functional >>>> 
 [7F4C28B37350] FIND pycS copy *
 [7F4C289BF830] CREA LAZY [7F4C289BF380] copy .... 
 [7F4C289BE4D0] EXEC LOAD [7F4C289BE3E0] django.utils|functional ++++ 
 [7F4C289BE0C0] EXEC LOAD [7F4C289BDFD0] django.utils|regex_helper ++++ 
 [7F4C289BD800] EXEC LOAD [7F4C289BD490] django.utils|version ++++ 
-[7F4C289BD5D0] EXEC LOAD [7F4C28C4A160] django ++++ 
+[7F4C289BD5D0] EXEC LOAD [7F4C28C4A160] django ++++  # This is where a lazy module is fully loaded. 
 (4, 2, 1, 'final', 0)
 >>> exit()
 [7F4C289BF830] LAZY DEAD [7F4C289BF380] copy
 [7F4C289BE4D0] LOAD DEAD [7F4C289BE3E0] django.utils|functional
 [7F4C289BE0C0] LOAD DEAD [7F4C289BDFD0] django.utils|regex_helper
 [7F4C289BE020] LAZY DEAD [7F4C289BE070] subprocess
 [7F4C289BDF30] LAZY DEAD [7F4C289BDF80] datetime
@@ -200,15 +200,16 @@
 lazi.core.loader.Loader.Error: [7F899C139260] EXEC DEAD [7F899C1382C0] pandas.core|nanops !!!! OptionError
 >>> _
 ```
 
 _Unforunately_... This isn't something that can be worked around without outer dependency tracking, which
 generally results in entire packages getting loaded anyway.
 
-If you're more interested in just tracking imports with Lazi, use the `NO_HOOK` config variable (see below).
+If you're more interested in just tracking imports with Lazi, use the `NO_HOOK`
+or `NO_LAZY` config variables (see below and [lazi/conf/base.py](lazi/conf/base.py)).
 
 ## Configuration
 
 The `lazi.conf` namespace package contains configuration modules
 that get autoloaded (in import order) by `lazi.conf.conf`.
 It is fully decoupled from the rest of the codebase.
```

