# Comparing `tmp/interactive_multi_category_table-0.0.2.tar.gz` & `tmp/interactive_multi_category_table-0.0.3.tar.gz`

## Comparing `interactive_multi_category_table-0.0.2.tar` & `interactive_multi_category_table-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.2/examples/ai4science.json
--rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.2/examples/dinner.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.2/interactive_multi_category_table/__init__.py
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.2/interactive_multi_category_table/main.py
--rw-r--r--   0        0        0     7200 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.2/interactive_multi_category_table/utils.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.2/LICENSE
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.2/README.md
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.3/examples/ai4science.json
+-rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.3/examples/dinner.json
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.3/interactive_multi_category_table/__init__.py
+-rw-r--r--   0        0        0    13455 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.3/interactive_multi_category_table/template.html
+-rw-r--r--   0        0        0     9077 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.3/interactive_multi_category_table/to_dash.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.3/interactive_multi_category_table/to_html.py
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.3/interactive_multi_category_table/utils.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.3/README.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.3/PKG-INFO
```

### Comparing `interactive_multi_category_table-0.0.2/examples/ai4science.json` & `interactive_multi_category_table-0.0.3/examples/ai4science.json`

 * *Files identical despite different names*

### Comparing `interactive_multi_category_table-0.0.2/examples/dinner.json` & `interactive_multi_category_table-0.0.3/examples/dinner.json`

 * *Files identical despite different names*

### Comparing `interactive_multi_category_table-0.0.2/.gitignore` & `interactive_multi_category_table-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `interactive_multi_category_table-0.0.2/LICENSE` & `interactive_multi_category_table-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `interactive_multi_category_table-0.0.2/README.md` & `interactive_multi_category_table-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 # interactive-multi-category-table
 
-In many different scenarios, contents are single-categorized and multi-tagged, by which I mean there are multiple tags but one single (though may be hierarchical) category system, e.g., file systems, blogs, etc. However, sometimes contents can be categorized from different category views. For storage or lookup, one category system is OK; but for visualization and analysis, flexibly organizing the contents with different category views will be very handy.
+In many different scenarios, contents are single-categorized and multi-tagged, by which I mean there exist multiple tags but one single (though maybe hierarchical) category system, e.g., file systems, blogs, etc. However, sometimes contents can be categorized from different category views. For storage or lookup, one category system is OK; but for visualization and analysis, flexibly organizing the contents with different category views will be very handy.
 
-This repo targets addressing such demand by creating interactive tables with alternative category views, from formatted json input, based on [dash](https://dash.plotly.com/).
+This repo targets addressing such demand by creating interactive tables with alternative category views from formatted json input. It can both run as a service on the server side based on [dash](https://dash.plotly.com/), or generate a static webpage on the client side.
 
 # usage
 
-Simply run
+## run on the server side
+
 ```python
 import interactive_multi_category_table as imct
 
-imct.run_app(json_file_path)
+imct.run_dash_app(json_file_path)
 ```
 and the generated webpage can be accessed at http://127.0.0.1:8050/.
 
-Refer to the provided examples for the json file format.
+## generate a static webpage
 
-# requirements
+```python
+import interactive_multi_category_table as imct
 
-- dash
+imct.json_to_html(json_file_path)
+```
+
+## input json file format
 
-# known limitations
+Refer to the provided examples for the json file format.
 
+Note that:
+- There have to be at least two category trees.
 - Leaf category items in the same category tree cannot be the same.
```

### Comparing `interactive_multi_category_table-0.0.2/pyproject.toml` & `interactive_multi_category_table-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "interactive_multi_category_table"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     {name="Xiang CHEN", email="xiangchen.ai@outlook.com"},
 ]
-description = "A python package to create interactive tables with alternative category views, from formatted json input, based on dash."
+description = "A python package to create interactive tables with alternative category views from formatted json input."
 
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
-dependencies = [
-    "dash",
-]
-
 [project.urls]
 "Homepage" = "https://github.com/XiangCHEN-dvi/interactive-multi-category-table"
 "Bug Tracker" = "https://github.com/XiangCHEN-dvi/interactive-multi-category-table/issues"
```

### Comparing `interactive_multi_category_table-0.0.2/PKG-INFO` & `interactive_multi_category_table-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 Metadata-Version: 2.1
 Name: interactive_multi_category_table
-Version: 0.0.2
-Summary: A python package to create interactive tables with alternative category views, from formatted json input, based on dash.
+Version: 0.0.3
+Summary: A python package to create interactive tables with alternative category views from formatted json input.
 Project-URL: Homepage, https://github.com/XiangCHEN-dvi/interactive-multi-category-table
 Project-URL: Bug Tracker, https://github.com/XiangCHEN-dvi/interactive-multi-category-table/issues
 Author-email: Xiang CHEN <xiangchen.ai@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: dash
 Description-Content-Type: text/markdown
 
 # interactive-multi-category-table
 
-In many different scenarios, contents are single-categorized and multi-tagged, by which I mean there are multiple tags but one single (though may be hierarchical) category system, e.g., file systems, blogs, etc. However, sometimes contents can be categorized from different category views. For storage or lookup, one category system is OK; but for visualization and analysis, flexibly organizing the contents with different category views will be very handy.
+In many different scenarios, contents are single-categorized and multi-tagged, by which I mean there exist multiple tags but one single (though maybe hierarchical) category system, e.g., file systems, blogs, etc. However, sometimes contents can be categorized from different category views. For storage or lookup, one category system is OK; but for visualization and analysis, flexibly organizing the contents with different category views will be very handy.
 
-This repo targets addressing such demand by creating interactive tables with alternative category views, from formatted json input, based on [dash](https://dash.plotly.com/).
+This repo targets addressing such demand by creating interactive tables with alternative category views from formatted json input. It can both run as a service on the server side based on [dash](https://dash.plotly.com/), or generate a static webpage on the client side.
 
 # usage
 
-Simply run
+## run on the server side
+
 ```python
 import interactive_multi_category_table as imct
 
-imct.run_app(json_file_path)
+imct.run_dash_app(json_file_path)
 ```
 and the generated webpage can be accessed at http://127.0.0.1:8050/.
 
-Refer to the provided examples for the json file format.
+## generate a static webpage
 
-# requirements
+```python
+import interactive_multi_category_table as imct
 
-- dash
+imct.json_to_html(json_file_path)
+```
+
+## input json file format
 
-# known limitations
+Refer to the provided examples for the json file format.
 
+Note that:
+- There have to be at least two category trees.
 - Leaf category items in the same category tree cannot be the same.
```

