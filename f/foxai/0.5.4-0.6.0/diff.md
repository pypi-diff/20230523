# Comparing `tmp/foxai-0.5.4.tar.gz` & `tmp/foxai-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxai-0.5.4.tar", max compression
+gzip compressed data, was "foxai-0.6.0.tar", max compression
```

## Comparing `foxai-0.5.4.tar` & `foxai-0.6.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0    11357 2023-05-22 11:45:51.749264 foxai-0.5.4/LICENSE
--rw-r--r--   0        0        0     7626 2023-05-22 11:45:51.749264 foxai-0.5.4/README.md
--rw-r--r--   0        0        0      162 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/__init__.py
--rw-r--r--   0        0        0     3735 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/array_utils.py
--rw-r--r--   0        0        0        0 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/callbacks/__init__.py
--rw-r--r--   0        0        0     8744 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/callbacks/wandb_callback.py
--rw-r--r--   0        0        0        0 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/cli/__init__.py
--rw-r--r--   0        0        0      486 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/cli/config_model.py
--rw-r--r--   0        0        0     7650 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/cli/experiment_update.py
--rw-r--r--   0        0        0     9778 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/context_manager.py
--rw-r--r--   0        0        0     1603 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/__init__.py
--rw-r--r--   0        0        0     1118 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/base_explainer.py
--rw-r--r--   0        0        0        0 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/__init__.py
--rw-r--r--   0        0        0     8381 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/conductance.py
--rw-r--r--   0        0        0     4859 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/deconv.py
--rw-r--r--   0        0        0    13218 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/deeplift.py
--rw-r--r--   0        0        0    13386 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/deeplift_shap.py
--rw-r--r--   0        0        0    24493 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/gradcam.py
--rw-r--r--   0        0        0    12414 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/gradient_shap.py
--rw-r--r--   0        0        0     5076 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/guided_backprop.py
--rw-r--r--   0        0        0     8346 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/input_x_gradient.py
--rw-r--r--   0        0        0    14085 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/integrated_gradients.py
--rw-r--r--   0        0        0     7867 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/lrp.py
--rw-r--r--   0        0        0     7588 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/noise_tunnel.py
--rw-r--r--   0        0        0     7990 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/occlusion.py
--rw-r--r--   0        0        0     4135 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/saliency.py
--rw-r--r--   0        0        0     1253 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/model_utils.py
--rw-r--r--   0        0        0        0 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/object_detection/__init__.py
--rw-r--r--   0        0        0     2639 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/object_detection/base_object_detector.py
--rw-r--r--   0        0        0      679 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/object_detection/types.py
--rw-r--r--   0        0        0     1745 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/object_detection/utils.py
--rw-r--r--   0        0        0      752 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/logger.py
--rw-r--r--   0        0        0    10221 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/visualizer.py
--rw-r--r--   0        0        0     1940 2023-05-22 11:45:51.757264 foxai-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     9185 1970-01-01 00:00:00.000000 foxai-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-12-08 09:03:39.885460 foxai-0.6.0/LICENSE
+-rw-r--r--   0        0        0     7626 2023-05-22 10:57:44.428483 foxai-0.6.0/README.md
+-rw-r--r--   0        0        0      162 2023-03-15 11:48:52.158777 foxai-0.6.0/foxai/__init__.py
+-rw-r--r--   0        0        0     3735 2023-04-04 06:20:02.541333 foxai-0.6.0/foxai/array_utils.py
+-rw-r--r--   0        0        0        0 2023-03-15 11:48:52.158777 foxai-0.6.0/foxai/callbacks/__init__.py
+-rw-r--r--   0        0        0     8744 2023-05-22 10:57:44.428483 foxai-0.6.0/foxai/callbacks/wandb_callback.py
+-rw-r--r--   0        0        0        0 2023-03-15 11:48:52.158777 foxai-0.6.0/foxai/cli/__init__.py
+-rw-r--r--   0        0        0      486 2023-04-04 06:59:57.556158 foxai-0.6.0/foxai/cli/config_model.py
+-rw-r--r--   0        0        0     7650 2023-05-22 10:57:44.428483 foxai-0.6.0/foxai/cli/experiment_update.py
+-rw-r--r--   0        0        0     9778 2023-05-22 10:57:44.428483 foxai-0.6.0/foxai/context_manager.py
+-rw-r--r--   0        0        0     1603 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/__init__.py
+-rw-r--r--   0        0        0     1118 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/base_explainer.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/computer_vision/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/computer_vision/algorithm/__init__.py
+-rw-r--r--   0        0        0     8381 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/computer_vision/algorithm/conductance.py
+-rw-r--r--   0        0        0     4859 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/computer_vision/algorithm/deconv.py
+-rw-r--r--   0        0        0    13218 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/computer_vision/algorithm/deeplift.py
+-rw-r--r--   0        0        0    13386 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/computer_vision/algorithm/deeplift_shap.py
+-rw-r--r--   0        0        0    24493 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/computer_vision/algorithm/gradcam.py
+-rw-r--r--   0        0        0    12414 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/computer_vision/algorithm/gradient_shap.py
+-rw-r--r--   0        0        0     5076 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/computer_vision/algorithm/guided_backprop.py
+-rw-r--r--   0        0        0     8346 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/computer_vision/algorithm/input_x_gradient.py
+-rw-r--r--   0        0        0    14085 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/computer_vision/algorithm/integrated_gradients.py
+-rw-r--r--   0        0        0     7867 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/computer_vision/algorithm/lrp.py
+-rw-r--r--   0        0        0     7588 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/computer_vision/algorithm/noise_tunnel.py
+-rw-r--r--   0        0        0     7990 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/computer_vision/algorithm/occlusion.py
+-rw-r--r--   0        0        0     4135 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/computer_vision/algorithm/saliency.py
+-rw-r--r--   0        0        0     1253 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/computer_vision/model_utils.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/computer_vision/object_detection/__init__.py
+-rw-r--r--   0        0        0     2639 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/computer_vision/object_detection/base_object_detector.py
+-rw-r--r--   0        0        0      679 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/computer_vision/object_detection/types.py
+-rw-r--r--   0        0        0     1745 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/explainer/computer_vision/object_detection/utils.py
+-rw-r--r--   0        0        0      752 2023-03-15 11:48:52.162777 foxai-0.6.0/foxai/logger.py
+-rw-r--r--   0        0        0    10221 2023-05-22 10:57:44.432483 foxai-0.6.0/foxai/visualizer.py
+-rw-r--r--   0        0        0     1940 2023-05-22 11:50:34.953302 foxai-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     9135 1970-01-01 00:00:00.000000 foxai-0.6.0/setup.py
+-rw-r--r--   0        0        0     9185 1970-01-01 00:00:00.000000 foxai-0.6.0/PKG-INFO
```

### Comparing `foxai-0.5.4/LICENSE` & `foxai-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/README.md` & `foxai-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/array_utils.py` & `foxai-0.6.0/foxai/array_utils.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/callbacks/wandb_callback.py` & `foxai-0.6.0/foxai/callbacks/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/cli/experiment_update.py` & `foxai-0.6.0/foxai/cli/experiment_update.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/context_manager.py` & `foxai-0.6.0/foxai/context_manager.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/explainer/__init__.py` & `foxai-0.6.0/foxai/explainer/__init__.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/explainer/base_explainer.py` & `foxai-0.6.0/foxai/explainer/base_explainer.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/conductance.py` & `foxai-0.6.0/foxai/explainer/computer_vision/algorithm/conductance.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/deconv.py` & `foxai-0.6.0/foxai/explainer/computer_vision/algorithm/deconv.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/deeplift.py` & `foxai-0.6.0/foxai/explainer/computer_vision/algorithm/deeplift.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/deeplift_shap.py` & `foxai-0.6.0/foxai/explainer/computer_vision/algorithm/deeplift_shap.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/gradcam.py` & `foxai-0.6.0/foxai/explainer/computer_vision/algorithm/gradcam.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/gradient_shap.py` & `foxai-0.6.0/foxai/explainer/computer_vision/algorithm/gradient_shap.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/guided_backprop.py` & `foxai-0.6.0/foxai/explainer/computer_vision/algorithm/guided_backprop.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/input_x_gradient.py` & `foxai-0.6.0/foxai/explainer/computer_vision/algorithm/input_x_gradient.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/integrated_gradients.py` & `foxai-0.6.0/foxai/explainer/computer_vision/algorithm/integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/lrp.py` & `foxai-0.6.0/foxai/explainer/computer_vision/algorithm/lrp.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/noise_tunnel.py` & `foxai-0.6.0/foxai/explainer/computer_vision/algorithm/noise_tunnel.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/occlusion.py` & `foxai-0.6.0/foxai/explainer/computer_vision/algorithm/occlusion.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/saliency.py` & `foxai-0.6.0/foxai/explainer/computer_vision/algorithm/saliency.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/explainer/computer_vision/model_utils.py` & `foxai-0.6.0/foxai/explainer/computer_vision/model_utils.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/explainer/computer_vision/object_detection/base_object_detector.py` & `foxai-0.6.0/foxai/explainer/computer_vision/object_detection/base_object_detector.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/explainer/computer_vision/object_detection/types.py` & `foxai-0.6.0/foxai/explainer/computer_vision/object_detection/types.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/explainer/computer_vision/object_detection/utils.py` & `foxai-0.6.0/foxai/explainer/computer_vision/object_detection/utils.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/logger.py` & `foxai-0.6.0/foxai/logger.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/foxai/visualizer.py` & `foxai-0.6.0/foxai/visualizer.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.4/pyproject.toml` & `foxai-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foxai"
-version = "0.5.4"
+version = "0.6.0"
 description = "Model Interpretability for PyTorch."
 authors = ["ReasonField Lab Team"]
 maintainers = [
 	"Adam Jan Kaczmarek <adam.kaczmarek@reasonfieldlab.com>",
 	"Adam Wawrzyński <adam.wawrzynski@reasonfieldlab.com>",
 	"Kamil Rzechowski <kamil.rzechowski@reasonfieldlab.com>",
 	"Rafał Pytel <rafal.pytel@reasonfieldlab.com>"
```

### Comparing `foxai-0.5.4/PKG-INFO` & `foxai-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxai
-Version: 0.5.4
+Version: 0.6.0
 Summary: Model Interpretability for PyTorch.
 Home-page: https://github.com/softwaremill/FoXAI
 License: Apache-2.0
 Keywords: Model Interpretability,XAI,explainable AI,Model Understanding,Feature Importance,PyTorch
 Author: ReasonField Lab Team
 Maintainer: Adam Jan Kaczmarek
 Maintainer-email: adam.kaczmarek@reasonfieldlab.com
```

