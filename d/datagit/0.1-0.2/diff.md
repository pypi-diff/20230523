# Comparing `tmp/datagit-0.1.tar.gz` & `tmp/datagit-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagit-0.1.tar", last modified: Mon May 22 17:09:05 2023, max compression
+gzip compressed data, was "datagit-0.2.tar", last modified: Tue May 23 14:59:50 2023, max compression
```

## Comparing `datagit-0.1.tar` & `datagit-0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-05-22 17:09:05.243488 datagit-0.1/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     1203 2023-05-22 17:09:05.243371 datagit-0.1/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      766 2023-05-22 17:03:46.000000 datagit-0.1/README.md
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-05-22 17:09:05.242710 datagit-0.1/datagit/
--rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-05-22 13:02:30.000000 datagit-0.1/datagit/__init__.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)     1076 2023-05-22 16:59:28.000000 datagit-0.1/datagit/github_connector.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      721 2023-05-22 15:11:55.000000 datagit-0.1/datagit/query_builder.py
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-05-22 17:09:05.243192 datagit-0.1/datagit.egg-info/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     1203 2023-05-22 17:09:04.000000 datagit-0.1/datagit.egg-info/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      215 2023-05-22 17:09:05.000000 datagit-0.1/datagit.egg-info/SOURCES.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-05-22 17:09:05.000000 datagit-0.1/datagit.egg-info/dependency_links.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        8 2023-05-22 17:09:05.000000 datagit-0.1/datagit.egg-info/top_level.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-05-22 17:09:05.243541 datagit-0.1/setup.cfg
--rw-r--r--   0 sammyteillet   (501) staff       (20)      581 2023-05-22 15:30:26.000000 datagit-0.1/setup.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-05-23 14:59:50.897602 datagit-0.2/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     1167 2023-05-23 14:59:50.897419 datagit-0.2/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      766 2023-05-22 17:03:46.000000 datagit-0.2/README.md
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-05-23 14:59:50.896276 datagit-0.2/datagit/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-05-22 13:02:30.000000 datagit-0.2/datagit/__init__.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      636 2023-05-23 14:46:32.000000 datagit-0.2/datagit/dataset_helpers.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     3665 2023-05-23 14:46:32.000000 datagit-0.2/datagit/github_connector.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      721 2023-05-23 14:01:11.000000 datagit-0.2/datagit/query_builder.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-05-23 14:59:50.897068 datagit-0.2/datagit.egg-info/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     1167 2023-05-23 14:59:50.000000 datagit-0.2/datagit.egg-info/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      242 2023-05-23 14:59:50.000000 datagit-0.2/datagit.egg-info/SOURCES.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-05-23 14:59:50.000000 datagit-0.2/datagit.egg-info/dependency_links.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        8 2023-05-23 14:59:50.000000 datagit-0.2/datagit.egg-info/top_level.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-05-23 14:59:50.897666 datagit-0.2/setup.cfg
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      581 2023-05-23 14:59:49.000000 datagit-0.2/setup.py
```

### Comparing `datagit-0.1/PKG-INFO` & `datagit-0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: datagit
-Version: 0.1
+Version: 0.2
 Summary: Git based metric store
 Home-page: https://github.com/data-drift/datagit
 Author: Sammy Teillet
 Author-email: sammy.teillet@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Datagit
@@ -25,8 +23,7 @@
 
 >>> dataframe = bigquery.Client().query(query).to_dataframe() # Get a dataframe anyway you want
 >>> github_connector.store_metric(Github("Token"), dataframe=dataframe, filename="data/act_metrics_finance/mrr", assignee=["Samox"])
 'data/act_metrics_finance/mrr.csv pushed on production branch'
 'Historical data change detected'
 'Pull request was open from production to main, Samox was assigned to it'
 ```
-
```

### Comparing `datagit-0.1/README.md` & `datagit-0.2/README.md`

 * *Files identical despite different names*

### Comparing `datagit-0.1/datagit/query_builder.py` & `datagit-0.2/datagit/query_builder.py`

 * *Files identical despite different names*

### Comparing `datagit-0.1/datagit.egg-info/PKG-INFO` & `datagit-0.2/datagit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: datagit
-Version: 0.1
+Version: 0.2
 Summary: Git based metric store
 Home-page: https://github.com/data-drift/datagit
 Author: Sammy Teillet
 Author-email: sammy.teillet@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Datagit
@@ -25,8 +23,7 @@
 
 >>> dataframe = bigquery.Client().query(query).to_dataframe() # Get a dataframe anyway you want
 >>> github_connector.store_metric(Github("Token"), dataframe=dataframe, filename="data/act_metrics_finance/mrr", assignee=["Samox"])
 'data/act_metrics_finance/mrr.csv pushed on production branch'
 'Historical data change detected'
 'Pull request was open from production to main, Samox was assigned to it'
 ```
-
```

### Comparing `datagit-0.1/setup.py` & `datagit-0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="datagit",
-    version="0.1",
+    version="0.2",
     packages=find_packages(),
     author="Sammy Teillet",
     author_email="sammy.teillet@gmail.com",
     description="Git based metric store",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/data-drift/datagit",
```

