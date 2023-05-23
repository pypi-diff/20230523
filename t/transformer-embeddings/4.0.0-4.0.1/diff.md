# Comparing `tmp/transformer_embeddings-4.0.0.tar.gz` & `tmp/transformer_embeddings-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformer_embeddings-4.0.0.tar", max compression
+gzip compressed data, was "transformer_embeddings-4.0.1.tar", max compression
```

## Comparing `transformer_embeddings-4.0.0.tar` & `transformer_embeddings-4.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11334 2023-03-28 00:03:45.690806 transformer_embeddings-4.0.0/LICENSE
--rw-r--r--   0        0        0     5529 2023-03-28 00:03:45.690806 transformer_embeddings-4.0.0/README.md
--rw-r--r--   0        0        0     1833 2023-03-28 00:04:04.052140 transformer_embeddings-4.0.0/pyproject.toml
--rw-r--r--   0        0        0      192 2023-03-28 00:04:04.032138 transformer_embeddings-4.0.0/src/transformer_embeddings/__init__.py
--rw-r--r--   0        0        0     2100 2023-03-28 00:03:45.690806 transformer_embeddings-4.0.0/src/transformer_embeddings/helpers.py
--rw-r--r--   0        0        0    11612 2023-03-28 00:03:45.690806 transformer_embeddings-4.0.0/src/transformer_embeddings/model.py
--rw-r--r--   0        0        0     1828 2023-03-28 00:03:45.690806 transformer_embeddings-4.0.0/src/transformer_embeddings/poolers.py
--rw-r--r--   0        0        0     6579 1970-01-01 00:00:00.000000 transformer_embeddings-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-05-23 15:08:44.693585 transformer_embeddings-4.0.1/LICENSE
+-rw-r--r--   0        0        0     5529 2023-05-23 15:08:44.693585 transformer_embeddings-4.0.1/README.md
+-rw-r--r--   0        0        0     1833 2023-05-23 15:09:07.689742 transformer_embeddings-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0      192 2023-05-23 15:09:07.669742 transformer_embeddings-4.0.1/src/transformer_embeddings/__init__.py
+-rw-r--r--   0        0        0     2100 2023-05-23 15:08:44.693585 transformer_embeddings-4.0.1/src/transformer_embeddings/helpers.py
+-rw-r--r--   0        0        0    11612 2023-05-23 15:08:44.693585 transformer_embeddings-4.0.1/src/transformer_embeddings/model.py
+-rw-r--r--   0        0        0     1828 2023-05-23 15:08:44.693585 transformer_embeddings-4.0.1/src/transformer_embeddings/poolers.py
+-rw-r--r--   0        0        0     6579 1970-01-01 00:00:00.000000 transformer_embeddings-4.0.1/PKG-INFO
```

### Comparing `transformer_embeddings-4.0.0/LICENSE` & `transformer_embeddings-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `transformer_embeddings-4.0.0/README.md` & `transformer_embeddings-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `transformer_embeddings-4.0.0/pyproject.toml` & `transformer_embeddings-4.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "transformer-embeddings"
-version = "4.0.0"
+version = "4.0.1"
 description = "Transformer Embeddings"
 authors = ["Headspace Health <transformer-embeddings@headspace.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/ginger-io/transformer-embeddings"
 repository = "https://github.com/ginger-io/transformer-embeddings"
 documentation = "https://github.com/ginger-io/transformer-embeddings"
```

### Comparing `transformer_embeddings-4.0.0/src/transformer_embeddings/helpers.py` & `transformer_embeddings-4.0.1/src/transformer_embeddings/helpers.py`

 * *Files identical despite different names*

### Comparing `transformer_embeddings-4.0.0/src/transformer_embeddings/model.py` & `transformer_embeddings-4.0.1/src/transformer_embeddings/model.py`

 * *Files identical despite different names*

### Comparing `transformer_embeddings-4.0.0/src/transformer_embeddings/poolers.py` & `transformer_embeddings-4.0.1/src/transformer_embeddings/poolers.py`

 * *Files identical despite different names*

### Comparing `transformer_embeddings-4.0.0/PKG-INFO` & `transformer_embeddings-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformer-embeddings
-Version: 4.0.0
+Version: 4.0.1
 Summary: Transformer Embeddings
 Home-page: https://github.com/ginger-io/transformer-embeddings
 License: Apache-2.0
 Author: Headspace Health
 Author-email: transformer-embeddings@headspace.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 5 - Production/Stable
```

