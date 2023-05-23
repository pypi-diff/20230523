# Comparing `tmp/memory_graph-0.1.8.tar.gz` & `tmp/memory_graph-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memory_graph-0.1.8.tar", last modified: Mon May 22 07:56:15 2023, max compression
+gzip compressed data, was "memory_graph-0.1.9.tar", last modified: Mon May 22 08:03:45 2023, max compression
```

## Comparing `memory_graph-0.1.8.tar` & `memory_graph-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-22 07:56:15.214232 memory_graph-0.1.8/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2023-05-19 18:17:38.000000 memory_graph-0.1.8/LICENSE.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2023-05-19 18:17:38.000000 memory_graph-0.1.8/MANIFEST.in
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     5271 2023-05-22 07:56:15.214232 memory_graph-0.1.8/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4696 2023-05-22 07:47:22.000000 memory_graph-0.1.8/README.md
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-22 07:56:15.214232 memory_graph-0.1.8/memory_graph/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1538 2023-05-19 18:17:38.000000 memory_graph-0.1.8/memory_graph/Node.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      865 2023-05-22 07:55:43.000000 memory_graph-0.1.8/memory_graph/__init__.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     5234 2023-05-21 18:05:01.000000 memory_graph-0.1.8/memory_graph/graphviz_nodes.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4288 2023-05-22 07:48:47.000000 memory_graph-0.1.8/memory_graph/rewrite.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1098 2023-05-22 07:43:38.000000 memory_graph-0.1.8/memory_graph/rewrite_to_node.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      551 2023-05-19 18:17:38.000000 memory_graph-0.1.8/memory_graph/rewrite_to_string.py
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-22 07:56:15.214232 memory_graph-0.1.8/memory_graph.egg-info/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     5271 2023-05-22 07:56:15.000000 memory_graph-0.1.8/memory_graph.egg-info/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      388 2023-05-22 07:56:15.000000 memory_graph-0.1.8/memory_graph.egg-info/SOURCES.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2023-05-22 07:56:15.000000 memory_graph-0.1.8/memory_graph.egg-info/dependency_links.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2023-05-22 07:56:15.000000 memory_graph-0.1.8/memory_graph.egg-info/requires.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2023-05-22 07:56:15.000000 memory_graph-0.1.8/memory_graph.egg-info/top_level.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2023-05-22 07:56:15.214232 memory_graph-0.1.8/setup.cfg
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      966 2023-05-22 07:55:56.000000 memory_graph-0.1.8/setup.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-22 08:03:45.849437 memory_graph-0.1.9/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2023-05-19 18:17:38.000000 memory_graph-0.1.9/LICENSE.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2023-05-19 18:17:38.000000 memory_graph-0.1.9/MANIFEST.in
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     5271 2023-05-22 08:03:45.849437 memory_graph-0.1.9/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4696 2023-05-22 07:47:22.000000 memory_graph-0.1.9/README.md
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-22 08:03:45.849437 memory_graph-0.1.9/memory_graph/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1538 2023-05-19 18:17:38.000000 memory_graph-0.1.9/memory_graph/Node.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      865 2023-05-22 08:03:00.000000 memory_graph-0.1.9/memory_graph/__init__.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     5234 2023-05-21 18:05:01.000000 memory_graph-0.1.9/memory_graph/graphviz_nodes.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4302 2023-05-22 08:01:42.000000 memory_graph-0.1.9/memory_graph/rewrite.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1098 2023-05-22 07:43:38.000000 memory_graph-0.1.9/memory_graph/rewrite_to_node.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      551 2023-05-19 18:17:38.000000 memory_graph-0.1.9/memory_graph/rewrite_to_string.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-22 08:03:45.849437 memory_graph-0.1.9/memory_graph.egg-info/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     5271 2023-05-22 08:03:45.000000 memory_graph-0.1.9/memory_graph.egg-info/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      388 2023-05-22 08:03:45.000000 memory_graph-0.1.9/memory_graph.egg-info/SOURCES.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2023-05-22 08:03:45.000000 memory_graph-0.1.9/memory_graph.egg-info/dependency_links.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2023-05-22 08:03:45.000000 memory_graph-0.1.9/memory_graph.egg-info/requires.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2023-05-22 08:03:45.000000 memory_graph-0.1.9/memory_graph.egg-info/top_level.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2023-05-22 08:03:45.849437 memory_graph-0.1.9/setup.cfg
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      966 2023-05-22 08:03:08.000000 memory_graph-0.1.9/setup.py
```

### Comparing `memory_graph-0.1.8/LICENSE.txt` & `memory_graph-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.8/PKG-INFO` & `memory_graph-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory_graph
-Version: 0.1.8
+Version: 0.1.9
 Summary: Draw a graph of your data to see the structure of its references.
 Home-page: https://github.com/bterwijn/memory_graph
 Author: Bas Terwijn
 Author-email: bterwijn@gmail.com
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `memory_graph-0.1.8/README.md` & `memory_graph-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.8/memory_graph/Node.py` & `memory_graph-0.1.9/memory_graph/Node.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.8/memory_graph/__init__.py` & `memory_graph-0.1.9/memory_graph/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from memory_graph import rewrite
 from memory_graph import Node
 from memory_graph import rewrite_to_node
 from memory_graph import graphviz_nodes
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 __author__ = 'Bas Terwijn'
 
 def create_graph(data):
     all_nodes=rewrite_to_node.rewrite_data(data)
     return graphviz_nodes.create_graph(all_nodes)
 
 def show(data,block=False):
```

### Comparing `memory_graph-0.1.8/memory_graph/graphviz_nodes.py` & `memory_graph-0.1.9/memory_graph/graphviz_nodes.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.8/memory_graph/rewrite.py` & `memory_graph-0.1.9/memory_graph/rewrite.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                 add_to_iterable_fun(new_iterable,rewrite(i))
     return new_iterable
 
 def rewrite_dict(dictionary):
     new_iterable,is_just_constructed=remember_or_construct_iterable(dictionary)
     if is_just_constructed:
         for key in dictionary:
-            if not type(key) or not is_dunder_name(key):
+            if not type(key) is str or not is_dunder_name(key):
                 if not is_ignore_type(key):
                     value=dictionary[key]
                     if not is_ignore_type(value):
                         add_to_iterable_fun(new_iterable,rewrite(key))
                         add_to_iterable_fun(new_iterable,rewrite(value))
     return new_iterable
 
@@ -111,15 +111,15 @@
     new_iterable,is_just_constructed=remember_or_construct_iterable(obj)
     if is_just_constructed:
         add_to_iterable_fun(new_iterable,rewrite(get_dict_attribute(obj)))
     return new_iterable
 
 def rewrite(data):
     if is_ignore_type(data):
-        rewrite_singular("ignore_type")
+        return rewrite_singular("ignore_type")
     elif type(data) is types.NoneType:
         return rewrite_singular("None") # special case, make a string because value 'None' is later used for not-specified in this software
     elif is_singular_type(data):
         return rewrite_singular(data)
     elif is_linear_type(data):
         return rewrite_iterable(data)
     elif is_dict_type(data):
```

### Comparing `memory_graph-0.1.8/memory_graph/rewrite_to_node.py` & `memory_graph-0.1.9/memory_graph/rewrite_to_node.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.8/memory_graph/rewrite_to_string.py` & `memory_graph-0.1.9/memory_graph/rewrite_to_string.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.8/memory_graph.egg-info/PKG-INFO` & `memory_graph-0.1.9/memory_graph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory-graph
-Version: 0.1.8
+Version: 0.1.9
 Summary: Draw a graph of your data to see the structure of its references.
 Home-page: https://github.com/bterwijn/memory_graph
 Author: Bas Terwijn
 Author-email: bterwijn@gmail.com
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `memory_graph-0.1.8/setup.py` & `memory_graph-0.1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description_from_readme = (this_directory / "README.md").read_text()
 
 setup(
     name = 'memory_graph',
-    version = '0.1.8',
+    version = '0.1.9',
     description = 'Draw a graph of your data to see the structure of its references.',
     long_description = long_description_from_readme,
     long_description_content_type = 'text/markdown',
     readme = 'README.md',
     url = 'https://github.com/bterwijn/memory_graph',
     author = 'Bas Terwijn',
     author_email = 'bterwijn@gmail.com',
```

