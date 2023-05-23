# Comparing `tmp/zod-0.2.4.tar.gz` & `tmp/zod-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zod-0.2.4.tar", max compression
+gzip compressed data, was "zod-0.2.5.tar", max compression
```

## Comparing `zod-0.2.4.tar` & `zod-0.2.5.tar`

### file list

```diff
@@ -1,68 +1,67 @@
--rw-r--r--   0        0        0     1073 2022-12-12 15:34:08.451623 zod-0.2.4/LICENSE
--rw-r--r--   0        0        0     4809 2023-05-11 13:41:27.984739 zod-0.2.4/README.md
--rw-r--r--   0        0        0     1783 2023-05-11 13:41:28.034721 zod-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      982 2023-04-13 11:46:50.226836 zod-0.2.4/zod/__init__.py
--rw-r--r--   0        0        0     4083 2023-04-21 14:37:12.341966 zod-0.2.4/zod/_zod_dataset.py
--rw-r--r--   0        0        0     4945 2023-03-14 14:11:58.653137 zod-0.2.4/zod/anno/lane.py
--rw-r--r--   0        0        0     4354 2023-03-27 08:16:00.340536 zod-0.2.4/zod/anno/object.py
--rw-r--r--   0        0        0     2850 2023-04-20 13:14:41.392219 zod-0.2.4/zod/anno/parser.py
--rw-r--r--   0        0        0      349 2023-03-14 10:29:04.430175 zod-0.2.4/zod/anno/road_condition.py
--rw-r--r--   0        0        0    20456 2023-04-12 11:17:00.636182 zod-0.2.4/zod/anno/tsr/class_map.py
--rw-r--r--   0        0        0     1686 2023-04-12 11:17:00.636357 zod-0.2.4/zod/anno/tsr/traffic_sign.py
--rw-r--r--   0        0        0    14121 2023-04-24 12:30:20.218578 zod-0.2.4/zod/cli/download_zod.py
--rw-r--r--   0        0        0     7431 2023-05-11 13:41:28.035021 zod-0.2.4/zod/cli/extract_tsr_patches.py
--rw-r--r--   0        0        0     6049 2023-03-14 09:59:25.750357 zod-0.2.4/zod/cli/generate_coco_json.py
--rw-r--r--   0        0        0     1324 2023-05-11 13:39:43.695013 zod-0.2.4/zod/cli/main.py
--rw-r--r--   0        0        0      655 2023-04-13 11:46:50.648380 zod-0.2.4/zod/cli/utils.py
--rw-r--r--   0        0        0     3682 2023-03-16 14:47:39.444887 zod-0.2.4/zod/cli/visualize_lidar.py
--rw-r--r--   0        0        0     2403 2023-04-20 13:15:16.698507 zod-0.2.4/zod/constants.py
--rw-r--r--   0        0        0      184 2023-03-27 15:11:15.562233 zod-0.2.4/zod/data_classes/__init__.py
--rw-r--r--   0        0        0      400 2023-01-23 08:46:58.517084 zod-0.2.4/zod/data_classes/_serializable.py
--rw-r--r--   0        0        0    10575 2023-04-13 11:46:50.163290 zod-0.2.4/zod/data_classes/box.py
--rw-r--r--   0        0        0     3021 2023-03-14 14:11:59.064736 zod-0.2.4/zod/data_classes/calibration.py
--rw-r--r--   0        0        0     7226 2023-03-16 14:56:16.137698 zod-0.2.4/zod/data_classes/ego_motion.py
--rw-r--r--   0        0        0     5044 2023-04-20 13:14:41.392777 zod-0.2.4/zod/data_classes/frame.py
--rw-r--r--   0        0        0     1271 2023-03-14 14:11:59.065050 zod-0.2.4/zod/data_classes/geometry.py
--rw-r--r--   0        0        0     4911 2023-04-24 10:58:56.916101 zod-0.2.4/zod/data_classes/info.py
--rw-r--r--   0        0        0      894 2023-01-23 08:46:58.518295 zod-0.2.4/zod/data_classes/metadata.py
--rw-r--r--   0        0        0      317 2023-03-28 15:45:20.205955 zod-0.2.4/zod/data_classes/oxts.py
--rw-r--r--   0        0        0     5268 2023-04-20 13:14:41.393348 zod-0.2.4/zod/data_classes/sensor.py
--rw-r--r--   0        0        0     4441 2023-04-24 08:58:20.139574 zod-0.2.4/zod/data_classes/sequence.py
--rw-r--r--   0        0        0     1004 2023-04-20 13:14:41.393582 zod-0.2.4/zod/data_classes/vehicle_data.py
--rw-r--r--   0        0        0       65 2023-02-08 17:58:06.326973 zod-0.2.4/zod/eval/README.md
--rw-r--r--   0        0        0      299 2023-02-16 13:07:21.333304 zod-0.2.4/zod/eval/detection/__init__.py
--rw-r--r--   0        0        0     4427 2023-03-14 10:01:11.503425 zod-0.2.4/zod/eval/detection/_experimental/eval.py
--rw-r--r--   0        0        0    12061 2023-03-14 10:01:37.539418 zod-0.2.4/zod/eval/detection/_experimental/matching.py
--rw-r--r--   0        0        0     4614 2023-03-14 10:01:46.422883 zod-0.2.4/zod/eval/detection/_experimental/utils.py
--rw-r--r--   0        0        0      548 2023-02-08 17:15:18.717865 zod-0.2.4/zod/eval/detection/_nuscenes_eval/LICENCE.txt
--rw-r--r--   0        0        0      661 2023-02-08 17:15:18.718293 zod-0.2.4/zod/eval/detection/_nuscenes_eval/changes.txt
--rw-r--r--   0        0        0     4576 2023-03-13 16:23:47.678938 zod-0.2.4/zod/eval/detection/_nuscenes_eval/common/data_classes.py
--rw-r--r--   0        0        0     4046 2023-03-13 16:23:47.678986 zod-0.2.4/zod/eval/detection/_nuscenes_eval/common/utils.py
--rw-r--r--   0        0        0    21852 2023-02-08 17:15:18.719837 zod-0.2.4/zod/eval/detection/_nuscenes_eval/detection/README.md
--rw-r--r--   0        0        0     7651 2023-03-13 16:23:47.679037 zod-0.2.4/zod/eval/detection/_nuscenes_eval/detection/algo.py
--rw-r--r--   0        0        0     1016 2023-03-13 16:23:47.679090 zod-0.2.4/zod/eval/detection/_nuscenes_eval/detection/constants.py
--rw-r--r--   0        0        0    15069 2023-03-13 16:23:47.679143 zod-0.2.4/zod/eval/detection/_nuscenes_eval/detection/data_classes.py
--rw-r--r--   0        0        0      123 2023-02-16 12:56:34.415895 zod-0.2.4/zod/eval/detection/constants.py
--rw-r--r--   0        0        0     8031 2023-03-14 10:34:15.457857 zod-0.2.4/zod/eval/detection/eval_nuscenes_style.py
--rw-r--r--   0        0        0       67 2023-02-08 17:57:26.772171 zod-0.2.4/zod/eval/tsr.py
--rw-r--r--   0        0        0     1996 2023-03-28 15:25:47.429197 zod-0.2.4/zod/utils/compensation.py
--rw-r--r--   0        0        0     4443 2023-03-27 08:16:01.603789 zod-0.2.4/zod/utils/geometry.py
--rw-r--r--   0        0        0     1044 2023-04-24 14:18:19.989141 zod-0.2.4/zod/utils/polygon_transformations.py
--rw-r--r--   0        0        0      914 2023-01-19 05:12:36.969853 zod-0.2.4/zod/utils/utils.py
--rw-r--r--   0        0        0     2703 2023-02-09 13:20:16.173558 zod-0.2.4/zod/utils/visualization.py
--rw-r--r--   0        0        0     5481 2023-02-16 10:43:41.878456 zod-0.2.4/zod/visualization/bev_utils.py
--rw-r--r--   0        0        0     2941 2022-12-16 13:30:48.921636 zod-0.2.4/zod/visualization/colorlabeler.py
--rw-r--r--   0        0        0      259 2022-12-12 13:33:36.526169 zod-0.2.4/zod/visualization/ego_road_visualization.py
--rw-r--r--   0        0        0      264 2022-12-12 13:33:36.525601 zod-0.2.4/zod/visualization/lane_markings_visualization.py
--rw-r--r--   0        0        0     8041 2023-05-11 13:41:27.985551 zod-0.2.4/zod/visualization/lidar_3d.py
--rw-r--r--   0        0        0     6028 2023-02-09 13:20:16.173620 zod-0.2.4/zod/visualization/lidar_bev.py
--rw-r--r--   0        0        0     4410 2023-03-27 08:16:02.030051 zod-0.2.4/zod/visualization/lidar_on_image.py
--rw-r--r--   0        0        0     4639 2023-04-13 11:46:50.163979 zod-0.2.4/zod/visualization/object_visualization.py
--rw-r--r--   0        0        0     1769 2023-03-28 15:25:46.191938 zod-0.2.4/zod/visualization/oxts_on_image.py
--rw-r--r--   0        0        0     3259 2023-03-28 15:25:44.860709 zod-0.2.4/zod/visualization/oxts_visualization.py
--rw-r--r--   0        0        0      762 2023-02-09 13:20:16.173776 zod-0.2.4/zod/visualization/polygon_utils.py
--rw-r--r--   0        0        0      685 2023-04-13 11:46:50.227093 zod-0.2.4/zod/zod_drives.py
--rw-r--r--   0        0        0      577 2023-05-02 07:55:05.724595 zod-0.2.4/zod/zod_frames.py
--rw-r--r--   0        0        0      576 2023-04-13 11:46:50.227331 zod-0.2.4/zod/zod_sequences.py
--rw-r--r--   0        0        0     6511 1970-01-01 00:00:00.000000 zod-0.2.4/setup.py
--rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 zod-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-23 09:03:14.560827 zod-0.2.5/LICENSE
+-rw-r--r--   0        0        0     4809 2023-05-23 09:03:14.560827 zod-0.2.5/README.md
+-rw-r--r--   0        0        0     1783 2023-05-23 09:03:14.560827 zod-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      982 2023-05-23 09:03:14.560827 zod-0.2.5/zod/__init__.py
+-rw-r--r--   0        0        0     4083 2023-05-23 09:03:14.560827 zod-0.2.5/zod/_zod_dataset.py
+-rw-r--r--   0        0        0     4945 2023-05-23 09:03:14.560827 zod-0.2.5/zod/anno/lane.py
+-rw-r--r--   0        0        0     4354 2023-05-23 09:03:14.564827 zod-0.2.5/zod/anno/object.py
+-rw-r--r--   0        0        0     2850 2023-05-23 09:03:14.564827 zod-0.2.5/zod/anno/parser.py
+-rw-r--r--   0        0        0      349 2023-05-23 09:03:14.564827 zod-0.2.5/zod/anno/road_condition.py
+-rw-r--r--   0        0        0    20456 2023-05-23 09:03:14.564827 zod-0.2.5/zod/anno/tsr/class_map.py
+-rw-r--r--   0        0        0     1686 2023-05-23 09:03:14.564827 zod-0.2.5/zod/anno/tsr/traffic_sign.py
+-rw-r--r--   0        0        0    14282 2023-05-23 09:03:14.564827 zod-0.2.5/zod/cli/download_zod.py
+-rw-r--r--   0        0        0     7431 2023-05-23 09:03:14.564827 zod-0.2.5/zod/cli/extract_tsr_patches.py
+-rw-r--r--   0        0        0     6049 2023-05-23 09:03:14.564827 zod-0.2.5/zod/cli/generate_coco_json.py
+-rw-r--r--   0        0        0     1324 2023-05-23 09:03:14.564827 zod-0.2.5/zod/cli/main.py
+-rw-r--r--   0        0        0      655 2023-05-23 09:03:14.564827 zod-0.2.5/zod/cli/utils.py
+-rw-r--r--   0        0        0     3682 2023-05-23 09:03:14.564827 zod-0.2.5/zod/cli/visualize_lidar.py
+-rw-r--r--   0        0        0     2403 2023-05-23 09:03:14.564827 zod-0.2.5/zod/constants.py
+-rw-r--r--   0        0        0      184 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/__init__.py
+-rw-r--r--   0        0        0      400 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/_serializable.py
+-rw-r--r--   0        0        0    10575 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/box.py
+-rw-r--r--   0        0        0     3021 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/calibration.py
+-rw-r--r--   0        0        0     7226 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/ego_motion.py
+-rw-r--r--   0        0        0     5044 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/frame.py
+-rw-r--r--   0        0        0     1271 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/geometry.py
+-rw-r--r--   0        0        0     4911 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/info.py
+-rw-r--r--   0        0        0      894 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/metadata.py
+-rw-r--r--   0        0        0      317 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/oxts.py
+-rw-r--r--   0        0        0     5268 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/sensor.py
+-rw-r--r--   0        0        0     4441 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/sequence.py
+-rw-r--r--   0        0        0     1004 2023-05-23 09:03:14.564827 zod-0.2.5/zod/data_classes/vehicle_data.py
+-rw-r--r--   0        0        0       65 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/README.md
+-rw-r--r--   0        0        0      299 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/__init__.py
+-rw-r--r--   0        0        0     4427 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_experimental/eval.py
+-rw-r--r--   0        0        0    12061 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_experimental/matching.py
+-rw-r--r--   0        0        0     4614 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_experimental/utils.py
+-rw-r--r--   0        0        0      548 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_nuscenes_eval/LICENCE.txt
+-rw-r--r--   0        0        0      661 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_nuscenes_eval/changes.txt
+-rw-r--r--   0        0        0     4576 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_nuscenes_eval/common/data_classes.py
+-rw-r--r--   0        0        0     4046 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_nuscenes_eval/common/utils.py
+-rw-r--r--   0        0        0    21852 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_nuscenes_eval/detection/README.md
+-rw-r--r--   0        0        0     7651 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_nuscenes_eval/detection/algo.py
+-rw-r--r--   0        0        0     1016 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_nuscenes_eval/detection/constants.py
+-rw-r--r--   0        0        0    15069 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/_nuscenes_eval/detection/data_classes.py
+-rw-r--r--   0        0        0      123 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/constants.py
+-rw-r--r--   0        0        0     8031 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/detection/eval_nuscenes_style.py
+-rw-r--r--   0        0        0       67 2023-05-23 09:03:14.564827 zod-0.2.5/zod/eval/tsr.py
+-rw-r--r--   0        0        0     1996 2023-05-23 09:03:14.564827 zod-0.2.5/zod/utils/compensation.py
+-rw-r--r--   0        0        0     4443 2023-05-23 09:03:14.564827 zod-0.2.5/zod/utils/geometry.py
+-rw-r--r--   0        0        0     1044 2023-05-23 09:03:14.564827 zod-0.2.5/zod/utils/polygon_transformations.py
+-rw-r--r--   0        0        0      914 2023-05-23 09:03:14.564827 zod-0.2.5/zod/utils/utils.py
+-rw-r--r--   0        0        0     2703 2023-05-23 09:03:14.564827 zod-0.2.5/zod/utils/visualization.py
+-rw-r--r--   0        0        0     5481 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/bev_utils.py
+-rw-r--r--   0        0        0     2941 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/colorlabeler.py
+-rw-r--r--   0        0        0      259 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/ego_road_visualization.py
+-rw-r--r--   0        0        0      264 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/lane_markings_visualization.py
+-rw-r--r--   0        0        0     8041 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/lidar_3d.py
+-rw-r--r--   0        0        0     6028 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/lidar_bev.py
+-rw-r--r--   0        0        0     4410 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/lidar_on_image.py
+-rw-r--r--   0        0        0     4639 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/object_visualization.py
+-rw-r--r--   0        0        0     1769 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/oxts_on_image.py
+-rw-r--r--   0        0        0     3259 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/oxts_visualization.py
+-rw-r--r--   0        0        0      762 2023-05-23 09:03:14.564827 zod-0.2.5/zod/visualization/polygon_utils.py
+-rw-r--r--   0        0        0      685 2023-05-23 09:03:14.564827 zod-0.2.5/zod/zod_drives.py
+-rw-r--r--   0        0        0      577 2023-05-23 09:03:14.564827 zod-0.2.5/zod/zod_frames.py
+-rw-r--r--   0        0        0      576 2023-05-23 09:03:14.564827 zod-0.2.5/zod/zod_sequences.py
+-rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 zod-0.2.5/PKG-INFO
```

### Comparing `zod-0.2.4/LICENSE` & `zod-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/README.md` & `zod-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/pyproject.toml` & `zod-0.2.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zod"
-version = "0.2.4"
+version = "0.2.5"
 description = "Zenseact Open Dataset"
 authors = ["Zenseact <opendataset@zenseact.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://zod.zenseact.com"
 repository = "https://github.com/zenseact/zod"
```

### Comparing `zod-0.2.4/zod/__init__.py` & `zod-0.2.5/zod/__init__.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/_zod_dataset.py` & `zod-0.2.5/zod/_zod_dataset.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/anno/lane.py` & `zod-0.2.5/zod/anno/lane.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/anno/object.py` & `zod-0.2.5/zod/anno/object.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/anno/parser.py` & `zod-0.2.5/zod/anno/parser.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/anno/tsr/class_map.py` & `zod-0.2.5/zod/anno/tsr/class_map.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/anno/tsr/traffic_sign.py` & `zod-0.2.5/zod/anno/tsr/traffic_sign.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/cli/download_zod.py` & `zod-0.2.5/zod/cli/download_zod.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,19 +230,21 @@
     if not settings.infos and "infos" in entry.name:
         return False
     if not settings.vehicle_data and "vehicle_data" in entry.name:
         return False
     if "lidar" in entry.name:
         if not settings.lidar:
             return False
-        distance = entry.name.split("_")[2][:2]
-        if "after" in entry.name and (int(distance) > settings.num_scans_after):
-            return False
-        if "before" in entry.name and (int(distance) > settings.num_scans_before):
-            return False
+        if "after" in entry.name or "before" in entry.name:
+            # this is only the case for frames, where we have surrounding frames
+            distance = entry.name.split("_")[2][:2]
+            if "after" in entry.name and (int(distance) > settings.num_scans_after):
+                return False
+            if "before" in entry.name and (int(distance) > settings.num_scans_before):
+                return False
     return True
 
 
 def _download_dataset(dl_settings: DownloadSettings, filter_settings: FilterSettings, dirname: str):
     dbx = ResumableDropbox(app_key=APP_KEY, oauth2_refresh_token=REFRESH_TOKEN, timeout=TIMEOUT)
     url, entries = _list_folder(dl_settings.url, dbx, dirname)
     dl_dir = osp.join(dl_settings.output_dir, "downloads", dirname)
```

### Comparing `zod-0.2.4/zod/cli/extract_tsr_patches.py` & `zod-0.2.5/zod/cli/extract_tsr_patches.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/cli/generate_coco_json.py` & `zod-0.2.5/zod/cli/generate_coco_json.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/cli/main.py` & `zod-0.2.5/zod/cli/main.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/cli/utils.py` & `zod-0.2.5/zod/cli/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/cli/visualize_lidar.py` & `zod-0.2.5/zod/cli/visualize_lidar.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/constants.py` & `zod-0.2.5/zod/constants.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/data_classes/box.py` & `zod-0.2.5/zod/data_classes/box.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/data_classes/calibration.py` & `zod-0.2.5/zod/data_classes/calibration.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/data_classes/ego_motion.py` & `zod-0.2.5/zod/data_classes/ego_motion.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/data_classes/frame.py` & `zod-0.2.5/zod/data_classes/frame.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/data_classes/geometry.py` & `zod-0.2.5/zod/data_classes/geometry.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/data_classes/info.py` & `zod-0.2.5/zod/data_classes/info.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/data_classes/metadata.py` & `zod-0.2.5/zod/data_classes/metadata.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/data_classes/sensor.py` & `zod-0.2.5/zod/data_classes/sensor.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/data_classes/sequence.py` & `zod-0.2.5/zod/data_classes/sequence.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/data_classes/vehicle_data.py` & `zod-0.2.5/zod/data_classes/vehicle_data.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/eval/detection/_experimental/eval.py` & `zod-0.2.5/zod/eval/detection/_experimental/eval.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/eval/detection/_experimental/matching.py` & `zod-0.2.5/zod/eval/detection/_experimental/matching.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/eval/detection/_experimental/utils.py` & `zod-0.2.5/zod/eval/detection/_experimental/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/eval/detection/_nuscenes_eval/LICENCE.txt` & `zod-0.2.5/zod/eval/detection/_nuscenes_eval/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/eval/detection/_nuscenes_eval/changes.txt` & `zod-0.2.5/zod/eval/detection/_nuscenes_eval/changes.txt`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/eval/detection/_nuscenes_eval/common/data_classes.py` & `zod-0.2.5/zod/eval/detection/_nuscenes_eval/common/data_classes.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/eval/detection/_nuscenes_eval/common/utils.py` & `zod-0.2.5/zod/eval/detection/_nuscenes_eval/common/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/eval/detection/_nuscenes_eval/detection/README.md` & `zod-0.2.5/zod/eval/detection/_nuscenes_eval/detection/README.md`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/eval/detection/_nuscenes_eval/detection/algo.py` & `zod-0.2.5/zod/eval/detection/_nuscenes_eval/detection/algo.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/eval/detection/_nuscenes_eval/detection/constants.py` & `zod-0.2.5/zod/eval/detection/_nuscenes_eval/detection/constants.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/eval/detection/_nuscenes_eval/detection/data_classes.py` & `zod-0.2.5/zod/eval/detection/_nuscenes_eval/detection/data_classes.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/eval/detection/eval_nuscenes_style.py` & `zod-0.2.5/zod/eval/detection/eval_nuscenes_style.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/utils/compensation.py` & `zod-0.2.5/zod/utils/compensation.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/utils/geometry.py` & `zod-0.2.5/zod/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/utils/polygon_transformations.py` & `zod-0.2.5/zod/utils/polygon_transformations.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/utils/utils.py` & `zod-0.2.5/zod/utils/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/utils/visualization.py` & `zod-0.2.5/zod/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/visualization/bev_utils.py` & `zod-0.2.5/zod/visualization/bev_utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/visualization/colorlabeler.py` & `zod-0.2.5/zod/visualization/colorlabeler.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/visualization/lidar_3d.py` & `zod-0.2.5/zod/visualization/lidar_3d.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/visualization/lidar_bev.py` & `zod-0.2.5/zod/visualization/lidar_bev.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/visualization/lidar_on_image.py` & `zod-0.2.5/zod/visualization/lidar_on_image.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/visualization/object_visualization.py` & `zod-0.2.5/zod/visualization/object_visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/visualization/oxts_on_image.py` & `zod-0.2.5/zod/visualization/oxts_on_image.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/visualization/oxts_visualization.py` & `zod-0.2.5/zod/visualization/oxts_visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/visualization/polygon_utils.py` & `zod-0.2.5/zod/visualization/polygon_utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/zod_drives.py` & `zod-0.2.5/zod/zod_drives.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/zod_frames.py` & `zod-0.2.5/zod/zod_frames.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/zod/zod_sequences.py` & `zod-0.2.5/zod/zod_sequences.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.4/setup.py` & `zod-0.2.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,66 +1,122 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['zod',
- 'zod.anno',
- 'zod.anno.tsr',
- 'zod.cli',
- 'zod.data_classes',
- 'zod.eval',
- 'zod.eval.detection',
- 'zod.eval.detection._experimental',
- 'zod.eval.detection._nuscenes_eval.common',
- 'zod.eval.detection._nuscenes_eval.detection',
- 'zod.utils',
- 'zod.visualization']
-
-package_data = \
-{'': ['*'], 'zod.eval.detection': ['_nuscenes_eval/*']}
-
-install_requires = \
-['dataclass-wizard>=0.22.2',
- 'h5py>=3.1',
- 'numpy-quaternion>=2022.4.2',
- 'numpy>=1.19,<2.0',
- 'pillow>=7',
- 'pyquaternion>=0.9',
- 'scipy>=1.5,<2.0',
- 'tqdm>=4.60']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib-metadata', 'typing-extensions'],
- 'all': ['typer[all]>=0.7.0',
-         'dropbox>=11.36.0',
-         'opencv-python>=4',
-         'matplotlib>=3',
-         'plotly>=5,<6',
-         'dash-bootstrap-components>=1.1',
-         'pandas>=1.3,<2.0',
-         'notebook>=5',
-         'imageio>=2,<3'],
- 'cli': ['typer[all]>=0.7.0', 'dropbox>=11.36.0']}
-
-entry_points = \
-{'console_scripts': ['zod = zod.cli.main:app']}
-
-setup_kwargs = {
-    'name': 'zod',
-    'version': '0.2.4',
-    'description': 'Zenseact Open Dataset',
-    'long_description': '# Zenseact Open Dataset\n\n[![Stable Version](https://img.shields.io/pypi/v/zod?label=stable)](https://pypi.org/project/zod/#history)\n[![Python Versions](https://img.shields.io/pypi/pyversions/zod)](https://pypi.org/project/zod/)\n[![Download Stats](https://img.shields.io/pypi/dm/zod)](https://pypistats.org/packages/zod)\n\nThe Zenseact Open Dataset (ZOD) is a large multi-modal autonomous driving dataset developed by a team of researchers at [Zenseact](https://zenseact.com/). The dataset is split into three categories: *Frames*, *Sequences*, and *Drives*. For more information about the dataset, please refer to our [coming soon](), or visit our [website](https://zod.zenseact.com).\n\n## Examples\nFind examples of how to use the dataset in the [examples](examples/) folder. Here you will find a set of jupyter notebooks that demonstrate how to use the dataset, as well as an example of how to train an object detection model using [Detectron2](https://github.com/facebookresearch/detectron2).\n\n## Installation\n\nThe install the library with minimal dependencies, for instance to be used in a training environment without need for interactivity och visualization, run:\n```bash\npip install zod\n```\n\nTo install the library along with the CLI, which can be used to download the dataset, convert between formats, and perform visualization, run:\n```bash\npip install "zod[cli]"\n```\n\nTo install the full devkit, with the CLI and all dependencies, run:\n```bash\npip install "zod[all]"\n```\n\n## Download using the CLI\n\nThis is an example of how to download the ZOD Frames mini-dataset using the CLI. Prerequisites are that you have applied for access and received a download link.\nThe simplest way to download the dataset is to use the CLI interactively:\n```bash\nzod download\n```\nThis will prompt you for the required information, present you with a summary of the download, and then ask for confirmation. You can of course also specify all the required information directly on the command line, and avoid the confirmation using `--no-confirm` or `-y`. For example:\n```bash\nzod download -y --url="<download-link>" --output-dir=<path/to/outputdir> --subset=frames --version=mini\n```\nBy default, all data streams are downloaded for ZodSequences and ZodDrives. For ZodFrames, DNAT versions of the images, and surrounding (non-keyframe) lidar scans are excluded. To download them as well, run:\n```bash\nzod download -y --url="<download-link>" --output-dir=<path/to/outputdir> --subset=frames --version=full --num-scans-before=-1 --num-scans-after=-1 --dnat\n```\nIf you want to exclude some of the data streams, you can do so by specifying the `--no-<stream>` flag. For example, to download only the DNAT images, infos, and annotations, run:\n```bash\nzod download --dnat --no-blur --no-lidar --no-oxts --no-vehicle-data\n```\nFinally, for a full list of options you can of course run:\n```bash\nzod download --help\n```\n\n## Anonymization\nTo preserve privacy, the dataset is anonymized. The anonymization is performed by [brighterAI](https://brighter.ai/), and we provide two separate modes of anonymization: deep fakes (DNAT) and blur. In our paper, we show that the performance of an object detector is not affected by the anonymization method. For more details regarding this experiment, please refer to our [coming soon]().\n\n## Citation\nIf you publish work that uses Zenseact Open Dataset, please cite [our arxiv paper](https://arxiv.org/abs/2305.02008):\n\n```\n@article{zod2023,\n  author = {Alibeigi, Mina and Ljungbergh, William and Tonderski, Adam and Hess, Georg and Lilja, Adam and Lindstr{\\"o}m, Carl and Motorniuk, Daria and Fu, Junsheng and Widahl, Jenny and Petersson, Christoffer},\n  title = {Zenseact Open Dataset: A large-scale and diverse multimodal dataset for autonomous driving},\n  year = {2023},\n  journal = {arXiv preprint arXiv:2305.02008},\n}\n```\n\n## Contact\nFor questions about the dataset, please [Contact Us](mailto:opendataset@zenseact.com).\n\n## Contributing\nWe welcome contributions to the development kit. If you would like to contribute, please open a pull request.\n\n## License\n**Dataset**:\nThis dataset is the property of Zenseact AB (© 2023 Zenseact AB) and is licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Any public use, distribution, or display of this dataset must contain this notice in full:\n\n> For this dataset, Zenseact AB has taken all reasonable measures to remove all personally identifiable information, including faces and license plates. To the extent that you like to request the removal of specific images from the dataset, please contact [privacy@zenseact.com](mailto:privacy@zenseact.com).\n\n\n**Development kit**:\nThis development kit is the property of Zenseact AB (© 2023 Zenseact AB) and is licensed under [MIT](https://opensource.org/licenses/MIT).\n',
-    'author': 'Zenseact',
-    'author_email': 'opendataset@zenseact.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://zod.zenseact.com',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<4.0.0',
+Metadata-Version: 2.1
+Name: zod
+Version: 0.2.5
+Summary: Zenseact Open Dataset
+Home-page: https://zod.zenseact.com
+License: MIT
+Author: Zenseact
+Author-email: opendataset@zenseact.com
+Requires-Python: >=3.7.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
+Provides-Extra: cli
+Requires-Dist: dash-bootstrap-components (>=1.1) ; extra == "all"
+Requires-Dist: dataclass-wizard (>=0.22.2)
+Requires-Dist: dropbox (>=11.36.0) ; extra == "cli" or extra == "all"
+Requires-Dist: h5py (>=3.1)
+Requires-Dist: imageio (>=2,<3) ; extra == "all"
+Requires-Dist: importlib-metadata ; python_version < "3.8"
+Requires-Dist: matplotlib (>=3) ; extra == "all"
+Requires-Dist: notebook (>=5) ; extra == "all"
+Requires-Dist: numpy (>=1.19,<2.0)
+Requires-Dist: numpy-quaternion (>=2022.4.2)
+Requires-Dist: opencv-python (>=4) ; extra == "all"
+Requires-Dist: pandas (>=1.3,<2.0) ; extra == "all"
+Requires-Dist: pillow (>=7)
+Requires-Dist: plotly (>=5,<6) ; extra == "all"
+Requires-Dist: pyquaternion (>=0.9)
+Requires-Dist: scipy (>=1.5,<2.0)
+Requires-Dist: tqdm (>=4.60)
+Requires-Dist: typer[all] (>=0.7.0) ; extra == "cli" or extra == "all"
+Requires-Dist: typing-extensions ; python_version < "3.8"
+Project-URL: Repository, https://github.com/zenseact/zod
+Description-Content-Type: text/markdown
+
+# Zenseact Open Dataset
+
+[![Stable Version](https://img.shields.io/pypi/v/zod?label=stable)](https://pypi.org/project/zod/#history)
+[![Python Versions](https://img.shields.io/pypi/pyversions/zod)](https://pypi.org/project/zod/)
+[![Download Stats](https://img.shields.io/pypi/dm/zod)](https://pypistats.org/packages/zod)
+
+The Zenseact Open Dataset (ZOD) is a large multi-modal autonomous driving dataset developed by a team of researchers at [Zenseact](https://zenseact.com/). The dataset is split into three categories: *Frames*, *Sequences*, and *Drives*. For more information about the dataset, please refer to our [coming soon](), or visit our [website](https://zod.zenseact.com).
+
+## Examples
+Find examples of how to use the dataset in the [examples](examples/) folder. Here you will find a set of jupyter notebooks that demonstrate how to use the dataset, as well as an example of how to train an object detection model using [Detectron2](https://github.com/facebookresearch/detectron2).
+
+## Installation
+
+The install the library with minimal dependencies, for instance to be used in a training environment without need for interactivity och visualization, run:
+```bash
+pip install zod
+```
+
+To install the library along with the CLI, which can be used to download the dataset, convert between formats, and perform visualization, run:
+```bash
+pip install "zod[cli]"
+```
+
+To install the full devkit, with the CLI and all dependencies, run:
+```bash
+pip install "zod[all]"
+```
+
+## Download using the CLI
+
+This is an example of how to download the ZOD Frames mini-dataset using the CLI. Prerequisites are that you have applied for access and received a download link.
+The simplest way to download the dataset is to use the CLI interactively:
+```bash
+zod download
+```
+This will prompt you for the required information, present you with a summary of the download, and then ask for confirmation. You can of course also specify all the required information directly on the command line, and avoid the confirmation using `--no-confirm` or `-y`. For example:
+```bash
+zod download -y --url="<download-link>" --output-dir=<path/to/outputdir> --subset=frames --version=mini
+```
+By default, all data streams are downloaded for ZodSequences and ZodDrives. For ZodFrames, DNAT versions of the images, and surrounding (non-keyframe) lidar scans are excluded. To download them as well, run:
+```bash
+zod download -y --url="<download-link>" --output-dir=<path/to/outputdir> --subset=frames --version=full --num-scans-before=-1 --num-scans-after=-1 --dnat
+```
+If you want to exclude some of the data streams, you can do so by specifying the `--no-<stream>` flag. For example, to download only the DNAT images, infos, and annotations, run:
+```bash
+zod download --dnat --no-blur --no-lidar --no-oxts --no-vehicle-data
+```
+Finally, for a full list of options you can of course run:
+```bash
+zod download --help
+```
+
+## Anonymization
+To preserve privacy, the dataset is anonymized. The anonymization is performed by [brighterAI](https://brighter.ai/), and we provide two separate modes of anonymization: deep fakes (DNAT) and blur. In our paper, we show that the performance of an object detector is not affected by the anonymization method. For more details regarding this experiment, please refer to our [coming soon]().
+
+## Citation
+If you publish work that uses Zenseact Open Dataset, please cite [our arxiv paper](https://arxiv.org/abs/2305.02008):
+
+```
+@article{zod2023,
+  author = {Alibeigi, Mina and Ljungbergh, William and Tonderski, Adam and Hess, Georg and Lilja, Adam and Lindstr{\"o}m, Carl and Motorniuk, Daria and Fu, Junsheng and Widahl, Jenny and Petersson, Christoffer},
+  title = {Zenseact Open Dataset: A large-scale and diverse multimodal dataset for autonomous driving},
+  year = {2023},
+  journal = {arXiv preprint arXiv:2305.02008},
 }
+```
+
+## Contact
+For questions about the dataset, please [Contact Us](mailto:opendataset@zenseact.com).
+
+## Contributing
+We welcome contributions to the development kit. If you would like to contribute, please open a pull request.
+
+## License
+**Dataset**:
+This dataset is the property of Zenseact AB (© 2023 Zenseact AB) and is licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Any public use, distribution, or display of this dataset must contain this notice in full:
+
+> For this dataset, Zenseact AB has taken all reasonable measures to remove all personally identifiable information, including faces and license plates. To the extent that you like to request the removal of specific images from the dataset, please contact [privacy@zenseact.com](mailto:privacy@zenseact.com).
+
 
+**Development kit**:
+This development kit is the property of Zenseact AB (© 2023 Zenseact AB) and is licensed under [MIT](https://opensource.org/licenses/MIT).
 
-setup(**setup_kwargs)
```

