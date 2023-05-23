# Comparing `tmp/fluss-0.1.8.tar.gz` & `tmp/fluss-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluss-0.1.8.tar", max compression
+gzip compressed data, was "fluss-0.1.9.tar", max compression
```

## Comparing `fluss-0.1.8.tar` & `fluss-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0       55 2021-09-15 12:18:44.843141 fluss-0.1.8/fluss/__init__.py
--rw-r--r--   0        0        0      211 2021-09-15 12:46:19.667176 fluss-0.1.8/fluss/convenience.py
--rw-r--r--   0        0        0     3316 2021-09-20 10:52:11.624293 fluss-0.1.8/fluss/diagram.py
--rw-r--r--   0        0        0        0 2021-09-15 13:17:00.787458 fluss-0.1.8/fluss/graphql/__init__.py
--rw-r--r--   0        0        0      150 2021-09-15 13:17:12.723458 fluss-0.1.8/fluss/graphql/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0        0 2021-09-15 13:17:00.791458 fluss-0.1.8/fluss/graphql/mutations/__init__.py
--rw-r--r--   0        0        0      160 2021-09-15 13:17:12.723458 fluss-0.1.8/fluss/graphql/mutations/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      461 2021-09-16 08:36:59.524351 fluss-0.1.8/fluss/graphql/mutations/__pycache__/metric.cpython-38.pyc
--rw-r--r--   0        0        0      780 2021-09-15 13:17:12.723458 fluss-0.1.8/fluss/graphql/mutations/__pycache__/representation.cpython-38.pyc
--rw-r--r--   0        0        0      484 2021-09-15 13:17:12.727458 fluss-0.1.8/fluss/graphql/mutations/__pycache__/sample.cpython-38.pyc
--rw-r--r--   0        0        0        0 2021-09-15 13:17:00.791458 fluss-0.1.8/fluss/graphql/queries/__init__.py
--rw-r--r--   0        0        0      158 2021-09-15 13:17:12.727458 fluss-0.1.8/fluss/graphql/queries/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      342 2021-09-15 13:17:13.003458 fluss-0.1.8/fluss/graphql/queries/__pycache__/experiment.cpython-38.pyc
--rw-r--r--   0        0        0      373 2021-09-17 09:01:50.042755 fluss-0.1.8/fluss/graphql/queries/__pycache__/graph.cpython-38.pyc
--rw-r--r--   0        0        0      374 2021-09-16 08:36:59.524351 fluss-0.1.8/fluss/graphql/queries/__pycache__/metric.cpython-38.pyc
--rw-r--r--   0        0        0      687 2021-09-15 13:17:13.003458 fluss-0.1.8/fluss/graphql/queries/__pycache__/representation.cpython-38.pyc
--rw-r--r--   0        0        0      535 2021-09-15 13:17:12.727458 fluss-0.1.8/fluss/graphql/queries/__pycache__/sample.cpython-38.pyc
--rw-r--r--   0        0        0      223 2021-09-17 09:01:47.298758 fluss-0.1.8/fluss/graphql/queries/graph.py
--rw-r--r--   0        0        0      642 2021-09-16 13:28:09.302199 fluss-0.1.8/fluss/schema.py
--rw-r--r--   0        0        0      584 2021-10-08 12:37:27.844580 fluss-0.1.8/fluss/ward.py
--rw-r--r--   0        0        0      766 2021-09-15 12:18:37.139141 fluss-0.1.8/fluss/widgets.py
--rw-r--r--   0        0        0      404 2021-10-08 15:48:50.164864 fluss-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      666 2021-10-08 15:48:50.468946 fluss-0.1.8/setup.py
--rw-r--r--   0        0        0      362 2021-10-08 15:48:50.469092 fluss-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       43 2021-10-21 08:17:50.149299 fluss-0.1.9/fluss/__init__.py
+-rw-r--r--   0        0        0      211 2021-09-15 12:46:19.667176 fluss-0.1.9/fluss/convenience.py
+-rw-r--r--   0        0        0     3316 2021-09-20 10:52:11.624293 fluss-0.1.9/fluss/diagram.py
+-rw-r--r--   0        0        0        0 2021-09-15 13:17:00.787458 fluss-0.1.9/fluss/graphql/__init__.py
+-rw-r--r--   0        0        0      150 2021-09-15 13:17:12.723458 fluss-0.1.9/fluss/graphql/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2021-09-15 13:17:00.791458 fluss-0.1.9/fluss/graphql/mutations/__init__.py
+-rw-r--r--   0        0        0      160 2021-09-15 13:17:12.723458 fluss-0.1.9/fluss/graphql/mutations/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      461 2021-09-16 08:36:59.524351 fluss-0.1.9/fluss/graphql/mutations/__pycache__/metric.cpython-38.pyc
+-rw-r--r--   0        0        0      780 2021-09-15 13:17:12.723458 fluss-0.1.9/fluss/graphql/mutations/__pycache__/representation.cpython-38.pyc
+-rw-r--r--   0        0        0      484 2021-09-15 13:17:12.727458 fluss-0.1.9/fluss/graphql/mutations/__pycache__/sample.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2021-09-15 13:17:00.791458 fluss-0.1.9/fluss/graphql/queries/__init__.py
+-rw-r--r--   0        0        0      158 2021-09-15 13:17:12.727458 fluss-0.1.9/fluss/graphql/queries/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      342 2021-09-15 13:17:13.003458 fluss-0.1.9/fluss/graphql/queries/__pycache__/experiment.cpython-38.pyc
+-rw-r--r--   0        0        0      373 2021-09-17 09:01:50.042755 fluss-0.1.9/fluss/graphql/queries/__pycache__/graph.cpython-38.pyc
+-rw-r--r--   0        0        0      374 2021-09-16 08:36:59.524351 fluss-0.1.9/fluss/graphql/queries/__pycache__/metric.cpython-38.pyc
+-rw-r--r--   0        0        0      687 2021-09-15 13:17:13.003458 fluss-0.1.9/fluss/graphql/queries/__pycache__/representation.cpython-38.pyc
+-rw-r--r--   0        0        0      535 2021-09-15 13:17:12.727458 fluss-0.1.9/fluss/graphql/queries/__pycache__/sample.cpython-38.pyc
+-rw-r--r--   0        0        0      223 2021-09-17 09:01:47.298758 fluss-0.1.9/fluss/graphql/queries/graph.py
+-rw-r--r--   0        0        0      642 2021-09-16 13:28:09.302199 fluss-0.1.9/fluss/schema.py
+-rw-r--r--   0        0        0      562 2021-10-21 08:40:18.920082 fluss-0.1.9/fluss/ward.py
+-rw-r--r--   0        0        0      406 2021-10-21 12:08:18.218163 fluss-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      668 2021-10-21 12:08:18.519109 fluss-0.1.9/setup.py
+-rw-r--r--   0        0        0      364 2021-10-21 12:08:18.519241 fluss-0.1.9/PKG-INFO
```

### Comparing `fluss-0.1.8/fluss/diagram.py` & `fluss-0.1.9/fluss/diagram.py`

 * *Files identical despite different names*

### Comparing `fluss-0.1.8/fluss/graphql/mutations/__pycache__/representation.cpython-38.pyc` & `fluss-0.1.9/fluss/graphql/mutations/__pycache__/representation.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fluss-0.1.8/fluss/graphql/queries/__pycache__/representation.cpython-38.pyc` & `fluss-0.1.9/fluss/graphql/queries/__pycache__/representation.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fluss-0.1.8/fluss/graphql/queries/__pycache__/sample.cpython-38.pyc` & `fluss-0.1.9/fluss/graphql/queries/__pycache__/sample.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fluss-0.1.8/fluss/schema.py` & `fluss-0.1.9/fluss/schema.py`

 * *Files identical despite different names*

### Comparing `fluss-0.1.8/setup.py` & `fluss-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['fluss', 'fluss.graphql', 'fluss.graphql.mutations', 'fluss.graphql.queries']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['arkitekt>=0.1.6,<0.2.0', 'herre>=0.1.5,<0.2.0']
+['arkitekt>=0.1.48,<0.2.0', 'herre>=0.1.28,<0.2.0']
 
 setup_kwargs = {
     'name': 'fluss',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': None,
     'author': 'jhnnsrs',
     'author_email': 'jhnnsrs@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

