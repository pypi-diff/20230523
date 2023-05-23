# Comparing `tmp/ghevaluator-2.1.0.tar.gz` & `tmp/ghevaluator-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghevaluator-2.1.0.tar", last modified: Mon May 22 09:46:08 2023, max compression
+gzip compressed data, was "ghevaluator-2.1.1.tar", last modified: Tue May 23 14:16:53 2023, max compression
```

## Comparing `ghevaluator-2.1.0.tar` & `ghevaluator-2.1.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-22 09:46:08.989394 ghevaluator-2.1.0/
--rw-r--r--   0 bebatut    (502) staff       (20)     1066 2023-05-11 09:08:31.000000 ghevaluator-2.1.0/LICENSE
--rw-r--r--   0 bebatut    (502) staff       (20)       52 2023-05-11 09:08:31.000000 ghevaluator-2.1.0/MANIFEST.in
--rw-r--r--   0 bebatut    (502) staff       (20)     4253 2023-05-22 09:46:08.988940 ghevaluator-2.1.0/PKG-INFO
--rw-r--r--   0 bebatut    (502) staff       (20)     2293 2023-05-22 09:44:16.000000 ghevaluator-2.1.0/README.md
-drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-22 09:46:08.971939 ghevaluator-2.1.0/docs/
--rw-r--r--   0 bebatut    (502) staff       (20)      230 2023-05-22 09:28:28.000000 ghevaluator-2.1.0/docs/.buildinfo
--rw-r--r--   0 bebatut    (502) staff       (20)     3678 2023-05-22 09:28:27.000000 ghevaluator-2.1.0/docs/api_documentation.html
--rw-r--r--   0 bebatut    (502) staff       (20)    10043 2023-05-22 09:44:16.000000 ghevaluator-2.1.0/docs/contributing.html
--rw-r--r--   0 bebatut    (502) staff       (20)     3624 2023-05-22 09:28:28.000000 ghevaluator-2.1.0/docs/genindex.html
--rw-r--r--   0 bebatut    (502) staff       (20)     5817 2023-05-22 09:44:16.000000 ghevaluator-2.1.0/docs/index.html
--rw-r--r--   0 bebatut    (502) staff       (20)     4377 2023-05-22 09:28:27.000000 ghevaluator-2.1.0/docs/installation.html
--rw-r--r--   0 bebatut    (502) staff       (20)      371 2023-05-22 09:28:28.000000 ghevaluator-2.1.0/docs/objects.inv
--rw-r--r--   0 bebatut    (502) staff       (20)     3503 2023-05-22 09:28:28.000000 ghevaluator-2.1.0/docs/py-modindex.html
--rw-r--r--   0 bebatut    (502) staff       (20)     3235 2023-05-22 09:28:28.000000 ghevaluator-2.1.0/docs/search.html
--rw-r--r--   0 bebatut    (502) staff       (20)     5570 2023-05-22 09:44:16.000000 ghevaluator-2.1.0/docs/searchindex.js
--rw-r--r--   0 bebatut    (502) staff       (20)     8176 2023-05-22 09:44:16.000000 ghevaluator-2.1.0/docs/usage.html
-drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-22 09:46:08.975711 ghevaluator-2.1.0/ghevaluator/
--rw-r--r--   0 bebatut    (502) staff       (20)    12098 2023-05-22 09:44:16.000000 ghevaluator-2.1.0/ghevaluator/__init__.py
--rw-r--r--   0 bebatut    (502) staff       (20)     1241 2023-05-11 14:54:26.000000 ghevaluator-2.1.0/ghevaluator/__main__.py
-drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-22 09:46:08.985492 ghevaluator-2.1.0/ghevaluator.egg-info/
--rw-r--r--   0 bebatut    (502) staff       (20)     4253 2023-05-22 09:46:08.000000 ghevaluator-2.1.0/ghevaluator.egg-info/PKG-INFO
--rw-r--r--   0 bebatut    (502) staff       (20)      564 2023-05-22 09:46:08.000000 ghevaluator-2.1.0/ghevaluator.egg-info/SOURCES.txt
--rw-r--r--   0 bebatut    (502) staff       (20)        1 2023-05-22 09:46:08.000000 ghevaluator-2.1.0/ghevaluator.egg-info/dependency_links.txt
--rw-r--r--   0 bebatut    (502) staff       (20)       58 2023-05-22 09:46:08.000000 ghevaluator-2.1.0/ghevaluator.egg-info/entry_points.txt
--rw-r--r--   0 bebatut    (502) staff       (20)       18 2023-05-22 09:46:08.000000 ghevaluator-2.1.0/ghevaluator.egg-info/requires.txt
--rw-r--r--   0 bebatut    (502) staff       (20)       45 2023-05-22 09:46:08.000000 ghevaluator-2.1.0/ghevaluator.egg-info/top_level.txt
--rw-r--r--   0 bebatut    (502) staff       (20)      981 2023-05-22 09:31:24.000000 ghevaluator-2.1.0/pyproject.toml
--rw-r--r--   0 bebatut    (502) staff       (20)       38 2023-05-22 09:46:08.989509 ghevaluator-2.1.0/setup.cfg
-drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-22 09:46:08.958589 ghevaluator-2.1.0/src/
-drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-22 09:46:08.986025 ghevaluator-2.1.0/src/docs/
--rw-r--r--   0 bebatut    (502) staff       (20)     1115 2023-05-11 14:25:17.000000 ghevaluator-2.1.0/src/docs/conf.py
-drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-22 09:46:08.986795 ghevaluator-2.1.0/tests/
--rw-r--r--   0 bebatut    (502) staff       (20)    10637 2023-05-22 09:44:16.000000 ghevaluator-2.1.0/tests/test_ghevaluator.py
+drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-23 14:16:53.248072 ghevaluator-2.1.1/
+-rw-r--r--   0 bebatut    (502) staff       (20)     1066 2023-05-11 09:08:31.000000 ghevaluator-2.1.1/LICENSE
+-rw-r--r--   0 bebatut    (502) staff       (20)       52 2023-05-11 09:08:31.000000 ghevaluator-2.1.1/MANIFEST.in
+-rw-r--r--   0 bebatut    (502) staff       (20)     4253 2023-05-23 14:16:53.247336 ghevaluator-2.1.1/PKG-INFO
+-rw-r--r--   0 bebatut    (502) staff       (20)     2293 2023-05-22 09:44:16.000000 ghevaluator-2.1.1/README.md
+drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-23 14:16:53.208584 ghevaluator-2.1.1/docs/
+-rw-r--r--   0 bebatut    (502) staff       (20)      230 2023-05-23 13:49:33.000000 ghevaluator-2.1.1/docs/.buildinfo
+-rw-r--r--   0 bebatut    (502) staff       (20)        0 2023-05-23 13:49:34.000000 ghevaluator-2.1.1/docs/.nojekyll
+-rw-r--r--   0 bebatut    (502) staff       (20)     3678 2023-05-23 13:49:33.000000 ghevaluator-2.1.1/docs/api_documentation.html
+-rw-r--r--   0 bebatut    (502) staff       (20)    10043 2023-05-23 13:49:33.000000 ghevaluator-2.1.1/docs/contributing.html
+-rw-r--r--   0 bebatut    (502) staff       (20)     3624 2023-05-23 13:49:33.000000 ghevaluator-2.1.1/docs/genindex.html
+-rw-r--r--   0 bebatut    (502) staff       (20)     5817 2023-05-23 13:49:33.000000 ghevaluator-2.1.1/docs/index.html
+-rw-r--r--   0 bebatut    (502) staff       (20)     4377 2023-05-23 13:49:33.000000 ghevaluator-2.1.1/docs/installation.html
+-rw-r--r--   0 bebatut    (502) staff       (20)      371 2023-05-23 13:49:33.000000 ghevaluator-2.1.1/docs/objects.inv
+-rw-r--r--   0 bebatut    (502) staff       (20)     3503 2023-05-23 13:49:33.000000 ghevaluator-2.1.1/docs/py-modindex.html
+-rw-r--r--   0 bebatut    (502) staff       (20)     3235 2023-05-23 13:49:33.000000 ghevaluator-2.1.1/docs/search.html
+-rw-r--r--   0 bebatut    (502) staff       (20)     5570 2023-05-23 13:49:33.000000 ghevaluator-2.1.1/docs/searchindex.js
+-rw-r--r--   0 bebatut    (502) staff       (20)     8176 2023-05-23 13:49:33.000000 ghevaluator-2.1.1/docs/usage.html
+drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-23 14:16:53.215890 ghevaluator-2.1.1/ghevaluator/
+-rw-r--r--   0 bebatut    (502) staff       (20)    12085 2023-05-23 14:06:42.000000 ghevaluator-2.1.1/ghevaluator/__init__.py
+-rw-r--r--   0 bebatut    (502) staff       (20)     1241 2023-05-11 14:54:26.000000 ghevaluator-2.1.1/ghevaluator/__main__.py
+drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-23 14:16:53.241776 ghevaluator-2.1.1/ghevaluator.egg-info/
+-rw-r--r--   0 bebatut    (502) staff       (20)     4253 2023-05-23 14:16:53.000000 ghevaluator-2.1.1/ghevaluator.egg-info/PKG-INFO
+-rw-r--r--   0 bebatut    (502) staff       (20)      579 2023-05-23 14:16:53.000000 ghevaluator-2.1.1/ghevaluator.egg-info/SOURCES.txt
+-rw-r--r--   0 bebatut    (502) staff       (20)        1 2023-05-23 14:16:53.000000 ghevaluator-2.1.1/ghevaluator.egg-info/dependency_links.txt
+-rw-r--r--   0 bebatut    (502) staff       (20)       58 2023-05-23 14:16:53.000000 ghevaluator-2.1.1/ghevaluator.egg-info/entry_points.txt
+-rw-r--r--   0 bebatut    (502) staff       (20)       25 2023-05-23 14:16:53.000000 ghevaluator-2.1.1/ghevaluator.egg-info/requires.txt
+-rw-r--r--   0 bebatut    (502) staff       (20)       45 2023-05-23 14:16:53.000000 ghevaluator-2.1.1/ghevaluator.egg-info/top_level.txt
+-rw-r--r--   0 bebatut    (502) staff       (20)      994 2023-05-23 14:09:18.000000 ghevaluator-2.1.1/pyproject.toml
+-rw-r--r--   0 bebatut    (502) staff       (20)       38 2023-05-23 14:16:53.248195 ghevaluator-2.1.1/setup.cfg
+drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-23 14:16:53.149168 ghevaluator-2.1.1/src/
+drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-23 14:16:53.242606 ghevaluator-2.1.1/src/docs/
+-rw-r--r--   0 bebatut    (502) staff       (20)     1115 2023-05-11 14:25:17.000000 ghevaluator-2.1.1/src/docs/conf.py
+drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-23 14:16:53.244032 ghevaluator-2.1.1/tests/
+-rw-r--r--   0 bebatut    (502) staff       (20)    10637 2023-05-22 09:44:16.000000 ghevaluator-2.1.1/tests/test_ghevaluator.py
```

### Comparing `ghevaluator-2.1.0/LICENSE` & `ghevaluator-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ghevaluator-2.1.0/PKG-INFO` & `ghevaluator-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghevaluator
-Version: 2.1.0
+Version: 2.1.1
 Summary: A command-line Python tool to compare Galaxy histories to a template workflow and generate a JSON report file.
 Author: Teresa Müller
 Author-email: Siyu Chen <chensy96@gmail.com>, Bérénice Batut <berenice.batut@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Siyu Chen
```

### Comparing `ghevaluator-2.1.0/README.md` & `ghevaluator-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ghevaluator-2.1.0/docs/api_documentation.html` & `ghevaluator-2.1.1/docs/api_documentation.html`

 * *Files identical despite different names*

### Comparing `ghevaluator-2.1.0/docs/contributing.html` & `ghevaluator-2.1.1/docs/contributing.html`

 * *Files identical despite different names*

### Comparing `ghevaluator-2.1.0/docs/genindex.html` & `ghevaluator-2.1.1/docs/genindex.html`

 * *Files identical despite different names*

### Comparing `ghevaluator-2.1.0/docs/index.html` & `ghevaluator-2.1.1/docs/index.html`

 * *Files identical despite different names*

### Comparing `ghevaluator-2.1.0/docs/installation.html` & `ghevaluator-2.1.1/docs/installation.html`

 * *Files identical despite different names*

### Comparing `ghevaluator-2.1.0/docs/py-modindex.html` & `ghevaluator-2.1.1/docs/py-modindex.html`

 * *Files identical despite different names*

### Comparing `ghevaluator-2.1.0/docs/search.html` & `ghevaluator-2.1.1/docs/search.html`

 * *Files identical despite different names*

### Comparing `ghevaluator-2.1.0/docs/searchindex.js` & `ghevaluator-2.1.1/docs/searchindex.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -317,38 +317,23 @@
         "sphinx.domains.std": 2,
         "sphinx": 57
     },
     "alltitles": {
         "API documentation": [
             [0, "module-__main__"]
         ],
-        "Welcome to Galaxy History Evaluator\u2019s documentation!": [
-            [2, "welcome-to-galaxy-history-evaluator-s-documentation"]
-        ],
-        "Contents:": [
-            [2, null]
-        ],
-        "Indices and tables": [
-            [2, "indices-and-tables"]
-        ],
         "Installation": [
             [3, "installation"]
         ],
         "Requirements": [
             [3, "requirements"]
         ],
         "Installation via pip": [
             [3, "installation-via-pip"]
         ],
-        "Usage": [
-            [4, "usage"]
-        ],
-        "Output": [
-            [4, "output"]
-        ],
         "Contributing": [
             [1, "contributing"]
         ],
         "What should I know before I get started?": [
             [1, "what-should-i-know-before-i-get-started"]
         ],
         "How can I contribute?": [
@@ -364,14 +349,29 @@
             [1, "development"]
         ],
         "Tests": [
             [1, "tests"]
         ],
         "Documentation": [
             [1, "documentation"]
+        ],
+        "Welcome to Galaxy History Evaluator\u2019s documentation!": [
+            [2, "welcome-to-galaxy-history-evaluator-s-documentation"]
+        ],
+        "Contents:": [
+            [2, null]
+        ],
+        "Indices and tables": [
+            [2, "indices-and-tables"]
+        ],
+        "Usage": [
+            [4, "usage"]
+        ],
+        "Output": [
+            [4, "output"]
         ]
     },
     "indexentries": {
         "__main__": [
             [0, "module-__main__"]
         ],
         "module": [
```

### Comparing `ghevaluator-2.1.0/docs/usage.html` & `ghevaluator-2.1.1/docs/usage.html`

 * *Files identical despite different names*

### Comparing `ghevaluator-2.1.0/ghevaluator/__init__.py` & `ghevaluator-2.1.1/ghevaluator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,15 @@
 def generate_html_report_content(data):
     """
     Generate HTML report
 
     :param data: dictionary holding the information of the status of key features of user history
     """
     env = Environment(
-        loader=PackageLoader("ghevaluator", "templates"),
+        loader=PackageLoader("ghevaluator"),
         autoescape=select_autoescape()
     )
     template = env.get_template("report.html")
     return template.render(report=data)
 
 
 def generate_report_files(data, output_dp):
```

### Comparing `ghevaluator-2.1.0/ghevaluator/__main__.py` & `ghevaluator-2.1.1/ghevaluator/__main__.py`

 * *Files identical despite different names*

### Comparing `ghevaluator-2.1.0/ghevaluator.egg-info/PKG-INFO` & `ghevaluator-2.1.1/ghevaluator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghevaluator
-Version: 2.1.0
+Version: 2.1.1
 Summary: A command-line Python tool to compare Galaxy histories to a template workflow and generate a JSON report file.
 Author: Teresa Müller
 Author-email: Siyu Chen <chensy96@gmail.com>, Bérénice Batut <berenice.batut@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Siyu Chen
```

### Comparing `ghevaluator-2.1.0/ghevaluator.egg-info/SOURCES.txt` & `ghevaluator-2.1.1/ghevaluator.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 docs/.buildinfo
+docs/.nojekyll
 docs/api_documentation.html
 docs/contributing.html
 docs/genindex.html
 docs/index.html
 docs/installation.html
 docs/objects.inv
 docs/py-modindex.html
```

### Comparing `ghevaluator-2.1.0/pyproject.toml` & `ghevaluator-2.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghevaluator"
-version = "2.1.0"
+version = "2.1.1"
 authors = [
   { name="Siyu Chen", email="chensy96@gmail.com" },
   { name="Teresa Müller" },
   { name="Bérénice Batut", email="berenice.batut@gmail.com" },
 ]
 description = "A command-line Python tool to compare Galaxy histories to a template workflow and generate a JSON report file."
 readme = "README.md"
@@ -16,14 +16,15 @@
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering"
 ]
 
 dependencies = [
     "bioblend",
     "requests",
+    "Jinja2"
 ]
 
 [project.scripts]
 ghevaluator = "ghevaluator.__main__:main"
 
 [project.urls]
 repository = "https://github.com/SteetScienceCommunity/ghevaluator"
```

### Comparing `ghevaluator-2.1.0/src/docs/conf.py` & `ghevaluator-2.1.1/src/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ghevaluator-2.1.0/tests/test_ghevaluator.py` & `ghevaluator-2.1.1/tests/test_ghevaluator.py`

 * *Files identical despite different names*

