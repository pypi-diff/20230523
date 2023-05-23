# Comparing `tmp/bmsdna_lakeapi-0.2.3.tar.gz` & `tmp/bmsdna_lakeapi-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.2.3.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.2.4.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.2.3.tar` & `bmsdna_lakeapi-0.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1081 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/LICENSE
--rw-r--r--   0        0        0     4722 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/README.md
--rw-r--r--   0        0        0      166 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1135 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      926 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     5349 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0     3699 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/context/df_datafusion.py
--rw-r--r--   0        0        0     8721 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6281 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    12190 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    12625 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0    15707 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6566 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     7822 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     3601 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     1692 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2361 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1847 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      326 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1784 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1095 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     1842 2023-05-22 07:39:19.648234 bmsdna_lakeapi-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     6016 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-22 08:17:54.917119 bmsdna_lakeapi-0.2.4/LICENSE
+-rw-r--r--   0        0        0     4722 2023-05-22 08:17:54.917119 bmsdna_lakeapi-0.2.4/README.md
+-rw-r--r--   0        0        0      166 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1135 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      926 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     5349 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0     3699 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/context/df_datafusion.py
+-rw-r--r--   0        0        0     8721 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6281 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    12248 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    12625 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0    15770 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6566 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     7822 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     3601 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     1692 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2361 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1847 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      326 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1784 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1095 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     1842 2023-05-22 08:17:54.921119 bmsdna_lakeapi-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     6016 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.2.4/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.2.3/LICENSE` & `bmsdna_lakeapi-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.3/README.md` & `bmsdna_lakeapi-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/context/df_base.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/context/df_datafusion.py` & `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/context/df_datafusion.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/context/df_polars.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,25 +33,27 @@
 @dataclass(frozen=True)
 class BasicConfig:
     username_retriever: Callable[[Request, "BasicConfig", "Sequence[UserConfig]"], str | Awaitable[str]]
     enable_sql_endpoint: bool
     temp_folder_path: str
     data_path: str
     token_jwt_secret: str | None  # None disables the token feature
+    min_search_length: int
 
 
 def get_default_config():
     from bmsdna.lakeapi.core.uservalidation import get_username
 
     return BasicConfig(
         username_retriever=get_username,
         enable_sql_endpoint=os.getenv("ENABLE_SQL_ENDPOINT", "0") == "1",
         temp_folder_path=os.getenv("TEMP", "/tmp"),
         data_path=os.environ.get("DATA_PATH", "data"),
         token_jwt_secret=os.getenv("JWT_SECRET", None),
+        min_search_length=3,
     )
 
 
 @dataclass
 class Param:
     name: str
     combi: Optional[Optional[List[str]]] = None
```

### Comparing `bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,15 +280,15 @@
                 new_query = new_query.offset(offset or 0).limit(limit)
 
             if config.search is not None and params is not None:
                 search_dict = {c.name.lower(): c for c in config.search}
                 searches = {
                     k: (v, search_dict[k.lower()])
                     for k, v in params.dict(exclude_unset=True).items()
-                    if k.lower() in search_dict
+                    if k.lower() in search_dict and v is not None and len(v) >= basic_config.min_search_length
                 }
                 if len(searches) > 0:
                     import pypika.queries
                     import pypika.terms
 
                     source_view = realdataframe.tablename
                     context.init_search(source_view, config.search)
```

### Comparing `bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/route.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.3/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.2.4/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.3/pyproject.toml` & `bmsdna_lakeapi-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.2.3/PKG-INFO` & `bmsdna_lakeapi-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

