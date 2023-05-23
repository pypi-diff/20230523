# Comparing `tmp/mlcvzoo_base-5.3.2.tar.gz` & `tmp/mlcvzoo_base-5.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcvzoo_base-5.3.2.tar", max compression
+gzip compressed data, was "mlcvzoo_base-5.3.3.tar", max compression
```

## Comparing `mlcvzoo_base-5.3.2.tar` & `mlcvzoo_base-5.3.3.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0      546 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/README.md
--rw-r--r--   0        0        0      177 2023-03-21 12:52:16.680345 mlcvzoo_base-5.3.2/mlcvzoo_base/__init__.py
--rw-r--r--   0        0        0      154 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/api/__init__.py
--rw-r--r--   0        0        0      979 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/api/configuration.py
--rw-r--r--   0        0        0      154 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/__init__.py
--rw-r--r--   0        0        0    11228 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/annotation.py
--rw-r--r--   0        0        0      774 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/annotation_attributes.py
--rw-r--r--   0        0        0     2387 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/annotation_builder.py
--rw-r--r--   0        0        0    26735 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/annotation_class_mapper.py
--rw-r--r--   0        0        0     1088 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/annotation_parser.py
--rw-r--r--   0        0        0      933 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/annotation_writer.py
--rw-r--r--   0        0        0     6104 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/bounding_box.py
--rw-r--r--   0        0        0    12979 2023-03-21 13:20:34.265290 mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/box.py
--rw-r--r--   0        0        0     2692 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/class_identifier.py
--rw-r--r--   0        0        0     5211 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/classification.py
--rw-r--r--   0        0        0     3899 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/dataset_info.py
--rw-r--r--   0        0        0     3226 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/ocr_perception.py
--rw-r--r--   0        0        0    11613 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/segmentation.py
--rw-r--r--   0        0        0      320 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/types.py
--rw-r--r--   0        0        0      864 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/api/exceptions.py
--rw-r--r--   0        0        0     4987 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/api/interfaces.py
--rw-r--r--   0        0        0    12201 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/api/model.py
--rw-r--r--   0        0        0     2291 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/api/registry.py
--rw-r--r--   0        0        0      154 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/__init__.py
--rw-r--r--   0        0        0     8178 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/annotation_handler_config.py
--rw-r--r--   0        0        0     3900 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/class_mapping_config.py
--rw-r--r--   0        0        0      614 2023-03-20 17:23:38.508115 mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/config_registry.py
--rw-r--r--   0        0        0      730 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/device_query.py
--rw-r--r--   0        0        0     1656 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/mlfow_config.py
--rw-r--r--   0        0        0     3051 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/model_config.py
--rw-r--r--   0        0        0     2553 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/reduction_mapping_config.py
--rw-r--r--   0        0        0     3847 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/replacement_config.py
--rw-r--r--   0        0        0     3897 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/structs.py
--rw-r--r--   0        0        0     7269 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/utils.py
--rw-r--r--   0        0        0      586 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/visualization_config.py
--rw-r--r--   0        0        0      154 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/__init__.py
--rw-r--r--   0        0        0      214 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_builder/__init__.py
--rw-r--r--   0        0        0     8621 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_builder/coco_annotation_builder.py
--rw-r--r--   0        0        0     7079 2023-03-21 12:56:56.843107 mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_builder/csv_annotation_builder.py
--rw-r--r--   0        0        0     2416 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_builder/cvat_annotation_builder.py
--rw-r--r--   0        0        0     8820 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_builder/mot_annotation_builder.py
--rw-r--r--   0        0        0     6024 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_builder/pascal_voc_annotation_builder.py
--rw-r--r--   0        0        0    14606 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_handler.py
--rw-r--r--   0        0        0      154 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_parser/__init__.py
--rw-r--r--   0        0        0     3247 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_parser/coco_annotation_parser.py
--rw-r--r--   0        0        0     8126 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_parser/csv_annotation_parser.py
--rw-r--r--   0        0        0    11586 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_parser/cvat_annotation_parser.py
--rw-r--r--   0        0        0     7799 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_parser/label_studio_annotation_parser.py
--rw-r--r--   0        0        0    10575 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_parser/mot_annotation_parser.py
--rw-r--r--   0        0        0     9163 2023-03-21 12:56:56.843107 mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_parser/pascal_voc_annotation_parser.py
--rw-r--r--   0        0        0      154 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_writer/__init__.py
--rw-r--r--   0        0        0    14675 2023-03-21 12:56:56.847107 mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_writer/csv_annotation_writer.py
--rw-r--r--   0        0        0     8642 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_writer/cvat_annotation_writer.py
--rw-r--r--   0        0        0     4055 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_writer/darknet_annotation_writer.py
--rw-r--r--   0        0        0      459 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/structs.py
--rw-r--r--   0        0        0    11192 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/utils.py
--rw-r--r--   0        0        0      154 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/evaluation/__init__.py
--rw-r--r--   0        0        0      154 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/evaluation/object_detection/__init__.py
--rw-r--r--   0        0        0     2191 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/evaluation/object_detection/configuration.py
--rw-r--r--   0        0        0     6794 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/evaluation/object_detection/data_classes.py
--rw-r--r--   0        0        0    54055 2023-03-21 12:56:56.847107 mlcvzoo_base-5.3.2/mlcvzoo_base/evaluation/object_detection/metrics_computation.py
--rw-r--r--   0        0        0    12253 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/evaluation/object_detection/metrics_logging.py
--rw-r--r--   0        0        0     4092 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/evaluation/object_detection/model_evaluation.py
--rw-r--r--   0        0        0      591 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/evaluation/object_detection/structs.py
--rw-r--r--   0        0        0    15604 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/evaluation/object_detection/utils.py
--rw-r--r--   0        0        0      154 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/metrics/__init__.py
--rw-r--r--   0        0        0      154 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/metrics/mlflow/__init__.py
--rw-r--r--   0        0        0     7219 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/metrics/mlflow/mlflow_runner.py
--rw-r--r--   0        0        0     1634 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/metrics/mlflow/utils.py
--rw-r--r--   0        0        0      154 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/models/__init__.py
--rw-r--r--   0        0        0      215 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/models/constants.py
--rw-r--r--   0        0        0    10663 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/models/model_registry.py
--rw-r--r--   0        0        0      154 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/models/read_from_file/__init__.py
--rw-r--r--   0        0        0     1498 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/models/read_from_file/configuration.py
--rw-r--r--   0        0        0    10671 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/models/read_from_file/model.py
--rw-r--r--   0        0        0      154 2023-03-20 17:23:38.512115 mlcvzoo_base-5.3.2/mlcvzoo_base/py.typed
--rw-r--r--   0        0        0        0 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/third_party/__init__.py
--rw-r--r--   0        0        0     1078 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/third_party/efficientdet_pytorch/LICENSE
--rw-r--r--   0        0        0      138 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/third_party/efficientdet_pytorch/README.md
--rw-r--r--   0        0        0      249 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/third_party/efficientdet_pytorch/__init__.py
--rw-r--r--   0        0        0     1774 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/third_party/efficientdet_pytorch/computer_overlap.py
--rw-r--r--   0        0        0     1117 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/third_party/imutils/LICENSE.txt
--rw-r--r--   0        0        0      108 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/third_party/imutils/README.md
--rw-r--r--   0        0        0      296 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/third_party/imutils/__init__.py
--rw-r--r--   0        0        0     2794 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/third_party/imutils/perspective.py
--rw-r--r--   0        0        0     3744 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/third_party/py_faster_rcnn/LICENSE
--rw-r--r--   0        0        0      127 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/third_party/py_faster_rcnn/README.md
--rw-r--r--   0        0        0      249 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/third_party/py_faster_rcnn/__init__.py
--rw-r--r--   0        0        0     1649 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/third_party/py_faster_rcnn/voc_ap.py
--rw-r--r--   0        0        0      446 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/utils/__init__.py
--rw-r--r--   0        0        0     4683 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/utils/annotation_utils.py
--rw-r--r--   0        0        0     2311 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/utils/common_utils.py
--rw-r--r--   0        0        0    11794 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/utils/draw_utils.py
--rw-r--r--   0        0        0     5950 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/utils/file_utils.py
--rw-r--r--   0        0        0     5810 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/utils/gpu_util.py
--rw-r--r--   0        0        0     2967 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/utils/implicit_path_replacements.py
--rw-r--r--   0        0        0     2393 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/utils/versioning_utils.py
--rw-r--r--   0        0        0     3769 2023-03-20 17:23:38.516115 mlcvzoo_base-5.3.2/mlcvzoo_base/utils/xml_utils.py
--rw-r--r--   0        0        0     3943 2023-03-21 13:44:47.046399 mlcvzoo_base-5.3.2/pyproject.toml
--rw-r--r--   0        0        0     2249 1970-01-01 00:00:00.000000 mlcvzoo_base-5.3.2/setup.py
--rw-r--r--   0        0        0     2164 1970-01-01 00:00:00.000000 mlcvzoo_base-5.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11412 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/LICENSE
+-rw-r--r--   0        0        0      546 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/README.md
+-rw-r--r--   0        0        0      244 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/__init__.py
+-rw-r--r--   0        0        0      196 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/__init__.py
+-rw-r--r--   0        0        0     1021 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/configuration.py
+-rw-r--r--   0        0        0      196 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/__init__.py
+-rw-r--r--   0        0        0    11270 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation.py
+-rw-r--r--   0        0        0      816 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation_attributes.py
+-rw-r--r--   0        0        0     2429 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation_builder.py
+-rw-r--r--   0        0        0    26777 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation_class_mapper.py
+-rw-r--r--   0        0        0     1130 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation_parser.py
+-rw-r--r--   0        0        0      975 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation_writer.py
+-rw-r--r--   0        0        0     6146 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/bounding_box.py
+-rw-r--r--   0        0        0    13021 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/box.py
+-rw-r--r--   0        0        0     2734 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/class_identifier.py
+-rw-r--r--   0        0        0     5253 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/classification.py
+-rw-r--r--   0        0        0     3941 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/dataset_info.py
+-rw-r--r--   0        0        0     3268 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/ocr_perception.py
+-rw-r--r--   0        0        0    11655 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/segmentation.py
+-rw-r--r--   0        0        0      362 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/types.py
+-rw-r--r--   0        0        0      906 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/exceptions.py
+-rw-r--r--   0        0        0     5029 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/interfaces.py
+-rw-r--r--   0        0        0    12243 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/model.py
+-rw-r--r--   0        0        0     2333 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/api/registry.py
+-rw-r--r--   0        0        0      196 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/__init__.py
+-rw-r--r--   0        0        0     8184 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/annotation_handler_config.py
+-rw-r--r--   0        0        0     3942 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/class_mapping_config.py
+-rw-r--r--   0        0        0      656 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/config_registry.py
+-rw-r--r--   0        0        0      772 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/device_query.py
+-rw-r--r--   0        0        0     1692 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/mlfow_config.py
+-rw-r--r--   0        0        0     3093 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/model_config.py
+-rw-r--r--   0        0        0     2589 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/reduction_mapping_config.py
+-rw-r--r--   0        0        0     3889 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/replacement_config.py
+-rw-r--r--   0        0        0     3939 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/structs.py
+-rw-r--r--   0        0        0     7286 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/utils.py
+-rw-r--r--   0        0        0      628 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/visualization_config.py
+-rw-r--r--   0        0        0      196 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/__init__.py
+-rw-r--r--   0        0        0      256 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/__init__.py
+-rw-r--r--   0        0        0     8663 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/coco_annotation_builder.py
+-rw-r--r--   0        0        0     7121 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/csv_annotation_builder.py
+-rw-r--r--   0        0        0     2458 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/cvat_annotation_builder.py
+-rw-r--r--   0        0        0     8862 2023-05-22 13:12:23.124028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/mot_annotation_builder.py
+-rw-r--r--   0        0        0     6066 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/pascal_voc_annotation_builder.py
+-rw-r--r--   0        0        0    14648 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_handler.py
+-rw-r--r--   0        0        0      196 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/__init__.py
+-rw-r--r--   0        0        0     3289 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/coco_annotation_parser.py
+-rw-r--r--   0        0        0     8168 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/csv_annotation_parser.py
+-rw-r--r--   0        0        0    11628 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/cvat_annotation_parser.py
+-rw-r--r--   0        0        0     7841 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/label_studio_annotation_parser.py
+-rw-r--r--   0        0        0    10617 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/mot_annotation_parser.py
+-rw-r--r--   0        0        0     9205 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/pascal_voc_annotation_parser.py
+-rw-r--r--   0        0        0      196 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_writer/__init__.py
+-rw-r--r--   0        0        0    14717 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_writer/csv_annotation_writer.py
+-rw-r--r--   0        0        0     8684 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_writer/cvat_annotation_writer.py
+-rw-r--r--   0        0        0     4097 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_writer/darknet_annotation_writer.py
+-rw-r--r--   0        0        0      501 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/structs.py
+-rw-r--r--   0        0        0    11234 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/utils.py
+-rw-r--r--   0        0        0      196 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/__init__.py
+-rw-r--r--   0        0        0      196 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/__init__.py
+-rw-r--r--   0        0        0     2227 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/configuration.py
+-rw-r--r--   0        0        0     6836 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/data_classes.py
+-rw-r--r--   0        0        0    54097 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/metrics_computation.py
+-rw-r--r--   0        0        0    12295 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/metrics_logging.py
+-rw-r--r--   0        0        0     4134 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/model_evaluation.py
+-rw-r--r--   0        0        0      633 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/structs.py
+-rw-r--r--   0        0        0    15646 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/utils.py
+-rw-r--r--   0        0        0      196 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/metrics/__init__.py
+-rw-r--r--   0        0        0      196 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/metrics/mlflow/__init__.py
+-rw-r--r--   0        0        0     7255 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/metrics/mlflow/mlflow_runner.py
+-rw-r--r--   0        0        0     1676 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/metrics/mlflow/utils.py
+-rw-r--r--   0        0        0      196 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/models/__init__.py
+-rw-r--r--   0        0        0      257 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/models/constants.py
+-rw-r--r--   0        0        0    10705 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/models/model_registry.py
+-rw-r--r--   0        0        0      196 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/models/read_from_file/__init__.py
+-rw-r--r--   0        0        0     1540 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/models/read_from_file/configuration.py
+-rw-r--r--   0        0        0    10713 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/models/read_from_file/model.py
+-rw-r--r--   0        0        0        0 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/__init__.py
+-rw-r--r--   0        0        0     1078 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/efficientdet_pytorch/LICENSE
+-rw-r--r--   0        0        0      138 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/efficientdet_pytorch/README.md
+-rw-r--r--   0        0        0      249 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/efficientdet_pytorch/__init__.py
+-rw-r--r--   0        0        0     1774 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/efficientdet_pytorch/computer_overlap.py
+-rw-r--r--   0        0        0     1117 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/imutils/LICENSE.txt
+-rw-r--r--   0        0        0      108 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/imutils/README.md
+-rw-r--r--   0        0        0      296 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/imutils/__init__.py
+-rw-r--r--   0        0        0     2794 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/imutils/perspective.py
+-rw-r--r--   0        0        0     3744 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/py_faster_rcnn/LICENSE
+-rw-r--r--   0        0        0      127 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/py_faster_rcnn/README.md
+-rw-r--r--   0        0        0      249 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/py_faster_rcnn/__init__.py
+-rw-r--r--   0        0        0     1649 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/py_faster_rcnn/voc_ap.py
+-rw-r--r--   0        0        0      488 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/utils/__init__.py
+-rw-r--r--   0        0        0     4725 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/utils/annotation_utils.py
+-rw-r--r--   0        0        0     2353 2023-05-22 13:12:23.128028 mlcvzoo_base-5.3.3/mlcvzoo_base/utils/common_utils.py
+-rw-r--r--   0        0        0    11836 2023-05-22 13:12:23.132028 mlcvzoo_base-5.3.3/mlcvzoo_base/utils/draw_utils.py
+-rw-r--r--   0        0        0     5992 2023-05-22 13:12:23.132028 mlcvzoo_base-5.3.3/mlcvzoo_base/utils/file_utils.py
+-rw-r--r--   0        0        0     5852 2023-05-22 13:12:23.132028 mlcvzoo_base-5.3.3/mlcvzoo_base/utils/gpu_util.py
+-rw-r--r--   0        0        0     3009 2023-05-22 13:12:23.132028 mlcvzoo_base-5.3.3/mlcvzoo_base/utils/implicit_path_replacements.py
+-rw-r--r--   0        0        0     2435 2023-05-22 13:12:23.132028 mlcvzoo_base-5.3.3/mlcvzoo_base/utils/versioning_utils.py
+-rw-r--r--   0        0        0     3811 2023-05-22 13:12:23.132028 mlcvzoo_base-5.3.3/mlcvzoo_base/utils/xml_utils.py
+-rw-r--r--   0        0        0     4007 2023-05-22 13:12:23.132028 mlcvzoo_base-5.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2254 1970-01-01 00:00:00.000000 mlcvzoo_base-5.3.3/setup.py
+-rw-r--r--   0        0        0     2183 1970-01-01 00:00:00.000000 mlcvzoo_base-5.3.3/PKG-INFO
```

### Comparing `mlcvzoo_base-5.3.2/README.md` & `mlcvzoo_base-5.3.3/README.md`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/annotation.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """ Base class for image annotations """
 
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass, field
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/annotation_attributes.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation_attributes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Dataclass that holds attributes of Annotation objects"""
 
 
 class AnnotationAttributes:
     """Class for describing different annotation attributes"""
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/annotation_builder.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for building BaseAnnotation objects"""
 
 from abc import ABC, abstractmethod
 from typing import List
 
 from mlcvzoo_base.api.data.annotation import BaseAnnotation
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/annotation_class_mapper.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation_class_mapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module that holds the class for storing and accessing annotation class mapping information."""
 
 from __future__ import annotations
 
 import logging
 from typing import Any, Dict, List, Optional
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/annotation_parser.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for parsing annotations"""
 from abc import ABC, abstractmethod
 from typing import List
 
 from mlcvzoo_base.api.data.annotation import BaseAnnotation
 from mlcvzoo_base.api.data.annotation_class_mapper import AnnotationClassMapper
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/annotation_writer.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/annotation_writer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for writing annotations to a file"""
 from abc import abstractmethod
 from typing import List, Optional
 
 from mlcvzoo_base.api.data.annotation import BaseAnnotation
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/bounding_box.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/bounding_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """ Class for Bounding Box Annotation"""
 
 from __future__ import annotations
 
 import math
 from typing import Any, Dict, List, Optional
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/box.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/box.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """ Class for Bounding Box information"""
 
 from __future__ import annotations
 
 import logging
 from typing import Any, Dict, List, Optional, Tuple
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/class_identifier.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/class_identifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Data class for storing information that is needed to classify an object instance"""
 
 from __future__ import annotations
 
 from typing import Any, Dict
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/classification.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/classification.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Data class that holds attributes of Classification objects"""
 
 from __future__ import annotations
 
 import math
 from typing import Any, Dict, Optional
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/dataset_info.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/dataset_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module that holds classes for different types of basic dataset information."""
 import os
 from dataclasses import dataclass, field
 from typing import Dict
 
 from dataclasses_json import dataclass_json
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/ocr_perception.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/ocr_perception.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 # TODO: Consider naming this "TextPerception" instead
 """Module for handling attributes of OCR objects"""
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Any, Dict, List
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/api/data/segmentation.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/api/data/segmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """ Class for Segmentation (polygon areas) annotations"""
 from __future__ import annotations
 
 import math
 from typing import Any, Dict, List, Optional, Tuple, Type
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/api/exceptions.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/api/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for custom exceptions"""
 
 
 class ForbiddenClassError(Exception):
     """
     Error which indicates that an invalid class-name has been tried to be mapped
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/api/interfaces.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/api/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Definition of interfaces / abstract classes that define additional features of mlcvzoo models.
 """
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/api/model.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/api/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for creating machine learning models in the MLCVZoo"""
 
 from abc import ABC, abstractmethod
 from typing import Dict, Generic, List, Optional, Tuple, TypeVar
 
 from mlcvzoo_base.api.configuration import ModelConfiguration
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/api/registry.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/api/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2022 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for defining a component that enables to create registries for generic class types
 """
 
 import importlib
 import logging
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/annotation_handler_config.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/annotation_handler_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for parsing information from yaml in python accessible attributes for the
 AnnotationHandler class.
 """
 import logging
 import os
-from dataclasses import field
-from typing import Dict, List, Optional
+from typing import List, Optional
 
 import related
 from attr import define
 from config_builder import BaseConfigClass
 
 from mlcvzoo_base.configuration.class_mapping_config import ClassMappingConfig
 from mlcvzoo_base.configuration.reduction_mapping_config import ReductionMappingConfig
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/class_mapping_config.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/class_mapping_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for parsing information from yaml in python accessible attributes for different
 annotation handling classes like AnnotationClassMapper and several configuration classes
 where a class mapping is used.
 """
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/device_query.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/device_query.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2022 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 from typing import Optional
 
 import related
 from attr import define
 from config_builder import BaseConfigClass
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/mlfow_config.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/mlfow_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for parsing information from yaml in python accessible attributes for using mlflow.
 """
-from typing import Dict, List, Optional
+from typing import List, Optional
 
 import related
 from attr import define
 from config_builder import BaseConfigClass
 
 
 @define
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/model_config.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/model_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for parsing information from yaml in python accessible attributes for different
 configuration classes and also for the ModelRegistry class.
 """
 
 from inspect import getfullargspec
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/reduction_mapping_config.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/reduction_mapping_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module that defines the ReductionMappingConfig that is used in the
 mlcvzoo_base.data_preparation.annotation_class_mapper.AnnotationClassMapper.
 """
 
 import logging
-from typing import Dict, List, Optional
+from typing import List, Optional
 
 import related
 from attr import define
 from config_builder import BaseConfigClass
 
 logger = logging.getLogger(__name__)
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/replacement_config.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/replacement_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for parsing information from yaml in python accessible attributes about the program
 environment for different configuration classes.
 """
 import related
 from attr import define
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/structs.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/structs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for enumerating options of annotation and file formats, as well as data subsets and
 respective phases. Furthermore mlflow configuration options can be found here.
 """
 from enum import Enum
 from typing import Any, List
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/utils.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for different utility operations regarding configuration operations."""
 import logging
 import os
 from argparse import ArgumentTypeError
 from typing import Dict, Optional, Tuple, Type, Union, cast
 
 import yaml
-from attrs import asdict
 from config_builder import BaseConfigClass, ConfigBuilder
 from config_builder.yaml_constructors import (
     join_object,
     join_object_from_config_dir,
     join_path,
     join_string,
     join_string_with_delimiter,
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/configuration/visualization_config.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/configuration/visualization_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for configuring the visualization of model outputs
 """
 
 import related
 from attr import define
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_builder/coco_annotation_builder.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/coco_annotation_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for building COCO formatted annotations."""
 
 import logging
 from typing import Any, Dict, List, Tuple, cast
 
 import numpy as np
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_builder/csv_annotation_builder.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/csv_annotation_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for building CSV formatted annotations."""
 import logging
 import os
 from typing import List, Tuple
 
 from mlcvzoo_base.api.data.annotation import BaseAnnotation
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_builder/cvat_annotation_builder.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/cvat_annotation_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for building CVAT formatted annotations."""
 import logging
 import os
 from typing import List, Tuple
 
 from mlcvzoo_base.api.data.annotation import BaseAnnotation
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_builder/mot_annotation_builder.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/mot_annotation_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for building MOT formatted annotations."""
 import logging
 from typing import Dict, List, Tuple
 
 from mlcvzoo_base.api.data.annotation import BaseAnnotation
 from mlcvzoo_base.api.data.annotation_builder import AnnotationBuilder
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_builder/pascal_voc_annotation_builder.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_builder/pascal_voc_annotation_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for building Pascal VOC formatted annotations."""
 import logging
 import os
 import xml.etree.ElementTree as ET_xml
 from typing import List, Tuple
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_handler.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """ Module for handling annotations according to configuration"""
 
 import logging
 import xml.etree.ElementTree as ET_xml
 from typing import Any, Dict, List, Optional, Tuple, cast
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_parser/coco_annotation_parser.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/coco_annotation_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for parsing COCO formatted annotations"""
 import json
 import logging
 import os
 from typing import List
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_parser/csv_annotation_parser.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/csv_annotation_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for parsing CSV formatted annotations"""
 import logging
 import os
 from dataclasses import field
 from typing import List, Optional, Tuple
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_parser/cvat_annotation_parser.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/cvat_annotation_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for parsing CVAT formatted annotations"""
 import logging
 import xml.etree.ElementTree as ET_xml
 from typing import List, Tuple
 
 from mlcvzoo_base.api.data.annotation import BaseAnnotation
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_parser/label_studio_annotation_parser.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/label_studio_annotation_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2022 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for parsing Label Studio formatted annotations"""
 
 import json
 import logging
 import os
 from pathlib import Path
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_parser/mot_annotation_parser.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/mot_annotation_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for parsing MOT formatted annotations"""
 
 import logging
 import os
 from typing import Dict, List
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_parser/pascal_voc_annotation_parser.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_parser/pascal_voc_annotation_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for parsing PascalVOC formatted annotations"""
 import logging
 import os
 from typing import List, Tuple
 from xml.etree.ElementTree import ParseError
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_writer/csv_annotation_writer.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_writer/csv_annotation_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for writing CSV formatted annotations."""
 import logging
 import os
 from typing import List, Optional, Tuple
 
 from mlcvzoo_base.api.data.annotation import BaseAnnotation
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_writer/cvat_annotation_writer.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_writer/cvat_annotation_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for writing CVAT formatted annotations."""
 import logging
 import xml.etree.ElementTree as ET_xml
 from typing import List, Optional
 
 from mlcvzoo_base.api.data.annotation import BaseAnnotation
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/annotation_writer/darknet_annotation_writer.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/annotation_writer/darknet_annotation_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for writing Darknet formatted annotations."""
 import logging
 import os
 import random
 from pathlib import Path
 from shutil import copyfile, rmtree
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/data_preparation/utils.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/data_preparation/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for different utility operations during data preparation
 """
 
 import logging
 import os
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/evaluation/object_detection/configuration.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 import logging
-from typing import Dict, List, Optional
+from typing import List, Optional
 
 import related
 from attr import define
 from config_builder import BaseConfigClass
 
 from mlcvzoo_base.configuration.annotation_handler_config import AnnotationHandlerConfig
 from mlcvzoo_base.configuration.mlfow_config import MLFlowConfig
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/evaluation/object_detection/data_classes.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/data_classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for storing data classes and complex type definitions that are used in the context of the
 mlcvzoo_base.evaluation.object_detection package
 """
 from __future__ import annotations
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/evaluation/object_detection/metrics_computation.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/metrics_computation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 import copy
 import logging
 from typing import Dict, List, Optional, Tuple
 
 import numpy as np
 from tqdm import tqdm
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/evaluation/object_detection/metrics_logging.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/metrics_logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Gathering of utility methods that are generating metric output in any
 kind of form.
 """
 
 import logging
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/evaluation/object_detection/model_evaluation.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/model_evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2022 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for evaluating currently trained model checkpoints"""
 
 import logging
 from typing import Dict, List, Optional
 
 from tqdm import tqdm
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/evaluation/object_detection/structs.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/structs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 from mlcvzoo_base.configuration.structs import BaseType
 
 
 class BBoxSizeTypes(BaseType):
     BBOX_ALL: str = "ALL"
     BBOX_SMALL: str = "S"
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/evaluation/object_detection/utils.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/evaluation/object_detection/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for different utility operations during object detection evaluation"""
 
 import logging
 import math
 import os
 from pathlib import Path
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/metrics/mlflow/mlflow_runner.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/metrics/mlflow/mlflow_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for using MLFlow tool in MLCVZoo"""
 import copy
 import logging
 import re
 import typing
-from typing import Dict, List, Optional
+from typing import Dict, Optional
 
 import mlflow
 from config_builder import ConfigBuilder
 from mlflow import ActiveRun
 from mlflow.entities import Experiment
 
 from mlcvzoo_base.configuration.mlfow_config import MLFlowConfig
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/metrics/mlflow/utils.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/metrics/mlflow/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 import logging
 import os
 
 import mlflow
 from config_builder import BaseConfigClass
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/models/model_registry.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/models/model_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module to provide a registry for model and configuration constructors"""
 
 import copy
 import inspect
 import logging
 from typing import Any, Dict, List, Optional, Type
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/models/read_from_file/configuration.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/models/read_from_file/configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for configuring the parsing of information from yaml in python
 accessible attributes for the ReadFromFileModel class
 """
 from typing import Optional
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/models/read_from_file/model.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/models/read_from_file/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for creating a look-up model based on existing annotations"""
 import hashlib
 import logging
 import os
 import typing
 from abc import ABC
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/third_party/efficientdet_pytorch/LICENSE` & `mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/efficientdet_pytorch/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/third_party/efficientdet_pytorch/computer_overlap.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/efficientdet_pytorch/computer_overlap.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/third_party/imutils/LICENSE.txt` & `mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/imutils/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/third_party/imutils/perspective.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/imutils/perspective.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/third_party/py_faster_rcnn/LICENSE` & `mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/py_faster_rcnn/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/third_party/py_faster_rcnn/voc_ap.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/third_party/py_faster_rcnn/voc_ap.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/utils/annotation_utils.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/utils/annotation_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for different utility operations regarding annotations in lists"""
 import logging
 import random
 from typing import List, Optional, Tuple
 
 from mlcvzoo_base.api.data.annotation import BaseAnnotation
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/utils/common_utils.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/utils/common_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for different utility operations regarding time and json operations"""
 import inspect
 import json
 from datetime import datetime, timedelta
 from typing import Any
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/utils/draw_utils.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/utils/draw_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for different utility operations regarding drawing on images"""
 
 import colorsys
 import copy
 from typing import List, Optional, Tuple, Union
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/utils/file_utils.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/utils/file_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for different utility operations regarding files and file access"""
 import logging
 import os
 import shutil
 import zipfile
 from pathlib import Path
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/utils/gpu_util.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/utils/gpu_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 import os
 from dataclasses import dataclass
 from subprocess import PIPE, Popen
 from typing import Any, Callable, Dict, List, Optional
 
 from mlcvzoo_base.configuration.device_query import ModelTimerDeviceQueryConfig
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/utils/implicit_path_replacements.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/utils/implicit_path_replacements.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for handling implicit replacements"""
 
 __author__ = "Oliver Bredtmann"
 __license__ = "Open Logistics License 1.0"
 __email__ = "Oliver.Bredtmann@dbschenker.com"
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/utils/versioning_utils.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/utils/versioning_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for defining methods that handle everything that
 is related to versioning and dependencies of software.
 """
 import logging
 from typing import Dict, List, Tuple
```

### Comparing `mlcvzoo_base-5.3.2/mlcvzoo_base/utils/xml_utils.py` & `mlcvzoo_base-5.3.3/mlcvzoo_base/utils/xml_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for different utility operations regarding xml documents and objects"""
 import logging
 import os
 import xml.etree.ElementTree as ET_xml
 
 from mlcvzoo_base.utils import ensure_dir
```

### Comparing `mlcvzoo_base-5.3.2/pyproject.toml` & `mlcvzoo_base-5.3.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "mlcvzoo_base"
-version = "5.3.2"
-license = "Open Logistics License Version 1.0"
 description = "MLCVZoo Base Package"
+version = "5.3.3"
+license = "Open Logistics Foundation License v1.3"
 readme = "README.md"
-homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
-repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
-documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc"
+homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base"
+repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base"
+documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base/-/blob/main/documentation/index.adoc"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Natural Language :: English",
 ]
 authors = [
     "Maximilian Otten <maximilian.otten@iml.fraunhofer.de>",
@@ -56,15 +56,16 @@
 [tool.poetry.dev-dependencies]
 mock = { version = ">=4.0" }
 pytest = { version = ">=7.0" }
 pytest-cov = { version = ">=3.0.0" }
 black = { version = ">=22" }
 mypy = { version = ">=0.961" }
 pylint = { version = ">=2.9.6" }
-isort = { version = ">=5.9" }
+# Isort guarantees formatting results for 5.X
+isort = { version = "^5.0" }
 pytest-mock = { version = ">=3.7" }
 
 [build-system]
 # NOTE: Don't remove setuptools, therefore require it from the build system
 requires = ["setuptools", "poetry_core>=1.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mlcvzoo_base-5.3.2/setup.py` & `mlcvzoo_base-5.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,22 +40,22 @@
  'tensorboardX>=2.5',
  'terminaltables>=3.1',
  'tqdm>=4.61',
  'yaml-config-builder>=8,<9']
 
 setup_kwargs = {
     'name': 'mlcvzoo-base',
-    'version': '5.3.2',
+    'version': '5.3.3',
     'description': 'MLCVZoo Base Package',
     'long_description': '# MLCVZoo Base\n\nThe MLCVZoo is an SDK for simplifying the usage of various (machine learning driven)\ncomputer vision algorithms. The package **mlcvzoo_base** provides the base modules\nthat are defining the MLCVZoo API. Furthermore, it includes modules that allow to handle\nand process the data structures of the MLCVZoo, as well as providing modules for\nrunning evaluations / calculation of metrics.\n\nFurther information about the MLCVZoo can be found [here](../README.md).\n\n## Install\n`\npip install mlcvzoo-base\n`\n\n## Technology stack\n\n- Python\n',
     'author': 'Maximilian Otten',
     'author_email': 'maximilian.otten@iml.fraunhofer.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo',
+    'url': 'https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `mlcvzoo_base-5.3.2/PKG-INFO` & `mlcvzoo_base-5.3.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mlcvzoo-base
-Version: 5.3.2
+Version: 5.3.3
 Summary: MLCVZoo Base Package
-Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
-License: Open Logistics License Version 1.0
+Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base
+License: Open Logistics Foundation License v1.3
 Author: Maximilian Otten
 Author-email: maximilian.otten@iml.fraunhofer.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
@@ -27,16 +27,16 @@
 Requires-Dist: opencv-python (>=4.5,!=4.5.5.64)
 Requires-Dist: pillow (>=8.2)
 Requires-Dist: related-mltoolbox (>=1.0,<2.0)
 Requires-Dist: tensorboardX (>=2.5)
 Requires-Dist: terminaltables (>=3.1)
 Requires-Dist: tqdm (>=4.61)
 Requires-Dist: yaml-config-builder (>=8,<9)
-Project-URL: Documentation, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc
-Project-URL: Repository, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
+Project-URL: Documentation, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base/-/blob/main/documentation/index.adoc
+Project-URL: Repository, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-base
 Description-Content-Type: text/markdown
 
 # MLCVZoo Base
 
 The MLCVZoo is an SDK for simplifying the usage of various (machine learning driven)
 computer vision algorithms. The package **mlcvzoo_base** provides the base modules
 that are defining the MLCVZoo API. Furthermore, it includes modules that allow to handle
```

