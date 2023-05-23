# Comparing `tmp/okama-1.3.0.tar.gz` & `tmp/okama-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okama-1.3.0.tar", max compression
+gzip compressed data, was "okama-1.3.1.tar", max compression
```

## Comparing `okama-1.3.0.tar` & `okama-1.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1058 2021-06-16 07:17:39.219198 okama-1.3.0/LICENSE.txt
--rw-r--r--   0        0        0     2157 2023-05-19 15:03:56.216688 okama-1.3.0/okama/__init__.py
--rw-r--r--   0        0        0        0 2021-06-16 07:17:39.317201 okama-1.3.0/okama/api/__init__.py
--rw-r--r--   0        0        0     6130 2022-07-29 14:30:04.739588 okama-1.3.0/okama/api/api_methods.py
--rw-r--r--   0        0        0     4083 2022-06-04 17:56:18.764145 okama-1.3.0/okama/api/data_queries.py
--rw-r--r--   0        0        0     1409 2023-05-19 11:53:16.721825 okama-1.3.0/okama/api/namespaces.py
--rw-r--r--   0        0        0     1384 2022-06-04 17:56:18.770175 okama-1.3.0/okama/api/search.py
--rw-r--r--   0        0        0     5944 2023-05-19 11:53:16.724825 okama-1.3.0/okama/asset.py
--rw-r--r--   0        0        0    57439 2023-05-19 11:53:16.727824 okama-1.3.0/okama/asset_list.py
--rw-r--r--   0        0        0        0 2021-06-16 07:17:39.333202 okama-1.3.0/okama/common/__init__.py
--rw-r--r--   0        0        0        0 2021-10-12 14:31:44.977602 okama-1.3.0/okama/common/helpers/__init__.py
--rw-r--r--   0        0        0    23790 2023-05-19 11:53:16.732824 okama-1.3.0/okama/common/helpers/helpers.py
--rw-r--r--   0        0        0      555 2022-01-30 15:06:03.393518 okama-1.3.0/okama/common/helpers/ratios.py
--rw-r--r--   0        0        0    22059 2023-05-19 11:53:16.735825 okama-1.3.0/okama/common/make_asset_list.py
--rw-r--r--   0        0        0     2857 2022-04-21 06:30:03.465033 okama-1.3.0/okama/common/validators.py
--rw-r--r--   0        0        0        0 2021-06-16 07:17:39.341199 okama-1.3.0/okama/frontier/__init__.py
--rw-r--r--   0        0        0    32120 2023-05-19 11:53:16.741829 okama-1.3.0/okama/frontier/multi_period.py
--rw-r--r--   0        0        0    46553 2023-05-19 15:03:02.297773 okama-1.3.0/okama/frontier/single_period.py
--rw-r--r--   0        0        0    19003 2022-06-05 13:19:20.083275 okama-1.3.0/okama/macro.py
--rw-r--r--   0        0        0    80308 2023-05-19 11:53:16.747828 okama-1.3.0/okama/portfolio.py
--rw-r--r--   0        0        0      387 2022-06-04 17:56:18.803142 okama-1.3.0/okama/settings.py
--rw-r--r--   0        0        0     1907 2023-05-19 11:53:16.750828 okama-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     7783 2023-05-19 14:52:52.231034 okama-1.3.0/README.md
--rw-r--r--   0        0        0     9444 1970-01-01 00:00:00.000000 okama-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1058 2021-06-16 07:17:39.219198 okama-1.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     2317 2023-05-23 07:34:37.592850 okama-1.3.1/okama/__init__.py
+-rw-r--r--   0        0        0        0 2021-06-16 07:17:39.317201 okama-1.3.1/okama/api/__init__.py
+-rw-r--r--   0        0        0     6130 2022-07-29 14:30:04.739588 okama-1.3.1/okama/api/api_methods.py
+-rw-r--r--   0        0        0     4083 2022-06-04 17:56:18.764145 okama-1.3.1/okama/api/data_queries.py
+-rw-r--r--   0        0        0     1409 2023-05-19 11:53:16.721825 okama-1.3.1/okama/api/namespaces.py
+-rw-r--r--   0        0        0     1384 2022-06-04 17:56:18.770175 okama-1.3.1/okama/api/search.py
+-rw-r--r--   0        0        0     5944 2023-05-19 11:53:16.724825 okama-1.3.1/okama/asset.py
+-rw-r--r--   0        0        0    57439 2023-05-19 11:53:16.727824 okama-1.3.1/okama/asset_list.py
+-rw-r--r--   0        0        0        0 2021-06-16 07:17:39.333202 okama-1.3.1/okama/common/__init__.py
+-rw-r--r--   0        0        0        0 2021-10-12 14:31:44.977602 okama-1.3.1/okama/common/helpers/__init__.py
+-rw-r--r--   0        0        0    23790 2023-05-19 11:53:16.732824 okama-1.3.1/okama/common/helpers/helpers.py
+-rw-r--r--   0        0        0      555 2022-01-30 15:06:03.393518 okama-1.3.1/okama/common/helpers/ratios.py
+-rw-r--r--   0        0        0    22059 2023-05-19 11:53:16.735825 okama-1.3.1/okama/common/make_asset_list.py
+-rw-r--r--   0        0        0     2857 2022-04-21 06:30:03.465033 okama-1.3.1/okama/common/validators.py
+-rw-r--r--   0        0        0        0 2021-06-16 07:17:39.341199 okama-1.3.1/okama/frontier/__init__.py
+-rw-r--r--   0        0        0    32120 2023-05-19 11:53:16.741829 okama-1.3.1/okama/frontier/multi_period.py
+-rw-r--r--   0        0        0    46553 2023-05-19 15:26:38.976415 okama-1.3.1/okama/frontier/single_period.py
+-rw-r--r--   0        0        0    19003 2022-06-05 13:19:20.083275 okama-1.3.1/okama/macro.py
+-rw-r--r--   0        0        0    80308 2023-05-19 11:53:16.747828 okama-1.3.1/okama/portfolio.py
+-rw-r--r--   0        0        0      387 2022-06-04 17:56:18.803142 okama-1.3.1/okama/settings.py
+-rw-r--r--   0        0        0     2048 2023-05-23 07:34:37.597916 okama-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7783 2023-05-19 15:26:38.957417 okama-1.3.1/README.md
+-rw-r--r--   0        0        0     9257 1970-01-01 00:00:00.000000 okama-1.3.1/PKG-INFO
```

### Comparing `okama-1.3.0/LICENSE.txt` & `okama-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `okama-1.3.0/okama/__init__.py` & `okama-1.3.1/okama/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,22 +27,25 @@
 from okama.macro import Inflation, Rate, Indicator
 from okama.frontier.multi_period import EfficientFrontierReb
 from okama.frontier.single_period import EfficientFrontier
 from okama.api.data_queries import QueryData
 from okama.api.search import search
 from okama.api.api_methods import API
 import okama.api.namespaces
+from okama.api.namespaces import symbols_in_namespace
 from okama.common.helpers.helpers import Float, Frame, Rebalance, Date
 import okama.settings
 
 
 def __getattr__(name):
     if name == "namespaces":
         return okama.api.namespaces.get_namespaces()
     elif name == "assets_namespaces":
         return okama.api.namespaces.get_assets_namespaces()
     elif name == "macro_namespaces":
         return okama.api.namespaces.get_macro_namespaces()
+    elif name == "no_dividends_namespaces":
+        return okama.api.namespaces.no_dividends_namespaces()
     raise AttributeError(f"module '{__name__}' has no attribute '{name}'")
 
 
 __version__ = version("okama")
```

### Comparing `okama-1.3.0/okama/api/api_methods.py` & `okama-1.3.1/okama/api/api_methods.py`

 * *Files identical despite different names*

### Comparing `okama-1.3.0/okama/api/data_queries.py` & `okama-1.3.1/okama/api/data_queries.py`

 * *Files identical despite different names*

### Comparing `okama-1.3.0/okama/api/namespaces.py` & `okama-1.3.1/okama/api/namespaces.py`

 * *Files identical despite different names*

### Comparing `okama-1.3.0/okama/api/search.py` & `okama-1.3.1/okama/api/search.py`

 * *Files identical despite different names*

### Comparing `okama-1.3.0/okama/asset.py` & `okama-1.3.1/okama/asset.py`

 * *Files identical despite different names*

### Comparing `okama-1.3.0/okama/asset_list.py` & `okama-1.3.1/okama/asset_list.py`

 * *Files identical despite different names*

### Comparing `okama-1.3.0/okama/common/helpers/helpers.py` & `okama-1.3.1/okama/common/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `okama-1.3.0/okama/common/helpers/ratios.py` & `okama-1.3.1/okama/common/helpers/ratios.py`

 * *Files identical despite different names*

### Comparing `okama-1.3.0/okama/common/make_asset_list.py` & `okama-1.3.1/okama/common/make_asset_list.py`

 * *Files identical despite different names*

### Comparing `okama-1.3.0/okama/common/validators.py` & `okama-1.3.1/okama/common/validators.py`

 * *Files identical despite different names*

### Comparing `okama-1.3.0/okama/frontier/multi_period.py` & `okama-1.3.1/okama/frontier/multi_period.py`

 * *Files identical despite different names*

### Comparing `okama-1.3.0/okama/frontier/single_period.py` & `okama-1.3.1/okama/frontier/single_period.py`

 * *Files identical despite different names*

### Comparing `okama-1.3.0/okama/macro.py` & `okama-1.3.1/okama/macro.py`

 * *Files identical despite different names*

### Comparing `okama-1.3.0/okama/portfolio.py` & `okama-1.3.1/okama/portfolio.py`

 * *Files identical despite different names*

### Comparing `okama-1.3.0/pyproject.toml` & `okama-1.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "okama"
-version = "1.3.0"
+version = "1.3.1"
 description = "Investment portfolio analyzing & optimization tools"
 authors = ["Sergey Kikevich <chilango74@gmail.com>"]
 license = "MIT"
 homepage = "https://okama.io"
 repository = "https://github.com/mbk-dev/okama"
 documentation = "https://okama.readthedocs.io/en/master"
 readme = "README.md"
@@ -17,26 +17,30 @@
     "Intended Audience :: Science/Research",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <4.0.0"
 pandas = ">=1.4.0, <=1.6.0"
 scipy = "^1.9.0"
 matplotlib = "^3.5.1"
-requests = "^2.27.1"
+requests = "<=2.31.0"   # Windows has an issue with 2.32.0
 joblib = "^1.1.0"
-pillow = "<=9.1.0"  # delete after issue with installing 9.2.0 is resolved
+
+[tool.poetry.group.test]
+optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^6.0.0"
 black = "^22.3.0"
 
 [tool.poetry.group.docs]
 optional = true
@@ -47,20 +51,22 @@
 numpydoc = "^1.2.1"
 nbsphinx = "^0.8.8"
 nbsphinx-link = "^1.3.0"
 pandoc = "^2.2"
 recommonmark = "^0.7.1"
 Jinja2 = "3.0.3"
 
+[tool.poetry.group.jupyter]
+optional = true
+
 [tool.poetry.group.jupyter.dependencies]
 jupyter = "^1.0.0"
 ipykernel = "^6.15.0"
 ipython = "^8.0.0"
 nbmake = "^1.2"  # test jupyter notebooks
 
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `okama-1.3.0/README.md` & `okama-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `okama-1.3.0/PKG-INFO` & `okama-1.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okama
-Version: 1.3.0
+Version: 1.3.1
 Summary: Investment portfolio analyzing & optimization tools
 Home-page: https://okama.io
 License: MIT
 Keywords: finance,investments,efficient frontier,python,optimization
 Author: Sergey Kikevich
 Author-email: chilango74@gmail.com
 Requires-Python: >=3.8,<4.0.0
@@ -16,25 +16,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: joblib (>=1.1.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
 Requires-Dist: pandas (>=1.4.0,<=1.6.0)
-Requires-Dist: pillow (<=9.1.0)
-Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: requests (<=2.31.0)
 Requires-Dist: scipy (>=1.9.0,<2.0.0)
 Project-URL: Documentation, https://okama.readthedocs.io/en/master
 Project-URL: Repository, https://github.com/mbk-dev/okama
 Description-Content-Type: text/markdown
 
 
 [![Documentation Status](https://img.shields.io/readthedocs/okama.svg?style=popout)](http://okama.readthedocs.io/)
```

