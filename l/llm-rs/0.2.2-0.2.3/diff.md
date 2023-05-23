# Comparing `tmp/llm_rs-0.2.2.tar.gz` & `tmp/llm_rs-0.2.3.tar.gz`

## Comparing `llm_rs-0.2.2.tar` & `llm_rs-0.2.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 llm_rs-0.2.2/Cargo.toml
--rw-r--r--   0     1001      123      610 2023-05-23 15:15:11.000000 llm_rs-0.2.2/.github/workflows/BuildDoc.yml
--rw-r--r--   0     1001      123     2796 2023-05-23 15:15:11.000000 llm_rs-0.2.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      564 2023-05-23 15:15:11.000000 llm_rs-0.2.2/.github/workflows/Clippy.yml
--rw-r--r--   0     1001      123      602 2023-05-23 15:15:11.000000 llm_rs-0.2.2/.github/workflows/PublishDocs.yml
--rw-r--r--   0     1001      123     3455 2023-05-23 15:15:11.000000 llm_rs-0.2.2/.gitignore
--rw-r--r--   0     1001      123       72 2023-05-23 15:15:11.000000 llm_rs-0.2.2/.vscode/settings.json
--rw-r--r--   0     1001      123     1071 2023-05-23 15:15:11.000000 llm_rs-0.2.2/LICENSE
--rw-r--r--   0     1001      123     2192 2023-05-23 15:15:11.000000 llm_rs-0.2.2/README.md
--rw-r--r--   0     1001      123     4799 2023-05-23 15:15:11.000000 llm_rs-0.2.2/docs/docs/conversion.md
--rw-r--r--   0     1001      123     9355 2023-05-23 15:15:11.000000 llm_rs-0.2.2/docs/docs/index.md
--rw-r--r--   0     1001      123     1181 2023-05-23 15:15:11.000000 llm_rs-0.2.2/docs/mkdocs.yml
--rw-r--r--   0     1001      123       31 2023-05-23 15:15:11.000000 llm_rs-0.2.2/docs/requirements.txt
--rw-r--r--   0     1001      123      334 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/__init__.py
--rw-r--r--   0     1001      123     6112 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/auto.py
--rw-r--r--   0     1001      123     1614 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/base_model.py
--rw-r--r--   0     1001      123     1351 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/config.pyi
--rw-r--r--   0     1001      123       78 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/convert/__init__.py
--rw-r--r--   0     1001      123     2223 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/convert/auto_converter.py
--rw-r--r--   0     1001      123      199 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/convert/models/__init__.py
--rw-r--r--   0     1001      123     5581 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/convert/models/_base.py
--rw-r--r--   0     1001      123     3177 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/convert/models/bloom.py
--rw-r--r--   0     1001      123     5221 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/convert/models/gpt2.py
--rw-r--r--   0     1001      123     2032 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/convert/models/gptj.py
--rw-r--r--   0     1001      123     2138 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/convert/models/gptneox.py
--rw-r--r--   0     1001      123     6334 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/convert/models/llama.py
--rw-r--r--   0     1001      123     1893 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/convert/models/mpt.py
--rw-r--r--   0     1001      123        0 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/llm_rs.pyi
--rw-r--r--   0     1001      123      579 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/models.pyi
--rw-r--r--   0     1001      123        0 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/py.typed
--rw-r--r--   0     1001      123      697 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/results.pyi
--rw-r--r--   0     1001      123      978 2023-05-23 15:15:11.000000 llm_rs-0.2.2/pyproject.toml
--rw-r--r--   0     1001      123     4274 2023-05-23 15:15:11.000000 llm_rs-0.2.2/src/configs.rs
--rw-r--r--   0     1001      123     1685 2023-05-23 15:15:11.000000 llm_rs-0.2.2/src/lib.rs
--rw-r--r--   0     1001      123     9658 2023-05-23 15:15:11.000000 llm_rs-0.2.2/src/model_base.rs
--rw-r--r--   0     1001      123      300 2023-05-23 15:15:11.000000 llm_rs-0.2.2/src/models.rs
--rw-r--r--   0     1001      123     2576 2023-05-23 15:15:11.000000 llm_rs-0.2.2/src/quantize.rs
--rw-r--r--   0     1001      123     1352 2023-05-23 15:15:11.000000 llm_rs-0.2.2/src/results.rs
--rw-r--r--   0     1001      123    20589 2023-05-23 15:16:44.000000 llm_rs-0.2.2/Cargo.lock
--rw-r--r--   0        0        0     3289 1970-01-01 00:00:00.000000 llm_rs-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 llm_rs-0.2.3/Cargo.toml
+-rw-r--r--   0     1001      123      610 2023-05-23 15:43:19.000000 llm_rs-0.2.3/.github/workflows/BuildDoc.yml
+-rw-r--r--   0     1001      123     2796 2023-05-23 15:43:19.000000 llm_rs-0.2.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      564 2023-05-23 15:43:19.000000 llm_rs-0.2.3/.github/workflows/Clippy.yml
+-rw-r--r--   0     1001      123      602 2023-05-23 15:43:19.000000 llm_rs-0.2.3/.github/workflows/PublishDocs.yml
+-rw-r--r--   0     1001      123     3455 2023-05-23 15:43:19.000000 llm_rs-0.2.3/.gitignore
+-rw-r--r--   0     1001      123       72 2023-05-23 15:43:19.000000 llm_rs-0.2.3/.vscode/settings.json
+-rw-r--r--   0     1001      123     1071 2023-05-23 15:43:19.000000 llm_rs-0.2.3/LICENSE
+-rw-r--r--   0     1001      123     2192 2023-05-23 15:43:19.000000 llm_rs-0.2.3/README.md
+-rw-r--r--   0     1001      123     4799 2023-05-23 15:43:19.000000 llm_rs-0.2.3/docs/docs/conversion.md
+-rw-r--r--   0     1001      123     9355 2023-05-23 15:43:19.000000 llm_rs-0.2.3/docs/docs/index.md
+-rw-r--r--   0     1001      123     1181 2023-05-23 15:43:19.000000 llm_rs-0.2.3/docs/mkdocs.yml
+-rw-r--r--   0     1001      123       31 2023-05-23 15:43:19.000000 llm_rs-0.2.3/docs/requirements.txt
+-rw-r--r--   0     1001      123      334 2023-05-23 15:43:19.000000 llm_rs-0.2.3/llm_rs/__init__.py
+-rw-r--r--   0     1001      123     6081 2023-05-23 15:43:19.000000 llm_rs-0.2.3/llm_rs/auto.py
+-rw-r--r--   0     1001      123     1614 2023-05-23 15:43:19.000000 llm_rs-0.2.3/llm_rs/base_model.py
+-rw-r--r--   0     1001      123     1351 2023-05-23 15:43:19.000000 llm_rs-0.2.3/llm_rs/config.pyi
+-rw-r--r--   0     1001      123       78 2023-05-23 15:43:19.000000 llm_rs-0.2.3/llm_rs/convert/__init__.py
+-rw-r--r--   0     1001      123     2223 2023-05-23 15:43:19.000000 llm_rs-0.2.3/llm_rs/convert/auto_converter.py
+-rw-r--r--   0     1001      123      199 2023-05-23 15:43:19.000000 llm_rs-0.2.3/llm_rs/convert/models/__init__.py
+-rw-r--r--   0     1001      123     5581 2023-05-23 15:43:19.000000 llm_rs-0.2.3/llm_rs/convert/models/_base.py
+-rw-r--r--   0     1001      123     3177 2023-05-23 15:43:19.000000 llm_rs-0.2.3/llm_rs/convert/models/bloom.py
+-rw-r--r--   0     1001      123     5221 2023-05-23 15:43:19.000000 llm_rs-0.2.3/llm_rs/convert/models/gpt2.py
+-rw-r--r--   0     1001      123     2032 2023-05-23 15:43:19.000000 llm_rs-0.2.3/llm_rs/convert/models/gptj.py
+-rw-r--r--   0     1001      123     2138 2023-05-23 15:43:19.000000 llm_rs-0.2.3/llm_rs/convert/models/gptneox.py
+-rw-r--r--   0     1001      123     6334 2023-05-23 15:43:19.000000 llm_rs-0.2.3/llm_rs/convert/models/llama.py
+-rw-r--r--   0     1001      123     1893 2023-05-23 15:43:19.000000 llm_rs-0.2.3/llm_rs/convert/models/mpt.py
+-rw-r--r--   0     1001      123        0 2023-05-23 15:43:19.000000 llm_rs-0.2.3/llm_rs/llm_rs.pyi
+-rw-r--r--   0     1001      123      579 2023-05-23 15:43:19.000000 llm_rs-0.2.3/llm_rs/models.pyi
+-rw-r--r--   0     1001      123        0 2023-05-23 15:43:19.000000 llm_rs-0.2.3/llm_rs/py.typed
+-rw-r--r--   0     1001      123      697 2023-05-23 15:43:19.000000 llm_rs-0.2.3/llm_rs/results.pyi
+-rw-r--r--   0     1001      123      978 2023-05-23 15:43:19.000000 llm_rs-0.2.3/pyproject.toml
+-rw-r--r--   0     1001      123     4274 2023-05-23 15:43:19.000000 llm_rs-0.2.3/src/configs.rs
+-rw-r--r--   0     1001      123     1685 2023-05-23 15:43:19.000000 llm_rs-0.2.3/src/lib.rs
+-rw-r--r--   0     1001      123     9658 2023-05-23 15:43:19.000000 llm_rs-0.2.3/src/model_base.rs
+-rw-r--r--   0     1001      123      300 2023-05-23 15:43:19.000000 llm_rs-0.2.3/src/models.rs
+-rw-r--r--   0     1001      123     2576 2023-05-23 15:43:19.000000 llm_rs-0.2.3/src/quantize.rs
+-rw-r--r--   0     1001      123     1352 2023-05-23 15:43:19.000000 llm_rs-0.2.3/src/results.rs
+-rw-r--r--   0     1001      123    20589 2023-05-23 15:44:49.000000 llm_rs-0.2.3/Cargo.lock
+-rw-r--r--   0        0        0     3289 1970-01-01 00:00:00.000000 llm_rs-0.2.3/PKG-INFO
```

### Comparing `llm_rs-0.2.2/.github/workflows/BuildDoc.yml` & `llm_rs-0.2.3/.github/workflows/BuildDoc.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/.github/workflows/CI.yml` & `llm_rs-0.2.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/.github/workflows/Clippy.yml` & `llm_rs-0.2.3/.github/workflows/Clippy.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/.github/workflows/PublishDocs.yml` & `llm_rs-0.2.3/.github/workflows/PublishDocs.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/.gitignore` & `llm_rs-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/LICENSE` & `llm_rs-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/README.md` & `llm_rs-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/docs/docs/conversion.md` & `llm_rs-0.2.3/docs/docs/conversion.md`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/docs/docs/index.md` & `llm_rs-0.2.3/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/docs/mkdocs.yml` & `llm_rs-0.2.3/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/llm_rs/auto.py` & `llm_rs-0.2.3/llm_rs/auto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from .config import QuantizationType,ContainerType,SessionConfig
-from pydantic import BaseModel
 import os
 import pathlib
 from .models import Mpt,GptNeoX,GptJ,Gpt2,Bloom,Llama
 from .base_model import Model
 import logging
 from typing import Optional, List, Union,Type
 import os
```

### Comparing `llm_rs-0.2.2/llm_rs/base_model.py` & `llm_rs-0.2.3/llm_rs/base_model.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/llm_rs/config.pyi` & `llm_rs-0.2.3/llm_rs/config.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/llm_rs/convert/auto_converter.py` & `llm_rs-0.2.3/llm_rs/convert/auto_converter.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/llm_rs/convert/models/_base.py` & `llm_rs-0.2.3/llm_rs/convert/models/_base.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/llm_rs/convert/models/bloom.py` & `llm_rs-0.2.3/llm_rs/convert/models/bloom.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/llm_rs/convert/models/gpt2.py` & `llm_rs-0.2.3/llm_rs/convert/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/llm_rs/convert/models/gptj.py` & `llm_rs-0.2.3/llm_rs/convert/models/gptj.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/llm_rs/convert/models/gptneox.py` & `llm_rs-0.2.3/llm_rs/convert/models/gptneox.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/llm_rs/convert/models/llama.py` & `llm_rs-0.2.3/llm_rs/convert/models/llama.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/llm_rs/convert/models/mpt.py` & `llm_rs-0.2.3/llm_rs/convert/models/mpt.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/llm_rs/models.pyi` & `llm_rs-0.2.3/llm_rs/models.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/llm_rs/results.pyi` & `llm_rs-0.2.3/llm_rs/results.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/pyproject.toml` & `llm_rs-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/src/configs.rs` & `llm_rs-0.2.3/src/configs.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/src/lib.rs` & `llm_rs-0.2.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/src/model_base.rs` & `llm_rs-0.2.3/src/model_base.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/src/quantize.rs` & `llm_rs-0.2.3/src/quantize.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/src/results.rs` & `llm_rs-0.2.3/src/results.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.2/Cargo.lock` & `llm_rs-0.2.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
 dependencies = [
  "bytemuck",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-rs"
-version = "0.2.2"
+version = "0.2.3"
 dependencies = [
  "ggml",
  "llm",
  "llm-base",
  "log",
  "pyo3",
  "rand",
```

### Comparing `llm_rs-0.2.2/PKG-INFO` & `llm_rs-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-rs
-Version: 0.2.2
+Version: 0.2.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: blake3
 Requires-Dist: huggingface-hub >= 0.14.1
@@ -17,16 +17,16 @@
 Provides-Extra: convert
 License-File: LICENSE
 Summary: Unofficial python bindings for llm-rs. 🐍❤️🦀
 Keywords: LLM,Transformers
 Author: Lukas Kreussel
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: repository, https://github.com/LLukas22/llm-rs-python
 Project-URL: documentation, https://llukas22.github.io/llm-rs-python/
+Project-URL: repository, https://github.com/LLukas22/llm-rs-python
 
 # llm-rs-python: Python Bindings for Rust's llm Library
 
 Welcome to `llm-rs`, an unofficial Python interface for the Rust-based [llm](https://github.com/rustformers/llm) library, made possible through [PyO3](https://github.com/PyO3/pyo3). Our package combines the convenience of Python with the performance of Rust to offer an efficient tool for your machine learning projects. 🐍❤️🦀
 
 With `llm-rs`, you can operate a variety of Large Language Models (LLMs) including LLama and GPT-NeoX directly on your CPU.
```

