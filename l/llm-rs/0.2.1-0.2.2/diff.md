# Comparing `tmp/llm_rs-0.2.1.tar.gz` & `tmp/llm_rs-0.2.2.tar.gz`

## Comparing `llm_rs-0.2.1.tar` & `llm_rs-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,40 @@
--rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 llm_rs-0.2.1/Cargo.toml
--rw-r--r--   0     1001      123      610 2023-05-19 16:34:02.000000 llm_rs-0.2.1/.github/workflows/BuildDoc.yml
--rw-r--r--   0     1001      123     2796 2023-05-19 16:34:02.000000 llm_rs-0.2.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      564 2023-05-19 16:34:02.000000 llm_rs-0.2.1/.github/workflows/Clippy.yml
--rw-r--r--   0     1001      123      602 2023-05-19 16:34:02.000000 llm_rs-0.2.1/.github/workflows/PublishDocs.yml
--rw-r--r--   0     1001      123     3455 2023-05-19 16:34:02.000000 llm_rs-0.2.1/.gitignore
--rw-r--r--   0     1001      123       72 2023-05-19 16:34:02.000000 llm_rs-0.2.1/.vscode/settings.json
--rw-r--r--   0     1001      123     1071 2023-05-19 16:34:02.000000 llm_rs-0.2.1/LICENSE
--rw-r--r--   0     1001      123     1134 2023-05-19 16:34:02.000000 llm_rs-0.2.1/README.md
--rw-r--r--   0     1001      123     1909 2023-05-19 16:34:02.000000 llm_rs-0.2.1/docs/docs/conversion.md
--rw-r--r--   0     1001      123     8622 2023-05-19 16:34:02.000000 llm_rs-0.2.1/docs/docs/index.md
--rw-r--r--   0     1001      123     1181 2023-05-19 16:34:02.000000 llm_rs-0.2.1/docs/mkdocs.yml
--rw-r--r--   0     1001      123       31 2023-05-19 16:34:02.000000 llm_rs-0.2.1/docs/requirements.txt
--rw-r--r--   0     1001      123      263 2023-05-19 16:34:02.000000 llm_rs-0.2.1/llm_rs/__init__.py
--rw-r--r--   0     1001      123     1299 2023-05-19 16:34:02.000000 llm_rs-0.2.1/llm_rs/config.pyi
--rw-r--r--   0     1001      123        0 2023-05-19 16:34:02.000000 llm_rs-0.2.1/llm_rs/llm_rs.pyi
--rw-r--r--   0     1001      123     2108 2023-05-19 16:34:02.000000 llm_rs-0.2.1/llm_rs/models.pyi
--rw-r--r--   0     1001      123        0 2023-05-19 16:34:02.000000 llm_rs-0.2.1/llm_rs/py.typed
--rw-r--r--   0     1001      123      697 2023-05-19 16:34:02.000000 llm_rs-0.2.1/llm_rs/results.pyi
--rw-r--r--   0     1001      123      925 2023-05-19 16:34:02.000000 llm_rs-0.2.1/pyproject.toml
--rw-r--r--   0     1001      123     1274 2023-05-19 16:34:02.000000 llm_rs-0.2.1/quantize.py
--rw-r--r--   0     1001      123     4274 2023-05-19 16:34:02.000000 llm_rs-0.2.1/src/configs.rs
--rw-r--r--   0     1001      123     1685 2023-05-19 16:34:02.000000 llm_rs-0.2.1/src/lib.rs
--rw-r--r--   0     1001      123     9645 2023-05-19 16:34:02.000000 llm_rs-0.2.1/src/model_base.rs
--rw-r--r--   0     1001      123      300 2023-05-19 16:34:02.000000 llm_rs-0.2.1/src/models.rs
--rw-r--r--   0     1001      123     2426 2023-05-19 16:34:02.000000 llm_rs-0.2.1/src/quantize.rs
--rw-r--r--   0     1001      123     1352 2023-05-19 16:34:02.000000 llm_rs-0.2.1/src/results.rs
--rw-r--r--   0     1001      123    20589 2023-05-19 16:35:27.000000 llm_rs-0.2.1/Cargo.lock
--rw-r--r--   0        0        0     2178 1970-01-01 00:00:00.000000 llm_rs-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 llm_rs-0.2.2/Cargo.toml
+-rw-r--r--   0     1001      123      610 2023-05-23 15:15:11.000000 llm_rs-0.2.2/.github/workflows/BuildDoc.yml
+-rw-r--r--   0     1001      123     2796 2023-05-23 15:15:11.000000 llm_rs-0.2.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      564 2023-05-23 15:15:11.000000 llm_rs-0.2.2/.github/workflows/Clippy.yml
+-rw-r--r--   0     1001      123      602 2023-05-23 15:15:11.000000 llm_rs-0.2.2/.github/workflows/PublishDocs.yml
+-rw-r--r--   0     1001      123     3455 2023-05-23 15:15:11.000000 llm_rs-0.2.2/.gitignore
+-rw-r--r--   0     1001      123       72 2023-05-23 15:15:11.000000 llm_rs-0.2.2/.vscode/settings.json
+-rw-r--r--   0     1001      123     1071 2023-05-23 15:15:11.000000 llm_rs-0.2.2/LICENSE
+-rw-r--r--   0     1001      123     2192 2023-05-23 15:15:11.000000 llm_rs-0.2.2/README.md
+-rw-r--r--   0     1001      123     4799 2023-05-23 15:15:11.000000 llm_rs-0.2.2/docs/docs/conversion.md
+-rw-r--r--   0     1001      123     9355 2023-05-23 15:15:11.000000 llm_rs-0.2.2/docs/docs/index.md
+-rw-r--r--   0     1001      123     1181 2023-05-23 15:15:11.000000 llm_rs-0.2.2/docs/mkdocs.yml
+-rw-r--r--   0     1001      123       31 2023-05-23 15:15:11.000000 llm_rs-0.2.2/docs/requirements.txt
+-rw-r--r--   0     1001      123      334 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/__init__.py
+-rw-r--r--   0     1001      123     6112 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/auto.py
+-rw-r--r--   0     1001      123     1614 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/base_model.py
+-rw-r--r--   0     1001      123     1351 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/config.pyi
+-rw-r--r--   0     1001      123       78 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/convert/__init__.py
+-rw-r--r--   0     1001      123     2223 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/convert/auto_converter.py
+-rw-r--r--   0     1001      123      199 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/convert/models/__init__.py
+-rw-r--r--   0     1001      123     5581 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/convert/models/_base.py
+-rw-r--r--   0     1001      123     3177 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/convert/models/bloom.py
+-rw-r--r--   0     1001      123     5221 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/convert/models/gpt2.py
+-rw-r--r--   0     1001      123     2032 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/convert/models/gptj.py
+-rw-r--r--   0     1001      123     2138 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/convert/models/gptneox.py
+-rw-r--r--   0     1001      123     6334 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/convert/models/llama.py
+-rw-r--r--   0     1001      123     1893 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/convert/models/mpt.py
+-rw-r--r--   0     1001      123        0 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/llm_rs.pyi
+-rw-r--r--   0     1001      123      579 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/models.pyi
+-rw-r--r--   0     1001      123        0 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/py.typed
+-rw-r--r--   0     1001      123      697 2023-05-23 15:15:11.000000 llm_rs-0.2.2/llm_rs/results.pyi
+-rw-r--r--   0     1001      123      978 2023-05-23 15:15:11.000000 llm_rs-0.2.2/pyproject.toml
+-rw-r--r--   0     1001      123     4274 2023-05-23 15:15:11.000000 llm_rs-0.2.2/src/configs.rs
+-rw-r--r--   0     1001      123     1685 2023-05-23 15:15:11.000000 llm_rs-0.2.2/src/lib.rs
+-rw-r--r--   0     1001      123     9658 2023-05-23 15:15:11.000000 llm_rs-0.2.2/src/model_base.rs
+-rw-r--r--   0     1001      123      300 2023-05-23 15:15:11.000000 llm_rs-0.2.2/src/models.rs
+-rw-r--r--   0     1001      123     2576 2023-05-23 15:15:11.000000 llm_rs-0.2.2/src/quantize.rs
+-rw-r--r--   0     1001      123     1352 2023-05-23 15:15:11.000000 llm_rs-0.2.2/src/results.rs
+-rw-r--r--   0     1001      123    20589 2023-05-23 15:16:44.000000 llm_rs-0.2.2/Cargo.lock
+-rw-r--r--   0        0        0     3289 1970-01-01 00:00:00.000000 llm_rs-0.2.2/PKG-INFO
```

### Comparing `llm_rs-0.2.1/.github/workflows/BuildDoc.yml` & `llm_rs-0.2.2/.github/workflows/BuildDoc.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.1/.github/workflows/CI.yml` & `llm_rs-0.2.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.1/.github/workflows/Clippy.yml` & `llm_rs-0.2.2/.github/workflows/Clippy.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.1/.github/workflows/PublishDocs.yml` & `llm_rs-0.2.2/.github/workflows/PublishDocs.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.1/.gitignore` & `llm_rs-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.1/LICENSE` & `llm_rs-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.1/docs/docs/index.md` & `llm_rs-0.2.2/docs/docs/index.md`

 * *Files 7% similar despite different names*

```diff
@@ -23,30 +23,44 @@
 
 ```shell
 git clone https://github.com/LLukas22/llm-rs-python
 cd ./llm-rs-python
 maturin develop -r
 ```
 
-### Model Loading
+### Model Loading and Deployment
 
-Right now, this library leverages [ggml](https://github.com/ggerganov/ggml) as a backend and requires ggml-converted models to perform inference. 
+This library presently utilizes the [ggml](https://github.com/ggerganov/ggml) backend, and necessitates ggml-converted models for inference. 
 
-You can find these models on the [HuggingfaceHub](https://huggingface.co/models?search=ggml) or in the "[Know-good-Models](https://github.com/rustformers/llm/blob/main/known-good-models.md)" list of the `rustformers/llm` repo.
+These converted models can be readily found on the [HuggingfaceHub](https://huggingface.co/models?search=ggml) or referenced in the "[Known-good-Models](https://github.com/rustformers/llm/blob/main/known-good-models.md)" list, curated in the `rustformers/llm` repository.
 
-All available model architectures can be accessed through the `llm_rs` module.
+Each model architecture can be conveniently loaded through the `llm_rs` module.
 
-Here's a simple illustration of how to load a MPT model (like [mpt-7b](https://huggingface.co/LLukas22/mpt-7b-ggml)):
+For instance, loading an MPT model (like [mpt-7b](https://huggingface.co/LLukas22/mpt-7b-ggml)) can be achieved as shown below:
 
 ```python
 from llm_rs import Mpt
 
 model = Mpt("path/to/model.bin")
 ```
 
+### Streamlined Model Loading 
+
+Models that have been converted or quantized using `llm-rs` include an additional `*.meta` file. This file enables streamlined loading via the `AutoModel` module. This feature is particularly advantageous as it allows you to load models without specifying the underlying architecture.
+
+The following is an illustrative example:
+
+```python
+from llm_rs import AutoModel
+
+model = AutoModel.load("path/to/model.bin")
+```
+
+In this streamlined approach, the `AutoModel` module automatically infers the architecture from the `*.meta` file associated with the model, providing an intuitive and straightforward method for loading your models.
+
 ### Text Generation
 
 Every model implements a `generate` function that you can use to generate text using the loaded model. 
 
 Here's a quick look at how it works:
 
 ```python
```

### Comparing `llm_rs-0.2.1/docs/mkdocs.yml` & `llm_rs-0.2.2/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.1/llm_rs/config.pyi` & `llm_rs-0.2.2/llm_rs/config.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import Optional,List
-from enum import Enum
+from enum import Enum, auto
 
 class ContainerType(Enum):
-    GGML=0,
-    GGJT=1,
+    GGML=auto(),
+    GGJT=auto(),
 
 class QuantizationType(Enum):
-    Q4_0=0,
-    Q4_1=1,
+    Q4_0=auto(),
+    Q4_1=auto(),
+    F16=auto(),
 
 class Precision(Enum):
-    FP32=0,
-    FP16=1,
+    FP32=auto(),
+    FP16=auto(),
     
 class GenerationConfig():
     """
     Configuration parameters for the generation process.
     """
     top_k:int
     top_p:float
```

### Comparing `llm_rs-0.2.1/llm_rs/models.pyi` & `llm_rs-0.2.2/llm_rs/base_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-from typing import Optional, Callable, List
+from typing import Optional, Callable, List, Union
 from abc import ABC
+import os
 
 from .config import GenerationConfig, SessionConfig, ContainerType, QuantizationType
 from .results import GenerationResult
 
+
+
 #Theoretically this is incorrect as the 'model' doesnt actually exist, but it is a good enough approximation for now. 
 class Model(ABC):
     """
     Wrapper around a llm model.
     """
     config:SessionConfig
     
@@ -17,17 +20,17 @@
     @property
     def verbose(self)->bool: ...
 
     @property
     def lora_paths(self)->Optional[List[str]]: ...
 
     def  __init__(self,
-                  path:str,
+                  path:Union[str,os.PathLike],
                   session_config:SessionConfig=SessionConfig(),
-                  lora_paths:Optional[List[str]]=None,
+                  lora_paths:Optional[List[Union[str,os.PathLike]]]=None,
                   verbose:bool=False) -> None: ...
     
     def generate(self,prompt:str,
                  generation_config:Optional[GenerationConfig]=None,
                  callback:Callable[[str],Optional[bool]]=None) -> GenerationResult: 
         """
         Generates text from a prompt.
@@ -47,46 +50,8 @@
         ...
 
     @staticmethod
     def quantize(source:str,destination:str,quantization:QuantizationType=QuantizationType.Q4_0,container:ContainerType=ContainerType.GGJT)->None:
         """
         Quantizes the model.
         """
-        ...
-    
-
-class Llama(Model):
-    """
-    Wrapper around all Llama based models.
-    """
-    ...
-    
-    
-class GptJ(Model):
-    """
-    Wrapper around all GPTJ based models.
-    """
-    ...
-    
-class Gpt2(Model):
-    """
-    Wrapper around all GPT2 based models.
-    """
-    ...
-    
-class Bloom(Model):
-    """
-    Wrapper around all Bloom based models.
-    """
-    ...
-    
-class GptNeoX(Model):
-    """
-    Wrapper around all GPT-NeoX based models.
-    """
-    ...
-
-class Mpt(Model):
-    """
-    Wrapper around all Mpt based models.
-    """
-    ...
+        ...
```

### Comparing `llm_rs-0.2.1/llm_rs/results.pyi` & `llm_rs-0.2.2/llm_rs/results.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.1/pyproject.toml` & `llm_rs-0.2.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -13,25 +13,29 @@
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
 ]
 keywords = ["LLM","Transformers"]
+dependencies =   [
+  "blake3",
+  "huggingface-hub >= 0.14.1",
+]
+
 
 [project.urls]
 repository = "https://github.com/LLukas22/llm-rs-python"
 documentation  = "https://llukas22.github.io/llm-rs-python/"
 
-
 [project.optional-dependencies]
 convert=[
   "transformers >= 4.29.0",
   "sentencepiece >= 0.1.99",
   "torch >= 2.0.0",
   "accelerate >= 0.19.0",
   "tqdm",
-  "huggingface-hub >= 0.14.1"
+  "einops >= 0.6.1"
 ]
 
 [tool.maturin]
-features = ["pyo3/extension-module"]
+features = ["pyo3/extension-module"]
```

### Comparing `llm_rs-0.2.1/src/configs.rs` & `llm_rs-0.2.2/src/configs.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.1/src/lib.rs` & `llm_rs-0.2.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.1/src/model_base.rs` & `llm_rs-0.2.2/src/model_base.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use pyo3::exceptions::PyException;
 use pyo3::prelude::*;
 use pyo3::types::PyTuple;
 
 use llm::{InferenceError, TokenUtf8Buffer};
-use llm_base::{InferenceFeedback, OutputRequest};
+use llm_base::{InferenceFeedback, OutputRequest, Prompt};
 
 use rand::prelude::*;
 use rand_chacha::ChaCha8Rng;
 
 use std::convert::Infallible;
 
 use crate::configs;
@@ -49,15 +49,15 @@
     let default_config = configs::GenerationConfig::default();
     let config_to_use = generation_config.unwrap_or(&default_config);
 
     let generation_params =
         config_to_use.to_llm_params(session_config.threads, session_config.batch_size);
 
     let mut rng = ChaCha8Rng::seed_from_u64(config_to_use.seed);
-    let prompt = prompt.as_str();
+    let prompt = Prompt::from(&prompt);
 
     let mut session = model.start_session(session_params);
 
     //Extract the callback function from the python object
     let mut callback_function: Option<&PyAny> = None;
     let pytohn_object: Py<PyAny>;
 
@@ -70,15 +70,15 @@
 
     let feed_start_at = std::time::SystemTime::now();
     //Feed the prompt
 
     let mut output_request_feeding = OutputRequest::default();
     _py.allow_threads(|| {
         session
-            .feed_prompt::<Infallible>(
+            .feed_prompt::<Infallible, _>(
                 model,
                 &generation_params,
                 prompt,
                 &mut output_request_feeding,
                 |_| Ok(InferenceFeedback::Continue),
             )
             .unwrap()
@@ -192,15 +192,15 @@
                 let default_config = crate::configs::SessionConfig::default();
                 let config_to_use = session_config.unwrap_or(default_config);
 
                 let path = std::path::Path::new(&path);
                 let lora_paths = lora_paths
                     .map(|strings| strings.into_iter().map(std::path::PathBuf::from).collect());
                 let model_params = llm_base::ModelParameters {
-                    n_context_tokens: config_to_use.context_length,
+                    context_size: config_to_use.context_length,
                     prefer_mmap: config_to_use.prefer_mmap,
                     lora_adapters: lora_paths.clone(),
                     ..Default::default()
                 };
                 let llm_model: $llm_model =
                     llm_base::load(&path, model_params, None, |load_progress| {
                         if should_log {
```

### Comparing `llm_rs-0.2.1/src/quantize.rs` & `llm_rs-0.2.2/src/quantize.rs`

 * *Files 4% similar despite different names*

```diff
@@ -17,31 +17,35 @@
 }
 
 #[pyclass]
 #[derive(Clone, Copy, Debug, PartialEq)]
 pub enum QuantizationType {
     Q4_0,
     Q4_1,
+    F16,
 }
 
 pub fn _quantize<M: llm::KnownModel + 'static>(
     source: PathBuf,
     destination: PathBuf,
     container: ContainerType,
     quantization: QuantizationType,
 ) -> Result<(), QuantizeError> {
     let container = match container {
         ContainerType::GGML => ggml::format::SaveContainerType::Ggml,
         ContainerType::GGJT => ggml::format::SaveContainerType::GgjtV2,
     };
 
     let quantization = match quantization {
-        QuantizationType::Q4_0 => ggml::Type::Q4_0,
-        QuantizationType::Q4_1 => ggml::Type::Q4_1,
-    };
+        QuantizationType::Q4_0 => Ok(ggml::Type::Q4_0),
+        QuantizationType::Q4_1 => Ok(ggml::Type::Q4_1),
+        QuantizationType::F16 => Err(QuantizeError::UnsupportedElementType {
+            element_type: ggml::Type::F16,
+        }),
+    }?;
 
     let mut source = BufReader::new(std::fs::File::open(source)?);
     let mut destination = BufWriter::new(std::fs::File::create(destination)?);
 
     quantize::<M, _, _>(
         &mut source,
         &mut destination,
```

### Comparing `llm_rs-0.2.1/src/results.rs` & `llm_rs-0.2.2/src/results.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.1/Cargo.lock` & `llm_rs-0.2.2/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -133,24 +133,24 @@
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "ggml"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#99adc84d2b4cbda400ff26bde187dd5c73b3b120"
+source = "git+https://github.com/rustformers/llm.git#861d694003fd4f82f5c49d85814f823d600b7c7e"
 dependencies = [
  "ggml-sys",
  "thiserror",
 ]
 
 [[package]]
 name = "ggml-sys"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#99adc84d2b4cbda400ff26bde187dd5c73b3b120"
+source = "git+https://github.com/rustformers/llm.git#861d694003fd4f82f5c49d85814f823d600b7c7e"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "half"
 version = "2.2.1"
@@ -211,30 +211,30 @@
 version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "llm"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#99adc84d2b4cbda400ff26bde187dd5c73b3b120"
+source = "git+https://github.com/rustformers/llm.git#861d694003fd4f82f5c49d85814f823d600b7c7e"
 dependencies = [
  "llm-base",
  "llm-bloom",
  "llm-gpt2",
  "llm-gptj",
  "llm-gptneox",
  "llm-llama",
  "llm-mpt",
  "serde",
 ]
 
 [[package]]
 name = "llm-base"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#99adc84d2b4cbda400ff26bde187dd5c73b3b120"
+source = "git+https://github.com/rustformers/llm.git#861d694003fd4f82f5c49d85814f823d600b7c7e"
 dependencies = [
  "bytemuck",
  "ggml",
  "half",
  "memmap2",
  "partial_sort",
  "rand",
@@ -242,75 +242,75 @@
  "serde_bytes",
  "thiserror",
 ]
 
 [[package]]
 name = "llm-bloom"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#99adc84d2b4cbda400ff26bde187dd5c73b3b120"
+source = "git+https://github.com/rustformers/llm.git#861d694003fd4f82f5c49d85814f823d600b7c7e"
 dependencies = [
  "bytemuck",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-gpt2"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#99adc84d2b4cbda400ff26bde187dd5c73b3b120"
+source = "git+https://github.com/rustformers/llm.git#861d694003fd4f82f5c49d85814f823d600b7c7e"
 dependencies = [
  "bytemuck",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-gptj"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#99adc84d2b4cbda400ff26bde187dd5c73b3b120"
+source = "git+https://github.com/rustformers/llm.git#861d694003fd4f82f5c49d85814f823d600b7c7e"
 dependencies = [
  "bytemuck",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-gptneox"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#99adc84d2b4cbda400ff26bde187dd5c73b3b120"
+source = "git+https://github.com/rustformers/llm.git#861d694003fd4f82f5c49d85814f823d600b7c7e"
 dependencies = [
  "bytemuck",
  "llm-base",
  "serde",
 ]
 
 [[package]]
 name = "llm-llama"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#99adc84d2b4cbda400ff26bde187dd5c73b3b120"
+source = "git+https://github.com/rustformers/llm.git#861d694003fd4f82f5c49d85814f823d600b7c7e"
 dependencies = [
  "bytemuck",
  "llm-base",
  "protobuf",
  "rand",
  "rust_tokenizers",
  "serde",
  "serde_json",
  "thiserror",
 ]
 
 [[package]]
 name = "llm-mpt"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#99adc84d2b4cbda400ff26bde187dd5c73b3b120"
+source = "git+https://github.com/rustformers/llm.git#861d694003fd4f82f5c49d85814f823d600b7c7e"
 dependencies = [
  "bytemuck",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-rs"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "ggml",
  "llm",
  "llm-base",
  "log",
  "pyo3",
  "rand",
@@ -554,28 +554,28 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.1"
+version = "1.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
+checksum = "d1a59b5d8e97dee33696bf13c5ba8ab85341c002922fba050069326b9c498974"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "rust_tokenizers"
 version = "3.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77c4313059ea8764ff2743ffaaa42fba0e4d5f8ff12febe4f3c74d598f629f62"
 dependencies = [
```

