# Comparing `tmp/nlp_service-1.4.0.tar.gz` & `tmp/nlp_service-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp_service-1.4.0.tar", max compression
+gzip compressed data, was "nlp_service-1.4.1.tar", max compression
```

## Comparing `nlp_service-1.4.0.tar` & `nlp_service-1.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-04-10 13:54:39.508267 nlp_service-1.4.0/LICENSE
--rw-r--r--   0        0        0     8218 2023-04-10 13:54:39.508267 nlp_service-1.4.0/README.md
--rw-r--r--   0        0        0      226 2023-04-10 13:54:39.508267 nlp_service-1.4.0/nlp_service/__init__.py
--rw-r--r--   0        0        0       42 2023-04-10 13:54:39.508267 nlp_service-1.4.0/nlp_service/__main__.py
--rw-r--r--   0        0        0     2259 2023-04-10 13:54:39.508267 nlp_service-1.4.0/nlp_service/client.py
--rw-r--r--   0        0        0    10441 2023-04-10 13:54:39.508267 nlp_service-1.4.0/nlp_service/infersent.py
--rw-r--r--   0        0        0        0 2023-04-10 13:54:39.508267 nlp_service-1.4.0/nlp_service/py.typed
--rw-r--r--   0        0        0    15633 2023-04-10 13:54:39.508267 nlp_service-1.4.0/nlp_service/server.py
--rw-r--r--   0        0        0     9147 2023-04-10 13:54:39.508267 nlp_service-1.4.0/nlp_service/similarity.py
--rw-r--r--   0        0        0      344 2023-04-10 13:54:39.508267 nlp_service-1.4.0/nlp_service/typing.py
--rw-r--r--   0        0        0     1509 2023-04-10 13:55:12.393848 nlp_service-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     9982 1970-01-01 00:00:00.000000 nlp_service-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-23 20:47:25.026725 nlp_service-1.4.1/LICENSE
+-rw-r--r--   0        0        0     8218 2023-05-23 20:47:25.030725 nlp_service-1.4.1/README.md
+-rw-r--r--   0        0        0      226 2023-05-23 20:47:25.030725 nlp_service-1.4.1/nlp_service/__init__.py
+-rw-r--r--   0        0        0       42 2023-05-23 20:47:25.030725 nlp_service-1.4.1/nlp_service/__main__.py
+-rw-r--r--   0        0        0     2259 2023-05-23 20:47:25.030725 nlp_service-1.4.1/nlp_service/client.py
+-rw-r--r--   0        0        0    10441 2023-05-23 20:47:25.030725 nlp_service-1.4.1/nlp_service/infersent.py
+-rw-r--r--   0        0        0        0 2023-05-23 20:47:25.030725 nlp_service-1.4.1/nlp_service/py.typed
+-rw-r--r--   0        0        0    15629 2023-05-23 20:47:25.030725 nlp_service-1.4.1/nlp_service/server.py
+-rw-r--r--   0        0        0     9147 2023-05-23 20:47:25.030725 nlp_service-1.4.1/nlp_service/similarity.py
+-rw-r--r--   0        0        0      344 2023-05-23 20:47:25.030725 nlp_service-1.4.1/nlp_service/typing.py
+-rw-r--r--   0        0        0     1519 2023-05-23 20:47:56.247040 nlp_service-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     9983 1970-01-01 00:00:00.000000 nlp_service-1.4.1/PKG-INFO
```

### Comparing `nlp_service-1.4.0/LICENSE` & `nlp_service-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.0/README.md` & `nlp_service-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.0/nlp_service/client.py` & `nlp_service-1.4.1/nlp_service/client.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.0/nlp_service/infersent.py` & `nlp_service-1.4.1/nlp_service/infersent.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.0/nlp_service/server.py` & `nlp_service-1.4.1/nlp_service/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,17 +172,17 @@
         def vector(self, text: str) -> SpacyVector:
             embeddings = t.cast(
                 NumpyVector, self.model.encode([text], convert_to_numpy=True)
             )
 
             return embeddings[0]
 
-    embedding_map[nlp_pb2.EmbeddingType.EMBEDDING_TYPE_SENTENCE_TRANSFORMERS] = (
-        SentenceTransformersModel
-    )
+    embedding_map[
+        nlp_pb2.EmbeddingType.EMBEDDING_TYPE_SENTENCE_TRANSFORMERS
+    ] = SentenceTransformersModel
 
 except ModuleNotFoundError:
     log.info("'sentence-transformers' not installed.")
 
 
 try:
     import tensorflow_hub as hub
@@ -192,17 +192,17 @@
             self.model: t.Any = hub.load(model.model_name)
 
         def vector(self, text: str) -> SpacyVector:
             embeddings: t.Sequence[t.Any] = self.model([text])
 
             return embeddings[0].numpy()
 
-    embedding_map[nlp_pb2.EmbeddingType.EMBEDDING_TYPE_TENSORFLOW_HUB] = (
-        TensorflowHubModel
-    )
+    embedding_map[
+        nlp_pb2.EmbeddingType.EMBEDDING_TYPE_TENSORFLOW_HUB
+    ] = TensorflowHubModel
 
 except ModuleNotFoundError:
     log.info("'tensorflow-hub' not installed.")
 
 
 try:
     import openai
```

### Comparing `nlp_service-1.4.0/nlp_service/similarity.py` & `nlp_service-1.4.1/nlp_service/similarity.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.0/pyproject.toml` & `nlp_service-1.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 [tool.poetry]
 name = "nlp-service"
-version = "1.4.0"
+version = "1.4.1"
 description = "Microservice for NLP tasks using gRPC"
 authors = ["Mirko Lenz <info@mirko-lenz.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://recap.uni-trier.de"
 repository = "https://github.com/recap-utr/nlp-service"
 packages = [{ include = "nlp_service" }]
 
 [tool.poetry.scripts]
 nlp-service = "nlp_service.server:app"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.12"
 numpy = "^1.23.5"
-scipy = "^1.9.3"
-spacy = "^3.5.1"
-arg-services = "^1.3.0"
+scipy = "^1.10.1"
+spacy = "^3.5.3"
+arg-services = "^1.3.1"
 nltk = "^3.8.1"
 nptyping = "^2.5.0"
-mashumaro = "^3.6"
-typer = "^0.7.0"
+mashumaro = "^3.7"
+typer = ">=0.7.0, <1.0.0"
 gensim = { version = "^4.3.1", optional = true }
-python-Levenshtein = { version = "^0.20.9", optional = true }
+python-Levenshtein = { version = "^0.21.0", optional = true }
 sentence-transformers = { version = "^2.2.2", optional = true }
 torch = { version = ">=1.13.1, <3.0", optional = true }
-transformers = { version = "^4.27.4", optional = true }
+transformers = { version = "^4.29.2", optional = true }
 tensorflow = { version = "^2.12.0", optional = true }
 tensorflow-hub = { version = "^0.13.0", optional = true }
-openai = { version = "^0.27.2", optional = true }
+openai = { version = "^0.27.7", optional = true }
 
 [tool.poetry.extras]
 wmd = ["gensim"]
 levenshtein = ["python-Levenshtein"]
 sentence-transformers = ["sentence-transformers", "torch"]
 transformers = ["transformers", "torch"]
 tensorflow = ["tensorflow", "tensorflow-hub"]
```

### Comparing `nlp_service-1.4.0/PKG-INFO` & `nlp_service-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-service
-Version: 1.4.0
+Version: 1.4.1
 Summary: Microservice for NLP tasks using gRPC
 Home-page: http://recap.uni-trier.de
 License: MIT
 Author: Mirko Lenz
 Author-email: info@mirko-lenz.de
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -14,30 +14,30 @@
 Provides-Extra: all
 Provides-Extra: levenshtein
 Provides-Extra: openai
 Provides-Extra: sentence-transformers
 Provides-Extra: tensorflow
 Provides-Extra: transformers
 Provides-Extra: wmd
-Requires-Dist: arg-services (>=1.3.0,<2.0.0)
+Requires-Dist: arg-services (>=1.3.1,<2.0.0)
 Requires-Dist: gensim (>=4.3.1,<5.0.0) ; extra == "wmd" or extra == "all"
-Requires-Dist: mashumaro (>=3.6,<4.0)
+Requires-Dist: mashumaro (>=3.7,<4.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: nptyping (>=2.5.0,<3.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
-Requires-Dist: openai (>=0.27.2,<0.28.0) ; extra == "openai" or extra == "all"
-Requires-Dist: python-Levenshtein (>=0.20.9,<0.21.0) ; extra == "levenshtein" or extra == "all"
-Requires-Dist: scipy (>=1.9.3,<2.0.0)
+Requires-Dist: openai (>=0.27.7,<0.28.0) ; extra == "openai" or extra == "all"
+Requires-Dist: python-Levenshtein (>=0.21.0,<0.22.0) ; extra == "levenshtein" or extra == "all"
+Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0) ; extra == "sentence-transformers" or extra == "all"
-Requires-Dist: spacy (>=3.5.1,<4.0.0)
+Requires-Dist: spacy (>=3.5.3,<4.0.0)
 Requires-Dist: tensorflow (>=2.12.0,<3.0.0) ; extra == "tensorflow" or extra == "all"
 Requires-Dist: tensorflow-hub (>=0.13.0,<0.14.0) ; extra == "tensorflow"
 Requires-Dist: torch (>=1.13.1,<3.0) ; extra == "sentence-transformers" or extra == "transformers" or extra == "all"
-Requires-Dist: transformers (>=4.27.4,<5.0.0) ; extra == "transformers" or extra == "all"
-Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: transformers (>=4.29.2,<5.0.0) ; extra == "transformers" or extra == "all"
+Requires-Dist: typer (>=0.7.0,<1.0.0)
 Project-URL: Repository, https://github.com/recap-utr/nlp-service
 Description-Content-Type: text/markdown
 
 # NLP Microservice
 
 The goal of this project is to provide a [gRPC](https://grpc.io) server for resource-heavy NLP tasks&mdash;for instance, computing vectors/embeddings for words or sentences.
 By using [protobuf](https://developers.google.com/protocol-buffers) internally, our NLP server provides native and strongly typed interfaces for many programming languages.
```

