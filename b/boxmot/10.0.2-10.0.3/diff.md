# Comparing `tmp/boxmot-10.0.2.tar.gz` & `tmp/boxmot-10.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boxmot-10.0.2.tar", last modified: Mon May 22 21:10:16 2023, max compression
+gzip compressed data, was "boxmot-10.0.3.tar", last modified: Mon May 22 21:54:22 2023, max compression
```

## Comparing `boxmot-10.0.2.tar` & `boxmot-10.0.3.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:10:16.749525 boxmot-10.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-22 21:08:32.000000 boxmot-10.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-05-22 21:10:16.749525 boxmot-10.0.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    10579 2023-05-22 21:08:32.000000 boxmot-10.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:10:16.741525 boxmot-10.0.2/boxmot/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:10:16.741525 boxmot-10.0.2/boxmot/botsort/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/botsort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/botsort/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (123)    18661 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/botsort/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/botsort/gmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/botsort/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/botsort/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:10:16.741525 boxmot-10.0.2/boxmot/bytetrack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/bytetrack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/bytetrack/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (123)    12396 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/bytetrack/byte_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/bytetrack/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/bytetrack/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:10:16.741525 boxmot-10.0.2/boxmot/deep/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:10:16.745525 boxmot-10.0.2/boxmot/deep/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/bnneck.py
--rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/hacnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/inceptionresnetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/inceptionv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/lmbn_n.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/mlfn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/mobilenetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/mudeep.py
--rw-r--r--   0 runner    (1001) docker     (123)    36186 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17037 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/osnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/osnet_ain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/pcb.py
--rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8598 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/resnet_ibn_a.py
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/resnet_ibn_b.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/resnetmid.py
--rw-r--r--   0 runner    (1001) docker     (123)    20684 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/senet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/shufflenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/shufflenetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/squeezenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/models/xception.py
--rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/reid_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/reid_model_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deep/reid_multibackend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:10:16.745525 boxmot-10.0.2/boxmot/deepocsort/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deepocsort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deepocsort/args.py
--rw-r--r--   0 runner    (1001) docker     (123)    15827 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deepocsort/association.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deepocsort/cmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deepocsort/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    61669 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deepocsort/kalmanfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/deepocsort/ocsort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:10:16.745525 boxmot-10.0.2/boxmot/ocsort/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/ocsort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/ocsort/association.py
--rw-r--r--   0 runner    (1001) docker     (123)    59022 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/ocsort/kalmanfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/ocsort/ocsort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:10:16.745525 boxmot-10.0.2/boxmot/strongsort/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 21:08:32.000000 boxmot-10.0.2/boxmot/strongsort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:10:16.749525 boxmot-10.0.2/boxmot/strongsort/sort/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 21:08:33.000000 boxmot-10.0.2/boxmot/strongsort/sort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-22 21:08:33.000000 boxmot-10.0.2/boxmot/strongsort/sort/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-22 21:08:33.000000 boxmot-10.0.2/boxmot/strongsort/sort/iou_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-05-22 21:08:33.000000 boxmot-10.0.2/boxmot/strongsort/sort/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-22 21:08:33.000000 boxmot-10.0.2/boxmot/strongsort/sort/linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-05-22 21:08:33.000000 boxmot-10.0.2/boxmot/strongsort/sort/nn_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-22 21:08:33.000000 boxmot-10.0.2/boxmot/strongsort/sort/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-22 21:08:33.000000 boxmot-10.0.2/boxmot/strongsort/sort/track.py
--rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-05-22 21:08:33.000000 boxmot-10.0.2/boxmot/strongsort/sort/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-05-22 21:08:33.000000 boxmot-10.0.2/boxmot/strongsort/strong_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:10:16.749525 boxmot-10.0.2/boxmot/strongsort/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 21:08:33.000000 boxmot-10.0.2/boxmot/strongsort/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-22 21:08:33.000000 boxmot-10.0.2/boxmot/strongsort/utils/asserts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-22 21:08:33.000000 boxmot-10.0.2/boxmot/strongsort/utils/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-22 21:08:33.000000 boxmot-10.0.2/boxmot/strongsort/utils/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-22 21:08:33.000000 boxmot-10.0.2/boxmot/strongsort/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-05-22 21:08:33.000000 boxmot-10.0.2/boxmot/strongsort/utils/json_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-22 21:08:33.000000 boxmot-10.0.2/boxmot/strongsort/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-22 21:08:33.000000 boxmot-10.0.2/boxmot/strongsort/utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-22 21:08:33.000000 boxmot-10.0.2/boxmot/strongsort/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-22 21:08:33.000000 boxmot-10.0.2/boxmot/tracker_zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:10:16.741525 boxmot-10.0.2/boxmot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-05-22 21:10:16.000000 boxmot-10.0.2/boxmot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-22 21:10:16.000000 boxmot-10.0.2/boxmot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 21:10:16.000000 boxmot-10.0.2/boxmot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-22 21:10:16.000000 boxmot-10.0.2/boxmot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 21:10:16.000000 boxmot-10.0.2/boxmot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 21:10:16.749525 boxmot-10.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-22 21:08:33.000000 boxmot-10.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:54:22.575312 boxmot-10.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-22 21:53:06.000000 boxmot-10.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12092 2023-05-22 21:54:22.575312 boxmot-10.0.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10606 2023-05-22 21:53:06.000000 boxmot-10.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:54:22.567312 boxmot-10.0.3/boxmot/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:54:22.567312 boxmot-10.0.3/boxmot/botsort/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/botsort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/botsort/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18661 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/botsort/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/botsort/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/botsort/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/botsort/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:54:22.567312 boxmot-10.0.3/boxmot/bytetrack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/bytetrack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/bytetrack/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12396 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/bytetrack/byte_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/bytetrack/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/bytetrack/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:54:22.567312 boxmot-10.0.3/boxmot/deep/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:54:22.571313 boxmot-10.0.3/boxmot/deep/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/bnneck.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/hacnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/inceptionresnetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/inceptionv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/lmbn_n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/mlfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/mobilenetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/mudeep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36186 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17037 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/osnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/osnet_ain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/pcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8598 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/resnet_ibn_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/resnet_ibn_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/resnetmid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20684 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/shufflenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/shufflenetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/squeezenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/models/xception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/reid_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/reid_model_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deep/reid_multibackend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:54:22.571313 boxmot-10.0.3/boxmot/deepocsort/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deepocsort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deepocsort/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15827 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deepocsort/association.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deepocsort/cmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deepocsort/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61669 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deepocsort/kalmanfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/deepocsort/ocsort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:54:22.571313 boxmot-10.0.3/boxmot/ocsort/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/ocsort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/ocsort/association.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59022 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/ocsort/kalmanfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/ocsort/ocsort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:54:22.571313 boxmot-10.0.3/boxmot/strongsort/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 21:53:06.000000 boxmot-10.0.3/boxmot/strongsort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:54:22.571313 boxmot-10.0.3/boxmot/strongsort/sort/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 21:53:07.000000 boxmot-10.0.3/boxmot/strongsort/sort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-22 21:53:07.000000 boxmot-10.0.3/boxmot/strongsort/sort/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-22 21:53:07.000000 boxmot-10.0.3/boxmot/strongsort/sort/iou_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-05-22 21:53:07.000000 boxmot-10.0.3/boxmot/strongsort/sort/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-22 21:53:07.000000 boxmot-10.0.3/boxmot/strongsort/sort/linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-05-22 21:53:07.000000 boxmot-10.0.3/boxmot/strongsort/sort/nn_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-22 21:53:07.000000 boxmot-10.0.3/boxmot/strongsort/sort/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-22 21:53:07.000000 boxmot-10.0.3/boxmot/strongsort/sort/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-05-22 21:53:07.000000 boxmot-10.0.3/boxmot/strongsort/sort/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-05-22 21:53:07.000000 boxmot-10.0.3/boxmot/strongsort/strong_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:54:22.571313 boxmot-10.0.3/boxmot/strongsort/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 21:53:07.000000 boxmot-10.0.3/boxmot/strongsort/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-22 21:53:07.000000 boxmot-10.0.3/boxmot/strongsort/utils/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-22 21:53:07.000000 boxmot-10.0.3/boxmot/strongsort/utils/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-22 21:53:07.000000 boxmot-10.0.3/boxmot/strongsort/utils/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-22 21:53:07.000000 boxmot-10.0.3/boxmot/strongsort/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-05-22 21:53:07.000000 boxmot-10.0.3/boxmot/strongsort/utils/json_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-22 21:53:07.000000 boxmot-10.0.3/boxmot/strongsort/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-22 21:53:07.000000 boxmot-10.0.3/boxmot/strongsort/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-22 21:53:07.000000 boxmot-10.0.3/boxmot/strongsort/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-22 21:53:07.000000 boxmot-10.0.3/boxmot/tracker_zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:54:22.567312 boxmot-10.0.3/boxmot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12092 2023-05-22 21:54:22.000000 boxmot-10.0.3/boxmot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-22 21:54:22.000000 boxmot-10.0.3/boxmot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 21:54:22.000000 boxmot-10.0.3/boxmot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-22 21:54:22.000000 boxmot-10.0.3/boxmot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 21:54:22.000000 boxmot-10.0.3/boxmot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 21:54:22.575312 boxmot-10.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-22 21:53:07.000000 boxmot-10.0.3/setup.py
```

### Comparing `boxmot-10.0.2/LICENSE` & `boxmot-10.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/PKG-INFO` & `boxmot-10.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxmot
-Version: 10.0.2
+Version: 10.0.3
 Summary: SOTA tracking methods for detection, segmentation and pose estimation models.
 Home-page: https://github.com/mikel-brostrom/yolov8_tracking
 Author: Mikel Brostrom
 Author-email: yolov5.deepsort.pytorch@gmail.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/mikel-brostrom/yolov8_tracking/issues
 Project-URL: Source, https://github.com/mikel-brostrom/yolov8_tracking
@@ -46,44 +46,17 @@
 <a href="https://doi.org/10.5281/zenodo.7629840"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.7629840.svg" alt="DOI"></a>
   </div>
 </div>
 
 
 ## Introduction
 
-This repository contains a highly configurable two-stage-tracker that adjusts to different deployment scenarios. It can jointly perform multiple object tracking and instance segmentation (MOTS). The detections generated by [YOLOv8](https://github.com/ultralytics/ultralytics), a family of object detection architectures and models pretrained on the [COCO](https://arxiv.org/abs/1405.0312) dataset, are passed to the tracker of your choice. Supported ones at the moment are: [DeepOCSORT](https://arxiv.org/abs/2302.11813) [LightMBN](https://arxiv.org/pdf/2101.10774.pdf), [BoTSORT](https://arxiv.org/abs/2206.14651) [LightMBN](https://github.com/jixunbo/LightMBN)[](https://arxiv.org/pdf/2101.10774.pdf), [StrongSORT](https://github.com/dyhBUPT/StrongSORT)[](https://arxiv.org/abs/2202.13514) [LightMBN](https://github.com/jixunbo/LightMBN)[](https://arxiv.org/pdf/2101.10774.pdf), [OCSORT](https://github.com/noahcao/OC_SORT)[](https://arxiv.org/abs/2203.14360) and [ByteTrack](https://github.com/ifzhang/ByteTrack)[](https://arxiv.org/abs/2110.06864). They can track any object that your Yolov8 model was trained to detect.
+This repo contains a collections of state-of-the-art multi-object trackers. Some of them are based on motion only, others on motion + appearance description. For the latter, state-of-the-art ReID model are provided. Supported ones at the moment are: [DeepOCSORT](https://arxiv.org/abs/2302.11813) [LightMBN](https://arxiv.org/pdf/2101.10774.pdf), [BoTSORT](https://arxiv.org/abs/2206.14651) [LightMBN](https://github.com/jixunbo/LightMBN)[](https://arxiv.org/pdf/2101.10774.pdf), [StrongSORT](https://github.com/dyhBUPT/StrongSORT)[](https://arxiv.org/abs/2202.13514) [LightMBN](https://github.com/jixunbo/LightMBN)[](https://arxiv.org/pdf/2101.10774.pdf), [OCSORT](https://github.com/noahcao/OC_SORT)[](https://arxiv.org/abs/2203.14360) and [ByteTrack](https://github.com/ifzhang/ByteTrack)[](https://arxiv.org/abs/2110.06864).
 
-## Why using this tracking toolbox?
-
-Everything is designed with simplicity and flexibility in mind. We don't hyperfocus on results on a single dataset, we prioritize real-world results. If you don't get good tracking results on your custom dataset with the out-of-the-box tracker configurations, use the `evolve.py` script for tracker hyperparameter tuning.
-
-## Installation
-
-```
-pip install boxmot
-```
-
-## Custom model usage
-
-```python
-from boxmot import DeepOCSORT
-
-tracker = DeepOCSORT()
-cap = cv.VideoCapture(0)
-while True:
-    ret, im = cap.read()
-    ...
-    # dets: 
-    #  - your model's nms:ed outputs of shape Nx6 (x, y, x, y, conf, cls)
-    # im:
-    #  - the original image (for better ReID results)
-    #  - the downscaled one fed to you model
-    tracker_outputs = tracker.update(dets.cpu(), im)  # --> (x, y, x, y, id, conf, cls)
-    ...
-```
+We provide examples on how to use this package together with popular object detection models. Right now only [Yolov8](https://github.com/ultralytics) is available. Yolo-NAS & YOLOX coming soon.
 
 <details>
 <summary>Tutorials</summary>
 
 * [Yolov8 training (link to external repository)](https://docs.ultralytics.com/modes/train/)&nbsp;
 * [Deep appearance descriptor training (link to external repository)](https://kaiyangzhou.github.io/deep-person-reid/user_guide.html)&nbsp;
 * [ReID model export to ONNX, OpenVINO, TensorRT and TorchScript](https://github.com/mikel-brostrom/yolov8_tracking/wiki/ReID-multi-framework-model-export)&nbsp;
@@ -117,76 +90,82 @@
 * [Yolov5 StrongSORT OSNet vs other trackers MOT17](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/wiki/MOT-17-evaluation-(private-detector))&nbsp;
 
 * [StrongSORT MOT16 ablation study](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/wiki/Yolov5DeepSORTwithOSNet-vs-Yolov5StrongSORTwithOSNet-ablation-study-on-MOT16)&nbsp;
 
 * [Yolov5 StrongSORT OSNet vs other trackers MOT16 (deprecated)](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/wiki/MOT-16-evaluation)&nbsp;
 
   </details>
-  
-<details>
-<summary>Custom object detection architecture</summary>
 
-The trackers provided in this repo can be used with other object detectors than Yolov8. Make sure that the input to the trackers is of the following format:
+## Why using this tracking toolbox?
 
-```bash
-Nx6 (x, y, x, y, conf, cls)
+Everything is designed with simplicity and flexibility in mind. We don't hyperfocus on results on a single dataset, we prioritize real-world results. If you don't get good tracking results on your custom dataset with the out-of-the-box tracker configurations, use the `examples/evolve.py` script for tracker hyperparameter tuning.
+
+## Installation
+
+```
+pip install boxmot
 ```
 
-</details>
+## Yolov8 example
 
 <details>
-<summary>Tracking with Yolov8</summary>
+<summary>Click to expand!</summary>
+
+<details>
+<summary>Yolov8 model</summary>
   
 
 
 ```bash
-$ python track.py --yolo-model yolov8n.pt      # bboxes only
-                                 yolov8n-seg.pt  # bboxes + segmentation masks
-                                 yolov8n-pose.pt # bboxes + pose estimation
+$ python examples/track.py --yolo-model yolov8n.pt      # bboxes only
+                                        yolov8n-seg.pt  # bboxes + segmentation masks
+                                        yolov8n-pose.pt # bboxes + pose estimation
 ```
+  
+  </details>
 
 <details>
 <summary>Tracking methods</summary>
 
 ```bash
-$ python track.py --tracking-method deepocsort
-                                    strongsort
-                                    ocsort
-                                    bytetrack
-                                    botsort
+$ python examples/track.py --tracking-method deepocsort
+                                             strongsort
+                                             ocsort
+                                             bytetrack
+                                             botsort
 ```
   
 </details>
 
 <details>
 <summary>Tracking sources</summary>
 
 Tracking can be run on most video formats
 
 ```bash
-$ python track.py --source 0                               # webcam
-                           img.jpg                         # image
-                           vid.mp4                         # video
-                           path/                           # directory
-                           path/*.jpg                      # glob
-                           'https://youtu.be/Zgi9g1ksQHc'  # YouTube
-                           'rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP stream
+$ python examples/track.py --source 0                               # webcam
+                                    img.jpg                         # image
+                                    vid.mp4                         # video
+                                    path/                           # directory
+                                    path/*.jpg                      # glob
+                                    'https://youtu.be/Zgi9g1ksQHc'  # YouTube
+                                    'rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP stream
 ```
 
 </details>
 
 <details>
 <summary>Select Yolov8 model</summary>
 
 There is a clear trade-off between model inference speed and overall performance. In order to make it possible to fulfill your inference speed/accuracy needs you can select a Yolov5 family model for automatic download. These model can be further optimized for you needs by the [export.py](https://github.com/ultralytics/yolov5/blob/master/export.py) script
 
 ```bash
 
 
-$ python track.py --source 0 --yolo-model yolov8n.pt --img 640
+$ python examples/track.py --source 0 --yolo-model yolov8n.pt --img 640
                                           yolov8s.tflite
                                           yolov8m.pt
                                           yolov8l.onnx 
                                           yolov8x.pt --img 1280
                                           ...
 ```
   
@@ -194,63 +173,88 @@
 
 <details>
 <summary>Select ReID model</summary>
 
 Some tracking methods combine appearance description and motion in the process of tracking. For those which use appearance, you can choose a ReID model based on your needs from this [ReID model zoo](https://kaiyangzhou.github.io/deep-person-reid/MODEL_ZOO). These model can be further optimized for you needs by the [reid_export.py](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/blob/master/reid_export.py) script
 
 ```bash
-$ python track.py --source 0 --reid-model lmbn_n_cuhk03_d.pt
-                                          osnet_x0_25_market1501.pt
-                                          mobilenetv2_x1_4_msmt17.engine
-                                          resnet50_msmt17.onnx
-                                          osnet_x1_0_msmt17.pt
-                                          ...
+$ python examples/track.py --source 0 --reid-model lmbn_n_cuhk03_d.pt
+                                                   osnet_x0_25_market1501.pt
+                                                   mobilenetv2_x1_4_msmt17.engine
+                                                   resnet50_msmt17.onnx
+                                                   osnet_x1_0_msmt17.pt
+                                                   ...
 ```
 
 </details>
   
 <details>
 <summary>Filter tracked classes</summary>
 
 By default the tracker tracks all MS COCO classes.
 
 If you want to track a subset of the classes that you model predicts, add their corresponding index after the classes flag,
 
 ```bash
-python track.py --source 0 --yolo-model yolov8s.pt --classes 16 17  # COCO yolov8 model. Track cats and dogs, only
+python examples/track.py --source 0 --yolo-model yolov8s.pt --classes 16 17  # COCO yolov8 model. Track cats and dogs, only
 ```
 
 [Here](https://tech.amikelive.com/node-718/what-object-categories-labels-are-in-coco-dataset/) is a list of all the possible objects that a Yolov8 model trained on MS COCO can detect. Notice that the indexing for the classes in this repo starts at zero
 
 </details>
 
 <details>
 <summary>MOT compliant results</summary>
   
 Can be saved to your experiment folder `runs/track/<yolo_model>_<deep_sort_model>/` by 
 
 ```bash
-python track.py --source ... --save-txt
+python examples/track.py --source ... --save-txt
 ```
 
 </details>
 
 <details>
 <summary>Tracker hyperparameter tuning</summary>
 
 We use a fast and elitist multiobjective genetic algorithm for tracker hyperparameter tuning. By default the objectives are: HOTA, MOTA, IDF1. Run it by
 
 ```bash
-$ python evolve.py --tracking-method strongsort --benchmark MOT17 --n-trials 100  # tune strongsort for MOT17
-                   --tracking-method ocsort     --benchmark <your-custom-dataset> --objective HOTA # tune ocsort for maximizing HOTA on your custom tracking dataset
+$ python examples/evolve.py --tracking-method strongsort --benchmark MOT17 --n-trials 100  # tune strongsort for MOT17
+                            --tracking-method ocsort     --benchmark <your-custom-dataset> --objective HOTA # tune ocsort for maximizing HOTA on your custom tracking dataset
 ```
 
 The set of hyperparameters leading to the best HOTA result are written to the tracker's config file.
 
 </details>
   
 </details>
 
+## Custom object detection model example
+  
+<details>
+<summary>Click to exapand!</summary>
+
+```python
+from boxmot import DeepOCSORT
+
+tracker = DeepOCSORT()
+cap = cv.VideoCapture(0)
+while True:
+    ret, im = cap.read()
+    ...
+    # dets: 
+    #  - your model's nms:ed outputs of shape Nx6 (x, y, x, y, conf, cls)
+    # im:
+    #  - the original image (for better ReID results)
+    #  - the downscaled one fed to you model (faster)
+    tracker_outputs = tracker.update(dets.cpu(), im)  # --> (x, y, x, y, id, conf, cls)
+    ...
+```
+  
+</details>
+  
+
 ## Contact 
 
 For Yolov8 tracking bugs and feature requests please visit [GitHub Issues](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/issues). 
 For business inquiries or professional support requests please send an email to: yolov5.deepsort.pytorch@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: boxmot Version: 10.0.2 Summary: SOTA tracking
+Metadata-Version: 2.1 Name: boxmot Version: 10.0.3 Summary: SOTA tracking
 methods for detection, segmentation and pose estimation models. Home-page:
 https://github.com/mikel-brostrom/yolov8_tracking Author: Mikel Brostrom
 Author-email: yolov5.deepsort.pytorch@gmail.com License: AGPL-3.0 Project-URL:
 Bug Reports, https://github.com/mikel-brostrom/yolov8_tracking/issues Project-
 URL: Source, https://github.com/mikel-brostrom/yolov8_tracking Keywords:
 machine-learning,deep-learning,vision,ML,DL,AI,YOLO Platform: linux Platform:
 windows Classifier: Development Status :: 3 - Alpha Classifier: Intended
@@ -19,46 +19,34 @@
 Engineering :: Image Processing Requires-Python: >=3.7 Description-Content-
 Type: text/markdown License-File: LICENSE # Real-time multi-object,
 segmentation and pose tracking using Yolov8 with DeepOCSORT and LightMBN
           [boxmot/strongsort/results/track_all_seg_1280_025conf.gif]
 
                                [CI_CPU_testing]
                              [Open_In_Colab] [DOI]
-## Introduction This repository contains a highly configurable two-stage-
-tracker that adjusts to different deployment scenarios. It can jointly perform
-multiple object tracking and instance segmentation (MOTS). The detections
-generated by [YOLOv8](https://github.com/ultralytics/ultralytics), a family of
-object detection architectures and models pretrained on the [COCO](https://
-arxiv.org/abs/1405.0312) dataset, are passed to the tracker of your choice.
-Supported ones at the moment are: [DeepOCSORT](https://arxiv.org/abs/
+## Introduction This repo contains a collections of state-of-the-art multi-
+object trackers. Some of them are based on motion only, others on motion +
+appearance description. For the latter, state-of-the-art ReID model are
+provided. Supported ones at the moment are: [DeepOCSORT](https://arxiv.org/abs/
 2302.11813) [LightMBN](https://arxiv.org/pdf/2101.10774.pdf), [BoTSORT](https:/
 /arxiv.org/abs/2206.14651) [LightMBN](https://github.com/jixunbo/LightMBN)[]
 (https://arxiv.org/pdf/2101.10774.pdf), [StrongSORT](https://github.com/
 dyhBUPT/StrongSORT)[](https://arxiv.org/abs/2202.13514) [LightMBN](https://
 github.com/jixunbo/LightMBN)[](https://arxiv.org/pdf/2101.10774.pdf), [OCSORT]
 (https://github.com/noahcao/OC_SORT)[](https://arxiv.org/abs/2203.14360) and
 [ByteTrack](https://github.com/ifzhang/ByteTrack)[](https://arxiv.org/abs/
-2110.06864). They can track any object that your Yolov8 model was trained to
-detect. ## Why using this tracking toolbox? Everything is designed with
-simplicity and flexibility in mind. We don't hyperfocus on results on a single
-dataset, we prioritize real-world results. If you don't get good tracking
-results on your custom dataset with the out-of-the-box tracker configurations,
-use the `evolve.py` script for tracker hyperparameter tuning. ## Installation
-``` pip install boxmot ``` ## Custom model usage ```python from boxmot import
-DeepOCSORT tracker = DeepOCSORT() cap = cv.VideoCapture(0) while True: ret, im
-= cap.read() ... # dets: # - your model's nms:ed outputs of shape Nx6 (x, y, x,
-y, conf, cls) # im: # - the original image (for better ReID results) # - the
-downscaled one fed to you model tracker_outputs = tracker.update(dets.cpu(),
-im) # --> (x, y, x, y, id, conf, cls) ... ```  Tutorials * [Yolov8 training
-(link to external repository)](https://docs.ultralytics.com/modes/train/)  *
-[Deep appearance descriptor training (link to external repository)](https://
-kaiyangzhou.github.io/deep-person-reid/user_guide.html)  * [ReID model export
-to ONNX, OpenVINO, TensorRT and TorchScript](https://github.com/mikel-brostrom/
-yolov8_tracking/wiki/ReID-multi-framework-model-export)  * [Evaluation on
-custom tracking dataset](https://github.com/mikel-brostrom/yolov8_tracking/
+2110.06864). We provide examples on how to use this package together with
+popular object detection models. Right now only [Yolov8](https://github.com/
+ultralytics) is available. Yolo-NAS & YOLOX coming soon.  Tutorials * [Yolov8
+training (link to external repository)](https://docs.ultralytics.com/modes/
+train/)  * [Deep appearance descriptor training (link to external repository)]
+(https://kaiyangzhou.github.io/deep-person-reid/user_guide.html)  * [ReID model
+export to ONNX, OpenVINO, TensorRT and TorchScript](https://github.com/mikel-
+brostrom/yolov8_tracking/wiki/ReID-multi-framework-model-export)  * [Evaluation
+on custom tracking dataset](https://github.com/mikel-brostrom/yolov8_tracking/
 wiki/How-to-evaluate-on-custom-tracking-dataset)  * [ReID inference
 acceleration with Nebullvm](https://colab.research.google.com/drive/
 1APUZ1ijCiQFBR9xD0gUvFUOC8yOJIvHm?usp=sharing)    Experiments In inverse
 chronological order: * [Evaluation of the params evolved for first half of
 MOT17 on the complete MOT17](https://github.com/mikel-brostrom/
 Yolov5_StrongSORT_OSNet/wiki/Evaluation-of-the-params-evolved-for-first-half-
 of-MOT17-on-the-complete-MOT17) * [Segmentation model vs object detetion model
@@ -82,54 +70,63 @@
 brostrom/Yolov5_StrongSORT_OSNet/tree/botsort * [Yolov5 StrongSORT OSNet vs
 other trackers MOT17](https://github.com/mikel-brostrom/
 Yolov5_StrongSORT_OSNet/wiki/MOT-17-evaluation-(private-detector))  *
 [StrongSORT MOT16 ablation study](https://github.com/mikel-brostrom/
 Yolov5_StrongSORT_OSNet/wiki/Yolov5DeepSORTwithOSNet-vs-
 Yolov5StrongSORTwithOSNet-ablation-study-on-MOT16)  * [Yolov5 StrongSORT OSNet
 vs other trackers MOT16 (deprecated)](https://github.com/mikel-brostrom/
-Yolov5_StrongSORT_OSNet/wiki/MOT-16-evaluation)    Custom object detection
-architecture The trackers provided in this repo can be used with other object
-detectors than Yolov8. Make sure that the input to the trackers is of the
-following format: ```bash Nx6 (x, y, x, y, conf, cls) ```   Tracking with
-Yolov8 ```bash $ python track.py --yolo-model yolov8n.pt # bboxes only yolov8n-
-seg.pt # bboxes + segmentation masks yolov8n-pose.pt # bboxes + pose estimation
-```  Tracking methods ```bash $ python track.py --tracking-method deepocsort
+Yolov5_StrongSORT_OSNet/wiki/MOT-16-evaluation)   ## Why using this tracking
+toolbox? Everything is designed with simplicity and flexibility in mind. We
+don't hyperfocus on results on a single dataset, we prioritize real-world
+results. If you don't get good tracking results on your custom dataset with the
+out-of-the-box tracker configurations, use the `examples/evolve.py` script for
+tracker hyperparameter tuning. ## Installation ``` pip install boxmot ``` ##
+Yolov8 example  Click to expand!  Yolov8 model ```bash $ python examples/
+track.py --yolo-model yolov8n.pt # bboxes only yolov8n-seg.pt # bboxes +
+segmentation masks yolov8n-pose.pt # bboxes + pose estimation ```   Tracking
+methods ```bash $ python examples/track.py --tracking-method deepocsort
 strongsort ocsort bytetrack botsort ```   Tracking sources Tracking can be run
-on most video formats ```bash $ python track.py --source 0 # webcam img.jpg #
-image vid.mp4 # video path/ # directory path/*.jpg # glob 'https://youtu.be/
-Zgi9g1ksQHc' # YouTube 'rtsp://example.com/media.mp4' # RTSP, RTMP, HTTP stream
-```   Select Yolov8 model There is a clear trade-off between model inference
-speed and overall performance. In order to make it possible to fulfill your
-inference speed/accuracy needs you can select a Yolov5 family model for
-automatic download. These model can be further optimized for you needs by the
-[export.py](https://github.com/ultralytics/yolov5/blob/master/export.py) script
-```bash $ python track.py --source 0 --yolo-model yolov8n.pt --img 640
-yolov8s.tflite yolov8m.pt yolov8l.onnx yolov8x.pt --img 1280 ... ```   Select
-ReID model Some tracking methods combine appearance description and motion in
-the process of tracking. For those which use appearance, you can choose a ReID
-model based on your needs from this [ReID model zoo](https://
-kaiyangzhou.github.io/deep-person-reid/MODEL_ZOO). These model can be further
-optimized for you needs by the [reid_export.py](https://github.com/mikel-
-brostrom/Yolov5_StrongSORT_OSNet/blob/master/reid_export.py) script ```bash $
-python track.py --source 0 --reid-model lmbn_n_cuhk03_d.pt
-osnet_x0_25_market1501.pt mobilenetv2_x1_4_msmt17.engine resnet50_msmt17.onnx
-osnet_x1_0_msmt17.pt ... ```   Filter tracked classes By default the tracker
-tracks all MS COCO classes. If you want to track a subset of the classes that
-you model predicts, add their corresponding index after the classes flag,
-```bash python track.py --source 0 --yolo-model yolov8s.pt --classes 16 17 #
-COCO yolov8 model. Track cats and dogs, only ``` [Here](https://
-tech.amikelive.com/node-718/what-object-categories-labels-are-in-coco-dataset/
-) is a list of all the possible objects that a Yolov8 model trained on MS COCO
-can detect. Notice that the indexing for the classes in this repo starts at
-zero   MOT compliant results Can be saved to your experiment folder `runs/
-track/_/` by ```bash python track.py --source ... --save-txt ```   Tracker
-hyperparameter tuning We use a fast and elitist multiobjective genetic
-algorithm for tracker hyperparameter tuning. By default the objectives are:
-HOTA, MOTA, IDF1. Run it by ```bash $ python evolve.py --tracking-method
-strongsort --benchmark MOT17 --n-trials 100 # tune strongsort for MOT17 --
-tracking-method ocsort --benchmark  --objective HOTA # tune ocsort for
-maximizing HOTA on your custom tracking dataset ``` The set of hyperparameters
-leading to the best HOTA result are written to the tracker's config file.   ##
-Contact For Yolov8 tracking bugs and feature requests please visit [GitHub
-Issues](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/issues). For
-business inquiries or professional support requests please send an email to:
-yolov5.deepsort.pytorch@gmail.com
+on most video formats ```bash $ python examples/track.py --source 0 # webcam
+img.jpg # image vid.mp4 # video path/ # directory path/*.jpg # glob 'https://
+youtu.be/Zgi9g1ksQHc' # YouTube 'rtsp://example.com/media.mp4' # RTSP, RTMP,
+HTTP stream ```   Select Yolov8 model There is a clear trade-off between model
+inference speed and overall performance. In order to make it possible to
+fulfill your inference speed/accuracy needs you can select a Yolov5 family
+model for automatic download. These model can be further optimized for you
+needs by the [export.py](https://github.com/ultralytics/yolov5/blob/master/
+export.py) script ```bash $ python examples/track.py --source 0 --yolo-model
+yolov8n.pt --img 640 yolov8s.tflite yolov8m.pt yolov8l.onnx yolov8x.pt --img
+1280 ... ```   Select ReID model Some tracking methods combine appearance
+description and motion in the process of tracking. For those which use
+appearance, you can choose a ReID model based on your needs from this [ReID
+model zoo](https://kaiyangzhou.github.io/deep-person-reid/MODEL_ZOO). These
+model can be further optimized for you needs by the [reid_export.py](https://
+github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/blob/master/reid_export.py)
+script ```bash $ python examples/track.py --source 0 --reid-model
+lmbn_n_cuhk03_d.pt osnet_x0_25_market1501.pt mobilenetv2_x1_4_msmt17.engine
+resnet50_msmt17.onnx osnet_x1_0_msmt17.pt ... ```   Filter tracked classes By
+default the tracker tracks all MS COCO classes. If you want to track a subset
+of the classes that you model predicts, add their corresponding index after the
+classes flag, ```bash python examples/track.py --source 0 --yolo-model
+yolov8s.pt --classes 16 17 # COCO yolov8 model. Track cats and dogs, only ```
+[Here](https://tech.amikelive.com/node-718/what-object-categories-labels-are-
+in-coco-dataset/) is a list of all the possible objects that a Yolov8 model
+trained on MS COCO can detect. Notice that the indexing for the classes in this
+repo starts at zero   MOT compliant results Can be saved to your experiment
+folder `runs/track/_/` by ```bash python examples/track.py --source ... --save-
+txt ```   Tracker hyperparameter tuning We use a fast and elitist
+multiobjective genetic algorithm for tracker hyperparameter tuning. By default
+the objectives are: HOTA, MOTA, IDF1. Run it by ```bash $ python examples/
+evolve.py --tracking-method strongsort --benchmark MOT17 --n-trials 100 # tune
+strongsort for MOT17 --tracking-method ocsort --benchmark  --objective HOTA #
+tune ocsort for maximizing HOTA on your custom tracking dataset ``` The set of
+hyperparameters leading to the best HOTA result are written to the tracker's
+config file.   ## Custom object detection model example  Click to exapand!
+```python from boxmot import DeepOCSORT tracker = DeepOCSORT() cap =
+cv.VideoCapture(0) while True: ret, im = cap.read() ... # dets: # - your
+model's nms:ed outputs of shape Nx6 (x, y, x, y, conf, cls) # im: # - the
+original image (for better ReID results) # - the downscaled one fed to you
+model (faster) tracker_outputs = tracker.update(dets.cpu(), im) # --> (x, y, x,
+y, id, conf, cls) ... ```  ## Contact For Yolov8 tracking bugs and feature
+requests please visit [GitHub Issues](https://github.com/mikel-brostrom/
+Yolov5_StrongSORT_OSNet/issues). For business inquiries or professional support
+requests please send an email to: yolov5.deepsort.pytorch@gmail.com
```

### Comparing `boxmot-10.0.2/README.md` & `boxmot-10.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,44 +13,17 @@
 <a href="https://doi.org/10.5281/zenodo.7629840"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.7629840.svg" alt="DOI"></a>
   </div>
 </div>
 
 
 ## Introduction
 
-This repository contains a highly configurable two-stage-tracker that adjusts to different deployment scenarios. It can jointly perform multiple object tracking and instance segmentation (MOTS). The detections generated by [YOLOv8](https://github.com/ultralytics/ultralytics), a family of object detection architectures and models pretrained on the [COCO](https://arxiv.org/abs/1405.0312) dataset, are passed to the tracker of your choice. Supported ones at the moment are: [DeepOCSORT](https://arxiv.org/abs/2302.11813) [LightMBN](https://arxiv.org/pdf/2101.10774.pdf), [BoTSORT](https://arxiv.org/abs/2206.14651) [LightMBN](https://github.com/jixunbo/LightMBN)[](https://arxiv.org/pdf/2101.10774.pdf), [StrongSORT](https://github.com/dyhBUPT/StrongSORT)[](https://arxiv.org/abs/2202.13514) [LightMBN](https://github.com/jixunbo/LightMBN)[](https://arxiv.org/pdf/2101.10774.pdf), [OCSORT](https://github.com/noahcao/OC_SORT)[](https://arxiv.org/abs/2203.14360) and [ByteTrack](https://github.com/ifzhang/ByteTrack)[](https://arxiv.org/abs/2110.06864). They can track any object that your Yolov8 model was trained to detect.
+This repo contains a collections of state-of-the-art multi-object trackers. Some of them are based on motion only, others on motion + appearance description. For the latter, state-of-the-art ReID model are provided. Supported ones at the moment are: [DeepOCSORT](https://arxiv.org/abs/2302.11813) [LightMBN](https://arxiv.org/pdf/2101.10774.pdf), [BoTSORT](https://arxiv.org/abs/2206.14651) [LightMBN](https://github.com/jixunbo/LightMBN)[](https://arxiv.org/pdf/2101.10774.pdf), [StrongSORT](https://github.com/dyhBUPT/StrongSORT)[](https://arxiv.org/abs/2202.13514) [LightMBN](https://github.com/jixunbo/LightMBN)[](https://arxiv.org/pdf/2101.10774.pdf), [OCSORT](https://github.com/noahcao/OC_SORT)[](https://arxiv.org/abs/2203.14360) and [ByteTrack](https://github.com/ifzhang/ByteTrack)[](https://arxiv.org/abs/2110.06864).
 
-## Why using this tracking toolbox?
-
-Everything is designed with simplicity and flexibility in mind. We don't hyperfocus on results on a single dataset, we prioritize real-world results. If you don't get good tracking results on your custom dataset with the out-of-the-box tracker configurations, use the `evolve.py` script for tracker hyperparameter tuning.
-
-## Installation
-
-```
-pip install boxmot
-```
-
-## Custom model usage
-
-```python
-from boxmot import DeepOCSORT
-
-tracker = DeepOCSORT()
-cap = cv.VideoCapture(0)
-while True:
-    ret, im = cap.read()
-    ...
-    # dets: 
-    #  - your model's nms:ed outputs of shape Nx6 (x, y, x, y, conf, cls)
-    # im:
-    #  - the original image (for better ReID results)
-    #  - the downscaled one fed to you model
-    tracker_outputs = tracker.update(dets.cpu(), im)  # --> (x, y, x, y, id, conf, cls)
-    ...
-```
+We provide examples on how to use this package together with popular object detection models. Right now only [Yolov8](https://github.com/ultralytics) is available. Yolo-NAS & YOLOX coming soon.
 
 <details>
 <summary>Tutorials</summary>
 
 * [Yolov8 training (link to external repository)](https://docs.ultralytics.com/modes/train/)&nbsp;
 * [Deep appearance descriptor training (link to external repository)](https://kaiyangzhou.github.io/deep-person-reid/user_guide.html)&nbsp;
 * [ReID model export to ONNX, OpenVINO, TensorRT and TorchScript](https://github.com/mikel-brostrom/yolov8_tracking/wiki/ReID-multi-framework-model-export)&nbsp;
@@ -84,76 +57,82 @@
 * [Yolov5 StrongSORT OSNet vs other trackers MOT17](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/wiki/MOT-17-evaluation-(private-detector))&nbsp;
 
 * [StrongSORT MOT16 ablation study](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/wiki/Yolov5DeepSORTwithOSNet-vs-Yolov5StrongSORTwithOSNet-ablation-study-on-MOT16)&nbsp;
 
 * [Yolov5 StrongSORT OSNet vs other trackers MOT16 (deprecated)](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/wiki/MOT-16-evaluation)&nbsp;
 
   </details>
-  
-<details>
-<summary>Custom object detection architecture</summary>
 
-The trackers provided in this repo can be used with other object detectors than Yolov8. Make sure that the input to the trackers is of the following format:
+## Why using this tracking toolbox?
 
-```bash
-Nx6 (x, y, x, y, conf, cls)
+Everything is designed with simplicity and flexibility in mind. We don't hyperfocus on results on a single dataset, we prioritize real-world results. If you don't get good tracking results on your custom dataset with the out-of-the-box tracker configurations, use the `examples/evolve.py` script for tracker hyperparameter tuning.
+
+## Installation
+
+```
+pip install boxmot
 ```
 
-</details>
+## Yolov8 example
 
 <details>
-<summary>Tracking with Yolov8</summary>
+<summary>Click to expand!</summary>
+
+<details>
+<summary>Yolov8 model</summary>
   
 
 
 ```bash
-$ python track.py --yolo-model yolov8n.pt      # bboxes only
-                                 yolov8n-seg.pt  # bboxes + segmentation masks
-                                 yolov8n-pose.pt # bboxes + pose estimation
+$ python examples/track.py --yolo-model yolov8n.pt      # bboxes only
+                                        yolov8n-seg.pt  # bboxes + segmentation masks
+                                        yolov8n-pose.pt # bboxes + pose estimation
 ```
+  
+  </details>
 
 <details>
 <summary>Tracking methods</summary>
 
 ```bash
-$ python track.py --tracking-method deepocsort
-                                    strongsort
-                                    ocsort
-                                    bytetrack
-                                    botsort
+$ python examples/track.py --tracking-method deepocsort
+                                             strongsort
+                                             ocsort
+                                             bytetrack
+                                             botsort
 ```
   
 </details>
 
 <details>
 <summary>Tracking sources</summary>
 
 Tracking can be run on most video formats
 
 ```bash
-$ python track.py --source 0                               # webcam
-                           img.jpg                         # image
-                           vid.mp4                         # video
-                           path/                           # directory
-                           path/*.jpg                      # glob
-                           'https://youtu.be/Zgi9g1ksQHc'  # YouTube
-                           'rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP stream
+$ python examples/track.py --source 0                               # webcam
+                                    img.jpg                         # image
+                                    vid.mp4                         # video
+                                    path/                           # directory
+                                    path/*.jpg                      # glob
+                                    'https://youtu.be/Zgi9g1ksQHc'  # YouTube
+                                    'rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP stream
 ```
 
 </details>
 
 <details>
 <summary>Select Yolov8 model</summary>
 
 There is a clear trade-off between model inference speed and overall performance. In order to make it possible to fulfill your inference speed/accuracy needs you can select a Yolov5 family model for automatic download. These model can be further optimized for you needs by the [export.py](https://github.com/ultralytics/yolov5/blob/master/export.py) script
 
 ```bash
 
 
-$ python track.py --source 0 --yolo-model yolov8n.pt --img 640
+$ python examples/track.py --source 0 --yolo-model yolov8n.pt --img 640
                                           yolov8s.tflite
                                           yolov8m.pt
                                           yolov8l.onnx 
                                           yolov8x.pt --img 1280
                                           ...
 ```
   
@@ -161,63 +140,88 @@
 
 <details>
 <summary>Select ReID model</summary>
 
 Some tracking methods combine appearance description and motion in the process of tracking. For those which use appearance, you can choose a ReID model based on your needs from this [ReID model zoo](https://kaiyangzhou.github.io/deep-person-reid/MODEL_ZOO). These model can be further optimized for you needs by the [reid_export.py](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/blob/master/reid_export.py) script
 
 ```bash
-$ python track.py --source 0 --reid-model lmbn_n_cuhk03_d.pt
-                                          osnet_x0_25_market1501.pt
-                                          mobilenetv2_x1_4_msmt17.engine
-                                          resnet50_msmt17.onnx
-                                          osnet_x1_0_msmt17.pt
-                                          ...
+$ python examples/track.py --source 0 --reid-model lmbn_n_cuhk03_d.pt
+                                                   osnet_x0_25_market1501.pt
+                                                   mobilenetv2_x1_4_msmt17.engine
+                                                   resnet50_msmt17.onnx
+                                                   osnet_x1_0_msmt17.pt
+                                                   ...
 ```
 
 </details>
   
 <details>
 <summary>Filter tracked classes</summary>
 
 By default the tracker tracks all MS COCO classes.
 
 If you want to track a subset of the classes that you model predicts, add their corresponding index after the classes flag,
 
 ```bash
-python track.py --source 0 --yolo-model yolov8s.pt --classes 16 17  # COCO yolov8 model. Track cats and dogs, only
+python examples/track.py --source 0 --yolo-model yolov8s.pt --classes 16 17  # COCO yolov8 model. Track cats and dogs, only
 ```
 
 [Here](https://tech.amikelive.com/node-718/what-object-categories-labels-are-in-coco-dataset/) is a list of all the possible objects that a Yolov8 model trained on MS COCO can detect. Notice that the indexing for the classes in this repo starts at zero
 
 </details>
 
 <details>
 <summary>MOT compliant results</summary>
   
 Can be saved to your experiment folder `runs/track/<yolo_model>_<deep_sort_model>/` by 
 
 ```bash
-python track.py --source ... --save-txt
+python examples/track.py --source ... --save-txt
 ```
 
 </details>
 
 <details>
 <summary>Tracker hyperparameter tuning</summary>
 
 We use a fast and elitist multiobjective genetic algorithm for tracker hyperparameter tuning. By default the objectives are: HOTA, MOTA, IDF1. Run it by
 
 ```bash
-$ python evolve.py --tracking-method strongsort --benchmark MOT17 --n-trials 100  # tune strongsort for MOT17
-                   --tracking-method ocsort     --benchmark <your-custom-dataset> --objective HOTA # tune ocsort for maximizing HOTA on your custom tracking dataset
+$ python examples/evolve.py --tracking-method strongsort --benchmark MOT17 --n-trials 100  # tune strongsort for MOT17
+                            --tracking-method ocsort     --benchmark <your-custom-dataset> --objective HOTA # tune ocsort for maximizing HOTA on your custom tracking dataset
 ```
 
 The set of hyperparameters leading to the best HOTA result are written to the tracker's config file.
 
 </details>
   
 </details>
 
+## Custom object detection model example
+  
+<details>
+<summary>Click to exapand!</summary>
+
+```python
+from boxmot import DeepOCSORT
+
+tracker = DeepOCSORT()
+cap = cv.VideoCapture(0)
+while True:
+    ret, im = cap.read()
+    ...
+    # dets: 
+    #  - your model's nms:ed outputs of shape Nx6 (x, y, x, y, conf, cls)
+    # im:
+    #  - the original image (for better ReID results)
+    #  - the downscaled one fed to you model (faster)
+    tracker_outputs = tracker.update(dets.cpu(), im)  # --> (x, y, x, y, id, conf, cls)
+    ...
+```
+  
+</details>
+  
+
 ## Contact 
 
 For Yolov8 tracking bugs and feature requests please visit [GitHub Issues](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/issues). 
 For business inquiries or professional support requests please send an email to: yolov5.deepsort.pytorch@gmail.com
```

#### html2text {}

```diff
@@ -1,45 +1,33 @@
 # Real-time multi-object, segmentation and pose tracking using Yolov8 with
 DeepOCSORT and LightMBN
           [boxmot/strongsort/results/track_all_seg_1280_025conf.gif]
 
                                [CI_CPU_testing]
                              [Open_In_Colab] [DOI]
-## Introduction This repository contains a highly configurable two-stage-
-tracker that adjusts to different deployment scenarios. It can jointly perform
-multiple object tracking and instance segmentation (MOTS). The detections
-generated by [YOLOv8](https://github.com/ultralytics/ultralytics), a family of
-object detection architectures and models pretrained on the [COCO](https://
-arxiv.org/abs/1405.0312) dataset, are passed to the tracker of your choice.
-Supported ones at the moment are: [DeepOCSORT](https://arxiv.org/abs/
+## Introduction This repo contains a collections of state-of-the-art multi-
+object trackers. Some of them are based on motion only, others on motion +
+appearance description. For the latter, state-of-the-art ReID model are
+provided. Supported ones at the moment are: [DeepOCSORT](https://arxiv.org/abs/
 2302.11813) [LightMBN](https://arxiv.org/pdf/2101.10774.pdf), [BoTSORT](https:/
 /arxiv.org/abs/2206.14651) [LightMBN](https://github.com/jixunbo/LightMBN)[]
 (https://arxiv.org/pdf/2101.10774.pdf), [StrongSORT](https://github.com/
 dyhBUPT/StrongSORT)[](https://arxiv.org/abs/2202.13514) [LightMBN](https://
 github.com/jixunbo/LightMBN)[](https://arxiv.org/pdf/2101.10774.pdf), [OCSORT]
 (https://github.com/noahcao/OC_SORT)[](https://arxiv.org/abs/2203.14360) and
 [ByteTrack](https://github.com/ifzhang/ByteTrack)[](https://arxiv.org/abs/
-2110.06864). They can track any object that your Yolov8 model was trained to
-detect. ## Why using this tracking toolbox? Everything is designed with
-simplicity and flexibility in mind. We don't hyperfocus on results on a single
-dataset, we prioritize real-world results. If you don't get good tracking
-results on your custom dataset with the out-of-the-box tracker configurations,
-use the `evolve.py` script for tracker hyperparameter tuning. ## Installation
-``` pip install boxmot ``` ## Custom model usage ```python from boxmot import
-DeepOCSORT tracker = DeepOCSORT() cap = cv.VideoCapture(0) while True: ret, im
-= cap.read() ... # dets: # - your model's nms:ed outputs of shape Nx6 (x, y, x,
-y, conf, cls) # im: # - the original image (for better ReID results) # - the
-downscaled one fed to you model tracker_outputs = tracker.update(dets.cpu(),
-im) # --> (x, y, x, y, id, conf, cls) ... ```  Tutorials * [Yolov8 training
-(link to external repository)](https://docs.ultralytics.com/modes/train/)  *
-[Deep appearance descriptor training (link to external repository)](https://
-kaiyangzhou.github.io/deep-person-reid/user_guide.html)  * [ReID model export
-to ONNX, OpenVINO, TensorRT and TorchScript](https://github.com/mikel-brostrom/
-yolov8_tracking/wiki/ReID-multi-framework-model-export)  * [Evaluation on
-custom tracking dataset](https://github.com/mikel-brostrom/yolov8_tracking/
+2110.06864). We provide examples on how to use this package together with
+popular object detection models. Right now only [Yolov8](https://github.com/
+ultralytics) is available. Yolo-NAS & YOLOX coming soon.  Tutorials * [Yolov8
+training (link to external repository)](https://docs.ultralytics.com/modes/
+train/)  * [Deep appearance descriptor training (link to external repository)]
+(https://kaiyangzhou.github.io/deep-person-reid/user_guide.html)  * [ReID model
+export to ONNX, OpenVINO, TensorRT and TorchScript](https://github.com/mikel-
+brostrom/yolov8_tracking/wiki/ReID-multi-framework-model-export)  * [Evaluation
+on custom tracking dataset](https://github.com/mikel-brostrom/yolov8_tracking/
 wiki/How-to-evaluate-on-custom-tracking-dataset)  * [ReID inference
 acceleration with Nebullvm](https://colab.research.google.com/drive/
 1APUZ1ijCiQFBR9xD0gUvFUOC8yOJIvHm?usp=sharing)    Experiments In inverse
 chronological order: * [Evaluation of the params evolved for first half of
 MOT17 on the complete MOT17](https://github.com/mikel-brostrom/
 Yolov5_StrongSORT_OSNet/wiki/Evaluation-of-the-params-evolved-for-first-half-
 of-MOT17-on-the-complete-MOT17) * [Segmentation model vs object detetion model
@@ -63,54 +51,63 @@
 brostrom/Yolov5_StrongSORT_OSNet/tree/botsort * [Yolov5 StrongSORT OSNet vs
 other trackers MOT17](https://github.com/mikel-brostrom/
 Yolov5_StrongSORT_OSNet/wiki/MOT-17-evaluation-(private-detector))  *
 [StrongSORT MOT16 ablation study](https://github.com/mikel-brostrom/
 Yolov5_StrongSORT_OSNet/wiki/Yolov5DeepSORTwithOSNet-vs-
 Yolov5StrongSORTwithOSNet-ablation-study-on-MOT16)  * [Yolov5 StrongSORT OSNet
 vs other trackers MOT16 (deprecated)](https://github.com/mikel-brostrom/
-Yolov5_StrongSORT_OSNet/wiki/MOT-16-evaluation)    Custom object detection
-architecture The trackers provided in this repo can be used with other object
-detectors than Yolov8. Make sure that the input to the trackers is of the
-following format: ```bash Nx6 (x, y, x, y, conf, cls) ```   Tracking with
-Yolov8 ```bash $ python track.py --yolo-model yolov8n.pt # bboxes only yolov8n-
-seg.pt # bboxes + segmentation masks yolov8n-pose.pt # bboxes + pose estimation
-```  Tracking methods ```bash $ python track.py --tracking-method deepocsort
+Yolov5_StrongSORT_OSNet/wiki/MOT-16-evaluation)   ## Why using this tracking
+toolbox? Everything is designed with simplicity and flexibility in mind. We
+don't hyperfocus on results on a single dataset, we prioritize real-world
+results. If you don't get good tracking results on your custom dataset with the
+out-of-the-box tracker configurations, use the `examples/evolve.py` script for
+tracker hyperparameter tuning. ## Installation ``` pip install boxmot ``` ##
+Yolov8 example  Click to expand!  Yolov8 model ```bash $ python examples/
+track.py --yolo-model yolov8n.pt # bboxes only yolov8n-seg.pt # bboxes +
+segmentation masks yolov8n-pose.pt # bboxes + pose estimation ```   Tracking
+methods ```bash $ python examples/track.py --tracking-method deepocsort
 strongsort ocsort bytetrack botsort ```   Tracking sources Tracking can be run
-on most video formats ```bash $ python track.py --source 0 # webcam img.jpg #
-image vid.mp4 # video path/ # directory path/*.jpg # glob 'https://youtu.be/
-Zgi9g1ksQHc' # YouTube 'rtsp://example.com/media.mp4' # RTSP, RTMP, HTTP stream
-```   Select Yolov8 model There is a clear trade-off between model inference
-speed and overall performance. In order to make it possible to fulfill your
-inference speed/accuracy needs you can select a Yolov5 family model for
-automatic download. These model can be further optimized for you needs by the
-[export.py](https://github.com/ultralytics/yolov5/blob/master/export.py) script
-```bash $ python track.py --source 0 --yolo-model yolov8n.pt --img 640
-yolov8s.tflite yolov8m.pt yolov8l.onnx yolov8x.pt --img 1280 ... ```   Select
-ReID model Some tracking methods combine appearance description and motion in
-the process of tracking. For those which use appearance, you can choose a ReID
-model based on your needs from this [ReID model zoo](https://
-kaiyangzhou.github.io/deep-person-reid/MODEL_ZOO). These model can be further
-optimized for you needs by the [reid_export.py](https://github.com/mikel-
-brostrom/Yolov5_StrongSORT_OSNet/blob/master/reid_export.py) script ```bash $
-python track.py --source 0 --reid-model lmbn_n_cuhk03_d.pt
-osnet_x0_25_market1501.pt mobilenetv2_x1_4_msmt17.engine resnet50_msmt17.onnx
-osnet_x1_0_msmt17.pt ... ```   Filter tracked classes By default the tracker
-tracks all MS COCO classes. If you want to track a subset of the classes that
-you model predicts, add their corresponding index after the classes flag,
-```bash python track.py --source 0 --yolo-model yolov8s.pt --classes 16 17 #
-COCO yolov8 model. Track cats and dogs, only ``` [Here](https://
-tech.amikelive.com/node-718/what-object-categories-labels-are-in-coco-dataset/
-) is a list of all the possible objects that a Yolov8 model trained on MS COCO
-can detect. Notice that the indexing for the classes in this repo starts at
-zero   MOT compliant results Can be saved to your experiment folder `runs/
-track/_/` by ```bash python track.py --source ... --save-txt ```   Tracker
-hyperparameter tuning We use a fast and elitist multiobjective genetic
-algorithm for tracker hyperparameter tuning. By default the objectives are:
-HOTA, MOTA, IDF1. Run it by ```bash $ python evolve.py --tracking-method
-strongsort --benchmark MOT17 --n-trials 100 # tune strongsort for MOT17 --
-tracking-method ocsort --benchmark  --objective HOTA # tune ocsort for
-maximizing HOTA on your custom tracking dataset ``` The set of hyperparameters
-leading to the best HOTA result are written to the tracker's config file.   ##
-Contact For Yolov8 tracking bugs and feature requests please visit [GitHub
-Issues](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/issues). For
-business inquiries or professional support requests please send an email to:
-yolov5.deepsort.pytorch@gmail.com
+on most video formats ```bash $ python examples/track.py --source 0 # webcam
+img.jpg # image vid.mp4 # video path/ # directory path/*.jpg # glob 'https://
+youtu.be/Zgi9g1ksQHc' # YouTube 'rtsp://example.com/media.mp4' # RTSP, RTMP,
+HTTP stream ```   Select Yolov8 model There is a clear trade-off between model
+inference speed and overall performance. In order to make it possible to
+fulfill your inference speed/accuracy needs you can select a Yolov5 family
+model for automatic download. These model can be further optimized for you
+needs by the [export.py](https://github.com/ultralytics/yolov5/blob/master/
+export.py) script ```bash $ python examples/track.py --source 0 --yolo-model
+yolov8n.pt --img 640 yolov8s.tflite yolov8m.pt yolov8l.onnx yolov8x.pt --img
+1280 ... ```   Select ReID model Some tracking methods combine appearance
+description and motion in the process of tracking. For those which use
+appearance, you can choose a ReID model based on your needs from this [ReID
+model zoo](https://kaiyangzhou.github.io/deep-person-reid/MODEL_ZOO). These
+model can be further optimized for you needs by the [reid_export.py](https://
+github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/blob/master/reid_export.py)
+script ```bash $ python examples/track.py --source 0 --reid-model
+lmbn_n_cuhk03_d.pt osnet_x0_25_market1501.pt mobilenetv2_x1_4_msmt17.engine
+resnet50_msmt17.onnx osnet_x1_0_msmt17.pt ... ```   Filter tracked classes By
+default the tracker tracks all MS COCO classes. If you want to track a subset
+of the classes that you model predicts, add their corresponding index after the
+classes flag, ```bash python examples/track.py --source 0 --yolo-model
+yolov8s.pt --classes 16 17 # COCO yolov8 model. Track cats and dogs, only ```
+[Here](https://tech.amikelive.com/node-718/what-object-categories-labels-are-
+in-coco-dataset/) is a list of all the possible objects that a Yolov8 model
+trained on MS COCO can detect. Notice that the indexing for the classes in this
+repo starts at zero   MOT compliant results Can be saved to your experiment
+folder `runs/track/_/` by ```bash python examples/track.py --source ... --save-
+txt ```   Tracker hyperparameter tuning We use a fast and elitist
+multiobjective genetic algorithm for tracker hyperparameter tuning. By default
+the objectives are: HOTA, MOTA, IDF1. Run it by ```bash $ python examples/
+evolve.py --tracking-method strongsort --benchmark MOT17 --n-trials 100 # tune
+strongsort for MOT17 --tracking-method ocsort --benchmark  --objective HOTA #
+tune ocsort for maximizing HOTA on your custom tracking dataset ``` The set of
+hyperparameters leading to the best HOTA result are written to the tracker's
+config file.   ## Custom object detection model example  Click to exapand!
+```python from boxmot import DeepOCSORT tracker = DeepOCSORT() cap =
+cv.VideoCapture(0) while True: ret, im = cap.read() ... # dets: # - your
+model's nms:ed outputs of shape Nx6 (x, y, x, y, conf, cls) # im: # - the
+original image (for better ReID results) # - the downscaled one fed to you
+model (faster) tracker_outputs = tracker.update(dets.cpu(), im) # --> (x, y, x,
+y, id, conf, cls) ... ```  ## Contact For Yolov8 tracking bugs and feature
+requests please visit [GitHub Issues](https://github.com/mikel-brostrom/
+Yolov5_StrongSORT_OSNet/issues). For business inquiries or professional support
+requests please send an email to: yolov5.deepsort.pytorch@gmail.com
```

### Comparing `boxmot-10.0.2/boxmot/__init__.py` & `boxmot-10.0.3/boxmot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '10.0.2'
+__version__ = '10.0.3'
 
 from pathlib import Path
 
 from boxmot.strongsort.strong_sort import StrongSORT
 from boxmot.ocsort.ocsort import OCSort as OCSORT
 from boxmot.bytetrack.byte_tracker import BYTETracker
 from boxmot.botsort.bot_sort import BoTSORT
```

### Comparing `boxmot-10.0.2/boxmot/botsort/basetrack.py` & `boxmot-10.0.3/boxmot/botsort/basetrack.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/botsort/bot_sort.py` & `boxmot-10.0.3/boxmot/botsort/bot_sort.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/botsort/gmc.py` & `boxmot-10.0.3/boxmot/botsort/gmc.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/botsort/kalman_filter.py` & `boxmot-10.0.3/boxmot/botsort/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/botsort/matching.py` & `boxmot-10.0.3/boxmot/botsort/matching.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/bytetrack/basetrack.py` & `boxmot-10.0.3/boxmot/bytetrack/basetrack.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/bytetrack/byte_tracker.py` & `boxmot-10.0.3/boxmot/bytetrack/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/bytetrack/kalman_filter.py` & `boxmot-10.0.3/boxmot/bytetrack/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/bytetrack/matching.py` & `boxmot-10.0.3/boxmot/bytetrack/matching.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/__init__.py` & `boxmot-10.0.3/boxmot/deep/models/__init__.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/attention.py` & `boxmot-10.0.3/boxmot/deep/models/attention.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/bnneck.py` & `boxmot-10.0.3/boxmot/deep/models/bnneck.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/densenet.py` & `boxmot-10.0.3/boxmot/deep/models/densenet.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/hacnn.py` & `boxmot-10.0.3/boxmot/deep/models/hacnn.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/inceptionresnetv2.py` & `boxmot-10.0.3/boxmot/deep/models/inceptionresnetv2.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/inceptionv4.py` & `boxmot-10.0.3/boxmot/deep/models/inceptionv4.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/lmbn_n.py` & `boxmot-10.0.3/boxmot/deep/models/lmbn_n.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/mlfn.py` & `boxmot-10.0.3/boxmot/deep/models/mlfn.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/mobilenetv2.py` & `boxmot-10.0.3/boxmot/deep/models/mobilenetv2.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/mudeep.py` & `boxmot-10.0.3/boxmot/deep/models/mudeep.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/nasnet.py` & `boxmot-10.0.3/boxmot/deep/models/nasnet.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/osnet.py` & `boxmot-10.0.3/boxmot/deep/models/osnet.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/osnet_ain.py` & `boxmot-10.0.3/boxmot/deep/models/osnet_ain.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/pcb.py` & `boxmot-10.0.3/boxmot/deep/models/pcb.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/resnet.py` & `boxmot-10.0.3/boxmot/deep/models/resnet.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/resnet_ibn_a.py` & `boxmot-10.0.3/boxmot/deep/models/resnet_ibn_a.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/resnet_ibn_b.py` & `boxmot-10.0.3/boxmot/deep/models/resnet_ibn_b.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/resnetmid.py` & `boxmot-10.0.3/boxmot/deep/models/resnetmid.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/senet.py` & `boxmot-10.0.3/boxmot/deep/models/senet.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/shufflenet.py` & `boxmot-10.0.3/boxmot/deep/models/shufflenet.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/shufflenetv2.py` & `boxmot-10.0.3/boxmot/deep/models/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/squeezenet.py` & `boxmot-10.0.3/boxmot/deep/models/squeezenet.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/models/xception.py` & `boxmot-10.0.3/boxmot/deep/models/xception.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/reid_export.py` & `boxmot-10.0.3/boxmot/deep/reid_export.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/reid_model_factory.py` & `boxmot-10.0.3/boxmot/deep/reid_model_factory.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deep/reid_multibackend.py` & `boxmot-10.0.3/boxmot/deep/reid_multibackend.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deepocsort/args.py` & `boxmot-10.0.3/boxmot/deepocsort/args.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deepocsort/association.py` & `boxmot-10.0.3/boxmot/deepocsort/association.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deepocsort/cmc.py` & `boxmot-10.0.3/boxmot/deepocsort/cmc.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deepocsort/embedding.py` & `boxmot-10.0.3/boxmot/deepocsort/embedding.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deepocsort/kalmanfilter.py` & `boxmot-10.0.3/boxmot/deepocsort/kalmanfilter.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/deepocsort/ocsort.py` & `boxmot-10.0.3/boxmot/deepocsort/ocsort.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/ocsort/association.py` & `boxmot-10.0.3/boxmot/ocsort/association.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/ocsort/kalmanfilter.py` & `boxmot-10.0.3/boxmot/ocsort/kalmanfilter.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/ocsort/ocsort.py` & `boxmot-10.0.3/boxmot/ocsort/ocsort.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/strongsort/sort/detection.py` & `boxmot-10.0.3/boxmot/strongsort/sort/detection.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/strongsort/sort/iou_matching.py` & `boxmot-10.0.3/boxmot/strongsort/sort/iou_matching.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/strongsort/sort/kalman_filter.py` & `boxmot-10.0.3/boxmot/strongsort/sort/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/strongsort/sort/linear_assignment.py` & `boxmot-10.0.3/boxmot/strongsort/sort/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/strongsort/sort/nn_matching.py` & `boxmot-10.0.3/boxmot/strongsort/sort/nn_matching.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/strongsort/sort/preprocessing.py` & `boxmot-10.0.3/boxmot/strongsort/sort/preprocessing.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/strongsort/sort/track.py` & `boxmot-10.0.3/boxmot/strongsort/sort/track.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/strongsort/sort/tracker.py` & `boxmot-10.0.3/boxmot/strongsort/sort/tracker.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/strongsort/strong_sort.py` & `boxmot-10.0.3/boxmot/strongsort/strong_sort.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/strongsort/utils/draw.py` & `boxmot-10.0.3/boxmot/strongsort/utils/draw.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/strongsort/utils/evaluation.py` & `boxmot-10.0.3/boxmot/strongsort/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/strongsort/utils/io.py` & `boxmot-10.0.3/boxmot/strongsort/utils/io.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/strongsort/utils/json_logger.py` & `boxmot-10.0.3/boxmot/strongsort/utils/json_logger.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/strongsort/utils/parser.py` & `boxmot-10.0.3/boxmot/strongsort/utils/parser.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/strongsort/utils/tools.py` & `boxmot-10.0.3/boxmot/strongsort/utils/tools.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot/tracker_zoo.py` & `boxmot-10.0.3/boxmot/tracker_zoo.py`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/boxmot.egg-info/PKG-INFO` & `boxmot-10.0.3/boxmot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxmot
-Version: 10.0.2
+Version: 10.0.3
 Summary: SOTA tracking methods for detection, segmentation and pose estimation models.
 Home-page: https://github.com/mikel-brostrom/yolov8_tracking
 Author: Mikel Brostrom
 Author-email: yolov5.deepsort.pytorch@gmail.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/mikel-brostrom/yolov8_tracking/issues
 Project-URL: Source, https://github.com/mikel-brostrom/yolov8_tracking
@@ -46,44 +46,17 @@
 <a href="https://doi.org/10.5281/zenodo.7629840"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.7629840.svg" alt="DOI"></a>
   </div>
 </div>
 
 
 ## Introduction
 
-This repository contains a highly configurable two-stage-tracker that adjusts to different deployment scenarios. It can jointly perform multiple object tracking and instance segmentation (MOTS). The detections generated by [YOLOv8](https://github.com/ultralytics/ultralytics), a family of object detection architectures and models pretrained on the [COCO](https://arxiv.org/abs/1405.0312) dataset, are passed to the tracker of your choice. Supported ones at the moment are: [DeepOCSORT](https://arxiv.org/abs/2302.11813) [LightMBN](https://arxiv.org/pdf/2101.10774.pdf), [BoTSORT](https://arxiv.org/abs/2206.14651) [LightMBN](https://github.com/jixunbo/LightMBN)[](https://arxiv.org/pdf/2101.10774.pdf), [StrongSORT](https://github.com/dyhBUPT/StrongSORT)[](https://arxiv.org/abs/2202.13514) [LightMBN](https://github.com/jixunbo/LightMBN)[](https://arxiv.org/pdf/2101.10774.pdf), [OCSORT](https://github.com/noahcao/OC_SORT)[](https://arxiv.org/abs/2203.14360) and [ByteTrack](https://github.com/ifzhang/ByteTrack)[](https://arxiv.org/abs/2110.06864). They can track any object that your Yolov8 model was trained to detect.
+This repo contains a collections of state-of-the-art multi-object trackers. Some of them are based on motion only, others on motion + appearance description. For the latter, state-of-the-art ReID model are provided. Supported ones at the moment are: [DeepOCSORT](https://arxiv.org/abs/2302.11813) [LightMBN](https://arxiv.org/pdf/2101.10774.pdf), [BoTSORT](https://arxiv.org/abs/2206.14651) [LightMBN](https://github.com/jixunbo/LightMBN)[](https://arxiv.org/pdf/2101.10774.pdf), [StrongSORT](https://github.com/dyhBUPT/StrongSORT)[](https://arxiv.org/abs/2202.13514) [LightMBN](https://github.com/jixunbo/LightMBN)[](https://arxiv.org/pdf/2101.10774.pdf), [OCSORT](https://github.com/noahcao/OC_SORT)[](https://arxiv.org/abs/2203.14360) and [ByteTrack](https://github.com/ifzhang/ByteTrack)[](https://arxiv.org/abs/2110.06864).
 
-## Why using this tracking toolbox?
-
-Everything is designed with simplicity and flexibility in mind. We don't hyperfocus on results on a single dataset, we prioritize real-world results. If you don't get good tracking results on your custom dataset with the out-of-the-box tracker configurations, use the `evolve.py` script for tracker hyperparameter tuning.
-
-## Installation
-
-```
-pip install boxmot
-```
-
-## Custom model usage
-
-```python
-from boxmot import DeepOCSORT
-
-tracker = DeepOCSORT()
-cap = cv.VideoCapture(0)
-while True:
-    ret, im = cap.read()
-    ...
-    # dets: 
-    #  - your model's nms:ed outputs of shape Nx6 (x, y, x, y, conf, cls)
-    # im:
-    #  - the original image (for better ReID results)
-    #  - the downscaled one fed to you model
-    tracker_outputs = tracker.update(dets.cpu(), im)  # --> (x, y, x, y, id, conf, cls)
-    ...
-```
+We provide examples on how to use this package together with popular object detection models. Right now only [Yolov8](https://github.com/ultralytics) is available. Yolo-NAS & YOLOX coming soon.
 
 <details>
 <summary>Tutorials</summary>
 
 * [Yolov8 training (link to external repository)](https://docs.ultralytics.com/modes/train/)&nbsp;
 * [Deep appearance descriptor training (link to external repository)](https://kaiyangzhou.github.io/deep-person-reid/user_guide.html)&nbsp;
 * [ReID model export to ONNX, OpenVINO, TensorRT and TorchScript](https://github.com/mikel-brostrom/yolov8_tracking/wiki/ReID-multi-framework-model-export)&nbsp;
@@ -117,76 +90,82 @@
 * [Yolov5 StrongSORT OSNet vs other trackers MOT17](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/wiki/MOT-17-evaluation-(private-detector))&nbsp;
 
 * [StrongSORT MOT16 ablation study](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/wiki/Yolov5DeepSORTwithOSNet-vs-Yolov5StrongSORTwithOSNet-ablation-study-on-MOT16)&nbsp;
 
 * [Yolov5 StrongSORT OSNet vs other trackers MOT16 (deprecated)](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/wiki/MOT-16-evaluation)&nbsp;
 
   </details>
-  
-<details>
-<summary>Custom object detection architecture</summary>
 
-The trackers provided in this repo can be used with other object detectors than Yolov8. Make sure that the input to the trackers is of the following format:
+## Why using this tracking toolbox?
 
-```bash
-Nx6 (x, y, x, y, conf, cls)
+Everything is designed with simplicity and flexibility in mind. We don't hyperfocus on results on a single dataset, we prioritize real-world results. If you don't get good tracking results on your custom dataset with the out-of-the-box tracker configurations, use the `examples/evolve.py` script for tracker hyperparameter tuning.
+
+## Installation
+
+```
+pip install boxmot
 ```
 
-</details>
+## Yolov8 example
 
 <details>
-<summary>Tracking with Yolov8</summary>
+<summary>Click to expand!</summary>
+
+<details>
+<summary>Yolov8 model</summary>
   
 
 
 ```bash
-$ python track.py --yolo-model yolov8n.pt      # bboxes only
-                                 yolov8n-seg.pt  # bboxes + segmentation masks
-                                 yolov8n-pose.pt # bboxes + pose estimation
+$ python examples/track.py --yolo-model yolov8n.pt      # bboxes only
+                                        yolov8n-seg.pt  # bboxes + segmentation masks
+                                        yolov8n-pose.pt # bboxes + pose estimation
 ```
+  
+  </details>
 
 <details>
 <summary>Tracking methods</summary>
 
 ```bash
-$ python track.py --tracking-method deepocsort
-                                    strongsort
-                                    ocsort
-                                    bytetrack
-                                    botsort
+$ python examples/track.py --tracking-method deepocsort
+                                             strongsort
+                                             ocsort
+                                             bytetrack
+                                             botsort
 ```
   
 </details>
 
 <details>
 <summary>Tracking sources</summary>
 
 Tracking can be run on most video formats
 
 ```bash
-$ python track.py --source 0                               # webcam
-                           img.jpg                         # image
-                           vid.mp4                         # video
-                           path/                           # directory
-                           path/*.jpg                      # glob
-                           'https://youtu.be/Zgi9g1ksQHc'  # YouTube
-                           'rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP stream
+$ python examples/track.py --source 0                               # webcam
+                                    img.jpg                         # image
+                                    vid.mp4                         # video
+                                    path/                           # directory
+                                    path/*.jpg                      # glob
+                                    'https://youtu.be/Zgi9g1ksQHc'  # YouTube
+                                    'rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP stream
 ```
 
 </details>
 
 <details>
 <summary>Select Yolov8 model</summary>
 
 There is a clear trade-off between model inference speed and overall performance. In order to make it possible to fulfill your inference speed/accuracy needs you can select a Yolov5 family model for automatic download. These model can be further optimized for you needs by the [export.py](https://github.com/ultralytics/yolov5/blob/master/export.py) script
 
 ```bash
 
 
-$ python track.py --source 0 --yolo-model yolov8n.pt --img 640
+$ python examples/track.py --source 0 --yolo-model yolov8n.pt --img 640
                                           yolov8s.tflite
                                           yolov8m.pt
                                           yolov8l.onnx 
                                           yolov8x.pt --img 1280
                                           ...
 ```
   
@@ -194,63 +173,88 @@
 
 <details>
 <summary>Select ReID model</summary>
 
 Some tracking methods combine appearance description and motion in the process of tracking. For those which use appearance, you can choose a ReID model based on your needs from this [ReID model zoo](https://kaiyangzhou.github.io/deep-person-reid/MODEL_ZOO). These model can be further optimized for you needs by the [reid_export.py](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/blob/master/reid_export.py) script
 
 ```bash
-$ python track.py --source 0 --reid-model lmbn_n_cuhk03_d.pt
-                                          osnet_x0_25_market1501.pt
-                                          mobilenetv2_x1_4_msmt17.engine
-                                          resnet50_msmt17.onnx
-                                          osnet_x1_0_msmt17.pt
-                                          ...
+$ python examples/track.py --source 0 --reid-model lmbn_n_cuhk03_d.pt
+                                                   osnet_x0_25_market1501.pt
+                                                   mobilenetv2_x1_4_msmt17.engine
+                                                   resnet50_msmt17.onnx
+                                                   osnet_x1_0_msmt17.pt
+                                                   ...
 ```
 
 </details>
   
 <details>
 <summary>Filter tracked classes</summary>
 
 By default the tracker tracks all MS COCO classes.
 
 If you want to track a subset of the classes that you model predicts, add their corresponding index after the classes flag,
 
 ```bash
-python track.py --source 0 --yolo-model yolov8s.pt --classes 16 17  # COCO yolov8 model. Track cats and dogs, only
+python examples/track.py --source 0 --yolo-model yolov8s.pt --classes 16 17  # COCO yolov8 model. Track cats and dogs, only
 ```
 
 [Here](https://tech.amikelive.com/node-718/what-object-categories-labels-are-in-coco-dataset/) is a list of all the possible objects that a Yolov8 model trained on MS COCO can detect. Notice that the indexing for the classes in this repo starts at zero
 
 </details>
 
 <details>
 <summary>MOT compliant results</summary>
   
 Can be saved to your experiment folder `runs/track/<yolo_model>_<deep_sort_model>/` by 
 
 ```bash
-python track.py --source ... --save-txt
+python examples/track.py --source ... --save-txt
 ```
 
 </details>
 
 <details>
 <summary>Tracker hyperparameter tuning</summary>
 
 We use a fast and elitist multiobjective genetic algorithm for tracker hyperparameter tuning. By default the objectives are: HOTA, MOTA, IDF1. Run it by
 
 ```bash
-$ python evolve.py --tracking-method strongsort --benchmark MOT17 --n-trials 100  # tune strongsort for MOT17
-                   --tracking-method ocsort     --benchmark <your-custom-dataset> --objective HOTA # tune ocsort for maximizing HOTA on your custom tracking dataset
+$ python examples/evolve.py --tracking-method strongsort --benchmark MOT17 --n-trials 100  # tune strongsort for MOT17
+                            --tracking-method ocsort     --benchmark <your-custom-dataset> --objective HOTA # tune ocsort for maximizing HOTA on your custom tracking dataset
 ```
 
 The set of hyperparameters leading to the best HOTA result are written to the tracker's config file.
 
 </details>
   
 </details>
 
+## Custom object detection model example
+  
+<details>
+<summary>Click to exapand!</summary>
+
+```python
+from boxmot import DeepOCSORT
+
+tracker = DeepOCSORT()
+cap = cv.VideoCapture(0)
+while True:
+    ret, im = cap.read()
+    ...
+    # dets: 
+    #  - your model's nms:ed outputs of shape Nx6 (x, y, x, y, conf, cls)
+    # im:
+    #  - the original image (for better ReID results)
+    #  - the downscaled one fed to you model (faster)
+    tracker_outputs = tracker.update(dets.cpu(), im)  # --> (x, y, x, y, id, conf, cls)
+    ...
+```
+  
+</details>
+  
+
 ## Contact 
 
 For Yolov8 tracking bugs and feature requests please visit [GitHub Issues](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/issues). 
 For business inquiries or professional support requests please send an email to: yolov5.deepsort.pytorch@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: boxmot Version: 10.0.2 Summary: SOTA tracking
+Metadata-Version: 2.1 Name: boxmot Version: 10.0.3 Summary: SOTA tracking
 methods for detection, segmentation and pose estimation models. Home-page:
 https://github.com/mikel-brostrom/yolov8_tracking Author: Mikel Brostrom
 Author-email: yolov5.deepsort.pytorch@gmail.com License: AGPL-3.0 Project-URL:
 Bug Reports, https://github.com/mikel-brostrom/yolov8_tracking/issues Project-
 URL: Source, https://github.com/mikel-brostrom/yolov8_tracking Keywords:
 machine-learning,deep-learning,vision,ML,DL,AI,YOLO Platform: linux Platform:
 windows Classifier: Development Status :: 3 - Alpha Classifier: Intended
@@ -19,46 +19,34 @@
 Engineering :: Image Processing Requires-Python: >=3.7 Description-Content-
 Type: text/markdown License-File: LICENSE # Real-time multi-object,
 segmentation and pose tracking using Yolov8 with DeepOCSORT and LightMBN
           [boxmot/strongsort/results/track_all_seg_1280_025conf.gif]
 
                                [CI_CPU_testing]
                              [Open_In_Colab] [DOI]
-## Introduction This repository contains a highly configurable two-stage-
-tracker that adjusts to different deployment scenarios. It can jointly perform
-multiple object tracking and instance segmentation (MOTS). The detections
-generated by [YOLOv8](https://github.com/ultralytics/ultralytics), a family of
-object detection architectures and models pretrained on the [COCO](https://
-arxiv.org/abs/1405.0312) dataset, are passed to the tracker of your choice.
-Supported ones at the moment are: [DeepOCSORT](https://arxiv.org/abs/
+## Introduction This repo contains a collections of state-of-the-art multi-
+object trackers. Some of them are based on motion only, others on motion +
+appearance description. For the latter, state-of-the-art ReID model are
+provided. Supported ones at the moment are: [DeepOCSORT](https://arxiv.org/abs/
 2302.11813) [LightMBN](https://arxiv.org/pdf/2101.10774.pdf), [BoTSORT](https:/
 /arxiv.org/abs/2206.14651) [LightMBN](https://github.com/jixunbo/LightMBN)[]
 (https://arxiv.org/pdf/2101.10774.pdf), [StrongSORT](https://github.com/
 dyhBUPT/StrongSORT)[](https://arxiv.org/abs/2202.13514) [LightMBN](https://
 github.com/jixunbo/LightMBN)[](https://arxiv.org/pdf/2101.10774.pdf), [OCSORT]
 (https://github.com/noahcao/OC_SORT)[](https://arxiv.org/abs/2203.14360) and
 [ByteTrack](https://github.com/ifzhang/ByteTrack)[](https://arxiv.org/abs/
-2110.06864). They can track any object that your Yolov8 model was trained to
-detect. ## Why using this tracking toolbox? Everything is designed with
-simplicity and flexibility in mind. We don't hyperfocus on results on a single
-dataset, we prioritize real-world results. If you don't get good tracking
-results on your custom dataset with the out-of-the-box tracker configurations,
-use the `evolve.py` script for tracker hyperparameter tuning. ## Installation
-``` pip install boxmot ``` ## Custom model usage ```python from boxmot import
-DeepOCSORT tracker = DeepOCSORT() cap = cv.VideoCapture(0) while True: ret, im
-= cap.read() ... # dets: # - your model's nms:ed outputs of shape Nx6 (x, y, x,
-y, conf, cls) # im: # - the original image (for better ReID results) # - the
-downscaled one fed to you model tracker_outputs = tracker.update(dets.cpu(),
-im) # --> (x, y, x, y, id, conf, cls) ... ```  Tutorials * [Yolov8 training
-(link to external repository)](https://docs.ultralytics.com/modes/train/)  *
-[Deep appearance descriptor training (link to external repository)](https://
-kaiyangzhou.github.io/deep-person-reid/user_guide.html)  * [ReID model export
-to ONNX, OpenVINO, TensorRT and TorchScript](https://github.com/mikel-brostrom/
-yolov8_tracking/wiki/ReID-multi-framework-model-export)  * [Evaluation on
-custom tracking dataset](https://github.com/mikel-brostrom/yolov8_tracking/
+2110.06864). We provide examples on how to use this package together with
+popular object detection models. Right now only [Yolov8](https://github.com/
+ultralytics) is available. Yolo-NAS & YOLOX coming soon.  Tutorials * [Yolov8
+training (link to external repository)](https://docs.ultralytics.com/modes/
+train/)  * [Deep appearance descriptor training (link to external repository)]
+(https://kaiyangzhou.github.io/deep-person-reid/user_guide.html)  * [ReID model
+export to ONNX, OpenVINO, TensorRT and TorchScript](https://github.com/mikel-
+brostrom/yolov8_tracking/wiki/ReID-multi-framework-model-export)  * [Evaluation
+on custom tracking dataset](https://github.com/mikel-brostrom/yolov8_tracking/
 wiki/How-to-evaluate-on-custom-tracking-dataset)  * [ReID inference
 acceleration with Nebullvm](https://colab.research.google.com/drive/
 1APUZ1ijCiQFBR9xD0gUvFUOC8yOJIvHm?usp=sharing)    Experiments In inverse
 chronological order: * [Evaluation of the params evolved for first half of
 MOT17 on the complete MOT17](https://github.com/mikel-brostrom/
 Yolov5_StrongSORT_OSNet/wiki/Evaluation-of-the-params-evolved-for-first-half-
 of-MOT17-on-the-complete-MOT17) * [Segmentation model vs object detetion model
@@ -82,54 +70,63 @@
 brostrom/Yolov5_StrongSORT_OSNet/tree/botsort * [Yolov5 StrongSORT OSNet vs
 other trackers MOT17](https://github.com/mikel-brostrom/
 Yolov5_StrongSORT_OSNet/wiki/MOT-17-evaluation-(private-detector))  *
 [StrongSORT MOT16 ablation study](https://github.com/mikel-brostrom/
 Yolov5_StrongSORT_OSNet/wiki/Yolov5DeepSORTwithOSNet-vs-
 Yolov5StrongSORTwithOSNet-ablation-study-on-MOT16)  * [Yolov5 StrongSORT OSNet
 vs other trackers MOT16 (deprecated)](https://github.com/mikel-brostrom/
-Yolov5_StrongSORT_OSNet/wiki/MOT-16-evaluation)    Custom object detection
-architecture The trackers provided in this repo can be used with other object
-detectors than Yolov8. Make sure that the input to the trackers is of the
-following format: ```bash Nx6 (x, y, x, y, conf, cls) ```   Tracking with
-Yolov8 ```bash $ python track.py --yolo-model yolov8n.pt # bboxes only yolov8n-
-seg.pt # bboxes + segmentation masks yolov8n-pose.pt # bboxes + pose estimation
-```  Tracking methods ```bash $ python track.py --tracking-method deepocsort
+Yolov5_StrongSORT_OSNet/wiki/MOT-16-evaluation)   ## Why using this tracking
+toolbox? Everything is designed with simplicity and flexibility in mind. We
+don't hyperfocus on results on a single dataset, we prioritize real-world
+results. If you don't get good tracking results on your custom dataset with the
+out-of-the-box tracker configurations, use the `examples/evolve.py` script for
+tracker hyperparameter tuning. ## Installation ``` pip install boxmot ``` ##
+Yolov8 example  Click to expand!  Yolov8 model ```bash $ python examples/
+track.py --yolo-model yolov8n.pt # bboxes only yolov8n-seg.pt # bboxes +
+segmentation masks yolov8n-pose.pt # bboxes + pose estimation ```   Tracking
+methods ```bash $ python examples/track.py --tracking-method deepocsort
 strongsort ocsort bytetrack botsort ```   Tracking sources Tracking can be run
-on most video formats ```bash $ python track.py --source 0 # webcam img.jpg #
-image vid.mp4 # video path/ # directory path/*.jpg # glob 'https://youtu.be/
-Zgi9g1ksQHc' # YouTube 'rtsp://example.com/media.mp4' # RTSP, RTMP, HTTP stream
-```   Select Yolov8 model There is a clear trade-off between model inference
-speed and overall performance. In order to make it possible to fulfill your
-inference speed/accuracy needs you can select a Yolov5 family model for
-automatic download. These model can be further optimized for you needs by the
-[export.py](https://github.com/ultralytics/yolov5/blob/master/export.py) script
-```bash $ python track.py --source 0 --yolo-model yolov8n.pt --img 640
-yolov8s.tflite yolov8m.pt yolov8l.onnx yolov8x.pt --img 1280 ... ```   Select
-ReID model Some tracking methods combine appearance description and motion in
-the process of tracking. For those which use appearance, you can choose a ReID
-model based on your needs from this [ReID model zoo](https://
-kaiyangzhou.github.io/deep-person-reid/MODEL_ZOO). These model can be further
-optimized for you needs by the [reid_export.py](https://github.com/mikel-
-brostrom/Yolov5_StrongSORT_OSNet/blob/master/reid_export.py) script ```bash $
-python track.py --source 0 --reid-model lmbn_n_cuhk03_d.pt
-osnet_x0_25_market1501.pt mobilenetv2_x1_4_msmt17.engine resnet50_msmt17.onnx
-osnet_x1_0_msmt17.pt ... ```   Filter tracked classes By default the tracker
-tracks all MS COCO classes. If you want to track a subset of the classes that
-you model predicts, add their corresponding index after the classes flag,
-```bash python track.py --source 0 --yolo-model yolov8s.pt --classes 16 17 #
-COCO yolov8 model. Track cats and dogs, only ``` [Here](https://
-tech.amikelive.com/node-718/what-object-categories-labels-are-in-coco-dataset/
-) is a list of all the possible objects that a Yolov8 model trained on MS COCO
-can detect. Notice that the indexing for the classes in this repo starts at
-zero   MOT compliant results Can be saved to your experiment folder `runs/
-track/_/` by ```bash python track.py --source ... --save-txt ```   Tracker
-hyperparameter tuning We use a fast and elitist multiobjective genetic
-algorithm for tracker hyperparameter tuning. By default the objectives are:
-HOTA, MOTA, IDF1. Run it by ```bash $ python evolve.py --tracking-method
-strongsort --benchmark MOT17 --n-trials 100 # tune strongsort for MOT17 --
-tracking-method ocsort --benchmark  --objective HOTA # tune ocsort for
-maximizing HOTA on your custom tracking dataset ``` The set of hyperparameters
-leading to the best HOTA result are written to the tracker's config file.   ##
-Contact For Yolov8 tracking bugs and feature requests please visit [GitHub
-Issues](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/issues). For
-business inquiries or professional support requests please send an email to:
-yolov5.deepsort.pytorch@gmail.com
+on most video formats ```bash $ python examples/track.py --source 0 # webcam
+img.jpg # image vid.mp4 # video path/ # directory path/*.jpg # glob 'https://
+youtu.be/Zgi9g1ksQHc' # YouTube 'rtsp://example.com/media.mp4' # RTSP, RTMP,
+HTTP stream ```   Select Yolov8 model There is a clear trade-off between model
+inference speed and overall performance. In order to make it possible to
+fulfill your inference speed/accuracy needs you can select a Yolov5 family
+model for automatic download. These model can be further optimized for you
+needs by the [export.py](https://github.com/ultralytics/yolov5/blob/master/
+export.py) script ```bash $ python examples/track.py --source 0 --yolo-model
+yolov8n.pt --img 640 yolov8s.tflite yolov8m.pt yolov8l.onnx yolov8x.pt --img
+1280 ... ```   Select ReID model Some tracking methods combine appearance
+description and motion in the process of tracking. For those which use
+appearance, you can choose a ReID model based on your needs from this [ReID
+model zoo](https://kaiyangzhou.github.io/deep-person-reid/MODEL_ZOO). These
+model can be further optimized for you needs by the [reid_export.py](https://
+github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet/blob/master/reid_export.py)
+script ```bash $ python examples/track.py --source 0 --reid-model
+lmbn_n_cuhk03_d.pt osnet_x0_25_market1501.pt mobilenetv2_x1_4_msmt17.engine
+resnet50_msmt17.onnx osnet_x1_0_msmt17.pt ... ```   Filter tracked classes By
+default the tracker tracks all MS COCO classes. If you want to track a subset
+of the classes that you model predicts, add their corresponding index after the
+classes flag, ```bash python examples/track.py --source 0 --yolo-model
+yolov8s.pt --classes 16 17 # COCO yolov8 model. Track cats and dogs, only ```
+[Here](https://tech.amikelive.com/node-718/what-object-categories-labels-are-
+in-coco-dataset/) is a list of all the possible objects that a Yolov8 model
+trained on MS COCO can detect. Notice that the indexing for the classes in this
+repo starts at zero   MOT compliant results Can be saved to your experiment
+folder `runs/track/_/` by ```bash python examples/track.py --source ... --save-
+txt ```   Tracker hyperparameter tuning We use a fast and elitist
+multiobjective genetic algorithm for tracker hyperparameter tuning. By default
+the objectives are: HOTA, MOTA, IDF1. Run it by ```bash $ python examples/
+evolve.py --tracking-method strongsort --benchmark MOT17 --n-trials 100 # tune
+strongsort for MOT17 --tracking-method ocsort --benchmark  --objective HOTA #
+tune ocsort for maximizing HOTA on your custom tracking dataset ``` The set of
+hyperparameters leading to the best HOTA result are written to the tracker's
+config file.   ## Custom object detection model example  Click to exapand!
+```python from boxmot import DeepOCSORT tracker = DeepOCSORT() cap =
+cv.VideoCapture(0) while True: ret, im = cap.read() ... # dets: # - your
+model's nms:ed outputs of shape Nx6 (x, y, x, y, conf, cls) # im: # - the
+original image (for better ReID results) # - the downscaled one fed to you
+model (faster) tracker_outputs = tracker.update(dets.cpu(), im) # --> (x, y, x,
+y, id, conf, cls) ... ```  ## Contact For Yolov8 tracking bugs and feature
+requests please visit [GitHub Issues](https://github.com/mikel-brostrom/
+Yolov5_StrongSORT_OSNet/issues). For business inquiries or professional support
+requests please send an email to: yolov5.deepsort.pytorch@gmail.com
```

### Comparing `boxmot-10.0.2/boxmot.egg-info/SOURCES.txt` & `boxmot-10.0.3/boxmot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boxmot-10.0.2/setup.py` & `boxmot-10.0.3/setup.py`

 * *Files identical despite different names*

