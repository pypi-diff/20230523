# Comparing `tmp/mlcvzoo_mmdetection-5.0.1.tar.gz` & `tmp/mlcvzoo_mmdetection-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcvzoo_mmdetection-5.0.1.tar", max compression
+gzip compressed data, was "mlcvzoo_mmdetection-5.1.1.tar", max compression
```

## Comparing `mlcvzoo_mmdetection-5.0.1.tar` & `mlcvzoo_mmdetection-5.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      423 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/README.md
--rw-r--r--   0        0        0      177 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/__init__.py
--rw-r--r--   0        0        0     5279 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/configuration.py
--rw-r--r--   0        0        0     7641 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/mlcvzoo_mmdet_dataset.py
--rw-r--r--   0        0        0    15578 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/model.py
--rw-r--r--   0        0        0     6835 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/object_detection_model.py
--rw-r--r--   0        0        0      154 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/py.typed
--rw-r--r--   0        0        0    11398 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/third_party/LICENSE
--rw-r--r--   0        0        0      109 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/third_party/README.md
--rw-r--r--   0        0        0      154 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/third_party/__init__.py
--rw-r--r--   0        0        0     2590 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/third_party/mmdetection.py
--rw-r--r--   0        0        0     2643 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/utils.py
--rw-r--r--   0        0        0     3913 2023-05-02 10:18:08.293754 mlcvzoo_mmdetection-5.0.1/pyproject.toml
--rw-r--r--   0        0        0     1640 1970-01-01 00:00:00.000000 mlcvzoo_mmdetection-5.0.1/setup.py
--rw-r--r--   0        0        0     2070 1970-01-01 00:00:00.000000 mlcvzoo_mmdetection-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0      423 2023-05-22 10:51:20.525114 mlcvzoo_mmdetection-5.1.1/README.md
+-rw-r--r--   0        0        0      177 2023-05-22 10:51:20.525114 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/__init__.py
+-rw-r--r--   0        0        0     5279 2023-05-23 07:13:04.241771 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/configuration.py
+-rw-r--r--   0        0        0     8133 2023-05-23 07:13:04.241771 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/mlcvzoo_mmdet_dataset.py
+-rw-r--r--   0        0        0    15578 2023-05-23 07:13:04.245771 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/model.py
+-rw-r--r--   0        0        0     6835 2023-05-23 07:13:04.245771 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/object_detection_model.py
+-rw-r--r--   0        0        0      154 2023-05-22 10:51:20.525114 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/py.typed
+-rw-r--r--   0        0        0     9744 2023-05-23 08:40:45.799876 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/segmentation_model.py
+-rw-r--r--   0        0        0    11398 2023-05-23 07:13:04.245771 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/third_party/LICENSE
+-rw-r--r--   0        0        0      109 2023-05-23 07:13:04.245771 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/third_party/README.md
+-rw-r--r--   0        0        0      154 2023-05-23 07:13:04.245771 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/third_party/__init__.py
+-rw-r--r--   0        0        0     2590 2023-05-23 07:13:04.245771 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/third_party/mmdetection.py
+-rw-r--r--   0        0        0     2643 2023-05-23 07:13:04.245771 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/utils.py
+-rw-r--r--   0        0        0     4014 2023-05-23 09:26:31.124042 mlcvzoo_mmdetection-5.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1648 1970-01-01 00:00:00.000000 mlcvzoo_mmdetection-5.1.1/setup.py
+-rw-r--r--   0        0        0     2078 1970-01-01 00:00:00.000000 mlcvzoo_mmdetection-5.1.1/PKG-INFO
```

### Comparing `mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/configuration.py` & `mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/mlcvzoo_mmdet_dataset.py` & `mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/mlcvzoo_mmdet_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -177,15 +177,28 @@
         gt_bboxes_ignore: np.ndarray = np.zeros((0, 4), dtype=np.float32)  # type: ignore[type-arg]
 
         annotation = self.annotations[idx]
 
         for bounding_box in annotation.bounding_boxes:
             gt_labels.append(bounding_box.class_id)
             gt_bboxes.append(bounding_box.box.to_list(dst_type=float))
-            gt_masks_ann.append(None)
+            gt_masks_ann.append(
+                [
+                    [
+                        float(bounding_box.box.xmin),
+                        float(bounding_box.box.ymin),
+                        float(bounding_box.box.xmax),
+                        float(bounding_box.box.ymin),
+                        float(bounding_box.box.xmax),
+                        float(bounding_box.box.ymax),
+                        float(bounding_box.box.xmin),
+                        float(bounding_box.box.ymax),
+                    ]
+                ]
+            )
 
         for segmentation in annotation.segmentations:
             gt_labels.append(segmentation.class_id)
             if segmentation.box is not None:
                 gt_bboxes.append(segmentation.box.to_list(dst_type=float))
             else:
                 gt_bboxes.append([0.0, 0.0, 0.0, 0.0])
@@ -205,12 +218,11 @@
         seg_map = annotation.image_path
 
         ann: Dict[str, Any] = dict(
             labels=gt_labels_np,
             bboxes=gt_bboxes_np,
             bboxes_ignore=gt_bboxes_ignore,
             masks=gt_masks_ann,
-            masks_ignore=[],
             seg_map=seg_map,
         )
 
         return ann
```

### Comparing `mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/model.py` & `mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/model.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/object_detection_model.py` & `mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/object_detection_model.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/third_party/LICENSE` & `mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/third_party/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/third_party/mmdetection.py` & `mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/third_party/mmdetection.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmdetection-5.0.1/mlcvzoo_mmdetection/utils.py` & `mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmdetection-5.0.1/pyproject.toml` & `mlcvzoo_mmdetection-5.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlcvzoo_mmdetection"
-version = "5.0.1"
+version = "5.1.1"
 license = "Open Logistics License Version 1.0"
 description = "MLCVZoo MMDetection Package"
 readme = "README.md"
 homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc"
 classifiers = [
@@ -42,15 +42,16 @@
 opencv-contrib-python = { version = "^4.5,!=4.5.5.64,!=4.6.0.66" }
 mmdet = { version="^2.14.0" }
 mmcv-full = { version="^1.3,!=1.3.18" }
 pycocotools = { version=">=2.0.2", markers = "platform_machine == 'x86_64'" }
 # 1.19.2 is oldest available on aarch64 but 1.19.5 leads to unbuildable pytorch there, all is well on amd64
 numpy = { version = ">=1.19.2,!=1.19.5" }
 nptyping = { version = ">=2.0" }
-torch = { version = ">=1.9" }
+# torch 2.0.1 has missing cuda dependencies https://github.com/pytorch/pytorch/issues/100974
+torch = { version = ">=1.9,!=2.0.1" }
 torchvision = { version = ">=0.10" }
 
 [tool.poetry.dev-dependencies]
 mock = { version = ">=4.0" }
 pytest = { version = ">=7.0" }
 pytest-cov = { version = ">=3.0.0" }
 black = { version = ">=22" }
```

### Comparing `mlcvzoo_mmdetection-5.0.1/setup.py` & `mlcvzoo_mmdetection-5.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,24 +13,24 @@
  'mmcv-full>=1.3,<2.0,!=1.3.18',
  'mmdet>=2.14.0,<3.0.0',
  'nptyping>=2.0',
  'numpy>=1.19.2,!=1.19.5',
  'opencv-contrib-python>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66',
  'opencv-python>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66',
  'related-mltoolbox>=1,<2',
- 'torch>=1.9',
+ 'torch>=1.9,!=2.0.1',
  'torchvision>=0.10',
  'yaml-config-builder>=8,<9']
 
 extras_require = \
 {':platform_machine == "x86_64"': ['pycocotools>=2.0.2']}
 
 setup_kwargs = {
     'name': 'mlcvzoo-mmdetection',
-    'version': '5.0.1',
+    'version': '5.1.1',
     'description': 'MLCVZoo MMDetection Package',
     'long_description': '# MLCVZoo MMDetection\n\nThe MLCVZoo is an SDK for simplifying the usage of various (machine learning driven)\ncomputer vision algorithms. The package **mlcvzoo_mmdetection** is the wrapper module for\nthe [mmdetection framework](https://github.com/open-mmlab/mmdetection).\n\nFurther information about the MLCVZoo can be found [here](../README.md).\n\n## Install\n`\npip install mlcvzoo-mmdetection\n`\n\n## Technology stack\n\n- Python\n',
     'author': 'Maximilian Otten',
     'author_email': 'maximilian.otten@iml.fraunhofer.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo',
```

### Comparing `mlcvzoo_mmdetection-5.0.1/PKG-INFO` & `mlcvzoo_mmdetection-5.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlcvzoo-mmdetection
-Version: 5.0.1
+Version: 5.1.1
 Summary: MLCVZoo MMDetection Package
 Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
 License: Open Logistics License Version 1.0
 Author: Maximilian Otten
 Author-email: maximilian.otten@iml.fraunhofer.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,15 +22,15 @@
 Requires-Dist: mmdet (>=2.14.0,<3.0.0)
 Requires-Dist: nptyping (>=2.0)
 Requires-Dist: numpy (>=1.19.2,!=1.19.5)
 Requires-Dist: opencv-contrib-python (>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66)
 Requires-Dist: opencv-python (>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66)
 Requires-Dist: pycocotools (>=2.0.2) ; platform_machine == "x86_64"
 Requires-Dist: related-mltoolbox (>=1,<2)
-Requires-Dist: torch (>=1.9)
+Requires-Dist: torch (>=1.9,!=2.0.1)
 Requires-Dist: torchvision (>=0.10)
 Requires-Dist: yaml-config-builder (>=8,<9)
 Project-URL: Documentation, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc
 Project-URL: Repository, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
 Description-Content-Type: text/markdown
 
 # MLCVZoo MMDetection
```

