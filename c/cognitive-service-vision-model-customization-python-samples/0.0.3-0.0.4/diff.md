# Comparing `tmp/cognitive-service-vision-model-customization-python-samples-0.0.3.tar.gz` & `tmp/cognitive-service-vision-model-customization-python-samples-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognitive-service-vision-model-customization-python-samples-0.0.3.tar", last modified: Fri May  5 16:18:35 2023, max compression
+gzip compressed data, was "cognitive-service-vision-model-customization-python-samples-0.0.4.tar", last modified: Tue May 23 03:12:41 2023, max compression
```

## Comparing `cognitive-service-vision-model-customization-python-samples-0.0.3.tar` & `cognitive-service-vision-model-customization-python-samples-0.0.4.tar`

### file list

```diff
@@ -1,38 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:18:35.331731 cognitive-service-vision-model-customization-python-samples-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-05 16:18:35.331731 cognitive-service-vision-model-customization-python-samples-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:18:35.327731 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:18:35.327731 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/dataset_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/evaluation_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/prediction_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/training_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:18:35.327731 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/data/check_coco_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/data/export_cvs_data_to_blob_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:18:35.331731 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/models/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/models/dataset_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/models/evaluation_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/models/training_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:18:35.327731 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-05 16:18:35.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-05 16:18:35.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:18:35.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-05 16:18:35.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-05 16:18:35.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 16:18:35.331731 cognitive-service-vision-model-customization-python-samples-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:18:35.331731 cognitive-service-vision-model-customization-python-samples-0.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/test/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/test/test_coco_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/test/test_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:41.967618 cognitive-service-vision-model-customization-python-samples-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-23 03:12:41.967618 cognitive-service-vision-model-customization-python-samples-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:41.955618 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:41.963618 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/dataset_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/evaluation_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/image_composition_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/planogram_compliance_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/prediction_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/product_recognition_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/training_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:41.963618 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/data/check_coco_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/data/export_cvs_data_to_blob_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:41.967618 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/dataset_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/evaluation_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/image_composition_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/planogram_matching_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/product_recognition_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/training_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:41.967618 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/tools/select_rectification_control_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/tools/visualize_planogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/tools/visualize_planogram_matching_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/tools/visualize_product_recognition_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:41.955618 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-23 03:12:41.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-23 03:12:41.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 03:12:41.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 03:12:41.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-23 03:12:41.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 03:12:41.967618 cognitive-service-vision-model-customization-python-samples-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:41.967618 cognitive-service-vision-model-customization-python-samples-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/test/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/test/test_coco_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/test/test_e2e.py
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.3/LICENSE` & `cognitive-service-vision-model-customization-python-samples-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.3/LICENSE.md` & `cognitive-service-vision-model-customization-python-samples-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.3/PKG-INFO` & `cognitive-service-vision-model-customization-python-samples-0.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognitive-service-vision-model-customization-python-samples
-Version: 0.0.3
+Version: 0.0.4
 Summary: A sample code repo for model customization using Python for Cognitive Service for Vision.
 Home-page: 
 Author: Ping Jin
 License: MIT
 Keywords: vision datasets classification detection
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,33 +14,40 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
 
-# Cognitive Service Vision Model Customization using Python
+# Azure Cognitive Services Computer Vision - Python SDK Samples
 
-## Intro
+## Model Customization
 
-Cognitive Service Vision Model Customization is a model training service that allows users like developers to easily train an image classification model (Multiclass only for now) or object detection model, with low-code experience and very little understanding in machine learning or computer vision required.
+Computer Vision's Model Customization is a custom model training service that allows users like developers to easily train an image classification model (Multiclass only for now) or object detection model, with low-code experience and very little understanding of machine learning or computer vision required.
 
-This is a sample repository demonstrating how to train and predict a custom model with Cognitive Service for Vision, using Python. To get started, checkout [this tutorial in Python notebook](./docs/cognitive_service_vision_model_customization.ipynb).
+This is a sample repository demonstrating how to train and predict a custom model with Cognitive Service for Vision, using Python. To get started, check out [this tutorial in Python notebook](./docs/cognitive_service_vision_model_customization.ipynb).
 
-## Existing Custom Vision (customvision.ai) Customers
+### Product Recognition
+
+One of the scenarios we would like to introudce as a model customization scenario is Product Recognition. Computer Vision's product recognition service has been designed to be used in retail scenarios, where users would like to detect products, such as Consumer Packaged Goods (CPG), on a shelf. It comes with a set of APIs, a pre-built AI model, and a custom AI model that can be trained following the model customization guide above. You can try these out by following tutorials in Python notebooks: 
+* **[Image Composition](./docs/cognitive_service_vision_image_composition.ipynb)**: for stitching together the segmented shelf images using Image Stitching API, as well as adjusting any slanted or squished shelf images to a correct orientation using Image Rectification API
+* **[Product Recognition](./docs/cognitive_service_vision_product_recognition.ipynb)**: for detecting products and gaps on a shelf image using a pre-built model, and individually classifying the detected products using customized model, both using Product Understanding API
+* **[Planogram Compliance](./docs/cognitive_service_vision_planogram_compliance.ipynb)**: for assessing the matchings between a planogram schema and the detected products on a shelf using Planogram Compliance API
+
+### Existing Custom Vision (customvision.ai) Customers
 
 Refer to [export_cvs_data_to_blob_storage.ipynb](./docs/export_cvs_data_to_blob_storage.ipynb) for instructions or directly run [export_cvs_data_to_blob_storage.py](cognitive_service_vision_model_customization_python_samples/data/export_cvs_data_to_blob_storage.py) to export Custom Vision images and annotations to your own blob storage, which can be later used for model customization training.
 
 Once data is exported, you can use it with Cognitive Service Vision Model Customization.
 
-## FAQ
+### RESTful API & SDK
 
-For frequently asked questions or quick trouble shoot, checkout [FAQ](./docs/faq.md), including things like trouble shooting guide, quota information, etc.
+If you would like to explore more functionalities offered in Cognitive Service Vision, you can refer to [this link](https://learn.microsoft.com/en-us/azure/cognitive-services/computer-vision/quickstarts-sdk/image-analysis-client-library-40?pivots=programming-language-python&tabs=visual-studio%2Cwindows) for a quick start.
 
-## RESTful API & SDK
+### FAQ & Docs
 
-If you would like to exlpore more functionalities offered in Cognitive Service Vision, you can refer to [this link](https://learn.microsoft.com/en-us/azure/cognitive-services/computer-vision/quickstarts-sdk/image-analysis-client-library-40?pivots=programming-language-python&tabs=visual-studio%2Cwindows) for a quick start.
+For frequently asked questions or quick troubleshooting, check out [FAQ](./docs/faq.md), including things like troubleshooting guides, quota information, etc.
 
-For more documentation,
+For more documentation, check out:
 
 - API: [Here](https://learn.microsoft.com/en-us/rest/api/computervision/2023-02-01-preview/models)
-- SDK: [Here](https://github.com/Azure-Samples/azure-ai-vision-sdk/tree/main/samples/python/image-analysis) (note that model customization training is not supported in this SDK yet, while prediction is supported.)
+- SDK: [Here](https://github.com/Azure-Samples/azure-ai-vision-sdk/tree/main/samples/python/image-analysis) (note that model customization training and product recognition are not supported in this SDK yet, while prediction is supported.)
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.3/README.md` & `cognitive-service-vision-model-customization-python-samples-0.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,33 @@
-# Cognitive Service Vision Model Customization using Python
+# Azure Cognitive Services Computer Vision - Python SDK Samples
 
-## Intro
+## Model Customization
 
-Cognitive Service Vision Model Customization is a model training service that allows users like developers to easily train an image classification model (Multiclass only for now) or object detection model, with low-code experience and very little understanding in machine learning or computer vision required.
+Computer Vision's Model Customization is a custom model training service that allows users like developers to easily train an image classification model (Multiclass only for now) or object detection model, with low-code experience and very little understanding of machine learning or computer vision required.
 
-This is a sample repository demonstrating how to train and predict a custom model with Cognitive Service for Vision, using Python. To get started, checkout [this tutorial in Python notebook](./docs/cognitive_service_vision_model_customization.ipynb).
+This is a sample repository demonstrating how to train and predict a custom model with Cognitive Service for Vision, using Python. To get started, check out [this tutorial in Python notebook](./docs/cognitive_service_vision_model_customization.ipynb).
 
-## Existing Custom Vision (customvision.ai) Customers
+### Product Recognition
+
+One of the scenarios we would like to introudce as a model customization scenario is Product Recognition. Computer Vision's product recognition service has been designed to be used in retail scenarios, where users would like to detect products, such as Consumer Packaged Goods (CPG), on a shelf. It comes with a set of APIs, a pre-built AI model, and a custom AI model that can be trained following the model customization guide above. You can try these out by following tutorials in Python notebooks: 
+* **[Image Composition](./docs/cognitive_service_vision_image_composition.ipynb)**: for stitching together the segmented shelf images using Image Stitching API, as well as adjusting any slanted or squished shelf images to a correct orientation using Image Rectification API
+* **[Product Recognition](./docs/cognitive_service_vision_product_recognition.ipynb)**: for detecting products and gaps on a shelf image using a pre-built model, and individually classifying the detected products using customized model, both using Product Understanding API
+* **[Planogram Compliance](./docs/cognitive_service_vision_planogram_compliance.ipynb)**: for assessing the matchings between a planogram schema and the detected products on a shelf using Planogram Compliance API
+
+### Existing Custom Vision (customvision.ai) Customers
 
 Refer to [export_cvs_data_to_blob_storage.ipynb](./docs/export_cvs_data_to_blob_storage.ipynb) for instructions or directly run [export_cvs_data_to_blob_storage.py](cognitive_service_vision_model_customization_python_samples/data/export_cvs_data_to_blob_storage.py) to export Custom Vision images and annotations to your own blob storage, which can be later used for model customization training.
 
 Once data is exported, you can use it with Cognitive Service Vision Model Customization.
 
-## FAQ
+### RESTful API & SDK
 
-For frequently asked questions or quick trouble shoot, checkout [FAQ](./docs/faq.md), including things like trouble shooting guide, quota information, etc.
+If you would like to explore more functionalities offered in Cognitive Service Vision, you can refer to [this link](https://learn.microsoft.com/en-us/azure/cognitive-services/computer-vision/quickstarts-sdk/image-analysis-client-library-40?pivots=programming-language-python&tabs=visual-studio%2Cwindows) for a quick start.
 
-## RESTful API & SDK
+### FAQ & Docs
 
-If you would like to exlpore more functionalities offered in Cognitive Service Vision, you can refer to [this link](https://learn.microsoft.com/en-us/azure/cognitive-services/computer-vision/quickstarts-sdk/image-analysis-client-library-40?pivots=programming-language-python&tabs=visual-studio%2Cwindows) for a quick start.
+For frequently asked questions or quick troubleshooting, check out [FAQ](./docs/faq.md), including things like troubleshooting guides, quota information, etc.
 
-For more documentation,
+For more documentation, check out:
 
 - API: [Here](https://learn.microsoft.com/en-us/rest/api/computervision/2023-02-01-preview/models)
-- SDK: [Here](https://github.com/Azure-Samples/azure-ai-vision-sdk/tree/main/samples/python/image-analysis) (note that model customization training is not supported in this SDK yet, while prediction is supported.)
+- SDK: [Here](https://github.com/Azure-Samples/azure-ai-vision-sdk/tree/main/samples/python/image-analysis) (note that model customization training and product recognition are not supported in this SDK yet, while prediction is supported.)
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 import requests
 from ..clients.common import ResourceType
 
 logger = logging.getLogger(__name__)
 
 
 class Client:
-    def __init__(self, resource_type, resource_name: str, multi_service_endpoint, resource_key: str) -> None:
+    def __init__(self, resource_type, resource_name: str, multi_service_endpoint, resource_key: str, api_version: str='2023-04-01-preview') -> None:
         resource_type = ResourceType(resource_type) if isinstance(resource_type, str) else resource_type
 
         if resource_type == ResourceType.MULTI_SERVICE_RESOURCE:
             assert multi_service_endpoint
             self._endpoint = urllib.parse.urljoin(multi_service_endpoint, '/computervision')
         else:
             assert resource_name
             self._endpoint = f'https://{resource_name}.cognitiveservices.azure.com/computervision'
 
         self._headers = {'Ocp-Apim-Subscription-Key': resource_key}
-        self._params = {'api-version': '2023-02-01-preview'}
+        self._params = {'api-version': api_version}
 
     def _construct_url(self, path):
         return self._endpoint + '/' + path
 
     @staticmethod
     def _get_json_response(response):
         if not response.ok:
@@ -33,24 +33,30 @@
         logger.debug(f"Response: {json_response}")
         return json_response
 
     def request_get(self, path):
         r = requests.get(self._construct_url(path), params=self._params, headers=self._headers)
         return self._get_json_response(r)
 
-    def request_put(self, path, json):
-        r = requests.put(self._construct_url(path), json=json, params=self._params, headers=self._headers)
+    def request_put(self, path, json=None, data=None, content_type=None):
+        headers = dict(self._headers, **{'Content-Type': content_type}) if content_type else self._headers
+
+        r = requests.put(self._construct_url(path), json=json, params=self._params, data=data, headers=headers)
         return self._get_json_response(r)
 
     def request_post(self, path, params=None, data=None, content_type=None):
         assert data is None or content_type
 
         params = params or {}
         headers = dict(self._headers, **{'Content-Type': content_type}) if content_type else self._headers
         r = requests.post(self._construct_url(path), data=data, params=dict(self._params, **params), headers=headers)
+
+        if r.get(headers['Content-Type'], None) == 'image/jpeg':
+            return r.content
+
         return self._get_json_response(r)
 
     def request_patch(self, path, json):
         r = requests.patch(self._construct_url(path), json=json, params=self._params, headers=self._headers)
         return self._get_json_response(r)
 
     def request_delete(self, path):
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/dataset_client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/dataset_client.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/evaluation_client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/evaluation_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
     def query_run(self, name, model_name) -> EvaluationResponse:
         json_response = self.request_get(f'/models/{model_name}/evaluations/{name}')
         return EvaluationResponse.from_response(json_response)
 
     def wait_for_completion(self, name: str, model_name: str, check_wait_in_secs: int = 60) -> EvaluationResponse:
         start_time = time.time()
+        total_elapsed = 0
         while True:
             eval_run = self.query_run(name, model_name)
             status = eval_run.status
             if status in [EvaluationStatus.FAILED, EvaluationStatus.SUCCEEDED]:
                 break
             time.sleep(check_wait_in_secs)
             total_elapsed = time.time() - start_time
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/training_client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/training_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import time
 import logging
+from typing import Tuple, Any
 
 from .client import Client
 from ..models import Model, ModelResponse, ModelStatus, Evaluation, EvaluationStatus, EvaluationResponse
 
 logger = logging.getLogger(__name__)
 
 
@@ -62,15 +63,15 @@
             logger.warning(f'Evaluation failed: {evaluation.error.code}, {evaluation.error.message}')
         else:
             logger.info(f'Wall-clock time {total_elapsed} seconds.')
             logger.info(f'Model performance: {evaluation.model_performance}')
 
         return evaluation
 
-    def _wait_for_completion(self, query, ending_states, check_wait_in_secs: int = 60) -> ModelResponse:
+    def _wait_for_completion(self, query, ending_states, check_wait_in_secs: int = 60) -> Tuple[Any, float]:
         start_time = time.time()
         total_elapsed = 0
         while True:
             entity, status = query()
             if status in ending_states:
                 break
             time.sleep(check_wait_in_secs)
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/data/check_coco_annotations.py` & `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/data/check_coco_annotations.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/data/export_cvs_data_to_blob_storage.py` & `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/data/export_cvs_data_to_blob_storage.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/models/dataset_models.py` & `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/dataset_models.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/models/evaluation_models.py` & `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/evaluation_models.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/models/training_models.py` & `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/training_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import enum
+from typing import Optional
 
 from .common import Error
 from .evaluation_models import EvaluationParameters
 
 
 class ModelKind(enum.Enum):
     GENERIC_IC = 'Generic-Classifier'
     GENERIC_OD = 'Generic-Detector'
+    PRODUCT_RECOGNIZER = 'Product-Recognizer'
 
 
 class ModelStatus(enum.Enum):
     NOT_STARTED = 'notStarted'
     TRAINING = 'training'
     SUCCEEDED = 'succeeded'
     FAILED = 'failed'
@@ -37,15 +39,15 @@
         }
 
     def __str__(self):
         return f'TrainingParameters(dataset={self.training_dataset_name}, budget={self.time_budget_in_hours}, model_kind={self.model_kind})'
 
 
 class Model:
-    def __init__(self, name: str, trainingParams: TrainingParameters, evaluationParams: EvaluationParameters = None) -> None:
+    def __init__(self, name: str, trainingParams: TrainingParameters, evaluationParams: Optional[EvaluationParameters] = None) -> None:
         assert name
         self.name = name
         self.training_params = trainingParams
         self.evaluation_params = evaluationParams
 
     @property
     def params(self) -> dict:
@@ -56,15 +58,15 @@
 
     def __str__(self):
         return f'Model(name={self.name}, training_params={self.training_params}, evaluation_params={self.evaluation_params})'
 
 
 class ModelResponse(Model):
     def __init__(self, name: str, trainingParams: TrainingParameters, training_cost_in_minutes: int, status: ModelStatus, model_performance: dict, created_date_time: str, updated_date_time: str,
-                 error: Error, evaluationParams: EvaluationParameters = None) -> None:
+                 error: Error, evaluationParams: Optional[EvaluationParameters] = None) -> None:
         super().__init__(name, trainingParams, evaluationParams)
         self.training_cost_in_minutes = training_cost_in_minutes
         self.status = status
         self.model_performance = model_performance
         self.created_date_time = created_date_time
         self.updated_date_time = updated_date_time
         self.error = error
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples.egg-info/PKG-INFO` & `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognitive-service-vision-model-customization-python-samples
-Version: 0.0.3
+Version: 0.0.4
 Summary: A sample code repo for model customization using Python for Cognitive Service for Vision.
 Home-page: 
 Author: Ping Jin
 License: MIT
 Keywords: vision datasets classification detection
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,33 +14,40 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
 
-# Cognitive Service Vision Model Customization using Python
+# Azure Cognitive Services Computer Vision - Python SDK Samples
 
-## Intro
+## Model Customization
 
-Cognitive Service Vision Model Customization is a model training service that allows users like developers to easily train an image classification model (Multiclass only for now) or object detection model, with low-code experience and very little understanding in machine learning or computer vision required.
+Computer Vision's Model Customization is a custom model training service that allows users like developers to easily train an image classification model (Multiclass only for now) or object detection model, with low-code experience and very little understanding of machine learning or computer vision required.
 
-This is a sample repository demonstrating how to train and predict a custom model with Cognitive Service for Vision, using Python. To get started, checkout [this tutorial in Python notebook](./docs/cognitive_service_vision_model_customization.ipynb).
+This is a sample repository demonstrating how to train and predict a custom model with Cognitive Service for Vision, using Python. To get started, check out [this tutorial in Python notebook](./docs/cognitive_service_vision_model_customization.ipynb).
 
-## Existing Custom Vision (customvision.ai) Customers
+### Product Recognition
+
+One of the scenarios we would like to introudce as a model customization scenario is Product Recognition. Computer Vision's product recognition service has been designed to be used in retail scenarios, where users would like to detect products, such as Consumer Packaged Goods (CPG), on a shelf. It comes with a set of APIs, a pre-built AI model, and a custom AI model that can be trained following the model customization guide above. You can try these out by following tutorials in Python notebooks: 
+* **[Image Composition](./docs/cognitive_service_vision_image_composition.ipynb)**: for stitching together the segmented shelf images using Image Stitching API, as well as adjusting any slanted or squished shelf images to a correct orientation using Image Rectification API
+* **[Product Recognition](./docs/cognitive_service_vision_product_recognition.ipynb)**: for detecting products and gaps on a shelf image using a pre-built model, and individually classifying the detected products using customized model, both using Product Understanding API
+* **[Planogram Compliance](./docs/cognitive_service_vision_planogram_compliance.ipynb)**: for assessing the matchings between a planogram schema and the detected products on a shelf using Planogram Compliance API
+
+### Existing Custom Vision (customvision.ai) Customers
 
 Refer to [export_cvs_data_to_blob_storage.ipynb](./docs/export_cvs_data_to_blob_storage.ipynb) for instructions or directly run [export_cvs_data_to_blob_storage.py](cognitive_service_vision_model_customization_python_samples/data/export_cvs_data_to_blob_storage.py) to export Custom Vision images and annotations to your own blob storage, which can be later used for model customization training.
 
 Once data is exported, you can use it with Cognitive Service Vision Model Customization.
 
-## FAQ
+### RESTful API & SDK
 
-For frequently asked questions or quick trouble shoot, checkout [FAQ](./docs/faq.md), including things like trouble shooting guide, quota information, etc.
+If you would like to explore more functionalities offered in Cognitive Service Vision, you can refer to [this link](https://learn.microsoft.com/en-us/azure/cognitive-services/computer-vision/quickstarts-sdk/image-analysis-client-library-40?pivots=programming-language-python&tabs=visual-studio%2Cwindows) for a quick start.
 
-## RESTful API & SDK
+### FAQ & Docs
 
-If you would like to exlpore more functionalities offered in Cognitive Service Vision, you can refer to [this link](https://learn.microsoft.com/en-us/azure/cognitive-services/computer-vision/quickstarts-sdk/image-analysis-client-library-40?pivots=programming-language-python&tabs=visual-studio%2Cwindows) for a quick start.
+For frequently asked questions or quick troubleshooting, check out [FAQ](./docs/faq.md), including things like troubleshooting guides, quota information, etc.
 
-For more documentation,
+For more documentation, check out:
 
 - API: [Here](https://learn.microsoft.com/en-us/rest/api/computervision/2023-02-01-preview/models)
-- SDK: [Here](https://github.com/Azure-Samples/azure-ai-vision-sdk/tree/main/samples/python/image-analysis) (note that model customization training is not supported in this SDK yet, while prediction is supported.)
+- SDK: [Here](https://github.com/Azure-Samples/azure-ai-vision-sdk/tree/main/samples/python/image-analysis) (note that model customization training and product recognition are not supported in this SDK yet, while prediction is supported.)
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples.egg-info/SOURCES.txt` & `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -9,21 +9,32 @@
 cognitive_service_vision_model_customization_python_samples.egg-info/requires.txt
 cognitive_service_vision_model_customization_python_samples.egg-info/top_level.txt
 cognitive_service_vision_model_customization_python_samples/clients/__init__.py
 cognitive_service_vision_model_customization_python_samples/clients/client.py
 cognitive_service_vision_model_customization_python_samples/clients/common.py
 cognitive_service_vision_model_customization_python_samples/clients/dataset_client.py
 cognitive_service_vision_model_customization_python_samples/clients/evaluation_client.py
+cognitive_service_vision_model_customization_python_samples/clients/image_composition_client.py
+cognitive_service_vision_model_customization_python_samples/clients/planogram_compliance_client.py
 cognitive_service_vision_model_customization_python_samples/clients/prediction_client.py
+cognitive_service_vision_model_customization_python_samples/clients/product_recognition_client.py
 cognitive_service_vision_model_customization_python_samples/clients/training_client.py
 cognitive_service_vision_model_customization_python_samples/data/__init__.py
 cognitive_service_vision_model_customization_python_samples/data/check_coco_annotations.py
 cognitive_service_vision_model_customization_python_samples/data/export_cvs_data_to_blob_storage.py
 cognitive_service_vision_model_customization_python_samples/models/__init__.py
 cognitive_service_vision_model_customization_python_samples/models/common.py
 cognitive_service_vision_model_customization_python_samples/models/dataset_models.py
 cognitive_service_vision_model_customization_python_samples/models/evaluation_models.py
+cognitive_service_vision_model_customization_python_samples/models/image_composition_model.py
+cognitive_service_vision_model_customization_python_samples/models/planogram_matching_model.py
+cognitive_service_vision_model_customization_python_samples/models/product_recognition_model.py
 cognitive_service_vision_model_customization_python_samples/models/training_models.py
+cognitive_service_vision_model_customization_python_samples/tools/__init__.py
+cognitive_service_vision_model_customization_python_samples/tools/select_rectification_control_points.py
+cognitive_service_vision_model_customization_python_samples/tools/visualize_planogram.py
+cognitive_service_vision_model_customization_python_samples/tools/visualize_planogram_matching_result.py
+cognitive_service_vision_model_customization_python_samples/tools/visualize_product_recognition_result.py
 test/__init__.py
 test/test_clients.py
 test/test_coco_check.py
 test/test_e2e.py
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.3/setup.py` & `cognitive-service-vision-model-customization-python-samples-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 from os import path
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), 'r') as f:
     long_description = f.read()
 
@@ -22,15 +22,16 @@
                  keywords='vision datasets classification detection',
                  packages=setuptools.find_packages(),
                  install_requires=[
                      'requests',
                      'tqdm',
                      'azure-storage-blob',
                      'azure-cognitiveservices-vision-customvision',
-                     'cffi'
+                     'cffi',
+                     'opencv-python-headless'
                  ],
                  classifiers=[
                      'Development Status :: 4 - Beta',
                      'Intended Audience :: Developers',
                      'License :: OSI Approved :: MIT License',
                      'Programming Language :: Python :: 3.7',
                      'Programming Language :: Python :: 3.8',
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.3/test/test_clients.py` & `cognitive-service-vision-model-customization-python-samples-0.0.4/test/test_clients.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.3/test/test_coco_check.py` & `cognitive-service-vision-model-customization-python-samples-0.0.4/test/test_coco_check.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.3/test/test_e2e.py` & `cognitive-service-vision-model-customization-python-samples-0.0.4/test/test_e2e.py`

 * *Files 24% similar despite different names*

```diff
@@ -68,39 +68,63 @@
             dataset.custom_properties['key2'] = 'value2'
             response = dataset_client.update_dataset(dataset)
             self.assertEqual(response.custom_properties, {'key': 'value', 'key2': 'value2'})
         finally:
             dataset_client.delete_dataset(dataset_name)
 
     @unittest.skipUnless(is_configured(), "requires endpoint info")
-    def test_request_training(self):
+    def test_request_training_ic(self):
+        self.test_request_training_core(ModelKind.GENERIC_IC)
+
+    @unittest.skipUnless(is_configured(), "requires endpoint info")
+    def test_request_training_od(self):
+        self.test_request_training_core(ModelKind.GENERIC_OD)
+
+    @unittest.skipUnless(is_configured(), "requires endpoint info")
+    def test_request_training_pr(self):
+        self.test_request_training_core(ModelKind.PRODUCT_RECOGNITION)
+
+    @unittest.skipUnless(is_configured(), "requires endpoint info")
+    def test_request_training_core(self, model_kind=ModelKind.GENERIC_IC):
         dataset_name = str(uuid.uuid4())
         dataset_client = DatasetClient(ResourceType.MULTI_SERVICE_RESOURCE, None, self.endpoint, self.resource_key)
         dataset = Dataset(name=dataset_name, annotation_kind=AnnotationKind.OBJECT_DETECTION, annotation_file_uris=[self.od_dataset_url], custom_properties={'key': 'value'})
         model_name = dataset_name + '_model'
-        model = Model(model_name, TrainingParameters(training_dataset_name=dataset_name, time_budget_in_hours=1, model_kind=ModelKind.GENERIC_OD))
+        model = Model(model_name, TrainingParameters(training_dataset_name=dataset_name, time_budget_in_hours=1, model_kind=model_kind))
         training_client = TrainingClient(ResourceType.MULTI_SERVICE_RESOURCE, None, self.endpoint, self.resource_key)
         try:
             dataset_client.register_dataset(dataset)
             response = training_client.train_model(model)
             self.assertEqual(response.status, ModelStatus.NOT_STARTED)
             response = training_client.query_model(model_name)
             self.assertIn(response.status, [ModelStatus.NOT_STARTED, ModelStatus.TRAINING])
             training_client.cancel_model_training(model_name)
         finally:
             dataset_client.delete_dataset(dataset_name)
 
     @unittest.skipUnless(is_configured(), "requires endpoint info")
-    def test_request_evaluation(self):
+    def test_request_evaluation_ic(self):
+        self.test_request_evaluation_core(ModelKind.GENERIC_IC)
+
+    @unittest.skipUnless(is_configured(), "requires endpoint info")
+    def test_request_evaluation_od(self):
+        self.test_request_evaluation_core(ModelKind.GENERIC_OD)
+
+    @unittest.skipUnless(is_configured(), "requires endpoint info")
+    def test_request_evaluation_pr(self):
+        self.test_request_evaluation_core(ModelKind.PRODUCT_RECOGNITION)
+
+    @unittest.skipUnless(is_configured(), "requires endpoint info")
+    def test_request_evaluation_core(self, model_kind=ModelKind.GENERIC_IC):
         dataset_name = str(uuid.uuid4())
         dataset_client = DatasetClient(ResourceType.MULTI_SERVICE_RESOURCE, None, self.endpoint, self.resource_key)
         evaluation_client = EvaluationClient(ResourceType.MULTI_SERVICE_RESOURCE, None, self.endpoint, self.resource_key)
         dataset = Dataset(name=dataset_name, annotation_kind=AnnotationKind.OBJECT_DETECTION, annotation_file_uris=[self.od_dataset_url], custom_properties={'key': 'value'})
         model_name = dataset_name + '_model'
-        model = Model(model_name, TrainingParameters(training_dataset_name=dataset_name, time_budget_in_hours=1, model_kind=ModelKind.GENERIC_OD))
+        model = Model(model_name, TrainingParameters(training_dataset_name=dataset_name, time_budget_in_hours=1, model_kind=model_kind))
         training_client = TrainingClient(ResourceType.MULTI_SERVICE_RESOURCE, None, self.endpoint, self.resource_key)
         evaluation = Evaluation('test_eval', model_name, dataset_name)
         try:
             dataset_client.register_dataset(dataset)
             training_client.train_model(model)
             response = training_client.wait_for_completion(model_name)
             self.assertEqual(response.status, ModelStatus.SUCCEEDED)
```

