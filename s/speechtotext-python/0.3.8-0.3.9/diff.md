# Comparing `tmp/speechtotext-python-0.3.8.tar.gz` & `tmp/speechtotext-python-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speechtotext-python-0.3.8.tar", last modified: Wed Apr 26 12:31:12 2023, max compression
+gzip compressed data, was "speechtotext-python-0.3.9.tar", last modified: Tue May  2 12:18:11 2023, max compression
```

## Comparing `speechtotext-python-0.3.8.tar` & `speechtotext-python-0.3.9.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:31:12.595373 speechtotext-python-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-26 12:31:12.591373 speechtotext-python-0.3.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 12:31:12.595373 speechtotext-python-0.3.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4111 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:31:12.591373 speechtotext-python-0.3.8/speechtotext/
--rwxr-xr-x   0 runner    (1001) docker     (123)      108 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/speechtotext/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/speechtotext/__version__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3645 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/speechtotext/datasets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6847 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/speechtotext/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:31:12.591373 speechtotext-python-0.3.8/speechtotext_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-26 12:31:12.000000 speechtotext-python-0.3.8/speechtotext_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-26 12:31:12.000000 speechtotext-python-0.3.8/speechtotext_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 12:31:12.000000 speechtotext-python-0.3.8/speechtotext_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-26 12:31:12.000000 speechtotext-python-0.3.8/speechtotext_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 12:31:12.000000 speechtotext-python-0.3.8/speechtotext_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:31:12.591373 speechtotext-python-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/tests/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:18:11.040674 speechtotext-python-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-02 12:16:45.000000 speechtotext-python-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-02 12:18:11.040674 speechtotext-python-0.3.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-05-02 12:16:45.000000 speechtotext-python-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 12:18:11.040674 speechtotext-python-0.3.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4129 2023-05-02 12:16:45.000000 speechtotext-python-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:18:11.040674 speechtotext-python-0.3.9/speechtotext/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       87 2023-05-02 12:16:45.000000 speechtotext-python-0.3.9/speechtotext/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-05-02 12:16:45.000000 speechtotext-python-0.3.9/speechtotext/__version__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3645 2023-05-02 12:16:45.000000 speechtotext-python-0.3.9/speechtotext/datasets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6847 2023-05-02 12:16:45.000000 speechtotext-python-0.3.9/speechtotext/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:18:11.040674 speechtotext-python-0.3.9/speechtotext/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-02 12:16:45.000000 speechtotext-python-0.3.9/speechtotext/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-02 12:16:45.000000 speechtotext-python-0.3.9/speechtotext/metric/customMetrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7961 2023-05-02 12:16:45.000000 speechtotext-python-0.3.9/speechtotext/metric/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:18:11.040674 speechtotext-python-0.3.9/speechtotext_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-02 12:18:10.000000 speechtotext-python-0.3.9/speechtotext_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-02 12:18:11.000000 speechtotext-python-0.3.9/speechtotext_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:18:10.000000 speechtotext-python-0.3.9/speechtotext_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-02 12:18:10.000000 speechtotext-python-0.3.9/speechtotext_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 12:18:10.000000 speechtotext-python-0.3.9/speechtotext_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:18:11.040674 speechtotext-python-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-02 12:16:45.000000 speechtotext-python-0.3.9/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-05-02 12:16:45.000000 speechtotext-python-0.3.9/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-02 12:16:45.000000 speechtotext-python-0.3.9/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-02 12:16:45.000000 speechtotext-python-0.3.9/tests/test_metrics.py
```

### Comparing `speechtotext-python-0.3.8/LICENSE` & `speechtotext-python-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `speechtotext-python-0.3.8/PKG-INFO` & `speechtotext-python-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechtotext-python
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python package to benchmark speech2text models.
 Home-page: https://github.com/jarneamerlinck/speechtotext
 Author: Jarne Amerlinck
 Author-email: jarneamerlinck@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `speechtotext-python-0.3.8/setup.py` & `speechtotext-python-0.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 # What packages are required for this module to be executed?
 REQUIRED = [
 	'jiwer', 'pandas<2.0.0', 'numpy', 'torch>=2.0.0', 
 	'openai-whisper', 'openai', 'python-dotenv',
 	'matplotlib', 'ipywidgets', 'seaborn',
 	'dtale', 'boto3', 'google-cloud-speech',
 	'deepgram-sdk', 'azure-cognitiveservices-speech', 
-	'speechmatics-python==1.6.4', 'pydub', 'docstring_parser'
+	'speechmatics-python==1.6.4', 'pydub', 'docstring_parser',
+	'nltk', 'rouge'
 ]
 
 # What packages are optional?
 EXTRAS = {
 	'docs': ['Sphinx>=6.1.3', 'sphinx-markdown-builder>=0.5.5', 'sphinx_autodoc_typehints>=1.22', 
 			 'sphinx-press-theme>=0.8.0', 'sphinx_favicon', 'twine', 'graphviz']
 }
```

### Comparing `speechtotext-python-0.3.8/speechtotext/datasets.py` & `speechtotext-python-0.3.9/speechtotext/datasets.py`

 * *Files identical despite different names*

### Comparing `speechtotext-python-0.3.8/speechtotext/functions.py` & `speechtotext-python-0.3.9/speechtotext/functions.py`

 * *Files identical despite different names*

### Comparing `speechtotext-python-0.3.8/speechtotext_python.egg-info/PKG-INFO` & `speechtotext-python-0.3.9/speechtotext_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechtotext-python
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python package to benchmark speech2text models.
 Home-page: https://github.com/jarneamerlinck/speechtotext
 Author: Jarne Amerlinck
 Author-email: jarneamerlinck@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `speechtotext-python-0.3.8/tests/test_datasets.py` & `speechtotext-python-0.3.9/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `speechtotext-python-0.3.8/tests/test_functions.py` & `speechtotext-python-0.3.9/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `speechtotext-python-0.3.8/tests/test_imports.py` & `speechtotext-python-0.3.9/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `speechtotext-python-0.3.8/tests/test_metrics.py` & `speechtotext-python-0.3.9/tests/test_metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,8 +77,13 @@
 	def test_print(self):
 		"""Test get_all_metric_docs.
 		"""	
 		reference = "This is a test for the best"
 		hypothesis = "This is a test the best" 
 		m = Metrics(reference, hypothesis, self.audio_id, self.duration, with_cleaning=False)
 		to_print = f"wer: {1/7}, mer: {1/7}, wil: {1- 6/7}, wip: {6/7}, cer: {4/27}"
-		self.assertEqual(to_print, str(m))
+		self.assertEqual(to_print, str(m))
+
+	def test_lenght_of_metric_names(self):
+		"""Test get_all_metric_docs and get_all_metric_names.
+		"""
+		self.assertEqual(Metrics.get_all_metric_names().__len__(), Metrics.get_all_metric_docs().__len__())
```

