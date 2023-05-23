# Comparing `tmp/jupyter_Pandas_GUI-0.8.0.dev0.tar.gz` & `tmp/jupyter_Pandas_GUI-0.8.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_Pandas_GUI-0.8.0.dev0.tar", last modified: Mon May 22 20:04:23 2023, max compression
+gzip compressed data, was "jupyter_Pandas_GUI-0.8.0.dev1.tar", last modified: Tue May 23 00:47:05 2023, max compression
```

## Comparing `jupyter_Pandas_GUI-0.8.0.dev0.tar` & `jupyter_Pandas_GUI-0.8.0.dev1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-22 20:04:23.658833 jupyter_Pandas_GUI-0.8.0.dev0/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    35149 2020-05-31 15:03:56.000000 jupyter_Pandas_GUI-0.8.0.dev0/LICENSE
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     9058 2023-05-22 20:04:23.658833 jupyter_Pandas_GUI-0.8.0.dev0/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8312 2023-05-22 02:01:29.000000 jupyter_Pandas_GUI-0.8.0.dev0/README.md
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-22 20:04:23.658833 jupyter_Pandas_GUI-0.8.0.dev0/jupyter_Pandas_GUI.egg-info/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     9058 2023-05-22 20:04:23.000000 jupyter_Pandas_GUI-0.8.0.dev0/jupyter_Pandas_GUI.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      373 2023-05-22 20:04:23.000000 jupyter_Pandas_GUI-0.8.0.dev0/jupyter_Pandas_GUI.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2023-05-22 20:04:23.000000 jupyter_Pandas_GUI-0.8.0.dev0/jupyter_Pandas_GUI.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      156 2023-05-22 20:04:23.000000 jupyter_Pandas_GUI-0.8.0.dev0/jupyter_Pandas_GUI.egg-info/requires.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       11 2023-05-22 20:04:23.000000 jupyter_Pandas_GUI-0.8.0.dev0/jupyter_Pandas_GUI.egg-info/top_level.txt
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-22 20:04:23.658833 jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      568 2022-12-18 21:05:47.000000 jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    49764 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/fit_Pandas_GUI.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    12021 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/new_pandas_column_GUI.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    29470 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/plot_Pandas_GUI.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    14280 2023-05-22 19:12:16.000000 jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/utils.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2023-05-22 20:04:23.658833 jupyter_Pandas_GUI-0.8.0.dev0/setup.cfg
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1324 2023-05-22 02:01:29.000000 jupyter_Pandas_GUI-0.8.0.dev0/setup.py
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-23 00:47:05.629321 jupyter_Pandas_GUI-0.8.0.dev1/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    35149 2020-05-31 15:03:56.000000 jupyter_Pandas_GUI-0.8.0.dev1/LICENSE
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     9058 2023-05-23 00:47:05.629321 jupyter_Pandas_GUI-0.8.0.dev1/PKG-INFO
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8312 2023-05-22 02:01:29.000000 jupyter_Pandas_GUI-0.8.0.dev1/README.md
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-23 00:47:05.625321 jupyter_Pandas_GUI-0.8.0.dev1/jupyter_Pandas_GUI.egg-info/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     9058 2023-05-23 00:47:05.000000 jupyter_Pandas_GUI-0.8.0.dev1/jupyter_Pandas_GUI.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      373 2023-05-23 00:47:05.000000 jupyter_Pandas_GUI-0.8.0.dev1/jupyter_Pandas_GUI.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2023-05-23 00:47:05.000000 jupyter_Pandas_GUI-0.8.0.dev1/jupyter_Pandas_GUI.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      156 2023-05-23 00:47:05.000000 jupyter_Pandas_GUI-0.8.0.dev1/jupyter_Pandas_GUI.egg-info/requires.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       11 2023-05-23 00:47:05.000000 jupyter_Pandas_GUI-0.8.0.dev1/jupyter_Pandas_GUI.egg-info/top_level.txt
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-23 00:47:05.629321 jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      568 2022-12-18 21:05:47.000000 jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    49764 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/fit_Pandas_GUI.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    12021 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/new_pandas_column_GUI.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    29470 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/plot_Pandas_GUI.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    14289 2023-05-23 00:40:05.000000 jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/utils.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2023-05-23 00:47:05.629321 jupyter_Pandas_GUI-0.8.0.dev1/setup.cfg
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1325 2023-05-23 00:46:37.000000 jupyter_Pandas_GUI-0.8.0.dev1/setup.py
```

### Comparing `jupyter_Pandas_GUI-0.8.0.dev0/LICENSE` & `jupyter_Pandas_GUI-0.8.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev0/PKG-INFO` & `jupyter_Pandas_GUI-0.8.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_Pandas_GUI
-Version: 0.8.0.dev0
+Version: 0.8.0.dev1
 Summary: Pandas expression composers using Jupyter widgets.
 Home-page: https://jupyterphysscilab.github.io/jupyter_Pandas_GUI/
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Keywords: fitting,data-analysis,plotting,learning to code
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jupyter_Pandas_GUI-0.8.0.dev0/README.md` & `jupyter_Pandas_GUI-0.8.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev0/jupyter_Pandas_GUI.egg-info/PKG-INFO` & `jupyter_Pandas_GUI-0.8.0.dev1/jupyter_Pandas_GUI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-Pandas-GUI
-Version: 0.8.0.dev0
+Version: 0.8.0.dev1
 Summary: Pandas expression composers using Jupyter widgets.
 Home-page: https://jupyterphysscilab.github.io/jupyter_Pandas_GUI/
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Keywords: fitting,data-analysis,plotting,learning to code
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/__init__.py` & `jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/fit_Pandas_GUI.py` & `jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/fit_Pandas_GUI.py`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/new_pandas_column_GUI.py` & `jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/new_pandas_column_GUI.py`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/plot_Pandas_GUI.py` & `jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/plot_Pandas_GUI.py`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/utils.py` & `jupyter_Pandas_GUI-0.8.0.dev1/pandas_GUI/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,15 @@
             with output_elem:
                 display(HTML(
                 '<details><summary style="cursor:pointer;"><span style="font-weight:bold;"><a>' \
                 'Code that was run</a></span>(click to toggle visibility)</summary>' \
                 '<div style="background:#eff0f1;white-space:pre-line;white-space:pre-wrap;">' \
                 '<pre>' + self.sniptext.value + '</pre></div></details>'))
                 display(HTML('<h3>Result<h3>'))
-                exec(str(self.sniptext.value), shell.user_ns)
+                display(exec(str(self.sniptext.value), shell.user_ns))
             pass
 
         self.dobutton.on_click(onRunCode)
 
         super(build_run_snip_widget, self).__init__([self.sniptext,
                                              self.dobox],
                                             layout=Layout(
```

### Comparing `jupyter_Pandas_GUI-0.8.0.dev0/setup.py` & `jupyter_Pandas_GUI-0.8.0.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="jupyter_Pandas_GUI",
-    version="0.8.0dev",
+    version="0.8.0dev1",
     description="Pandas expression composers using Jupyter widgets.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://jupyterphysscilab.github.io/jupyter_Pandas_GUI/",
     author="Jonathan Gutow",
     author_email="gutow@uwosh.edu",
     keywords="fitting, data-analysis, plotting, learning to code",
```

