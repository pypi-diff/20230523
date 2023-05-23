# Comparing `tmp/dtflw-0.6.3.tar.gz` & `tmp/dtflw-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtflw-0.6.3.tar", last modified: Wed Apr 12 17:47:57 2023, max compression
+gzip compressed data, was "dtflw-0.6.4.tar", last modified: Tue May 23 08:16:50 2023, max compression
```

## Comparing `dtflw-0.6.3.tar` & `dtflw-0.6.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:47:57.637840 dtflw-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-12 17:47:47.000000 dtflw-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-12 17:47:57.637840 dtflw-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-04-12 17:47:47.000000 dtflw-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-12 17:47:47.000000 dtflw-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 17:47:57.641840 dtflw-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-12 17:47:47.000000 dtflw-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:47:57.633840 dtflw-0.6.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:47:57.637840 dtflw-0.6.3/src/dtflw/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/com.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/databricks.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/flow_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/input_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/lazy_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/output_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:47:57.637840 dtflw-0.6.3/src/dtflw/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/storage/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/storage/dbfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/storage/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/tables_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:47:57.637840 dtflw-0.6.3/src/dtflw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-12 17:47:57.000000 dtflw-0.6.3/src/dtflw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-12 17:47:57.000000 dtflw-0.6.3/src/dtflw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:47:57.000000 dtflw-0.6.3/src/dtflw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 17:47:57.000000 dtflw-0.6.3/src/dtflw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 17:47:57.000000 dtflw-0.6.3/src/dtflw.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:47:57.637840 dtflw-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_com.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_databricks.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_input_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_lazy_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_output_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_pipeline_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_tables_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:16:50.327579 dtflw-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-23 08:16:35.000000 dtflw-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-23 08:16:50.327579 dtflw-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-05-23 08:16:35.000000 dtflw-0.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-23 08:16:35.000000 dtflw-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-23 08:16:50.331579 dtflw-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-23 08:16:35.000000 dtflw-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:16:50.311579 dtflw-0.6.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:16:50.323579 dtflw-0.6.4/src/dtflw/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-23 08:16:35.000000 dtflw-0.6.4/src/dtflw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-23 08:16:35.000000 dtflw-0.6.4/src/dtflw/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-23 08:16:35.000000 dtflw-0.6.4/src/dtflw/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-23 08:16:35.000000 dtflw-0.6.4/src/dtflw/com.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-23 08:16:35.000000 dtflw-0.6.4/src/dtflw/databricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-23 08:16:35.000000 dtflw-0.6.4/src/dtflw/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-23 08:16:35.000000 dtflw-0.6.4/src/dtflw/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-23 08:16:35.000000 dtflw-0.6.4/src/dtflw/flow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-23 08:16:35.000000 dtflw-0.6.4/src/dtflw/input_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-05-23 08:16:35.000000 dtflw-0.6.4/src/dtflw/lazy_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-23 08:16:35.000000 dtflw-0.6.4/src/dtflw/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-23 08:16:35.000000 dtflw-0.6.4/src/dtflw/output_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-23 08:16:35.000000 dtflw-0.6.4/src/dtflw/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-23 08:16:35.000000 dtflw-0.6.4/src/dtflw/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:16:50.327579 dtflw-0.6.4/src/dtflw/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 08:16:35.000000 dtflw-0.6.4/src/dtflw/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-23 08:16:35.000000 dtflw-0.6.4/src/dtflw/storage/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-23 08:16:35.000000 dtflw-0.6.4/src/dtflw/storage/dbfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-05-23 08:16:35.000000 dtflw-0.6.4/src/dtflw/storage/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-23 08:16:35.000000 dtflw-0.6.4/src/dtflw/tables_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:16:50.323579 dtflw-0.6.4/src/dtflw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-23 08:16:50.000000 dtflw-0.6.4/src/dtflw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-23 08:16:50.000000 dtflw-0.6.4/src/dtflw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:16:50.000000 dtflw-0.6.4/src/dtflw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 08:16:50.000000 dtflw-0.6.4/src/dtflw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 08:16:50.000000 dtflw-0.6.4/src/dtflw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:16:50.327579 dtflw-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-23 08:16:35.000000 dtflw-0.6.4/tests/test_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-23 08:16:35.000000 dtflw-0.6.4/tests/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-23 08:16:35.000000 dtflw-0.6.4/tests/test_com.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-23 08:16:35.000000 dtflw-0.6.4/tests/test_databricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-23 08:16:35.000000 dtflw-0.6.4/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-23 08:16:35.000000 dtflw-0.6.4/tests/test_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-23 08:16:35.000000 dtflw-0.6.4/tests/test_input_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-05-23 08:16:35.000000 dtflw-0.6.4/tests/test_lazy_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-23 08:16:35.000000 dtflw-0.6.4/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-23 08:16:35.000000 dtflw-0.6.4/tests/test_output_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-23 08:16:35.000000 dtflw-0.6.4/tests/test_pipeline_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-23 08:16:35.000000 dtflw-0.6.4/tests/test_tables_repository.py
```

### Comparing `dtflw-0.6.3/LICENSE` & `dtflw-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/PKG-INFO` & `dtflw-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtflw
-Version: 0.6.3
+Version: 0.6.4
 Summary: dtflw is a Python framework for building modular data pipelines based on Databricks dbutils.notebook API.
 Home-page: https://github.com/SoleyIo/dtflw
 Author: Soley GmbH
 Author-email: codeofconduct@soley.io
 Project-URL: Bug Reports, https://github.com/SoleyIo/dtflw/issues
 Project-URL: Source, https://github.com/SoleyIo/dtflw
 Keywords: databricks,data pipelines,etl,data engineering
```

### Comparing `dtflw-0.6.3/README.md` & `dtflw-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/setup.py` & `dtflw-0.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="dtflw",
-    version="0.6.3",
+    version="0.6.4",
 
     description="dtflw is a Python framework for building modular data pipelines based on Databricks dbutils.notebook API.",
     long_description="See [the home page](https://github.com/SoleyIo/dtflw/blob/main/README.md) of the project for details.",
     long_description_content_type="text/markdown",
 
     url="https://github.com/SoleyIo/dtflw",
```

### Comparing `dtflw-0.6.3/src/dtflw/__init__.py` & `dtflw-0.6.4/src/dtflw/__init__.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/src/dtflw/arguments.py` & `dtflw-0.6.4/src/dtflw/arguments.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/src/dtflw/assertions.py` & `dtflw-0.6.4/src/dtflw/assertions.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/src/dtflw/com.py` & `dtflw-0.6.4/src/dtflw/com.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/src/dtflw/databricks.py` & `dtflw-0.6.4/src/dtflw/databricks.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/src/dtflw/display.py` & `dtflw-0.6.4/src/dtflw/display.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/src/dtflw/flow.py` & `dtflw-0.6.4/src/dtflw/flow.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/src/dtflw/flow_context.py` & `dtflw-0.6.4/src/dtflw/flow_context.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/src/dtflw/input_table.py` & `dtflw-0.6.4/src/dtflw/input_table.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/src/dtflw/lazy_notebook.py` & `dtflw-0.6.4/src/dtflw/lazy_notebook.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/src/dtflw/logger.py` & `dtflw-0.6.4/src/dtflw/logger.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/src/dtflw/output_table.py` & `dtflw-0.6.4/src/dtflw/output_table.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         strict: bool
             Default: False
             Do a strict validation on the table, meaning validation will also fail if more columns then expected are found.
         """
         if self.needs_eval():
             raise Exception("Expected output not found.")
 
-        df = self.__ctx.storage.read_table(self.abs_file_path)
+        if self.__expected_columns:
+            df = self.__ctx.storage.read_table(self.abs_file_path)
 
-        A.assert_schema_compatible(
-            df.dtypes,
-            self.__expected_columns or [],
-            strict
-        )
+            A.assert_schema_compatible(
+                df.dtypes,
+                self.__expected_columns,
+                strict
+            )
```

### Comparing `dtflw-0.6.3/src/dtflw/pipeline.py` & `dtflw-0.6.4/src/dtflw/pipeline.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/src/dtflw/plugin.py` & `dtflw-0.6.4/src/dtflw/plugin.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/src/dtflw/storage/azure.py` & `dtflw-0.6.4/src/dtflw/storage/azure.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/src/dtflw/storage/dbfs.py` & `dtflw-0.6.4/src/dtflw/storage/dbfs.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/src/dtflw/storage/fs.py` & `dtflw-0.6.4/src/dtflw/storage/fs.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/src/dtflw/tables_repo.py` & `dtflw-0.6.4/src/dtflw/tables_repo.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/src/dtflw.egg-info/PKG-INFO` & `dtflw-0.6.4/src/dtflw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtflw
-Version: 0.6.3
+Version: 0.6.4
 Summary: dtflw is a Python framework for building modular data pipelines based on Databricks dbutils.notebook API.
 Home-page: https://github.com/SoleyIo/dtflw
 Author: Soley GmbH
 Author-email: codeofconduct@soley.io
 Project-URL: Bug Reports, https://github.com/SoleyIo/dtflw/issues
 Project-URL: Source, https://github.com/SoleyIo/dtflw
 Keywords: databricks,data pipelines,etl,data engineering
```

### Comparing `dtflw-0.6.3/src/dtflw.egg-info/SOURCES.txt` & `dtflw-0.6.4/src/dtflw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/tests/test_arguments.py` & `dtflw-0.6.4/tests/test_arguments.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/tests/test_assertions.py` & `dtflw-0.6.4/tests/test_assertions.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/tests/test_com.py` & `dtflw-0.6.4/tests/test_com.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/tests/test_databricks.py` & `dtflw-0.6.4/tests/test_databricks.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/tests/test_flow.py` & `dtflw-0.6.4/tests/test_flow.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/tests/test_input_table.py` & `dtflw-0.6.4/tests/test_input_table.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/tests/test_lazy_notebook.py` & `dtflw-0.6.4/tests/test_lazy_notebook.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/tests/test_logger.py` & `dtflw-0.6.4/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/tests/test_output_table.py` & `dtflw-0.6.4/tests/test_output_table.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/tests/test_pipeline_state.py` & `dtflw-0.6.4/tests/test_pipeline_state.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.3/tests/test_tables_repository.py` & `dtflw-0.6.4/tests/test_tables_repository.py`

 * *Files identical despite different names*

