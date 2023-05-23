# Comparing `tmp/bmsdna_lakeapi-0.2.4.tar.gz` & `tmp/bmsdna_lakeapi-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.2.4.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.2.5.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.2.4.tar` & `bmsdna_lakeapi-0.2.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1081 2023-05-22 08:17:54.917119 bmsdna_lakeapi-0.2.4/LICENSE
--rw-r--r--   0        0        0     4722 2023-05-22 08:17:54.917119 bmsdna_lakeapi-0.2.4/README.md
--rw-r--r--   0        0        0      166 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1135 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      926 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     5349 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0     3699 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/context/df_datafusion.py
--rw-r--r--   0        0        0     8721 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6281 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    12248 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    12625 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0    15770 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6566 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     7822 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     3601 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     1692 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2361 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1847 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      326 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1784 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1095 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     1842 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     6016 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/LICENSE
+-rw-r--r--   0        0        0     4722 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/README.md
+-rw-r--r--   0        0        0      166 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1135 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      926 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     5349 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0     3699 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/context/df_datafusion.py
+-rw-r--r--   0        0        0     8721 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6281 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    12641 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    12625 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0    15770 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6566 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     7822 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     3601 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     1692 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2361 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1847 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      326 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1784 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1095 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     1842 2023-05-23 06:39:54.689208 bmsdna_lakeapi-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     6016 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.2.5/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.2.4/LICENSE` & `bmsdna_lakeapi-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.4/README.md` & `bmsdna_lakeapi-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/context/df_base.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/context/df_datafusion.py` & `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/context/df_datafusion.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/context/df_polars.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from dataclasses import dataclass, field
 from datetime import datetime
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
+    Iterable,
     List,
     Literal,
     Optional,
     Sequence,
     Tuple,
     TypedDict,
     Union,
@@ -181,15 +182,15 @@
         return "{}({})".format(type(self).__name__, ", ".join(kws))
 
     def __str__(self) -> str:
         kws = [f"{key}={value!r}" for key, value in self.__dict__.items()]
         return "{}({})".format(type(self).__name__, ", ".join(kws))
 
     @classmethod
-    def from_dict(cls, config: Dict, basic_config: BasicConfig) -> List["Config"]:
+    def from_dict(cls, config: Dict, basic_config: BasicConfig, table_names: List[tuple[int, str, str]]) -> List["Config"]:
         name = config["name"]
         tag = config["tag"]
         version = config.get("version", 1)
         engine = config.get("engine", "duckdb")
         api_method = cast(Literal["post", "get"], config.get("api_method", "get"))
         params = config.get("params")
         dataframe = config["dataframe"]
@@ -243,15 +244,18 @@
             root_folder = os.path.join(basic_config.data_path, folder)
             if not os.path.exists(root_folder):
                 logger.warning("Path not existing: " + root_folder)
                 return []
             else:
                 ls = []
                 for it in os.scandir(root_folder):
-                    if it.is_dir():
+                    res_name = (version, tag, it.name)
+                    if res_name not in table_names and (
+                        (it.is_dir() and file_type == "delta") or (it.is_file() and file_type != "delta")
+                    ):
                         dataframe = DataframeConfig(
                             uri=folder + "/" + it.name,
                             file_type=file_type,
                             select=select,
                             exclude=exclude,
                             groupby=groupby,
                             sortby=sortby,
@@ -375,9 +379,10 @@
                     if yaml_data_tables:
                         tables += [y for y in yaml_data_tables if y.get("name")]
                     yaml_data_users = y.get("users")
                     if yaml_data_users:
                         users += yaml_data_users
 
         flat_map = lambda f, xs: [y for ys in xs for y in f(ys)]
-        configs = flat_map(lambda x: Config.from_dict(x, basic_config=basic_config), tables)
+        table_names = [(t.get("version", 1), t["tag"], t["name"]) for t in tables if t["name"] != "*"]
+        configs = flat_map(lambda x: Config.from_dict(x, basic_config=basic_config, table_names=table_names), tables)
         return cls(configs, users)
```

### Comparing `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/route.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.4/pyproject.toml` & `bmsdna_lakeapi-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.2.4"
+version = "0.2.5"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.2.4/PKG-INFO` & `bmsdna_lakeapi-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

