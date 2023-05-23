# Comparing `tmp/pydeflate-1.3.5.tar.gz` & `tmp/pydeflate-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeflate-1.3.5.tar", max compression
+gzip compressed data, was "pydeflate-1.3.6.tar", max compression
```

## Comparing `pydeflate-1.3.5.tar` & `pydeflate-1.3.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1070 2023-04-13 15:58:40.696639 pydeflate-1.3.5/LICENSE
--rw-r--r--   0        0        0     8999 2023-04-13 15:58:40.696639 pydeflate-1.3.5/README.md
--rw-r--r--   0        0        0       25 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/.pydeflate_data/README.md
--rw-r--r--   0        0        0      775 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/deflate/__init__.py
--rw-r--r--   0        0        0    11829 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/deflate/deflate.py
--rw-r--r--   0        0        0     2684 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/deflate/deflator.py
--rw-r--r--   0        0        0        0 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/get_data/__init__.py
--rw-r--r--   0        0        0     2285 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/get_data/deflate_data.py
--rw-r--r--   0        0        0    12091 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/get_data/exchange_data.py
--rw-r--r--   0        0        0     2693 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/get_data/imf_data.py
--rw-r--r--   0        0        0     6177 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/get_data/oecd_data.py
--rw-r--r--   0        0        0     2103 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/get_data/wb_data.py
--rw-r--r--   0        0        0      894 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/pydeflate_config.py
--rw-r--r--   0        0        0      133 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/settings/emu.json
--rw-r--r--   0        0        0      911 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/settings/oecd_codes.json
--rw-r--r--   0        0        0       47 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/tools/__init__.py
--rw-r--r--   0        0        0     5465 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/tools/exchange.py
--rw-r--r--   0        0        0     2110 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/tools/update_data.py
--rw-r--r--   0        0        0     1573 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/utils.py
--rw-r--r--   0        0        0     1059 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pyproject.toml
--rw-r--r--   0        0        0    10147 1970-01-01 00:00:00.000000 pydeflate-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-23 15:39:27.024478 pydeflate-1.3.6/LICENSE
+-rw-r--r--   0        0        0     8999 2023-05-23 15:39:27.024478 pydeflate-1.3.6/README.md
+-rw-r--r--   0        0        0       25 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/.pydeflate_data/README.md
+-rw-r--r--   0        0        0      775 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/deflate/__init__.py
+-rw-r--r--   0        0        0    11850 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/deflate/deflate.py
+-rw-r--r--   0        0        0     2684 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/deflate/deflator.py
+-rw-r--r--   0        0        0        0 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/get_data/__init__.py
+-rw-r--r--   0        0        0     2285 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/get_data/deflate_data.py
+-rw-r--r--   0        0        0    12091 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/get_data/exchange_data.py
+-rw-r--r--   0        0        0     2693 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/get_data/imf_data.py
+-rw-r--r--   0        0        0     6177 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/get_data/oecd_data.py
+-rw-r--r--   0        0        0     2103 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/get_data/wb_data.py
+-rw-r--r--   0        0        0      894 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/pydeflate_config.py
+-rw-r--r--   0        0        0      133 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/settings/emu.json
+-rw-r--r--   0        0        0      911 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/settings/oecd_codes.json
+-rw-r--r--   0        0        0       47 2023-05-23 15:39:27.028478 pydeflate-1.3.6/pydeflate/tools/__init__.py
+-rw-r--r--   0        0        0     5465 2023-05-23 15:39:27.028478 pydeflate-1.3.6/pydeflate/tools/exchange.py
+-rw-r--r--   0        0        0     2110 2023-05-23 15:39:27.028478 pydeflate-1.3.6/pydeflate/tools/update_data.py
+-rw-r--r--   0        0        0     1573 2023-05-23 15:39:27.028478 pydeflate-1.3.6/pydeflate/utils.py
+-rw-r--r--   0        0        0     1059 2023-05-23 15:39:27.028478 pydeflate-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0    10048 1970-01-01 00:00:00.000000 pydeflate-1.3.6/PKG-INFO
```

### Comparing `pydeflate-1.3.5/LICENSE` & `pydeflate-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.5/README.md` & `pydeflate-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.5/pydeflate/__init__.py` & `pydeflate-1.3.6/pydeflate/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = """Jorge Rivera"""
-__version__ = "1.3.5"
+__version__ = "1.3.6"
 
 from pydeflate.deflate.deflate import deflate
 from pydeflate.tools.exchange import exchange
 from pydeflate.tools.update_data import update_all_data, warn_updates
 from pydeflate.get_data.oecd_data import update_dac1
 from pydeflate import get_data
```

### Comparing `pydeflate-1.3.5/pydeflate/deflate/deflate.py` & `pydeflate-1.3.6/pydeflate/deflate/deflate.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
             deflator_obj=DeflatorSources[deflator_source](),
             deflator_method=deflator_method,
             source_currency=source_currency,
             target_currency=target_currency,
             to_current=to_current,
         )
         .get_deflator()
-        .rename(columns={"iso_code": "id_"})
+        .rename(columns={"iso_code": "id_", "year": date_column})
     )
 
     # ----------------------------- Deflate ---------------------------
     # Merge the original data with the deflator DataFrame
     df = df.merge(
         deflator,
         on=["id_", date_column],
```

### Comparing `pydeflate-1.3.5/pydeflate/deflate/deflator.py` & `pydeflate-1.3.6/pydeflate/deflate/deflator.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.5/pydeflate/get_data/deflate_data.py` & `pydeflate-1.3.6/pydeflate/get_data/deflate_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.5/pydeflate/get_data/exchange_data.py` & `pydeflate-1.3.6/pydeflate/get_data/exchange_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.5/pydeflate/get_data/imf_data.py` & `pydeflate-1.3.6/pydeflate/get_data/imf_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.5/pydeflate/get_data/oecd_data.py` & `pydeflate-1.3.6/pydeflate/get_data/oecd_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.5/pydeflate/get_data/wb_data.py` & `pydeflate-1.3.6/pydeflate/get_data/wb_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.5/pydeflate/pydeflate_config.py` & `pydeflate-1.3.6/pydeflate/pydeflate_config.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.5/pydeflate/settings/oecd_codes.json` & `pydeflate-1.3.6/pydeflate/settings/oecd_codes.json`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.5/pydeflate/tools/exchange.py` & `pydeflate-1.3.6/pydeflate/tools/exchange.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.5/pydeflate/tools/update_data.py` & `pydeflate-1.3.6/pydeflate/tools/update_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.5/pydeflate/utils.py` & `pydeflate-1.3.6/pydeflate/utils.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.5/pyproject.toml` & `pydeflate-1.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydeflate"
-version = "1.3.5"
+version = "1.3.6"
 description = "Package to convert current prices figures to constant prices and vice versa"
 authors = ["Jorge Rivera <jorge.rivera@one.org>"]
 license = "MIT"
 readme = "README.md"
 classifiers=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: End Users/Desktop',
```

### Comparing `pydeflate-1.3.5/PKG-INFO` & `pydeflate-1.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: pydeflate
-Version: 1.3.5
+Version: 1.3.6
 Summary: Package to convert current prices figures to constant prices and vice versa
 License: MIT
 Author: Jorge Rivera
 Author-email: jorge.rivera@one.org
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: bblocks (>=1.0.2,<2.0.0)
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
 Requires-Dist: country-converter (>=0.8.0,<0.9.0)
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
```

