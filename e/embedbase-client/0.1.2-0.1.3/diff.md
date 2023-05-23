# Comparing `tmp/embedbase_client-0.1.2.tar.gz` & `tmp/embedbase_client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase_client-0.1.2.tar", max compression
+gzip compressed data, was "embedbase_client-0.1.3.tar", max compression
```

## Comparing `embedbase_client-0.1.2.tar` & `embedbase_client-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1077 2023-04-17 09:49:08.973283 embedbase_client-0.1.2/LICENSE
--rw-r--r--   0        0        0     1005 2023-05-12 15:05:38.517672 embedbase_client-0.1.2/README.md
--rw-r--r--   0        0        0      389 2023-05-20 14:15:09.469578 embedbase_client-0.1.2/embedbase_client/__init__.py
--rw-r--r--   0        0        0    15456 2023-05-20 17:11:14.788117 embedbase_client-0.1.2/embedbase_client/async_client.py
--rw-r--r--   0        0        0      913 2023-05-20 14:34:00.754341 embedbase_client-0.1.2/embedbase_client/base.py
--rw-r--r--   0        0        0       49 2023-05-20 14:19:44.624286 embedbase_client-0.1.2/embedbase_client/errors.py
--rw-r--r--   0        0        0     1752 2023-05-20 17:09:16.553457 embedbase_client-0.1.2/embedbase_client/model.py
--rw-r--r--   0        0        0     3388 2023-05-20 15:24:12.182673 embedbase_client-0.1.2/embedbase_client/split.py
--rw-r--r--   0        0        0    15373 2023-05-20 17:10:36.174358 embedbase_client-0.1.2/embedbase_client/sync_client.py
--rw-r--r--   0        0        0     1237 2023-05-20 17:05:35.334443 embedbase_client-0.1.2/embedbase_client/utils.py
--rw-r--r--   0        0        0     3516 2023-05-20 17:11:33.720202 embedbase_client-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2261 1970-01-01 00:00:00.000000 embedbase_client-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-23 15:09:22.788426 embedbase_client-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1005 2023-05-23 15:09:22.788426 embedbase_client-0.1.3/README.md
+-rw-r--r--   0        0        0      389 2023-05-23 15:09:22.788426 embedbase_client-0.1.3/embedbase_client/__init__.py
+-rw-r--r--   0        0        0    15456 2023-05-23 15:09:22.788426 embedbase_client-0.1.3/embedbase_client/async_client.py
+-rw-r--r--   0        0        0      913 2023-05-23 15:09:22.788426 embedbase_client-0.1.3/embedbase_client/base.py
+-rw-r--r--   0        0        0     1194 2023-05-23 15:09:22.788426 embedbase_client-0.1.3/embedbase_client/errors.py
+-rw-r--r--   0        0        0     1694 2023-05-23 15:09:22.788426 embedbase_client-0.1.3/embedbase_client/model.py
+-rw-r--r--   0        0        0     3388 2023-05-23 15:09:22.788426 embedbase_client-0.1.3/embedbase_client/split.py
+-rw-r--r--   0        0        0    15373 2023-05-23 15:09:22.788426 embedbase_client-0.1.3/embedbase_client/sync_client.py
+-rw-r--r--   0        0        0     2051 2023-05-23 15:09:22.788426 embedbase_client-0.1.3/embedbase_client/utils.py
+-rw-r--r--   0        0        0     3516 2023-05-23 15:09:22.788426 embedbase_client-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2062 1970-01-01 00:00:00.000000 embedbase_client-0.1.3/PKG-INFO
```

### Comparing `embedbase_client-0.1.2/LICENSE` & `embedbase_client-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.2/README.md` & `embedbase_client-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.2/embedbase_client/async_client.py` & `embedbase_client-0.1.3/embedbase_client/async_client.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.2/embedbase_client/base.py` & `embedbase_client-0.1.3/embedbase_client/base.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.2/embedbase_client/model.py` & `embedbase_client-0.1.3/embedbase_client/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from typing import Any, Dict, List, Literal, Optional
-
+from typing import Any, Dict, List, Optional
 from pydantic import BaseModel, Extra
 
 
 class Metadata(BaseModel):
     path: Optional[str]
 
     def __getitem__(self, key: str) -> Any:
@@ -68,17 +67,15 @@
 
 
 class AddData(BaseModel):
     results: Optional[List[AddDataResult]]
     error: Optional[str]
 
 
-Role = Literal["user", "system", "assistant"]
-
 
 class Chat(BaseModel):
-    role: Role
+    role: str
     content: str
 
 
 class GenerateOptions(BaseModel):
     history: List[Chat]
```

### Comparing `embedbase_client-0.1.2/embedbase_client/split.py` & `embedbase_client-0.1.3/embedbase_client/split.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.2/embedbase_client/sync_client.py` & `embedbase_client-0.1.3/embedbase_client/sync_client.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.2/pyproject.toml` & `embedbase_client-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase-client"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python client for Embedbase"
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py"
 homepage = "https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py"
 
@@ -48,16 +48,16 @@
 pytest = "^7.3.1"
 pyupgrade = "^2.29.1"
 safety = "^1.10.3"
 coverage = "^6.1.2"
 coverage-badge = "^1.1.0"
 pytest-html = "^3.1.1"
 pytest-cov = "^3.0.0"
-embedbase = "^1.1.9"
 pytest-asyncio = "^0.21.0"
+embedbase = "^1.2.0"
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py38"]
 line-length = 88
 color = true
```

### Comparing `embedbase_client-0.1.2/PKG-INFO` & `embedbase_client-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python client for Embedbase
 Home-page: https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence,llm
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
@@ -12,18 +12,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Project-URL: Repository, https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,24 +1,22 @@
-Metadata-Version: 2.1 Name: embedbase-client Version: 0.1.2 Summary: Python
+Metadata-Version: 2.1 Name: embedbase-client Version: 0.1.3 Summary: Python
 client for Embedbase Home-page: https://github.com/different-ai/embedbase/tree/
 main/sdk/embedbase-py License: MIT Keywords: embeddings,machine
 learning,artificial intelligence,llm Author: Different AI Author-email:
 louis@embedbase.xyz Requires-Python: >=3.8,<4.0 Classifier: Development Status
 :: 4 - Beta Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Requires-Dist: httpx (>=0.24.0,<0.25.0) Requires-Dist:
-pydantic (>=1.10.7,<2.0.0) Requires-Dist: tiktoken (>=0.3.3,<0.4.0) Project-
-URL: Repository, https://github.com/different-ai/embedbase/tree/main/sdk/
-embedbase-py Description-Content-Type: text/markdown # embedbase-py
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Requires-Dist: httpx
+(>=0.24.0,<0.25.0) Requires-Dist: pydantic (>=1.10.7,<2.0.0) Requires-Dist:
+tiktoken (>=0.3.3,<0.4.0) Project-URL: Repository, https://github.com/
+different-ai/embedbase/tree/main/sdk/embedbase-py Description-Content-Type:
+text/markdown # embedbase-py
  Embedbase-py - Python client for [Embedbase](https://github.com/different-ai/
                                   embedbase)
 
                      â ï¸ Status: Alpha release â ï¸
 
   [Discord] [![Code style: black](https://img.shields.io/badge/code%20style-
      black-000000.svg)](https://github.com/psf/black) [![License](https://
```

