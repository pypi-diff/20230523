# Comparing `tmp/zod-0.2.5.tar.gz` & `tmp/zod-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zod-0.2.5.tar", max compression
+gzip compressed data, was "zod-0.2.6.tar", max compression
```

## Comparing `zod-0.2.5.tar` & `zod-0.2.6.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1073 2023-05-23 09:03:14.560827 zod-0.2.5/LICENSE
--rw-r--r--   0        0        0     4809 2023-05-23 09:03:14.560827 zod-0.2.5/README.md
--rw-r--r--   0        0        0     1783 2023-05-23 09:03:14.560827 zod-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      982 2023-05-23 09:03:14.560827 zod-0.2.5/zod/__init__.py
--rw-r--r--   0        0        0     4083 2023-05-23 09:03:14.560827 zod-0.2.5/zod/_zod_dataset.py
--rw-r--r--   0        0        0     4945 2023-05-23 09:03:14.560827 zod-0.2.5/zod/anno/lane.py
--rw-r--r--   0        0        0     4354 2023-05-23 09:03:14.564827 zod-0.2.5/zod/anno/object.py
--rw-r--r--   0        0        0     2850 2023-05-23 09:03:14.564827 zod-0.2.5/zod/anno/parser.py
--rw-r--r--   0        0        0      349 2023-05-23 09:03:14.564827 zod-0.2.5/zod/anno/road_condition.py
--rw-r--r--   0        0        0    20456 2023-05-23 09:03:14.564827 zod-0.2.5/zod/anno/tsr/class_map.py
--rw-r--r--   0        0        0     1686 2023-05-23 09:03:14.564827 zod-0.2.5/zod/anno/tsr/traffic_sign.py
--rw-r--r--   0        0        0    14282 2023-05-23 09:03:14.564827 zod-0.2.5/zod/cli/download_zod.py
--rw-r--r--   0        0        0     7431 2023-05-23 09:03:14.564827 zod-0.2.5/zod/cli/extract_tsr_patches.py
--rw-r--r--   0        0        0     6049 2023-05-23 09:03:14.564827 zod-0.2.5/zod/cli/generate_coco_json.py
--rw-r--r--   0        0        0     1324 2023-05-23 09:03:14.564827 zod-0.2.5/zod/cli/main.py
--rw-r--r--   0        0        0      655 2023-05-23 09:03:14.564827 zod-0.2.5/zod/cli/utils.py
--rw-r--r--   0        0        0     3682 2023-05-23 09:03:14.564827 zod-0.2.5/zod/cli/visualize_lidar.py
--rw-r--r--   0        0        0     2403 2023-05-23 09:03:14.564827 zod-0.2.5/zod/constants.py
--rw-r--r--   0        0        0      184 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/__init__.py
--rw-r--r--   0        0        0      400 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/_serializable.py
--rw-r--r--   0        0        0    10575 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/box.py
--rw-r--r--   0        0        0     3021 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/calibration.py
--rw-r--r--   0        0        0     7226 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/ego_motion.py
--rw-r--r--   0        0        0     5044 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/frame.py
--rw-r--r--   0        0        0     1271 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/geometry.py
--rw-r--r--   0        0        0     4911 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/info.py
--rw-r--r--   0        0        0      894 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/metadata.py
--rw-r--r--   0        0        0      317 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/oxts.py
--rw-r--r--   0        0        0     5268 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/sensor.py
--rw-r--r--   0        0        0     4441 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/sequence.py
--rw-r--r--   0        0        0     1004 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/vehicle_data.py
--rw-r--r--   0        0        0       65 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/README.md
--rw-r--r--   0        0        0      299 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/__init__.py
--rw-r--r--   0        0        0     4427 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_experimental/eval.py
--rw-r--r--   0        0        0    12061 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_experimental/matching.py
--rw-r--r--   0        0        0     4614 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_experimental/utils.py
--rw-r--r--   0        0        0      548 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_nuscenes_eval/LICENCE.txt
--rw-r--r--   0        0        0      661 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_nuscenes_eval/changes.txt
--rw-r--r--   0        0        0     4576 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_nuscenes_eval/common/data_classes.py
--rw-r--r--   0        0        0     4046 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_nuscenes_eval/common/utils.py
--rw-r--r--   0        0        0    21852 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_nuscenes_eval/detection/README.md
--rw-r--r--   0        0        0     7651 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_nuscenes_eval/detection/algo.py
--rw-r--r--   0        0        0     1016 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_nuscenes_eval/detection/constants.py
--rw-r--r--   0        0        0    15069 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_nuscenes_eval/detection/data_classes.py
--rw-r--r--   0        0        0      123 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/constants.py
--rw-r--r--   0        0        0     8031 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/eval_nuscenes_style.py
--rw-r--r--   0        0        0       67 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/tsr.py
--rw-r--r--   0        0        0     1996 2023-05-23 09:03:14.564827 zod-0.2.5/zod/utils/compensation.py
--rw-r--r--   0        0        0     4443 2023-05-23 09:03:14.564827 zod-0.2.5/zod/utils/geometry.py
--rw-r--r--   0        0        0     1044 2023-05-23 09:03:14.564827 zod-0.2.5/zod/utils/polygon_transformations.py
--rw-r--r--   0        0        0      914 2023-05-23 09:03:14.564827 zod-0.2.5/zod/utils/utils.py
--rw-r--r--   0        0        0     2703 2023-05-23 09:03:14.564827 zod-0.2.5/zod/utils/visualization.py
--rw-r--r--   0        0        0     5481 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/bev_utils.py
--rw-r--r--   0        0        0     2941 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/colorlabeler.py
--rw-r--r--   0        0        0      259 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/ego_road_visualization.py
--rw-r--r--   0        0        0      264 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/lane_markings_visualization.py
--rw-r--r--   0        0        0     8041 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/lidar_3d.py
--rw-r--r--   0        0        0     6028 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/lidar_bev.py
--rw-r--r--   0        0        0     4410 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/lidar_on_image.py
--rw-r--r--   0        0        0     4639 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/object_visualization.py
--rw-r--r--   0        0        0     1769 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/oxts_on_image.py
--rw-r--r--   0        0        0     3259 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/oxts_visualization.py
--rw-r--r--   0        0        0      762 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/polygon_utils.py
--rw-r--r--   0        0        0      685 2023-05-23 09:03:14.564827 zod-0.2.5/zod/zod_drives.py
--rw-r--r--   0        0        0      577 2023-05-23 09:03:14.564827 zod-0.2.5/zod/zod_frames.py
--rw-r--r--   0        0        0      576 2023-05-23 09:03:14.564827 zod-0.2.5/zod/zod_sequences.py
--rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 zod-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-23 09:30:48.888967 zod-0.2.6/LICENSE
+-rw-r--r--   0        0        0     4809 2023-05-23 09:30:48.888967 zod-0.2.6/README.md
+-rw-r--r--   0        0        0     1783 2023-05-23 09:30:48.888967 zod-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      982 2023-05-23 09:30:48.888967 zod-0.2.6/zod/__init__.py
+-rw-r--r--   0        0        0     4083 2023-05-23 09:30:48.888967 zod-0.2.6/zod/_zod_dataset.py
+-rw-r--r--   0        0        0     4945 2023-05-23 09:30:48.888967 zod-0.2.6/zod/anno/lane.py
+-rw-r--r--   0        0        0     4354 2023-05-23 09:30:48.888967 zod-0.2.6/zod/anno/object.py
+-rw-r--r--   0        0        0     2850 2023-05-23 09:30:48.892967 zod-0.2.6/zod/anno/parser.py
+-rw-r--r--   0        0        0      349 2023-05-23 09:30:48.892967 zod-0.2.6/zod/anno/road_condition.py
+-rw-r--r--   0        0        0    20456 2023-05-23 09:30:48.892967 zod-0.2.6/zod/anno/tsr/class_map.py
+-rw-r--r--   0        0        0     1686 2023-05-23 09:30:48.892967 zod-0.2.6/zod/anno/tsr/traffic_sign.py
+-rw-r--r--   0        0        0    14547 2023-05-23 09:30:48.892967 zod-0.2.6/zod/cli/download_zod.py
+-rw-r--r--   0        0        0     7431 2023-05-23 09:30:48.892967 zod-0.2.6/zod/cli/extract_tsr_patches.py
+-rw-r--r--   0        0        0     6049 2023-05-23 09:30:48.892967 zod-0.2.6/zod/cli/generate_coco_json.py
+-rw-r--r--   0        0        0     1324 2023-05-23 09:30:48.892967 zod-0.2.6/zod/cli/main.py
+-rw-r--r--   0        0        0      655 2023-05-23 09:30:48.892967 zod-0.2.6/zod/cli/utils.py
+-rw-r--r--   0        0        0     3682 2023-05-23 09:30:48.892967 zod-0.2.6/zod/cli/visualize_lidar.py
+-rw-r--r--   0        0        0     2403 2023-05-23 09:30:48.892967 zod-0.2.6/zod/constants.py
+-rw-r--r--   0        0        0      184 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/__init__.py
+-rw-r--r--   0        0        0      400 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/_serializable.py
+-rw-r--r--   0        0        0    10575 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/box.py
+-rw-r--r--   0        0        0     3021 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/calibration.py
+-rw-r--r--   0        0        0     7226 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/ego_motion.py
+-rw-r--r--   0        0        0     5044 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/frame.py
+-rw-r--r--   0        0        0     1271 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/geometry.py
+-rw-r--r--   0        0        0     4911 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/info.py
+-rw-r--r--   0        0        0      894 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/metadata.py
+-rw-r--r--   0        0        0      317 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/oxts.py
+-rw-r--r--   0        0        0     5268 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/sensor.py
+-rw-r--r--   0        0        0     4441 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/sequence.py
+-rw-r--r--   0        0        0     1004 2023-05-23 09:30:48.892967 zod-0.2.6/zod/data_classes/vehicle_data.py
+-rw-r--r--   0        0        0       65 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/README.md
+-rw-r--r--   0        0        0      299 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/__init__.py
+-rw-r--r--   0        0        0     4427 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_experimental/eval.py
+-rw-r--r--   0        0        0    12061 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_experimental/matching.py
+-rw-r--r--   0        0        0     4614 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_experimental/utils.py
+-rw-r--r--   0        0        0      548 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_nuscenes_eval/LICENCE.txt
+-rw-r--r--   0        0        0      661 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_nuscenes_eval/changes.txt
+-rw-r--r--   0        0        0     4576 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_nuscenes_eval/common/data_classes.py
+-rw-r--r--   0        0        0     4046 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_nuscenes_eval/common/utils.py
+-rw-r--r--   0        0        0    21852 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_nuscenes_eval/detection/README.md
+-rw-r--r--   0        0        0     7651 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_nuscenes_eval/detection/algo.py
+-rw-r--r--   0        0        0     1016 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_nuscenes_eval/detection/constants.py
+-rw-r--r--   0        0        0    15069 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/_nuscenes_eval/detection/data_classes.py
+-rw-r--r--   0        0        0      123 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/constants.py
+-rw-r--r--   0        0        0     8031 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/detection/eval_nuscenes_style.py
+-rw-r--r--   0        0        0       67 2023-05-23 09:30:48.892967 zod-0.2.6/zod/eval/tsr.py
+-rw-r--r--   0        0        0     1996 2023-05-23 09:30:48.892967 zod-0.2.6/zod/utils/compensation.py
+-rw-r--r--   0        0        0     4443 2023-05-23 09:30:48.892967 zod-0.2.6/zod/utils/geometry.py
+-rw-r--r--   0        0        0     1044 2023-05-23 09:30:48.892967 zod-0.2.6/zod/utils/polygon_transformations.py
+-rw-r--r--   0        0        0      914 2023-05-23 09:30:48.892967 zod-0.2.6/zod/utils/utils.py
+-rw-r--r--   0        0        0     2703 2023-05-23 09:30:48.892967 zod-0.2.6/zod/utils/visualization.py
+-rw-r--r--   0        0        0     5481 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/bev_utils.py
+-rw-r--r--   0        0        0     2941 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/colorlabeler.py
+-rw-r--r--   0        0        0      259 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/ego_road_visualization.py
+-rw-r--r--   0        0        0      264 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/lane_markings_visualization.py
+-rw-r--r--   0        0        0     8041 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/lidar_3d.py
+-rw-r--r--   0        0        0     6028 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/lidar_bev.py
+-rw-r--r--   0        0        0     4410 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/lidar_on_image.py
+-rw-r--r--   0        0        0     4639 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/object_visualization.py
+-rw-r--r--   0        0        0     1769 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/oxts_on_image.py
+-rw-r--r--   0        0        0     3259 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/oxts_visualization.py
+-rw-r--r--   0        0        0      762 2023-05-23 09:30:48.892967 zod-0.2.6/zod/visualization/polygon_utils.py
+-rw-r--r--   0        0        0      685 2023-05-23 09:30:48.892967 zod-0.2.6/zod/zod_drives.py
+-rw-r--r--   0        0        0      577 2023-05-23 09:30:48.892967 zod-0.2.6/zod/zod_frames.py
+-rw-r--r--   0        0        0      576 2023-05-23 09:30:48.892967 zod-0.2.6/zod/zod_sequences.py
+-rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 zod-0.2.6/PKG-INFO
```

### Comparing `zod-0.2.5/LICENSE` & `zod-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/README.md` & `zod-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/pyproject.toml` & `zod-0.2.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zod"
-version = "0.2.5"
+version = "0.2.6"
 description = "Zenseact Open Dataset"
 authors = ["Zenseact <opendataset@zenseact.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://zod.zenseact.com"
 repository = "https://github.com/zenseact/zod"
```

### Comparing `zod-0.2.5/zod/__init__.py` & `zod-0.2.6/zod/__init__.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/_zod_dataset.py` & `zod-0.2.6/zod/_zod_dataset.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/anno/lane.py` & `zod-0.2.6/zod/anno/lane.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/anno/object.py` & `zod-0.2.6/zod/anno/object.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/anno/parser.py` & `zod-0.2.6/zod/anno/parser.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/anno/tsr/class_map.py` & `zod-0.2.6/zod/anno/tsr/class_map.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/anno/tsr/traffic_sign.py` & `zod-0.2.6/zod/anno/tsr/traffic_sign.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/cli/download_zod.py` & `zod-0.2.6/zod/cli/download_zod.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,15 +279,18 @@
 
 def _list_folder(url, dbx, path):
     shared_link = dropbox.files.SharedLink(url=url)
     try:
         res = dbx.files_list_folder(path=f"/{path}", shared_link=shared_link)
     except dropbox.exceptions.ApiError as err:
         raise click.exceptions.ClickException(
-            f"Dropbox raised the following error:\n\t{err}\nThis could be due to a bad url."
+            f"Dropbox raised the following error:\n\t{err}\nThis could be due to:"
+            '\n\ta) bad url. Please try it in a browser and specify with quotes (--url="<url>").'
+            "\n\tb) zod bandwidth limit. Sorry about this, and please try again the next day."
+            "\n\tc) other error (bad internet connection, dropbox outage, etc.)."
         )
 
     entries = res.entries
     while res.has_more:
         res = dbx.files_list_folder_continue(res.cursor)
         entries.extend(res.entries)
     return url, entries
```

### Comparing `zod-0.2.5/zod/cli/extract_tsr_patches.py` & `zod-0.2.6/zod/cli/extract_tsr_patches.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/cli/generate_coco_json.py` & `zod-0.2.6/zod/cli/generate_coco_json.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/cli/main.py` & `zod-0.2.6/zod/cli/main.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/cli/utils.py` & `zod-0.2.6/zod/cli/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/cli/visualize_lidar.py` & `zod-0.2.6/zod/cli/visualize_lidar.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/constants.py` & `zod-0.2.6/zod/constants.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/data_classes/box.py` & `zod-0.2.6/zod/data_classes/box.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/data_classes/calibration.py` & `zod-0.2.6/zod/data_classes/calibration.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/data_classes/ego_motion.py` & `zod-0.2.6/zod/data_classes/ego_motion.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/data_classes/frame.py` & `zod-0.2.6/zod/data_classes/frame.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/data_classes/geometry.py` & `zod-0.2.6/zod/data_classes/geometry.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/data_classes/info.py` & `zod-0.2.6/zod/data_classes/info.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/data_classes/metadata.py` & `zod-0.2.6/zod/data_classes/metadata.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/data_classes/sensor.py` & `zod-0.2.6/zod/data_classes/sensor.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/data_classes/sequence.py` & `zod-0.2.6/zod/data_classes/sequence.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/data_classes/vehicle_data.py` & `zod-0.2.6/zod/data_classes/vehicle_data.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/eval/detection/_experimental/eval.py` & `zod-0.2.6/zod/eval/detection/_experimental/eval.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/eval/detection/_experimental/matching.py` & `zod-0.2.6/zod/eval/detection/_experimental/matching.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/eval/detection/_experimental/utils.py` & `zod-0.2.6/zod/eval/detection/_experimental/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/eval/detection/_nuscenes_eval/LICENCE.txt` & `zod-0.2.6/zod/eval/detection/_nuscenes_eval/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/eval/detection/_nuscenes_eval/changes.txt` & `zod-0.2.6/zod/eval/detection/_nuscenes_eval/changes.txt`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/eval/detection/_nuscenes_eval/common/data_classes.py` & `zod-0.2.6/zod/eval/detection/_nuscenes_eval/common/data_classes.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/eval/detection/_nuscenes_eval/common/utils.py` & `zod-0.2.6/zod/eval/detection/_nuscenes_eval/common/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/eval/detection/_nuscenes_eval/detection/README.md` & `zod-0.2.6/zod/eval/detection/_nuscenes_eval/detection/README.md`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/eval/detection/_nuscenes_eval/detection/algo.py` & `zod-0.2.6/zod/eval/detection/_nuscenes_eval/detection/algo.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/eval/detection/_nuscenes_eval/detection/constants.py` & `zod-0.2.6/zod/eval/detection/_nuscenes_eval/detection/constants.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/eval/detection/_nuscenes_eval/detection/data_classes.py` & `zod-0.2.6/zod/eval/detection/_nuscenes_eval/detection/data_classes.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/eval/detection/eval_nuscenes_style.py` & `zod-0.2.6/zod/eval/detection/eval_nuscenes_style.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/utils/compensation.py` & `zod-0.2.6/zod/utils/compensation.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/utils/geometry.py` & `zod-0.2.6/zod/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/utils/polygon_transformations.py` & `zod-0.2.6/zod/utils/polygon_transformations.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/utils/utils.py` & `zod-0.2.6/zod/utils/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/utils/visualization.py` & `zod-0.2.6/zod/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/visualization/bev_utils.py` & `zod-0.2.6/zod/visualization/bev_utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/visualization/colorlabeler.py` & `zod-0.2.6/zod/visualization/colorlabeler.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/visualization/lidar_3d.py` & `zod-0.2.6/zod/visualization/lidar_3d.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/visualization/lidar_bev.py` & `zod-0.2.6/zod/visualization/lidar_bev.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/visualization/lidar_on_image.py` & `zod-0.2.6/zod/visualization/lidar_on_image.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/visualization/object_visualization.py` & `zod-0.2.6/zod/visualization/object_visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/visualization/oxts_on_image.py` & `zod-0.2.6/zod/visualization/oxts_on_image.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/visualization/oxts_visualization.py` & `zod-0.2.6/zod/visualization/oxts_visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/visualization/polygon_utils.py` & `zod-0.2.6/zod/visualization/polygon_utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/zod_drives.py` & `zod-0.2.6/zod/zod_drives.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/zod_frames.py` & `zod-0.2.6/zod/zod_frames.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/zod/zod_sequences.py` & `zod-0.2.6/zod/zod_sequences.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.5/PKG-INFO` & `zod-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zod
-Version: 0.2.5
+Version: 0.2.6
 Summary: Zenseact Open Dataset
 Home-page: https://zod.zenseact.com
 License: MIT
 Author: Zenseact
 Author-email: opendataset@zenseact.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

