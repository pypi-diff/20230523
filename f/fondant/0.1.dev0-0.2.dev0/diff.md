# Comparing `tmp/fondant-0.1.dev0.tar.gz` & `tmp/fondant-0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fondant-0.1.dev0.tar", max compression
+gzip compressed data, was "fondant-0.2.dev0.tar", max compression
```

## Comparing `fondant-0.1.dev0.tar` & `fondant-0.2.dev0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11356 2023-04-14 09:12:43.912402 fondant-0.1.dev0/LICENSE
--rw-r--r--   0        0        0     4290 2023-04-14 09:12:43.912577 fondant-0.1.dev0/README.md
--rw-r--r--   0        0        0        0 2023-04-14 09:12:43.929663 fondant-0.1.dev0/fondant/__init__.py
--rw-r--r--   0        0        0        1 2023-04-14 09:12:43.929762 fondant-0.1.dev0/fondant/components/__init__.py
--rw-r--r--   0        0        0    17668 2023-04-14 09:15:10.579020 fondant-0.1.dev0/fondant/components/common.py
--rw-r--r--   0        0        0     5456 2023-04-14 09:15:05.225089 fondant-0.1.dev0/fondant/components/hf_datasets_components.py
--rw-r--r--   0        0        0     4697 2023-04-14 09:15:06.732962 fondant-0.1.dev0/fondant/components/pandas_components.py
--rw-r--r--   0        0        0      342 2023-04-14 09:16:45.591739 fondant-0.1.dev0/fondant/exceptions.py
--rw-r--r--   0        0        0     5287 2023-04-14 09:19:51.255014 fondant-0.1.dev0/fondant/gcp_storage.py
--rw-r--r--   0        0        0     2241 2023-04-14 09:12:43.930278 fondant-0.1.dev0/fondant/import_utils.py
--rw-r--r--   0        0        0      874 2023-04-14 09:12:43.930343 fondant-0.1.dev0/fondant/io.py
--rw-r--r--   0        0        0      605 2023-04-14 09:12:43.930408 fondant-0.1.dev0/fondant/logger.py
--rw-r--r--   0        0        0     6594 2023-04-14 09:21:24.391801 fondant-0.1.dev0/fondant/manifest.py
--rw-r--r--   0        0        0     1444 2023-04-14 09:20:04.669266 fondant-0.1.dev0/fondant/pipeline_utils.py
--rw-r--r--   0        0        0     1672 2023-04-14 09:12:43.930673 fondant-0.1.dev0/fondant/schemas/manifest.json
--rw-r--r--   0        0        0     4361 2023-04-14 09:12:43.930743 fondant-0.1.dev0/fondant/storage_interface.py
--rw-r--r--   0        0        0     2162 2023-04-14 09:13:10.211721 fondant-0.1.dev0/pyproject.toml
--rw-r--r--   0        0        0     6225 1970-01-01 00:00:00.000000 fondant-0.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-04-14 09:12:43.912402 fondant-0.2.dev0/LICENSE
+-rw-r--r--   0        0        0     4290 2023-04-14 09:23:54.059098 fondant-0.2.dev0/README.md
+-rw-r--r--   0        0        0        0 2023-04-14 09:12:43.929663 fondant-0.2.dev0/fondant/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-14 09:12:43.929762 fondant-0.2.dev0/fondant/components/__init__.py
+-rw-r--r--   0        0        0    17668 2023-04-14 09:15:10.579020 fondant-0.2.dev0/fondant/components/common.py
+-rw-r--r--   0        0        0     5456 2023-04-14 09:15:05.225089 fondant-0.2.dev0/fondant/components/hf_datasets_components.py
+-rw-r--r--   0        0        0     4697 2023-04-14 09:15:06.732962 fondant-0.2.dev0/fondant/components/pandas_components.py
+-rw-r--r--   0        0        0      342 2023-04-14 09:16:45.591739 fondant-0.2.dev0/fondant/exceptions.py
+-rw-r--r--   0        0        0     5287 2023-04-14 09:19:51.255014 fondant-0.2.dev0/fondant/gcp_storage.py
+-rw-r--r--   0        0        0     2241 2023-04-14 09:12:43.930278 fondant-0.2.dev0/fondant/import_utils.py
+-rw-r--r--   0        0        0      874 2023-04-14 09:12:43.930343 fondant-0.2.dev0/fondant/io.py
+-rw-r--r--   0        0        0      605 2023-04-14 09:12:43.930408 fondant-0.2.dev0/fondant/logger.py
+-rw-r--r--   0        0        0     6594 2023-04-14 09:21:24.391801 fondant-0.2.dev0/fondant/manifest.py
+-rw-r--r--   0        0        0     1444 2023-04-14 09:20:04.669266 fondant-0.2.dev0/fondant/pipeline_utils.py
+-rw-r--r--   0        0        0     1672 2023-04-14 09:12:43.930673 fondant-0.2.dev0/fondant/schemas/manifest.json
+-rw-r--r--   0        0        0     4361 2023-04-14 09:12:43.930743 fondant-0.2.dev0/fondant/storage_interface.py
+-rw-r--r--   0        0        0     2162 2023-04-14 09:26:06.225285 fondant-0.2.dev0/pyproject.toml
+-rw-r--r--   0        0        0     6225 1970-01-01 00:00:00.000000 fondant-0.2.dev0/PKG-INFO
```

### Comparing `fondant-0.1.dev0/LICENSE` & `fondant-0.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `fondant-0.1.dev0/README.md` & `fondant-0.2.dev0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# Express
+# Fondant
 
-Express is a framework that speeds up the creation of KubeFlow pipelines to process big datasets and train [Foundation Models](https://fsi.stanford.edu/publication/opportunities-and-risks-foundation-models)
+Fondant is a framework that speeds up the creation of KubeFlow pipelines to process big datasets and train [Foundation Models](https://fsi.stanford.edu/publication/opportunities-and-risks-foundation-models)
 such as:
 
 - Stable Diffusion
 - CLIP
 - Large Language Models (LLMs like GPT-3)
 
 on them.
 
 ## Installation
 
-Express can be installed using pip:
+Fondant can be installed using pip:
 
 ```
-pip install express
+pip install fondant
 ```
 
 ## Usage
 
-Express is built upon [KubeFlow](https://www.kubeflow.org/), a cloud-agnostic framework built by Google to orchestrate machine learning workflows on Kubernetes. An important aspect of KubeFlow are pipelines, which consist of a set of components being executed, one after the other. This typically involves transforming data and optionally training a machine learning model on it. Check out [this page](https://www.kubeflow.org/docs/components/pipelines/v1/concepts/) if you want to learn more about KubeFlow pipelines and components.
+Fondant is built upon [KubeFlow](https://www.kubeflow.org/), a cloud-agnostic framework built by Google to orchestrate machine learning workflows on Kubernetes. An important aspect of KubeFlow are pipelines, which consist of a set of components being executed, one after the other. This typically involves transforming data and optionally training a machine learning model on it. Check out [this page](https://www.kubeflow.org/docs/components/pipelines/v1/concepts/) if you want to learn more about KubeFlow pipelines and components.
 
-Express offers ready-made components and helper functions that serve as boilerplate which you can use to speed up the creation of KubeFlow pipelines. To implement your own component, simply overwrite one of the components available in Express. In the example below, we leverage the `PandasTransformComponent` and overwrite its `transform` method.
+Fondant offers ready-made components and helper functions that serve as boilerplate which you can use to speed up the creation of KubeFlow pipelines. To implement your own component, simply overwrite one of the components available in Fondant. In the example below, we leverage the `PandasTransformComponent` and overwrite its `transform` method.
 
 ```
 import pandas as pd
 
-from express.components.pandas_components import PandasTransformComponent, PandasDataset, PandasDatasetDraft
+from fondant.components.pandas_components import PandasTransformComponent, PandasDataset, PandasDatasetDraft
 
 class MyFirstTransform(PandasTransformComponent):
     @classmethod
     def transform(cls, data: PandasDataset, extra_args: Optional[Dict] = None) -> PandasDatasetDraft:
 
         # Reading data
         index: List[str] = data.load_index()
@@ -49,15 +49,15 @@
                               Scanner.from_batches(table.to_batches())
 ```
 
 ## Components zoo
 
 Available components include:
 
-- Non-distributed Pandas components: `express.components.pandas_components.{PandasTransformComponent, PandasLoaderComponent}`
+- Non-distributed Pandas components: `fondant.components.pandas_components.{PandasTransformComponent, PandasLoaderComponent}`
 
 Planned components include:
 
 - Spark-based components and base image.
 - HuggingFace Datasets components.
 
 With Kubeflow, it's possible to share and re-use components across different pipelines. To see an example, checkout this [sample notebook](https://github.com/Svendegroote91/kfp_samples/blob/master/Reusable%20Components%20101.ipynb) that showcases how you can save and load a component.
@@ -73,15 +73,15 @@
 
 ## Pipeline zoo
 
 To do: add ready-made pipelines.
 
 ## Examples
 
-Example use cases of Express include:
+Example use cases of Fondant include:
 
 - collect additional image-text pairs based on a few seed images and fine-tune Stable Diffusion
 - filter an image-text dataset to only include "count" examples and fine-tune CLIP to improve its counting capabilities
 
 Check out the [examples folder](examples) for some illustrations.
 
 ## Contributing
```

### Comparing `fondant-0.1.dev0/fondant/components/common.py` & `fondant-0.2.dev0/fondant/components/common.py`

 * *Files identical despite different names*

### Comparing `fondant-0.1.dev0/fondant/components/hf_datasets_components.py` & `fondant-0.2.dev0/fondant/components/hf_datasets_components.py`

 * *Files identical despite different names*

### Comparing `fondant-0.1.dev0/fondant/components/pandas_components.py` & `fondant-0.2.dev0/fondant/components/pandas_components.py`

 * *Files identical despite different names*

### Comparing `fondant-0.1.dev0/fondant/gcp_storage.py` & `fondant-0.2.dev0/fondant/gcp_storage.py`

 * *Files identical despite different names*

### Comparing `fondant-0.1.dev0/fondant/import_utils.py` & `fondant-0.2.dev0/fondant/import_utils.py`

 * *Files identical despite different names*

### Comparing `fondant-0.1.dev0/fondant/io.py` & `fondant-0.2.dev0/fondant/io.py`

 * *Files identical despite different names*

### Comparing `fondant-0.1.dev0/fondant/logger.py` & `fondant-0.2.dev0/fondant/logger.py`

 * *Files identical despite different names*

### Comparing `fondant-0.1.dev0/fondant/manifest.py` & `fondant-0.2.dev0/fondant/manifest.py`

 * *Files identical despite different names*

### Comparing `fondant-0.1.dev0/fondant/pipeline_utils.py` & `fondant-0.2.dev0/fondant/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `fondant-0.1.dev0/fondant/schemas/manifest.json` & `fondant-0.2.dev0/fondant/schemas/manifest.json`

 * *Files identical despite different names*

### Comparing `fondant-0.1.dev0/fondant/storage_interface.py` & `fondant-0.2.dev0/fondant/storage_interface.py`

 * *Files identical despite different names*

### Comparing `fondant-0.1.dev0/pyproject.toml` & `fondant-0.2.dev0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fondant"
-version = "0.1.dev0"
+version = "0.2.dev0"
 description = "Fondant - Composable pipelines for foundation model finetuning"
 readme = "README.md"
 keywords = ["data", "machine learning", "finetuning", "foundation models"]
 license = "Apache-2.0"
 authors = [
     "Simon Slangen <simon.slangen@ml6.eu>",
     "Philippe Moussalli <philippe.moussalli@ml6.eu>",
```

### Comparing `fondant-0.1.dev0/PKG-INFO` & `fondant-0.2.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fondant
-Version: 0.1.dev0
+Version: 0.2.dev0
 Summary: Fondant - Composable pipelines for foundation model finetuning
 Home-page: https://github.com/ml6-team/fondant
 License: Apache-2.0
 Keywords: data,machine learning,finetuning,foundation models
 Author: Simon Slangen
 Author-email: simon.slangen@ml6.eu
 Maintainer: Philippe Moussalli
@@ -38,43 +38,43 @@
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: kfp (>=1.8.19,<2.0.0) ; extra == "pipelines"
 Requires-Dist: kubernetes (>=18.20.0,<19.0.0) ; extra == "pipelines"
 Requires-Dist: pandas (>=1.3.5,<2.0.0) ; extra == "pandas"
 Project-URL: Repository, https://github.com/ml6-team/fondant
 Description-Content-Type: text/markdown
 
-# Express
+# Fondant
 
-Express is a framework that speeds up the creation of KubeFlow pipelines to process big datasets and train [Foundation Models](https://fsi.stanford.edu/publication/opportunities-and-risks-foundation-models)
+Fondant is a framework that speeds up the creation of KubeFlow pipelines to process big datasets and train [Foundation Models](https://fsi.stanford.edu/publication/opportunities-and-risks-foundation-models)
 such as:
 
 - Stable Diffusion
 - CLIP
 - Large Language Models (LLMs like GPT-3)
 
 on them.
 
 ## Installation
 
-Express can be installed using pip:
+Fondant can be installed using pip:
 
 ```
-pip install express
+pip install fondant
 ```
 
 ## Usage
 
-Express is built upon [KubeFlow](https://www.kubeflow.org/), a cloud-agnostic framework built by Google to orchestrate machine learning workflows on Kubernetes. An important aspect of KubeFlow are pipelines, which consist of a set of components being executed, one after the other. This typically involves transforming data and optionally training a machine learning model on it. Check out [this page](https://www.kubeflow.org/docs/components/pipelines/v1/concepts/) if you want to learn more about KubeFlow pipelines and components.
+Fondant is built upon [KubeFlow](https://www.kubeflow.org/), a cloud-agnostic framework built by Google to orchestrate machine learning workflows on Kubernetes. An important aspect of KubeFlow are pipelines, which consist of a set of components being executed, one after the other. This typically involves transforming data and optionally training a machine learning model on it. Check out [this page](https://www.kubeflow.org/docs/components/pipelines/v1/concepts/) if you want to learn more about KubeFlow pipelines and components.
 
-Express offers ready-made components and helper functions that serve as boilerplate which you can use to speed up the creation of KubeFlow pipelines. To implement your own component, simply overwrite one of the components available in Express. In the example below, we leverage the `PandasTransformComponent` and overwrite its `transform` method.
+Fondant offers ready-made components and helper functions that serve as boilerplate which you can use to speed up the creation of KubeFlow pipelines. To implement your own component, simply overwrite one of the components available in Fondant. In the example below, we leverage the `PandasTransformComponent` and overwrite its `transform` method.
 
 ```
 import pandas as pd
 
-from express.components.pandas_components import PandasTransformComponent, PandasDataset, PandasDatasetDraft
+from fondant.components.pandas_components import PandasTransformComponent, PandasDataset, PandasDatasetDraft
 
 class MyFirstTransform(PandasTransformComponent):
     @classmethod
     def transform(cls, data: PandasDataset, extra_args: Optional[Dict] = None) -> PandasDatasetDraft:
 
         # Reading data
         index: List[str] = data.load_index()
@@ -93,15 +93,15 @@
                               Scanner.from_batches(table.to_batches())
 ```
 
 ## Components zoo
 
 Available components include:
 
-- Non-distributed Pandas components: `express.components.pandas_components.{PandasTransformComponent, PandasLoaderComponent}`
+- Non-distributed Pandas components: `fondant.components.pandas_components.{PandasTransformComponent, PandasLoaderComponent}`
 
 Planned components include:
 
 - Spark-based components and base image.
 - HuggingFace Datasets components.
 
 With Kubeflow, it's possible to share and re-use components across different pipelines. To see an example, checkout this [sample notebook](https://github.com/Svendegroote91/kfp_samples/blob/master/Reusable%20Components%20101.ipynb) that showcases how you can save and load a component.
@@ -117,15 +117,15 @@
 
 ## Pipeline zoo
 
 To do: add ready-made pipelines.
 
 ## Examples
 
-Example use cases of Express include:
+Example use cases of Fondant include:
 
 - collect additional image-text pairs based on a few seed images and fine-tune Stable Diffusion
 - filter an image-text dataset to only include "count" examples and fine-tune CLIP to improve its counting capabilities
 
 Check out the [examples folder](examples) for some illustrations.
 
 ## Contributing
```

