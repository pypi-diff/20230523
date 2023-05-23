# Comparing `tmp/ChessAnalysisPipeline-0.0.7.tar.gz` & `tmp/ChessAnalysisPipeline-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChessAnalysisPipeline-0.0.7.tar", last modified: Wed Apr 26 10:17:31 2023, max compression
+gzip compressed data, was "ChessAnalysisPipeline-0.0.8.tar", last modified: Tue May 23 18:02:46 2023, max compression
```

## Comparing `ChessAnalysisPipeline-0.0.7.tar` & `ChessAnalysisPipeline-0.0.8.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.312915 ChessAnalysisPipeline-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.308915 ChessAnalysisPipeline-0.0.7/CHAP/
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/TaskManager.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.308915 ChessAnalysisPipeline-0.0.7/CHAP/common/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.308915 ChessAnalysisPipeline-0.0.7/CHAP/common/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27105 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/models/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    27132 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/models/map.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24447 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3941 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.308915 ChessAnalysisPipeline-0.0.7/CHAP/common/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   121894 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/utils/fit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    51967 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/utils/general.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11359 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/utils/material.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    44627 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/utils/scanparsers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3070 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.308915 ChessAnalysisPipeline-0.0.7/CHAP/edd/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/edd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/edd/models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13698 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/edd/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/edd/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/edd/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.308915 ChessAnalysisPipeline-0.0.7/CHAP/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/inference/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2065 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/inference/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/inference/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/inference/writer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2020 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3378 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3950 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3896 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.308915 ChessAnalysisPipeline-0.0.7/CHAP/saxswaxs/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/saxswaxs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       97 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/saxswaxs/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/saxswaxs/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/saxswaxs/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.312915 ChessAnalysisPipeline-0.0.7/CHAP/sin2psi/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/sin2psi/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       97 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/sin2psi/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/sin2psi/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/sin2psi/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.312915 ChessAnalysisPipeline-0.0.7/CHAP/tomo/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/tomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/tomo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)   104883 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/tomo/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/tomo/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/tomo/writer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3038 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.312915 ChessAnalysisPipeline-0.0.7/ChessAnalysisPipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-26 10:17:31.000000 ChessAnalysisPipeline-0.0.7/ChessAnalysisPipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-26 10:17:31.000000 ChessAnalysisPipeline-0.0.7/ChessAnalysisPipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 10:17:31.000000 ChessAnalysisPipeline-0.0.7/ChessAnalysisPipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-26 10:17:31.000000 ChessAnalysisPipeline-0.0.7/ChessAnalysisPipeline.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 10:17:31.000000 ChessAnalysisPipeline-0.0.7/ChessAnalysisPipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 10:17:31.000000 ChessAnalysisPipeline-0.0.7/ChessAnalysisPipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.312915 ChessAnalysisPipeline-0.0.7/MLaaS/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/MLaaS/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7467 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/MLaaS/ktrain.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2738 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/MLaaS/mnist_img.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14889 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/MLaaS/tfaas_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-26 10:17:31.312915 ChessAnalysisPipeline-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 10:17:31.312915 ChessAnalysisPipeline-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-26 10:17:23.000000 ChessAnalysisPipeline-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:02:46.241003 ChessAnalysisPipeline-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:02:46.225002 ChessAnalysisPipeline-0.0.8/CHAP/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6803 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/TaskManager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      897 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:02:46.225002 ChessAnalysisPipeline-0.0.8/CHAP/common/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:02:46.229002 ChessAnalysisPipeline-0.0.8/CHAP/common/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      200 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/common/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27175 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/common/models/integration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27191 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/common/models/map.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24154 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/common/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2694 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/common/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:02:46.229002 ChessAnalysisPipeline-0.0.8/CHAP/common/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      183 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/common/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   121894 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/common/utils/fit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59457 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/common/utils/general.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11359 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/common/utils/material.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42703 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/common/utils/scanparsers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5087 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/common/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:02:46.233003 ChessAnalysisPipeline-0.0.8/CHAP/edd/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/edd/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11959 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/edd/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23295 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/edd/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/edd/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/edd/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:02:46.233003 ChessAnalysisPipeline-0.0.8/CHAP/inference/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      263 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/inference/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2065 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/inference/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/inference/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/inference/writer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5377 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2639 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2534 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3896 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:02:46.233003 ChessAnalysisPipeline-0.0.8/CHAP/saxswaxs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/saxswaxs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       97 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/saxswaxs/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/saxswaxs/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/saxswaxs/writer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3648 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:02:46.233003 ChessAnalysisPipeline-0.0.8/CHAP/sin2psi/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/sin2psi/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       97 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/sin2psi/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/sin2psi/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/sin2psi/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:02:46.237002 ChessAnalysisPipeline-0.0.8/CHAP/tomo/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      301 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/tomo/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8384 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/tomo/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   135965 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/tomo/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      123 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/tomo/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      123 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/tomo/writer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2585 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/CHAP/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:02:46.237002 ChessAnalysisPipeline-0.0.8/ChessAnalysisPipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-23 18:02:46.000000 ChessAnalysisPipeline-0.0.8/ChessAnalysisPipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-23 18:02:46.000000 ChessAnalysisPipeline-0.0.8/ChessAnalysisPipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:02:46.000000 ChessAnalysisPipeline-0.0.8/ChessAnalysisPipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-23 18:02:46.000000 ChessAnalysisPipeline-0.0.8/ChessAnalysisPipeline.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 18:02:46.000000 ChessAnalysisPipeline-0.0.8/ChessAnalysisPipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 18:02:46.000000 ChessAnalysisPipeline-0.0.8/ChessAnalysisPipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:02:46.241003 ChessAnalysisPipeline-0.0.8/MLaaS/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/MLaaS/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7467 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/MLaaS/ktrain.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2738 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/MLaaS/mnist_img.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14889 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/MLaaS/tfaas_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-23 18:02:46.241003 ChessAnalysisPipeline-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-23 18:02:35.000000 ChessAnalysisPipeline-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 18:02:46.241003 ChessAnalysisPipeline-0.0.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2450 2023-05-23 18:02:39.000000 ChessAnalysisPipeline-0.0.8/setup.py
```

### Comparing `ChessAnalysisPipeline-0.0.7/CHAP/TaskManager.py` & `ChessAnalysisPipeline-0.0.8/CHAP/TaskManager.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.7/CHAP/common/models/integration.py` & `ChessAnalysisPipeline-0.0.8/CHAP/common/models/integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+# System modules
 import copy
 from functools import cache
 import os
 from typing import Literal, Optional
 
+# Third party modules
 import numpy as np
 from pydantic import (BaseModel,
                       validator,
                       constr,
                       conlist,
                       conint,
                       confloat,
@@ -115,18 +117,20 @@
     :type mask_file: str
     :param poni_file: path to a PONI file
     :type poni_file: str
     :return: the mask array loaded from `mask_file`
     :rtype: numpy.ndarray
     """
     if mask_file is not None:
+        # Third party modules
+        from pyspec.file.tiff import TiffFile
+
         if not isinstance(mask_file, str):
             mask_file = str(mask_file)
 
-        from pyspec.file.tiff import TiffFile
         with TiffFile(mask_file) as tiff:
             mask_array = tiff.asarray()
     else:
         mask_array = np.zeros(azimuthal_integrator(poni_file).detector.shape)
     return mask_array
```

### Comparing `ChessAnalysisPipeline-0.0.7/CHAP/common/models/map.py` & `ChessAnalysisPipeline-0.0.8/CHAP/common/models/map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+# System modules
 from functools import cache, lru_cache
 import os
 from typing import Literal, Optional, Union
 
+# Third party modules
 import numpy as np
 from pydantic import (BaseModel,
                       conint,
                       conlist,
                       constr,
                       FilePath,
                       PrivateAttr,
@@ -651,14 +653,15 @@
     :type experiment: Literal["SAXSWAXS","EDD","XRF","Tomo","Powder"]
     :return: None
     """
 
     station = station.lower()
     experiment = experiment.lower()
 
+    # Local modules
     if station in ('id1a3', 'id3a'):
         if experiment in ('saxswaxs', 'powder'):
             from CHAP.common.utils.scanparsers \
                 import SMBLinearScanParser as ScanParser
         elif experiment == 'edd':
             from CHAP.common.utils.scanparsers \
                 import SMBMCAScanParser as ScanParser
```

### Comparing `ChessAnalysisPipeline-0.0.7/CHAP/common/processor.py` & `ChessAnalysisPipeline-0.0.8/CHAP/common/processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     :ivar mgr: The `Processor` used to process every set of input data
     :type mgr: Processor
     """
     def __init__(self, mgr):
         super().__init__()
         self.mgr = mgr
 
-    def _process(self, data):
+    def process(self, data):
         """Asynchronously process the input documents with the
         `self.mgr` `Processor`.
 
         :param data: input data documents to process
         :type docs: iterable
         """
 
@@ -63,15 +63,15 @@
 
         asyncio.run(execute_tasks(self.mgr, data))
 
 
 class IntegrationProcessor(Processor):
     """A processor for integrating 2D data with pyFAI"""
 
-    def _process(self, data):
+    def process(self, data):
         """Integrate the input data with the integration method and
         keyword arguments supplied and return the results.
 
         :param data: input data, including raw data, integration
             method, and keyword args for the integration method.
         :type data: tuple[typing.Union[numpy.ndarray,
                           list[numpy.ndarray]], callable, dict]
@@ -89,15 +89,15 @@
 
 class IntegrateMapProcessor(Processor):
     """Class representing a process that takes a map and integration
     configuration and returns a `nexusformat.nexus.NXprocess`
     containing a map of the integrated detector data requested.
     """
 
-    def _process(self, data):
+    def process(self, data):
         """Process the output of a `Reader` that contains a map and
         integration configuration and return a
         `nexusformat.nexus.NXprocess` containing a map of the
         integrated detector data requested
 
         :param data: Result of `Reader.read` where at least one item
             has the value `'MapConfig'` for the `'schema'` key, and at
@@ -268,15 +268,16 @@
                 'npt_rad': integration_config.radial_npt,
                 'npt_azim': integration_config.azimuthal_npt,
                 'method': 'bbox'
             }
 
         integration_processor = IntegrationProcessor()
         integration_processor.logger.setLevel(self.logger.getEffectiveLevel())
-        integration_processor.logger.addHandler(self.logger.handlers[0])
+        for handler in self.logger.handlers:
+            integration_processor.logger.addHandler(handler)
         for scans in map_config.spec_scans:
             for scan_number in scans.scan_numbers:
                 scanparser = scans.get_scanparser(scan_number)
                 for scan_step_index in range(scanparser.spec_scan_npts):
                     map_index = scans.get_index(
                         scan_number,
                         scan_step_index,
@@ -303,15 +304,15 @@
 class MapProcessor(Processor):
     """A Processor to take a map configuration and return a
     `nexusformat.nexus.NXentry` representing that map's metadata and
     any scalar-valued raw data requseted by the supplied map
     configuration.
     """
 
-    def _process(self, data):
+    def process(self, data):
         """Process the output of a `Reader` that contains a map
         configuration and return a `nexusformat.nexus.NXentry`
         representing the map.
 
         :param data: Result of `Reader.read` where at least one item
             has the value `'MapConfig'` for the `'schema'` key.
         :type data: list[dict[str,object]]
@@ -434,34 +435,40 @@
 
 
 class NexusToNumpyProcessor(Processor):
     """A Processor to convert the default plottable data in an
     `NXobject` into an `numpy.ndarray`.
     """
 
-    def _process(self, data):
+    def process(self, data):
         """Return the default plottable data signal in `data` as an
         `numpy.ndarray`.
 
         :param data: input NeXus structure
         :type data: nexusformat.nexus.tree.NXobject
         :raises ValueError: if `data` has no default plottable data
             signal
         :return: default plottable data signal in `data`
         :rtype: numpy.ndarray
         """
 
-        default_data = data.plottable_data
+        from nexusformat.nexus import NXdata
 
-        if default_data is None:
-            default_data_path = data.attrs['default']
-            default_data = data.get(default_data_path)
-        if default_data is None:
-            raise ValueError(
-                f'The structure of {data} contains no default data')
+        data = self.unwrap_pipelinedata(data)
+
+        if isinstance(data, NXdata):
+            default_data = data
+        else:
+            default_data = data.plottable_data
+            if default_data is None:
+                default_data_path = data.attrs.get('default')
+                default_data = data.get(default_data_path)
+            if default_data is None:
+                raise ValueError(
+                    f'The structure of {data} contains no default data')
 
         default_signal = default_data.attrs.get('signal')
         if default_signal is None:
             raise ValueError(f'The signal of {default_data} is unknown')
         default_signal = default_signal.nxdata
 
         np_data = default_data[default_signal].nxdata
@@ -470,45 +477,52 @@
 
 
 class NexusToXarrayProcessor(Processor):
     """A Processor to convert the default plottable data in an
     `NXobject` into an `xarray.DataArray`.
     """
 
-    def _process(self, data):
+    def process(self, data):
         """Return the default plottable data signal in `data` as an
         `xarray.DataArray`.
 
         :param data: input NeXus structure
         :type data: nexusformat.nexus.tree.NXobject
         :raises ValueError: if metadata for `xarray` is absent from
             `data`
         :return: default plottable data signal in `data`
         :rtype: xarray.DataArray
         """
 
+        from nexusformat.nexus import NXdata
         from xarray import DataArray
 
-        default_data = data.plottable_data
+        data = self.unwrap_pipelinedata(data)
 
-        if default_data is None:
-            default_data_path = data.attrs['default']
-            default_data = data.get(default_data_path)
-        if default_data is None:
-            raise ValueError(
-                f'The structure of {data} contains no default data')
+        if isinstance(data, NXdata):
+            default_data = data
+        else:
+            default_data = data.plottable_data
+            if default_data is None:
+                default_data_path = data.attrs.get('default')
+                default_data = data.get(default_data_path)
+            if default_data is None:
+                raise ValueError(
+                    f'The structure of {data} contains no default data')
 
         default_signal = default_data.attrs.get('signal')
         if default_signal is None:
             raise ValueError(f'The signal of {default_data} is unknown')
         default_signal = default_signal.nxdata
 
         signal_data = default_data[default_signal].nxdata
 
         axes = default_data.attrs['axes']
+        if isinstance(axes, str):
+            axes = [axes]
         coords = {}
         for axis_name in axes:
             axis = default_data[axis_name]
             coords[axis_name] = (axis_name,
                                  axis.nxdata,
                                  axis.attrs)
 
@@ -524,15 +538,15 @@
 
 
 class PrintProcessor(Processor):
     """A Processor to simply print the input data to stdout and return
     the original input data, unchanged in any way.
     """
 
-    def _process(self, data):
+    def process(self, data):
         """Print and return the input data.
 
         :param data: Input data
         :type data: object
         :return: `data`
         :rtype: object
         """
@@ -553,15 +567,15 @@
 class StrainAnalysisProcessor(Processor):
     """A Processor to compute a map of sample strains by fitting bragg
     peaks in 1D detector data and analyzing the difference between
     measured peak locations and expected peak locations for the sample
     measured.
     """
 
-    def _process(self, data):
+    def process(self, data):
         """Process the input map detector data & configuration for the
         strain analysis procedure, and return a map of sample strains.
 
         :param data: results of `MutlipleReader.read` containing input
             map detector data and strain analysis configuration
         :type data: dict[list[str,object]]
         :return: map of sample strains
@@ -597,62 +611,32 @@
         if not strain_analysis_config:
             raise ValueError(
                 'No strain analysis configuration found in input data')
 
         return strain_analysis_config
 
 
-class URLResponseProcessor(Processor):
-    """A Processor to decode and return data resulting from from
-    URLReader.read
-    """
-
-    def _process(self, data):
-        """Take data returned from URLReader.read and return a decoded
-        version of the content.
-
-        :param data: input data (output of URLReader.read)
-        :type data: list[dict]
-        :return: decoded data contents
-        :rtype: object
-        """
-
-        data = data[0]
-
-        content = data['data']
-        encoding = data['encoding']
-
-        self.logger.debug(
-            f'Decoding content of type {type(content)} with {encoding}')
-
-        try:
-            content = content.decode(encoding)
-        except:
-            self.logger.warning('Failed to decode content of type '
-                                f'{type(content)} with {encoding}')
-
-        return content
-
-
 class XarrayToNexusProcessor(Processor):
     """A Processor to convert the data in an `xarray` structure to an
     `nexusformat.nexus.NXdata`.
     """
 
-    def _process(self, data):
+    def process(self, data):
         """Return `data` represented as an `nexusformat.nexus.NXdata`.
 
         :param data: The input `xarray` structure
         :type data: typing.Union[xarray.DataArray, xarray.Dataset]
         :return: The data and metadata in `data`
         :rtype: nexusformat.nexus.NXdata
         """
 
         from nexusformat.nexus import NXdata, NXfield
 
+        data = self.unwrap_pipelinedata(data)
+
         signal = NXfield(value=data.data, name=data.name, attrs=data.attrs)
 
         axes = []
         for name, coord in data.coords.items():
             axes.append(
                 NXfield(value=coord.data, name=name, attrs=coord.attrs))
         axes = tuple(axes)
@@ -661,22 +645,22 @@
 
 
 class XarrayToNumpyProcessor(Processor):
     """A Processor to convert the data in an `xarray.DataArray`
     structure to an `numpy.ndarray`.
     """
 
-    def _process(self, data):
+    def process(self, data):
         """Return just the signal values contained in `data`.
 
         :param data: The input `xarray.DataArray`
         :type data: xarray.DataArray
         :return: The data in `data`
         :rtype: numpy.ndarray
         """
 
-        return data.data
+        return self.unwrap_pipelinedata(data).data
 
 
 if __name__ == '__main__':
     from CHAP.processor import main
     main()
```

### Comparing `ChessAnalysisPipeline-0.0.7/CHAP/common/utils/fit.py` & `ChessAnalysisPipeline-0.0.8/CHAP/common/utils/fit.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.7/CHAP/common/utils/general.py` & `ChessAnalysisPipeline-0.0.8/CHAP/common/utils/general.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from re import sub as re_sub
 from sys import float_info
 
 # Third party modules
 import numpy as np
 try:
     import matplotlib.pyplot as plt
+    import matplotlib.lines as mlines
     from matplotlib.widgets import Button
 except ImportError:
     pass
 
 logger = getLogger(__name__)
 
 
@@ -876,26 +877,73 @@
         raise ValueError(f'{f} is not a valid file')
     if not access(f, R_OK):
         raise ValueError(f'{f} is not accessible for reading')
     return f
 
 
 def draw_mask_1d(
-        ydata, xdata=None, current_index_ranges=None, current_mask=None,
-        select_mask=True, num_index_ranges_max=None, title=None, legend=None,
-        test_mode=False):
-    """Display a 2D plot and have the user select a mask."""
+        ydata, xdata=None, label=None, ref_data=[],
+        current_index_ranges=None, current_mask=None,
+        select_mask=True, num_index_ranges_max=None,
+        title=None, xlabel=None, ylabel=None, test_mode=False):
+    """Display a 2D plot and have the user select a mask.
+
+    :param ydata: data array for which a mask will be constructed
+    :type ydata: numpy.ndarray
+    :param xdata: x-coordinates of the reference data, defaults to
+        None
+    :type xdata: numpy.ndarray, optional
+    :param label: legend label for the reference data, defaults to
+        None
+    :type label: str, optional
+    :param ref_data: a list of additional reference data to
+        plot. Items in the list should be tuples of positional
+        arguments and keyword arguments to unpack and pass directly to
+        `matplotlib.axes.Axes.plot`, defaults to []
+    :type ref_data: list[tuple[tuple, dict]]
+    :param current_index_ranges: list of preselected index ranges to
+        mask, defaults to None
+    :type current_index_ranges: list[tuple[int, int]]
+    :param current_mask: preselected boolean mask array, defaults to
+        None
+    :type current_mask: numpy.ndarray, optional
+    :param select_mask: if True, user-selected ranges will be included
+        when the returned mask is applied to `ydata`. If False, they
+        will be excluded. Defaults to True.
+    :type select_mask: bool, optional
+    :param title: title for the displayed figure, defaults to None
+    :type title: str, optional
+    :param xlabel: label for the x-axis of the displayed figure,
+        defaults to None
+    :type xlabel: str, optional
+    :param ylabel: label for the y-axis of the displayed figure,
+        defaults to None
+    :type ylabel: str, optional
+    :param test_mode: if True, run as a non-interactive test
+        case. Defaults to False
+    :type test_mode: bool, optional
+    :return: a boolean mask array and the list of selected index
+        ranges
+    :rtype: numpy.ndarray, list[tuple[int, int]]
+    """
     # RV make color blind friendly
     def draw_selections(
             ax, current_include, current_exclude, selected_index_ranges):
         """Draw the selections."""
         ax.clear()
-        ax.set_title(title)
-        ax.legend([legend])
-        ax.plot(xdata, ydata, 'k')
+        if title is not None:
+            ax.set_title(title)
+        if xlabel is not None:
+            ax.set_xlabel(xlabel)
+        if ylabel is not None:
+            ax.set_ylabel(ylabel)
+        ax.plot(xdata, ydata, 'k', label=label)
+        for data in ref_data:
+            ax.plot(*data[0], **data[1])
+        ax.legend()
         for low, upp in current_include:
             xlow = 0.5 * (xdata[max(0, low-1)]+xdata[low])
             xupp = 0.5 * (xdata[upp]+xdata[min(num_data-1, 1+upp)])
             ax.axvspan(xlow, xupp, facecolor='green', alpha=0.5)
         for low, upp in current_exclude:
             xlow = 0.5 * (xdata[max(0, low-1)]+xdata[low])
             xupp = 0.5 * (xdata[upp]+xdata[min(num_data-1, 1+upp)])
@@ -1006,23 +1054,18 @@
         logger.warning(
             'num_index_ranges_max input not yet implemented in draw_mask_1d')
     if title is None:
         title = 'select ranges of data'
     elif not isinstance(title, str):
         illegal_value(title, 'title')
         title = ''
-    if legend is None and not isinstance(title, str):
-        illegal_value(legend, 'legend')
-        legend = None
 
     if select_mask:
-        title = f'Click and drag to {title} you wish to include'
         selection_color = 'green'
     else:
-        title = f'Click and drag to {title} you wish to exclude'
         selection_color = 'red'
 
     # Set initial selected mask and the selected/unselected index
     #     ranges as needed
     selected_index_ranges = []
     unselected_index_ranges = []
     selected_mask = np.full(xdata.shape, False, dtype=bool)
@@ -1076,16 +1119,16 @@
             ax, current_include, current_exclude, selected_index_ranges)
 
         # Set up event handling for click-and-drag range selection
         cid_click = fig.canvas.mpl_connect('button_press_event', onclick)
         cid_release = fig.canvas.mpl_connect('button_release_event', onrelease)
 
         # Set up confirm / clear range selection buttons
-        confirm_b = Button(plt.axes([0.75, 0.05, 0.15, 0.075]), 'Confirm')
-        clear_b = Button(plt.axes([0.59, 0.05, 0.15, 0.075]), 'Clear')
+        confirm_b = Button(plt.axes([0.75, 0.015, 0.15, 0.075]), 'Confirm')
+        clear_b = Button(plt.axes([0.59, 0.015, 0.15, 0.075]), 'Clear')
         cid_confirm = confirm_b.on_clicked(confirm_selection)
         cid_clear = clear_b.on_clicked(clear_last_selection)
 
         # Show figure
         plt.show(block=True)
 
         # Disconnect callbacks when figure is closed
@@ -1104,14 +1147,155 @@
         selected_mask, selected_index_ranges, unselected_index_ranges)
 
     # Update the currently included index ranges (where mask is True)
     current_include = update_index_ranges(selected_mask)
 
     return selected_mask, current_include
 
+def select_peaks(
+        ydata, xdata, peak_locations,
+        mask=None,
+        pre_selected_peak_indices=[],
+        return_sorted=True,
+        title='', xlabel='', ylabel=''):
+    """
+    Show a plot of the 1D data provided with user-selectable markers
+    at the given locations. Return the locations of the markers that
+    the user selected with their mouse interactions.
+
+    :param ydata: 1D array of values to plot
+    :type ydata: numpy.ndarray
+    :param xdata: values of the independent dimension corresponding to
+        ydata, defaults to None
+    :type xdata: numpy.ndarray, optional
+    :param peak_locations: locations of selectable markers in the same
+        units as xdata.
+    :type peak_locations: list
+    :param mask: boolean array representing a mask that will be
+        applied to the data at some later point, defaults to None
+    :type mask: np.ndarray, optional
+    :param pre_selected_peak_indices: indices of markers that should
+        already be selected when the figure shows up, defaults to []
+    :type pre_selected_peak_indices: list[int], optional
+    :param return_sorted: sort the indices of selected markers before
+        returning (otherwise: return them in the same order that the
+        user selected them), defaults to True
+    :type return_sorted: bool, optional
+    :param title: title for the plot, defaults to ''
+    :type title: str, optional
+    :param xlabel: x-axis label for the plot, defaults to ''
+    :type xlabel: str, optional
+    :param ylabel: y-axis label for the plot, defaults to ''
+    :type ylabel: str, optional
+    :return: the locations of the user-selected peaks
+    :rtype: list
+    """
+
+    if ydata.size != xdata.size:
+        raise ValueError('x and y data must have the same size')
+    if mask is not None and mask.size != ydata.size:
+        raise ValueError('mask must have the same size as data')
+
+
+    excluded_peak_props = {
+        'color': 'black', 'linestyle': '--','linewidth': 1,
+        'marker': 10, 'markersize': 5, 'fillstyle': 'none'}
+    included_peak_props = {
+        'color': 'green', 'linestyle': '-', 'linewidth': 2,
+        'marker': 10, 'markersize': 10, 'fillstyle': 'full'}
+    masked_peak_props = {
+        'color': 'gray', 'linestyle': ':', 'linewidth': 1}
+
+    # Setup reference data & plot
+    if mask is None:
+        mask = np.full(ydata.shape, True, dtype=bool)
+    fig, ax = plt.subplots()
+    handles = ax.plot(xdata, ydata, label='Reference data')
+    handles.append(mlines.Line2D(
+        [], [], label='Excluded / unselected', **excluded_peak_props))
+    handles.append(mlines.Line2D(
+        [], [], label='Included / selected', **included_peak_props))
+    handles.append(mlines.Line2D(
+        [], [], label='In masked region (unselectable)', **masked_peak_props))
+    ax.legend(handles=handles, loc='upper right')
+    ax.set(title=title, xlabel=xlabel, ylabel=ylabel)
+
+    # Plot a vertical line marker at each peak location
+    peak_vlines = []
+    x_indices = np.arange(ydata.size)
+    for i, loc in enumerate(peak_locations):
+        nearest_index = np.searchsorted(xdata, loc)
+        if nearest_index in x_indices[mask]:
+            if i in pre_selected_peak_indices:
+                peak_vline = ax.axvline(loc, **included_peak_props)
+            else:
+                peak_vline = ax.axvline(loc, **excluded_peak_props)
+            peak_vline.set_picker(5)
+        else:
+            if i in pre_selected_peak_indices:
+                logger.warning(
+                    f'Pre-selected peak index {i} is in a masked region and '
+                    'will not be selectable.')
+                pre_selected_peak_indices.remove(i)
+            peak_vline = ax.axvline(loc, **masked_peak_props)
+        peak_vlines.append(peak_vline)
+
+    # Indicate masked regions by gray-ing out the axes facecolor
+    exclude_bounds = []
+    for i, m in enumerate(mask):
+        if not m:
+            if (not exclude_bounds) or isinstance(exclude_bounds[-1], tuple):
+                exclude_bounds.append(i)
+        else:
+            if exclude_bounds and isinstance(exclude_bounds[-1], int):
+                exclude_bounds[-1] = (exclude_bounds[-1], i-1)
+    if exclude_bounds and isinstance(exclude_bounds[-1], int):
+        exclude_bounds[-1] = (exclude_bounds[-1], mask.size-1)
+    for (low, upp) in exclude_bounds:
+        xlow = xdata[low]
+        xupp = xdata[upp]
+        ax.axvspan(xlow, xupp, facecolor='gray', alpha=0.5)
+
+    # Setup interative peak selection
+    selected_peak_indices = pre_selected_peak_indices
+    def onpick(event):
+        try:
+            peak_index = peak_vlines.index(event.artist)
+        except:
+            pass
+        else:
+            peak_vline = event.artist
+            if peak_index in selected_peak_indices:
+                peak_vline.set(**excluded_peak_props)
+                selected_peak_indices.remove(peak_index)
+            else:
+                peak_vline.set(**included_peak_props)
+                selected_peak_indices.append(peak_index)
+            plt.draw()
+    cid_pick_peak = fig.canvas.mpl_connect('pick_event', onpick)
+
+    # Setup "Confirm" button
+    def confirm_selection(event):
+        plt.close()
+    plt.subplots_adjust(bottom=0.2)
+    confirm_b = Button(plt.axes([0.75, 0.05, 0.15, 0.075]), 'Confirm')
+    cid_confirm = confirm_b.on_clicked(confirm_selection)
+
+    # Show figure for user interaction
+    plt.show()
+
+    # Disconnect all widget callbacks when figure is closed
+    fig.canvas.mpl_disconnect(cid_pick_peak)
+    confirm_b.disconnect(cid_confirm)
+
+    selected_peaks = peak_locations[selected_peak_indices]
+    if return_sorted:
+        selected_peaks.sort()
+    return selected_peaks
+
 
 def select_image_bounds(
         a, axis, low=None, upp=None, num_min=None, title='select array bounds',
         raise_error=False):
     """
     Interactively select the lower and upper data bounds for a 2D
     numpy array.
```

### Comparing `ChessAnalysisPipeline-0.0.7/CHAP/common/utils/material.py` & `ChessAnalysisPipeline-0.0.8/CHAP/common/utils/material.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.7/CHAP/common/utils/scanparsers.py` & `ChessAnalysisPipeline-0.0.8/CHAP/common/utils/scanparsers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #!/usr/bin/env python3
 
 # -*- coding: utf-8 -*-
 
-# system modules
+# System modules
 from csv import reader
 from fnmatch import filter as fnmatch_filter
 from json import load
 import os
 import re
 
-# third party modules
+# Third party modules
 import numpy as np
 from pyspec.file.spec import FileSpec
+from pyspec.file.tiff import TiffFile
 
 
 class ScanParser:
     """Partial implementation of a class representing a SPEC scan and
     some of its metadata.
 
     :param spec_file_name: path to a SPEC file on the CLASSE DAQ
@@ -288,15 +289,15 @@
     collected at SMB or FAST.
     """
 
     def __init__(self, spec_file_name, scan_number):
         super().__init__(spec_file_name, scan_number)
 
         self._pars = None
-        self.par_file_pattern = f'*-*-{self.scan_name}'
+        self._par_file_pattern = f'*-*-{self.scan_name}'
 
     def get_scan_name(self):
         return os.path.basename(self.scan_path)
 
     def get_scan_title(self):
         return f'{self.scan_name}_{self.scan_number}'
 
@@ -311,15 +312,15 @@
         associated with this SPEC scan.
 
         :rtype: dict[str,object]
         """
         # JSON file holds titles for columns in the par file
         json_files = fnmatch_filter(
             os.listdir(self.scan_path),
-            f'{self.par_file_pattern}.json')
+            f'{self._par_file_pattern}.json')
         if len(json_files) != 1:
             raise RuntimeError(f'{self.scan_title}: cannot find the '
                                '.json file to decode the .par file')
         with open(os.path.join(self.scan_path, json_files[0])) as json_file:
             par_file_cols = load(json_file)
         try:
             par_col_names = list(par_file_cols.values())
@@ -327,15 +328,15 @@
             scann_col_idx = int(list(par_file_cols.keys())[scann_val_idx])
         except:
             raise RuntimeError(f'{self.scan_title}: cannot find scan pars '
                                'without a "SCAN_N" column in the par file')
 
         par_files = fnmatch_filter(
             os.listdir(self.scan_path),
-            f'{self.par_file_pattern}.par')
+            f'{self._par_file_pattern}.par')
         if len(par_files) != 1:
             raise RuntimeError(f'{self.scan_title}: cannot find the .par '
                                'file for this scan directory')
         par_dict = None
         with open(os.path.join(self.scan_path, par_files[0])) as par_file:
             par_reader = reader(par_file, delimiter=' ')
             for row in par_reader:
@@ -522,15 +523,15 @@
     """Partial implementation of a class representing a typical line
     or mesh scan in SPEC collected at FMB.
     """
 
     def get_spec_scan_motor_mnes(self):
         if self.spec_macro == 'flymesh':
             return (self.spec_args[0], self.spec_args[5])
-        if self.spec_macro == 'flyscan':
+        if self.spec_macro in ('flyscan', 'ascan'):
             return (self.spec_args[0],)
         if self.spec_macro in ('tseries', 'loopscan'):
             return ('Time',)
         raise RuntimeError(f'{self.scan_title}: cannot determine scan motors '
                            f'for scans of type {self.spec_macro}')
 
     def get_spec_scan_motor_vals(self):
@@ -538,39 +539,39 @@
             fast_mot_vals = np.linspace(float(self.spec_args[1]),
                                         float(self.spec_args[2]),
                                         int(self.spec_args[3])+1)
             slow_mot_vals = np.linspace(float(self.spec_args[6]),
                                         float(self.spec_args[7]),
                                         int(self.spec_args[8])+1)
             return (fast_mot_vals, slow_mot_vals)
-        if self.spec_macro == 'flyscan':
+        if self.spec_macro in ('flyscan', 'ascan'):
             mot_vals = np.linspace(float(self.spec_args[1]),
                                    float(self.spec_args[2]),
                                    int(self.spec_args[3])+1)
             return (mot_vals,)
         if self.spec_macro in ('tseries', 'loopscan'):
             return self.spec_scan.data[:,0]
         raise RuntimeError(f'{self.scan_title}: cannot determine scan motors '
                            f'for scans of type {self.spec_macro}')
 
     def get_spec_scan_shape(self):
         if self.spec_macro == 'flymesh':
             fast_mot_npts = int(self.spec_args[3])+1
             slow_mot_npts = int(self.spec_args[8])+1
             return (fast_mot_npts, slow_mot_npts)
-        if self.spec_macro == 'flyscan':
+        if self.spec_macro in ('flyscan', 'ascan'):
             mot_npts = int(self.spec_args[3])+1
             return (mot_npts,)
         if self.spec_macro in ('tseries', 'loopscan'):
             return len(np.array(self.spec_scan.data[:,0]))
         raise RuntimeError(f'{self.scan_title}: cannot determine scan shape '
                            f'for scans of type {self.spec_macro}')
 
     def get_spec_scan_dwell(self):
-        if self.spec_macro in ('flymesh', 'flyscan'):
+        if self.spec_macro in ('flymesh', 'flyscan', 'ascan'):
             return float(self.spec_args[4])
         if self.spec_macro in ('tseries', 'loopscan'):
             return float(self.spec_args[1])
         raise RuntimeError(f'{self.scan_title}: cannot determine dwell for '
                            f'scans of type {self.spec_macro}')
 
     def get_detector_data_path(self):
@@ -586,27 +587,26 @@
         return f'{self.scan_name}_{self.scan_number:03d}'
 
     def get_detector_data_file(self, detector_prefix, scan_step_index:int):
         scan_step = self.get_scan_step(scan_step_index)
         file_indices = [f'{scan_step[i]:03d}'
                         for i in range(len(self.spec_scan_shape))
                         if self.spec_scan_shape[i] != 1]
+        if len(file_indices) == 0:
+            file_indices = ['000']
         file_name = f'{self.scan_name}_{detector_prefix}_' \
                     f'{self.scan_number:03d}_{"_".join(file_indices)}.tiff'
         file_name_full = os.path.join(self.detector_data_path, file_name)
         if os.path.isfile(file_name_full):
             return file_name_full
         raise RuntimeError(f'{self.scan_title}: could not find detector image '
                            f'file for detector {detector_prefix} scan step '
                            f'({scan_step})')
 
     def get_detector_data(self, detector_prefix, scan_step_index:int):
-        # third party modules
-        from pyspec.file.tiff import TiffFile
-
         image_file = self.get_detector_data_file(detector_prefix,
                                                  scan_step_index)
         with TiffFile(image_file) as tiff_file:
             image_data = tiff_file.asarray()
         return image_data
 
 
@@ -625,15 +625,15 @@
         if os.path.isfile(file_name_full):
             return file_name_full
         raise RuntimeError(f'{self.scan_title}: could not find detector image '
                            f'file for detector {detector_prefix} scan step '
                            f'({scan_step_index})')
 
     def get_detector_data(self, detector_prefix, scan_step_index:int):
-        # third party modules
+        # Third party modules
         from h5py import File
 
         detector_file = self.get_detector_data_file(
             detector_prefix, scan_step_index)
         scan_step = self.get_scan_step(scan_step_index)
         with File(detector_file) as h5_file:
             detector_data = \
@@ -642,18 +642,28 @@
 
 
 class SMBLinearScanParser(LinearScanParser, SMBScanParser):
     """Concrete implementation of a class representing a scan taken
     with the typical powder diffraction setup at SMB.
     """
 
+    def get_spec_scan_dwell(self):
+        if self.spec_macro in ('flymesh', 'flyscan', 'ascan'):
+            return float(self.spec_args[4])
+        if self.spec_macro == 'tseries':
+            return float(self.spec_args[1])
+        if self.spec_macro == 'wbslew_scan':
+            return float(self.spec_args[3])
+        raise RuntimeError(f'{self.scan_title}: cannot determine dwell time '
+                           f'for scans of type {self.spec_macro}')
+
     def get_spec_scan_motor_mnes(self):
         if self.spec_macro == 'flymesh':
             return (self.spec_args[0], self.spec_args[5])
-        if self.spec_macro == 'flyscan':
+        if self.spec_macro in ('flyscan', 'ascan'):
             return (self.spec_args[0],)
         if self.spec_macro in ('tseries', 'loopscan'):
             return ('Time',)
         raise RuntimeError(f'{self.scan_title}: cannot determine scan motors '
                            f'for scans of type {self.spec_macro}')
 
     def get_spec_scan_motor_vals(self):
@@ -661,41 +671,41 @@
             fast_mot_vals = np.linspace(float(self.spec_args[1]),
                                         float(self.spec_args[2]),
                                         int(self.spec_args[3])+1)
             slow_mot_vals = np.linspace(float(self.spec_args[6]),
                                         float(self.spec_args[7]),
                                         int(self.spec_args[8])+1)
             return (fast_mot_vals, slow_mot_vals)
-        if self.spec_macro == 'flyscan':
+        if self.spec_macro in ('flyscan', 'ascan'):
             mot_vals = np.linspace(float(self.spec_args[1]),
                                    float(self.spec_args[2]),
                                    int(self.spec_args[3])+1)
             return (mot_vals,)
         if self.spec_macro in ('tseries', 'loopscan'):
             return self.spec_scan.data[:,0]
         raise RuntimeError(f'{self.scan_title}: cannot determine scan motors '
                            f'for scans of type {self.spec_macro}')
 
     def get_spec_scan_shape(self):
         if self.spec_macro == 'flymesh':
             fast_mot_npts = int(self.spec_args[3])+1
             slow_mot_npts = int(self.spec_args[8])+1
             return (fast_mot_npts, slow_mot_npts)
-        if self.spec_macro == 'flyscan':
+        if self.spec_macro in ('flyscan', 'ascan'):
             mot_npts = int(self.spec_args[3])+1
             return (mot_npts,)
         if self.spec_macro in ('tseries', 'loopscan'):
             return len(np.array(self.spec_scan.data[:,0]))
         raise RuntimeError(f'{self.scan_title}: cannot determine scan shape '
                            f'for scans of type {self.spec_macro}')
 
     def get_spec_scan_dwell(self):
         if self.spec_macro == 'flymesh':
             return float(self.spec_args[4])
-        if self.spec_macro == 'flyscan':
+        if self.spec_macro in ('flyscan', 'ascan'):
             return float(self.spec_args[-1])
         raise RuntimeError(f'{self.scan_title}: cannot determine dwell time '
                            f'for scans of type {self.spec_macro}')
 
     def get_detector_data_path(self):
         return os.path.join(self.scan_path, str(self.scan_number))
 
@@ -713,15 +723,15 @@
         if len(file_name_matches) == 1:
             return os.path.join(self.detector_data_path, file_name_matches[0])
         raise RuntimeError(f'{self.scan_title}: could not find detector image '
                            f'file for detector {detector_prefix} scan step '
                            f'({scan_step_index})')
 
     def get_detector_data(self, detector_prefix, scan_step_index:int):
-        # third party modules
+        # Third party modules
         from h5py import File
 
         image_file = self.get_detector_data_file(
             detector_prefix, scan_step_index)
         with File(image_file) as h5_file:
             image_data = h5_file['/entry/data/data'][0]
         return image_data
@@ -732,31 +742,31 @@
     scan.
     """
 
     def __init__(self, spec_file_name, scan_number):
         super().__init__(spec_file_name, scan_number)
 
         self._scan_type = None
-        self._theta_vals = None
+        self._rotation_angles= None
         self._horizontal_shift = None
         self._vertical_shift = None
         self._starting_image_index = None
         self._starting_image_offset = None
 
     @property
     def scan_type(self):
         if self._scan_type is None:
             self._scan_type = self.get_scan_type()
         return self._scan_type
 
     @property
-    def theta_vals(self):
-        if self._theta_vals is None:
-            self._theta_vals = self.get_theta_vals()
-        return self._theta_vals
+    def rotation_angles(self):
+        if self._rotation_angles is None:
+            self._rotation_angles = self.get_rotation_angles()
+        return self._rotation_angles
 
     @property
     def horizontal_shift(self):
         if self._horizontal_shift is None:
             self._horizontal_shift = self.get_horizontal_shift()
         return self._horizontal_shift
 
@@ -774,30 +784,31 @@
 
     @property
     def starting_image_offset(self):
         if self._starting_image_offset is None:
             self._starting_image_offset = self.get_starting_image_offset()
         return self._starting_image_offset
 
+    def get_spec_scan_npts(self):
+        return len(self.rotation_angles)
+
     def get_scan_type(self):
         """Return a string identifier for the type of tomography data
         being collected by this scan: df1 (dark field), bf1 (bright
         field), or tf1 (sample tomography data).
 
         :rtype: typing.Literal['df1', 'bf1', 'tf1']
         """
         return None
 
-    def get_theta_vals(self):
-        """Return a dictionary of information about the angular values
-        visited by the rotating motor at each point in the scan. The
-        dictionary may contain a single key, "num", or three keys:
-        "num", "start", and "end"
+    def get_rotation_angles(self):
+        """Return the angular values visited by the rotating motor at
+        each point in the scan.
 
-        :rtype: dict[str, float]"""
+        :rtype: np.array(float)"""
         raise NotImplementedError
 
     def get_horizontal_shift(self):
         """Return the value of the motor that shifts the sample in the
         +x direction (hutch frame). Useful when tomography scans are
         taken in a series of stacks when the sample is wider than the
         width of the beam.
@@ -829,76 +840,70 @@
         detector data collected by this scan from the index of the
         first frame of detector data collected by this scan.
 
         :rtype: int
         """
         raise NotImplementedError
 
-    def get_num_image(self, detector_prefix):
-        """Return the total number of "good" frames of detector data
-        collected by this scan
-
-        :rtype: int
-        """
-        raise NotImplementedError
-
 
 class FMBRotationScanParser(RotationScanParser, FMBScanParser):
     """Concrete implementation of a class representing a scan taken
     with the typical tomography setup at FMB.
     """
 
-    def get_spec_scan_npts(self):
+    def get_rotation_angles(self):
         if self.spec_macro == 'flyscan':
             if len(self.spec_args) == 2:
                 # Flat field (dark or bright)
-                return int(self.spec_args[0])+1
-            if len(self.spec_args) == 5:
-                return int(self.spec_args[3])+1
-            raise RuntimeError(f'{self.scan_title}: cannot obtain number of '
-                               f'points from {self.spec_macro} with '
+                return int(self.spec_args[0]) * [0]
+            if (len(self.spec_args) == 5
+                    and int(self.spec_args[3]) > 2*self.starting_image_offset):
+                all_rotation_angles = np.linspace(
+                    float(self.spec_args[1]), float(self.spec_args[2]),
+                    int(self.spec_args[3])+1)
+                return all_rotation_angles[
+                    self.starting_image_offset:-1-self.starting_image_offset]
+            raise RuntimeError(f'{self.scan_title}: cannot obtain rotation '
+                               f'angles from {self.spec_macro} with '
                                f'arguments {self.spec_args}')
-        raise RuntimeError(f'{self.scan_title}: cannot determine number of '
-                           f'points for scans of type {self.spec_macro}')
-
-    def get_theta_vals(self):
-        if self.spec_macro == 'flyscan':
-            if len(self.spec_args) == 2:
-                # Flat field (dark or bright)
-                return {'num': int(self.spec_args[0])}
-            if len(self.spec_args) == 5:
-                return {'start': float(self.spec_args[1]),
-                        'end': float(self.spec_args[2]),
-                        'num': int(self.spec_args[3])+1}
-            raise RuntimeError(f'{self.scan_title}: cannot obtain theta values'
-                               f' from {self.spec_macro} with arguments '
-                               f'{self.spec_args}')
-        raise RuntimeError(f'{self.scan_title}: cannot determine theta values '
-                           f'for scans of type {self.spec_macro}')
+        raise RuntimeError(f'{self.scan_title}: cannot determine rotation '
+                           f' angles for scans of type {self.spec_macro}')
 
     def get_horizontal_shift(self):
-        return 0.0
+        try:
+            horizontal_shift = float(self.get_spec_positioner_value('4C_samx'))
+        except:
+            try:
+                horizontal_shift = float(
+                    self.get_spec_positioner_value('GI_samx'))
+            except:
+                raise RuntimeError(
+                    f'{self.scan_title}: cannot determine the horizontal shift')
+        return horizontal_shift
 
     def get_vertical_shift(self):
-        return float(self.get_spec_positioner_value('4C_samz'))
+        try:
+            vertical_shift = float(self.get_spec_positioner_value('4C_samz'))
+        except:
+            try:
+                vertical_shift = float(self.get_spec_positioner_value('GI_samz'))
+            except:
+                raise RuntimeError(
+                    f'{self.scan_title}: cannot determine the vertical shift')
+        return vertical_shift
 
     def get_starting_image_index(self):
         return 0
 
     def get_starting_image_offset(self):
-        return 1
-
-    def get_num_image(self, detector_prefix):
-        # third party modules
-        from h5py import File
-
-        detector_file = self.get_detector_data_file(detector_prefix)
-        with File(detector_file) as h5_file:
-            num_image = h5_file['/entry/instrument/detector/data'].shape[0]
-        return num_image-self.starting_image_offset
+        if len(self.spec_args) == 2:
+            # Flat field (dark or bright)
+            return 0
+        if len(self.spec_args) == 5:
+            return 1
 
     def get_detector_data_path(self):
         return self.scan_path
 
     def get_detector_data_file(self, detector_prefix):
         prefix = detector_prefix.upper()
         file_name = f'{self.scan_name}_{prefix}_{self.scan_number:03d}.h5'
@@ -906,22 +911,22 @@
         if os.path.isfile(file_name_full):
             return file_name_full
         raise RuntimeError(f'{self.scan_title}: could not find detector image '
                            f'file for detector {detector_prefix}')
 
     def get_all_detector_data_in_file(
             self, detector_prefix, scan_step_index=None):
-        # third party modules
+        # Third party modules
         from h5py import File
 
         detector_file = self.get_detector_data_file(detector_prefix)
         with File(detector_file) as h5_file:
             if scan_step_index is None:
                 detector_data = h5_file['/entry/instrument/detector/data'][
-                    self.starting_image_index:]
+                    self.starting_image_index:-1-self.starting_image_offset]
             elif isinstance(scan_step_index, int):
                 detector_data = h5_file['/entry/instrument/detector/data'][
                     self.starting_image_index+scan_step_index]
             elif (isinstance(scan_step_index, (list, tuple))
                     and len(scan_step_index) == 2):
                 detector_data = h5_file['/entry/instrument/detector/data'][
                     self.starting_image_index+scan_step_index[0]:
@@ -940,34 +945,28 @@
     """Concrete implementation of a class representing a scan taken
     with the typical tomography setup at SMB.
     """
 
     def __init__(self, spec_file_name, scan_number):
         super().__init__(spec_file_name, scan_number)
 
-        self.par_file_pattern = f'id*-*tomo*-{self.scan_name}'
-
-    def get_spec_scan_npts(self):
-        if self.spec_macro in ('slew_ome','rams4_slew_ome'):
-            return int(self.pars['nframes_real'])
-        raise RuntimeError(f'{self.scan_title}: cannot determine number of '
-                           f'points for scans of type {self.spec_macro}')
+        self._par_file_pattern = f'id*-*tomo*-{self.scan_name}'
 
     def get_scan_type(self):
-        scan_type = self.pars.get('tomo_type',
-                                  self.pars.get('tomotype', None))
+        scan_type = self.pars.get(
+            'tomo_type', self.pars.get('tomotype', None))
         if scan_type is None:
-            raise RuntimeError(f'{self.scan_title}: cannot determine '
-                               'the scan_type')
+            raise RuntimeError(
+                f'{self.scan_title}: cannot determine the scan_type')
         return scan_type
 
-    def get_theta_vals(self):
-        return {'start': float(self.pars['ome_start_real']),
-                'end': float(self.pars['ome_end_real']),
-                'num': int(self.pars['nframes_real'])}
+    def get_rotation_angles(self):
+        return np.linspace(
+            float(self.pars['ome_start_real']),
+            float(self.pars['ome_end_real']), int(self.pars['nframes_real']))
 
     def get_horizontal_shift(self):
         horizontal_shift = self.pars.get(
             'rams4x', self.pars.get('ramsx', None))
         if horizontal_shift is None:
             raise RuntimeError(
                 f'{self.scan_title}: cannot determine the horizontal shift')
@@ -992,51 +991,33 @@
         try:
             return (int(self.pars['goodstart'])
                     - self.get_starting_image_index())
         except:
             raise RuntimeError(f'{self.scan_title}: cannot determine index '
                                'offset of first good detector image')
 
-    def get_num_image(self, detector_prefix=None):
-        try:
-            return int(self.pars['nframes_real'])
-#            index_regex = re.compile(r'\d+')
-#            # At this point only tiffs
-#            path = self.get_detector_data_path()
-#            files = sorted([f for f in os.listdir(path) \
-#                if os.path.isfile(os.path.join(path, f)) \
-#                and f.endswith('.tif') \
-#                and index_regex.search(f)])
-#            return len(files)-self.starting_image_offset
-        except:
-            raise RuntimeError(f'{self.scan_title}: cannot determine the '
-                               'number of good detector images')
-
     def get_detector_data_path(self):
         return os.path.join(self.scan_path, str(self.scan_number), 'nf')
 
     def get_detector_data_file(self, scan_step_index:int):
         file_name = f'nf_{self.starting_image_index+scan_step_index:06d}.tif'
         file_name_full = os.path.join(self.detector_data_path, file_name)
         if os.path.isfile(file_name_full):
             return file_name_full
         raise RuntimeError(f'{self.scan_title}: could not find detector image '
                            f'file for scan step ({scan_step_index})')
 
     def get_detector_data(self, detector_prefix, scan_step_index=None):
         if scan_step_index is None:
             detector_data = []
-            for index in range(len(self.get_num_image(detector_prefix))):
+            for index in range(len(self.get_spec_scan_npts())):
                 detector_data.append(
                     self.get_detector_data(detector_prefix, index))
             detector_data = np.asarray(detector_data)
         elif isinstance(scan_step_index, int):
-            # third party modules
-            from pyspec.file.tiff import TiffFile
-
             image_file = self.get_detector_data_file(scan_step_index)
             with TiffFile(image_file) as tiff_file:
                 detector_data = tiff_file.asarray()
         elif (isinstance(scan_step_index, (list, tuple))
                 and len(scan_step_index) == 2):
             detector_data = []
             for index in range(scan_step_index[0], scan_step_index[1]):
@@ -1053,68 +1034,33 @@
     """Partial implementation of a class representing a scan taken
     while collecting SPEC MCA data.
     """
 
     def __init__(self, spec_file_name, scan_number):
         super().__init__(spec_file_name, scan_number)
 
-        self._dwell_time = None
         self._detector_num_bins = None
 
-    @property
-    def dwell_time(self):
-        if self._dwell_time is None:
-            self._dwell_time = self.get_dwell_time()
-        return self._dwell_time
-
-    def get_dwell_time(self):
-        """Return the dwell time for each scan point as it appears in
-        the SPEC command.
-
-        :rtype: float
-        """
-        raise NotImplementedError
-
     def get_detector_num_bins(self, detector_prefix):
         """Return the number of bins for the detector with the given
         prefix.
 
         :param detector_prefix: the detector prefix as used in SPEC
             MCA data files
         :type detector_prefix: str
         :rtype: int
         """
         raise NotImplementedError
 
 
-class SMBMCAScanParser(MCAScanParser, SMBScanParser):
+class SMBMCAScanParser(MCAScanParser, SMBLinearScanParser):
     """Concrete implementation of a class representing a scan taken
     with the typical EDD setup at SMB or FAST.
     """
 
-    def get_spec_scan_npts(self):
-        if self.spec_macro == 'tseries':
-            return 1
-        if self.spec_macro == 'ascan':
-            return int(self.spec_args[3])
-        if self.spec_scan == 'wbslew_scan':
-            return 1
-        raise RuntimeError(f'{self.scan_title}: cannot determine number of '
-                           f'points for scans of type {self.spec_macro}')
-
-    def get_dwell_time(self):
-        if self.spec_macro == 'tseries':
-            return float(self.spec_args[1])
-        if self.spec_macro == 'ascan':
-            return float(self.spec_args[4])
-        if self.spec_macro == 'wbslew_scan':
-            return float(self.spec_args[3])
-        raise RuntimeError(f'{self.scan_title}: cannot determine dwell time '
-                           f'for scans of type {self.spec_macro}')
-
     def get_detector_num_bins(self, detector_prefix):
         with open(self.get_detector_data_file(detector_prefix)) \
              as detector_file:
             lines = detector_file.readlines()
         for line in lines:
             if line.startswith('#@CHANN'):
                 try:
@@ -1170,12 +1116,12 @@
             elif counter == (np.ceil(num_bins/25.)):
                 b = np.array(a).astype('uint16')
                 spectrum[(counter-1) * 25:
                          ((counter-1) * 25 + (np.mod(num_bins, 25)))] = b
                 data.append(spectrum)
                 counter = 0
 
-        return data
+        return np.array(data)
 
     def get_detector_data(self, detector_prefix, scan_step_index:int):
         detector_data = self.get_all_detector_data(detector_prefix)
         return detector_data[scan_step_index]
```

### Comparing `ChessAnalysisPipeline-0.0.7/CHAP/inference/processor.py` & `ChessAnalysisPipeline-0.0.8/CHAP/inference/processor.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.7/CHAP/processor.py` & `ChessAnalysisPipeline-0.0.8/CHAP/processor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,50 @@
 #!/usr/bin/env python
 #-*- coding: utf-8 -*-
 #pylint: disable=
 """
 File       : processor.py
 Author     : Valentin Kuznetsov <vkuznet AT gmail dot com>
 Description: Processor module
+
+Define a generic `Processor` object.
 """
 
 # system modules
 import argparse
 from inspect import getfullargspec
 import logging
 from sys import modules
 from time import time
 
+# local modules
+from CHAP.pipeline import PipelineItem
 
-class Processor():
-    """Processor represent generic processor"""
-    def __init__(self):
-        """Processor constructor"""
-        self.__name__ = self.__class__.__name__
-        self.logger = logging.getLogger(self.__name__)
-        self.logger.propagate = False
-
-    def process(self, data, **_process_kwargs):
-        """process data API
-
-        :param _process_kwargs: keyword arguments to pass to
-            `self._process`, defaults to `{}`
-        :type _process_kwargs: dict, optional
-        """
-
-        t0 = time()
-        self.logger.info(f'Executing "process" with type(data)={type(data)}')
-
-        _valid_process_args = {}
-        allowed_args = getfullargspec(self._process).args \
-            + getfullargspec(self._process).kwonlyargs
-        for k, v in _process_kwargs.items():
-            if k in allowed_args:
-                _valid_process_args[k] = v
-            else:
-                self.logger.warning(f'Ignoring invalid arg to _process: {k}')
-
-        data = self._process(data, **_valid_process_args)
-
-        self.logger.info(f'Finished "process" in {time()-t0:.3f} seconds\n')
-
-        return data
+class Processor(PipelineItem):
+    """Generic data processor.
 
-    def _process(self, data):
-        """Private method to carry out the mechanics of the specific
-        Processor.
+    The job of any `Processor` in a `Pipeline` is to receive data
+    returned by the previous `PipelineItem`, process it in some way,
+    and return the result for the next `PipelineItem` to use as input.
+    """
+
+    def process(self, data):
+        """Extract the contents of the input data, add a string to it,
+        and return the amended value.
 
         :param data: input data
         :return: processed data
         """
         # If needed, extract data from a returned value of Reader.read
         if isinstance(data, list):
             if all(isinstance(d, dict) for d in data):
                 data = data[0]['data']
         if data is None:
             return []
-        # process operation is a simple print function
+        # process operation is a simple string concatenation
         data += "process part\n"
         # and we return data back to pipeline
         return data
 
 
 class OptionParser():
     """User based option parser"""
```

### Comparing `ChessAnalysisPipeline-0.0.7/CHAP/runner.py` & `ChessAnalysisPipeline-0.0.8/CHAP/runner.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.7/CHAP/server.py` & `ChessAnalysisPipeline-0.0.8/CHAP/server.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.7/CHAP/tomo/processor.py` & `ChessAnalysisPipeline-0.0.8/CHAP/tomo/processor.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,66 +16,71 @@
 # Third party modules
 import numpy as np
 
 # Local modules
 from CHAP.common.utils.general import (
     is_num,
     input_int,
+    input_num,
     input_yesno,
     select_image_bounds,
     select_one_image_bound,
     draw_mask_1d,
     clear_plot,
     clear_imshow,
     quick_plot,
     quick_imshow,
 )
-#    input_num,
 from CHAP.common.utils.fit import Fit
 from CHAP.processor import Processor
 from CHAP.reader import main
 
 NUM_CORE_TOMOPY_LIMIT = 24
 
 
 class TomoDataProcessor(Processor):
     """
-    Class representing the processes to reconstruct a set of Tomographic
-    images returning either a dictionary or a `nexusformat.nexus.NXroot`
-    object containing the (meta) data after processing each individual
-    step.
+    A processor to reconstruct a set of tomographic images returning
+    either a dictionary or a `nexusformat.nexus.NXroot` object
+    containing the (meta) data after processing each individual step.
     """
 
-    def _process(
+    def process(
             self, data, interactive=False, reduce_data=False,
             find_center=False, reconstruct_data=False, combine_data=False,
             output_folder='.', save_figs=None, **kwargs):
         """
         Process the output of a `Reader` that contains a map or a
         `nexusformat.nexus.NXroot` object and one that contains the step
         specific instructions and return either a dictionary or a
-        `nexusformat.nexus.NXroot` returning the processed result.
+        `nexusformat.nexus.NXroot` with the processed result.
 
-        :param data: Result of `Reader.read`
-        :type data: list[dict[str,object]]
-        :param interactive: Allows interactive actions
-        :type bool, optional [False]
-        :param reduce_data: Generate reduced tomography images
-        :type bool, optional [False]
-        :param find_center: Find the calibrated center axis info
-        :type bool, optional [False]
-        :param reconstruct_data: Reconstruct the tomography data
-        :type bool, optional [False]
-        :param combine_data: Combine the reconstructed tomography stacks
-        :type bool, optional [False]
-        :param output_folder: Output folder name
-        :type str, optional ['.']
-        :param save_figs: Display and/or save figures to file
+        :param data: Input configuration for the individual steps in the
+            tomographic image reduction.
+        :type data: list[PipelineData]
+        :param interactive: Allows for user interactions,
+            defaults to False.
+        :type bool, optional
+        :param reduce_data: Generate reduced tomography images,
+            defaults to False.
+        :type bool, optional
+        :param find_center: Find the calibrated center axis info,
+            defaults to False.
+        :type bool, optional
+        :param reconstruct_data: Reconstruct the tomography data,
+            defaults to False.
+        :type bool, optional
+        :param combine_data: Combine the reconstructed tomography
+            stacks, defaults to False.
+        :type bool, optional
+        :param output_folder: Output folder name, defaults to '.'.
+        :type str, optional
+        :param save_figs: Display and/or save figures to file.
         :type str, optional
-        :return: processed (meta)data
+        :return: Processed (meta)data of the last step.
         :rtype: dict or nexusformat.nexus.NXroot
         """
 
         if not isinstance(reduce_data, bool):
             raise ValueError(f'Invalid parameter reduce_data ({reduce_data})')
         if not isinstance(find_center, bool):
             raise ValueError(f'Invalid parameter find_center ({find_center})')
@@ -100,89 +105,78 @@
             configs.pop('nxroot', None)
             nxroot = self.get_nxroot(configs.pop('map'), configs.pop('setup'))
         else:
             nxroot = configs.pop('nxroot', None)
 
         # Reduce tomography images
         if reduce_data or 'reduce' in configs:
+            args = {}
             if 'reduce' in configs:
                 tool_config = configs.pop('reduce')
-                img_x_bounds = tool_config.img_x_bounds
+                args['img_x_bounds'] = tool_config.img_x_bounds
+                args['delta_theta'] = tool_config.delta_theta
             else:
-                img_x_bounds = None
                 if nxroot is None:
                     raise RuntimeError(
                         'Unable to reduce the data without providing a '
                         + 'reduced_data config file')
             if nxroot is None:
                 map_config = configs.pop('map')
                 nxroot = self.get_nxroot(map_config, tool_config)
-            nxroot = tomo.gen_reduced_data(nxroot, img_x_bounds=img_x_bounds)
+            nxroot = tomo.gen_reduced_data(nxroot, **args)
 
         # Find rotation axis centers for the tomography stacks
         # RV pass tool_config directly to tomo.find_centers?
         if find_center or 'find_center' in configs:
+            args = {}
+            run_find_centers = False
             if 'find_center' in configs:
                 tool_config = configs.pop('find_center')
-                center_rows = (tool_config.lower_row, tool_config.upper_row)
+                args['center_rows'] = (
+                    tool_config.lower_row, tool_config.upper_row)
+                args['center_stack_index'] = tool_config.center_stack_index
                 lower_center_offset = tool_config.lower_center_offset
                 upper_center_offset = tool_config.upper_center_offset
-                center_stack_index = tool_config.center_stack_index
-            else:
-                center_rows = (None, None)
-                lower_center_offset = None
-                upper_center_offset = None
-                center_stack_index = None
-            if (None in center_rows or lower_center_offset is None
-                    or upper_center_offset is None):
-                center_config = tomo.find_centers(
-                    nxroot, center_rows=center_rows,
-                    center_stack_index=center_stack_index)
+                if (None in args['center_rows'] or lower_center_offset is None
+                        or upper_center_offset is None):
+                    run_find_centers = True
+            if run_find_centers or 'find_center' not in configs:
+                center_config = tomo.find_centers(nxroot, **args)
             else:
                 # RV make a convert to dict in basemodel?
                 center_config = {
                     'lower_row': tool_config.lower_row,
                     'lower_center_offset': tool_config.lower_center_offset,
                     'upper_row': tool_config.upper_row,
                     'upper_center_offset': tool_config.upper_center_offset,
                     'center_stack_index': tool_config.center_stack_index,
                 }
 
         # Reconstruct tomography stacks
         # RV pass tool_config and center_config directly to
         #     tomo.reconstruct_data?
         if reconstruct_data or 'reconstruct' in configs:
+            args = {}
             if 'reconstruct' in configs:
                 tool_config = configs.pop('reconstruct')
-                x_bounds = tool_config.x_bounds
-                y_bounds = tool_config.y_bounds
-                z_bounds = tool_config.z_bounds
-            else:
-                x_bounds = None
-                y_bounds = None
-                z_bounds = None
-            nxroot = tomo.reconstruct_data(
-                nxroot, center_config, x_bounds=x_bounds, y_bounds=y_bounds,
-                z_bounds=z_bounds)
+                args['x_bounds'] = tool_config.x_bounds
+                args['y_bounds'] = tool_config.y_bounds
+                args['z_bounds'] = tool_config.z_bounds
+            nxroot = tomo.reconstruct_data(nxroot, center_config, **args)
             center_config = None
 
         # Combine reconstructed tomography stacks
         if combine_data or 'combine' in configs:
+            args = {}
             if 'combine' in configs:
                 tool_config = configs.pop('combine')
-                x_bounds = tool_config.x_bounds
-                y_bounds = tool_config.y_bounds
-                z_bounds = tool_config.z_bounds
-            else:
-                x_bounds = None
-                y_bounds = None
-                z_bounds = None
-            nxroot = tomo.combine_data(
-                nxroot, x_bounds=x_bounds, y_bounds=y_bounds,
-                z_bounds=z_bounds)
+                args['x_bounds'] = tool_config.x_bounds
+                args['y_bounds'] = tool_config.y_bounds
+                args['z_bounds'] = tool_config.z_bounds
+            nxroot = tomo.combine_data(nxroot, **args)
 
         if center_config is not None:
             return center_config
         return nxroot
 
     def get_configs(self, data):
         """
@@ -191,23 +185,19 @@
 
         :param data: Result of `Reader.read` where at least one item
             is of type `nexusformat.nexus.NXroot` or has the value
             `'MapConfig'` for the `'schema'` key, and at least one item
             has the value `'TomoSetupConfig'`, or `'TomoReduceConfig'`,
             or `'TomoFindCenterConfig'`, or `'TomoReconstructConfig'`,
             or `'TomoCombineConfig'` for the `'schema'` key.
-        :type data: list[dict[str,object]]
-        :raises Exception: If valid config objects cannot be constructed
-            from `data`.
+        :type data: list[PipelineData]
         :return: valid instances of the configuration objects with field
             values taken from `data`.
         :rtype: dict
         """
-        # :rtype: dict{'map': MapConfig, 'reduce': TomoReduceConfig}
-        # RV is there a way to denote optional items?
         # Third party modules
         from nexusformat.nexus import NXroot
 
         # Local modules
         from CHAP.common.models.map import MapConfig
         from CHAP.tomo.models import (
             TomoSetupConfig,
@@ -243,28 +233,29 @@
                             **(item.get('data')))
 
         return configs
 
     def get_nxroot(self, map_config, tool_config):
         """
         Get a map of the collected tomography data from the scans in
-        `map_config`. The data will be reduced based on additional
-        parameters included in `tool_config`. The data will be returned
-        along with relevant metadata in the form of a NeXus structure.
+        `map_config` and the detector info in `tool_config'.
+        The map is returned as an `nexusformat.nexus.NXroot` object.
 
-        :param map_config: the map configuration
+        :param map_config: Map configuration
         :type map_config: MapConfig
-        :param tool_config: the tomography image reduction configuration
+        :param tool_config: The tomography image reduction configuration
+            containing at minimum the detector information.
         :type tool_config: TomoReduceConfig
         :return: a map of the collected tomography data along with the
         data reduction configuration
         :rtype: nexusformat.nexus.NXroot
         """
         # System modules
         from copy import deepcopy
+        from logging import getLogger
 
         # Third party modules
         from nexusformat.nexus import (
             NXcollection,
             NXdata,
             NXdetector,
             NXinstrument,
@@ -275,14 +266,17 @@
         )
 
         # Local modules
         from CHAP.common import MapProcessor
         from CHAP.common.models.map import import_scanparser
         from CHAP.common.utils.general import index_nearest
 
+        logger = getLogger(self.__name__)
+        logger.propagate = False
+
         include_raw_data = getattr(tool_config, 'include_raw_data', False)
 
         # Construct NXroot
         nxroot = NXroot()
 
         # Construct base NXentry and add to NXroot
         nxentry = MapProcessor.get_nxentry(map_config)
@@ -332,26 +326,35 @@
             # Add an NXsample to NXentry
             # (do not fill in data fields yet)
             nxsample = NXsample()
             nxentry.sample = nxsample
             nxsample.name = map_config.sample.name
             nxsample.description = map_config.sample.description
 
-        # Add NXcollection's to NXentry to hold metadata about the spec
+        # Add NXcollection's to NXentry to hold metadata about the SPEC
         #     scans in the map
         # Also obtain the data fields in NXsample and NXdetector if
         #     requested
         import_scanparser(map_config.station, map_config.experiment_type)
         image_keys = []
         sequence_numbers = []
         image_stacks = []
         rotation_angles = []
         x_translations = []
         z_translations = []
-        for scans in map_config.spec_scans:
+        spec_scans = map_config.spec_scans
+        if map_config.station == 'id3b':
+            scan_types = len(spec_scans)*['ts1']
+            if tool_config.dark_field is not None:
+                spec_scans += tool_config.dark_field
+                scan_types.append('df1')
+            if tool_config.bright_field is not None:
+                spec_scans += tool_config.bright_field
+                scan_types.append('bf1')
+        for n, scans in enumerate(spec_scans):
             for scan_number in scans.scan_numbers:
                 scanparser = scans.get_scanparser(scan_number)
                 if map_config.station in ('id1a3', 'id3a'):
                     scan_type = scanparser.scan_type
                     if scan_type == 'df1':
                         image_key = 2
                         field_name = 'dark_field'
@@ -359,20 +362,21 @@
                         image_key = 1
                         field_name = 'bright_field'
                     elif scan_type == 'ts1':
                         image_key = 0
                         field_name = 'tomo_fields'
                     else:
                         raise RuntimeError('Invalid scan type: {scan_type}')
-                elif map_config.station in ('id3b'):
-                    if scans.spec_file.endswith('_dark'):
+                elif map_config.station == 'id3b':
+                    if (scans.spec_file.endswith('_dark')
+                            or scan_types[n] == 'df1'):
                         image_key = 2
                         field_name = 'dark_field'
-                    elif scans.spec_file.endswith('_flat'):
-                        # RV not yet tested with an actual fmb run
+                    elif (scans.spec_file.endswith('_flat')
+                            or scan_types[n] == 'bf1'):
                         image_key = 1
                         field_name = 'bright_field'
                     else:
                         image_key = 0
                         field_name = 'tomo_fields'
                 else:
                     raise RuntimeError(
@@ -391,43 +395,32 @@
                     nxentry.spec_scans[field_name] = nxcollection
                     nxcollection.attrs['spec_file'] = str(scans.spec_file)
                     nxcollection.attrs['date'] = scanparser.spec_scan.file_date
 
                 # Get thetas
                 image_offset = scanparser.starting_image_offset
                 if map_config.station in ('id1a3', 'id3a'):
-                    theta_vals = scanparser.theta_vals
-                    thetas = np.linspace(
-                        theta_vals.get('start'), theta_vals.get('end'),
-                        theta_vals.get('num'))
+                    thetas = scanparser.rotation_angles
                 else:
-                    if len(scans.scan_numbers) != 1:
-                        raise RuntimeError(
-                            'Multiple scans not yet implemented for '
-                            + f'{map_config.station}')
-                    scan_number = scans.scan_numbers[0]
-                    thetas = []
-                    for dim in map_config.independent_dimensions:
-                        if dim.label != 'theta':
-                            continue
-                        for index in range(scanparser.spec_scan_npts):
-                            thetas.append(
-                                dim.get_value(scans, scan_number, index))
-                    if not thetas:
-                        raise RuntimeError(
-                            f'Unable to obtain thetas for {field_name}')
-                    if thetas[image_offset] <= 0.0 and thetas[-1] >= 180.0:
-                        image_offset = index_nearest(thetas, 0.0)
-                        image_end = index_nearest(thetas, 180.0)
-                        thetas = thetas[image_offset:image_end]
-                    elif thetas[-1]-thetas[image_offset] >= 180:
-                        image_end = index_nearest(thetas, thetas[0]+180.0)
-                        thetas = thetas[image_offset:image_end]
-                    else:
-                        thetas = thetas[image_offset:]
+                    try:
+                        thetas = []
+                        num_theta = scanparser.spec_scan_npts
+                        for dim in map_config.independent_dimensions:
+                            if dim.label != 'theta':
+                                continue
+                            for index in range(num_theta):
+                                thetas.append(dim.get_value(
+                                    scans, scan_number, index+image_offset))
+                        thetas = np.asarray(thetas)
+                        assert thetas == scanparser.rotation_angles
+                    except:
+                        thetas = scanparser.rotation_angles
+                    if thetas[-1]-thetas[0] > 180.:
+                        image_end = index_nearest(thetas, thetas[0]+180)
+                        thetas = thetas[:image_end]
 
                 # x and z translations
                 x_translation = scanparser.horizontal_shift
                 z_translation = scanparser.vertical_shift
 
                 # Add an NXsubentry to the NXcollection for each scan
                 entry_name = f'scan_{scan_number}'
@@ -574,15 +567,15 @@
         # Third party modules
         from numexpr import set_num_threads
 
         set_num_threads(self._num_core_org)
 
 
 class Tomo:
-    """Reconstruct a set of Tomographic images."""
+    """Reconstruct a set of tomographic images."""
 
     def __init__(
             self, interactive=False, num_core=-1, output_folder='.',
             save_figs=None, test_mode=False):
         """Initialize Tomo."""
         # System modules
         from logging import getLogger
@@ -593,16 +586,16 @@
         self._logger.propagate = False
 
         if not isinstance(interactive, bool):
             raise ValueError(f'Invalid parameter interactive ({interactive})')
         self._interactive = interactive
         self._num_core = num_core
         self._output_folder = os_path.abspath(output_folder)
-        if not os_path.isdir(output_folder):
-            mkdir(os_path.abspath(output_folder))
+        if not os_path.isdir(self._output_folder):
+            mkdir(self._output_folder)
         if self._interactive:
             self._test_mode = False
         else:
             if not isinstance(test_mode, bool):
                 raise ValueError(f'Invalid parameter test_mode ({test_mode})')
             self._test_mode = test_mode
             if save_figs is None:
@@ -633,15 +626,15 @@
             raise ValueError(f'Invalid parameter num_core ({num_core})')
         if self._num_core > cpu_count():
             self._logger.warning(
                 f'num_core = {self._num_core} is larger than the number '
                 + f'of available processors and reduced to {cpu_count()}')
             self._num_core = cpu_count()
 
-    def gen_reduced_data(self, data, img_x_bounds=None):
+    def gen_reduced_data(self, data, img_x_bounds=None, delta_theta=None):
         """
         Generate the reduced tomography images.
 
         :param data: Data object containing the raw data info and
             metadata required for a tomography data reduction
         :type data: nexusformat.nexus.NXroot
         :param img_x_bounds: Detector image bounds in the x-direction
@@ -659,33 +652,14 @@
         self._logger.info('Generate the reduced tomography images')
         if img_x_bounds is not None:
             if not isinstance(img_x_bounds, (tuple, list)):
                 raise ValueError(
                     f'Invalid parameter img_x_bounds ({img_x_bounds})')
             img_x_bounds = tuple(img_x_bounds)
 
-#        if isinstance(data, dict):
-#            # Create Nexus format object from input dictionary
-#            wf = TomoWorkflow(**data)
-#            if len(wf.sample_maps) > 1:
-#                raise ValueError('Multiple sample maps not yet implemented')
-#            nxroot = NXroot()
-#            t0 = time()
-#            for sample_map in wf.sample_maps:
-#                self._logger.info(
-#                    f'Start constructing the {sample_map.title} map')
-#                import_scanparser(sample_map.station)
-#                sample_map.construct_nxentry(nxroot, include_raw_data=False)
-#            self._logger.info(
-#                f'Constructed all sample maps in {time()-t0:.2f} seconds')
-#            nxentry = nxroot[nxroot.attrs['default']]
-#            # Get test mode configuration info
-#            if self._test_mode:
-#                self._test_config = data['sample_maps'][0]['test_mode']
-#        elif isinstance(data, NXroot):
         if isinstance(data, NXroot):
             nxentry = data[data.attrs['default']]
         else:
             raise ValueError(f'Invalid parameter data ({data})')
 
         # Create an NXprocess to store data reduction (meta)data
         reduced_data = NXprocess()
@@ -693,27 +667,55 @@
         # Generate dark field
         if 'dark_field' in nxentry['spec_scans']:
             reduced_data = self._gen_dark(nxentry, reduced_data)
 
         # Generate bright field
         reduced_data = self._gen_bright(nxentry, reduced_data)
 
+        # Get rotation angles for image stacks
+        thetas = self._gen_thetas(nxentry)
+
+        # Get the image stack mask to remove bad images from stack
+        image_mask = None
+        drop_fraction = 0 # fraction of images dropped as a percentage
+        if drop_fraction:
+            if delta_theta is not None:
+                delta_theta = None
+                self._logger.warning(
+                    'Ignore delta_theta when an image mask is used')
+            np.random.seed(0)
+            image_mask = np.where(np.random.rand(
+                len(thetas)) < drop_fraction/100, 0, 1).astype(bool)
+
+        # Set zoom and/or rotation angle interval to reduce memory
+        #     requirement
+        if image_mask is None:
+            zoom_perc, delta_theta = self._set_zoom_or_delta_theta(
+                thetas, delta_theta)
+            if delta_theta is not None:
+                image_mask = np.asarray(
+                    [0 if i%delta_theta else 1
+                        for i in range(len(thetas))], dtype=bool)
+            self._logger.debug(f'zoom_perc: {zoom_perc}')
+            self._logger.debug(f'delta_theta: {delta_theta}')
+            if zoom_perc is not None:
+                reduced_data.attrs['zoom_perc'] = zoom_perc
+        if image_mask is not None:
+            self._logger.debug(f'image_mask = {image_mask}')
+            reduced_data['image_mask'] = image_mask
+            thetas = thetas[image_mask]
+        self._logger.debug(f'thetas = {thetas}')
+        reduced_data['rotation_angle'] = thetas
+
         # Set vertical detector bounds for image stack
         img_x_bounds = self._set_detector_bounds(
-            nxentry, reduced_data, img_x_bounds=img_x_bounds)
+            nxentry, reduced_data, thetas[0], img_x_bounds=img_x_bounds)
         self._logger.info(f'img_x_bounds = {img_x_bounds}')
         reduced_data['img_x_bounds'] = img_x_bounds
 
-        # Set zoom and/or theta skip to reduce memory the requirement
-        zoom_perc, num_theta_skip = self._set_zoom_or_skip()
-        if zoom_perc is not None:
-            reduced_data.attrs['zoom_perc'] = zoom_perc
-        if num_theta_skip is not None:
-            reduced_data.attrs['num_theta_skip'] = num_theta_skip
-
         # Generate reduced tomography fields
         reduced_data = self._gen_tomo(nxentry, reduced_data)
 
         # Create a copy of the input Nexus object and remove raw and
         #     any existing reduced data
         if isinstance(data, NXroot):
             exclude_items = [
@@ -743,15 +745,16 @@
             nxentry.reduced_data.data.tomo_fields, name='reduced_data')
         nxentry.data.makelink(
             nxentry.reduced_data.rotation_angle, name='rotation_angle')
         nxentry.data.attrs['signal'] = 'reduced_data'
 
         return nxroot
 
-    def find_centers(self, nxroot, center_rows=None, center_stack_index=None):
+    def find_centers(self, nxroot, center_rows=None, center_stack_index=None,
+            gaussian_sigma=None, ring_width=None):
         """
         Find the calibrated center axis info
 
         :param nxroot: Data object containing the reduced data and
             metadata required to find the calibrated center axis info
         :type data: nexusformat.nexus.NXroot
         :param center_rows: Lower and upper row indices for center
@@ -808,37 +811,37 @@
         num_tomo_stacks = tomo_fields_shape[0]
         if num_tomo_stacks == 1:
             center_stack_index = 0
             default = 'n'
         else:
             if self._test_mode:
                 # Convert input value to offset 0
-                center_stack_index = self._test_config['center_stack_index']-1
+                center_stack_index = self._test_config['center_stack_index']
             elif self._interactive:
                 if center_stack_index is None:
                     center_stack_index = input_int(
                         '\nEnter tomography stack index to calibrate the '
-                        + 'center axis', ge=1, le=num_tomo_stacks,
-                        default=int(1 + num_tomo_stacks/2))
-                center_stack_index -= 1
+                        + 'center axis', ge=0, lt=num_tomo_stacks,
+                        default=int(num_tomo_stacks/2))
             else:
                 if center_stack_index is None:
                     center_stack_index = int(num_tomo_stacks/2)
                     self._logger.warning(
                         'center_stack_index unspecified, use stack '
-                        + f'{center_stack_index+1} to find centers')
+                        + f'{center_stack_index} to find centers')
             default = 'y'
 
         # Get thetas (in degrees)
         thetas = np.asarray(nxentry.reduced_data.rotation_angle)
+        assert len(thetas) == tomo_fields_shape[1]
 
         # Get effective pixel_size
         if 'zoom_perc' in nxentry.reduced_data:
             eff_pixel_size = \
-                100.0 * (nxentry.instrument.detector.x_pixel_size
+                100. * (nxentry.instrument.detector.x_pixel_size
                          / nxentry.reduced_data.attrs['zoom_perc'])
         else:
             eff_pixel_size = nxentry.instrument.detector.x_pixel_size
 
         # Get cross sectional diameter
         cross_sectional_dim = tomo_fields_shape[3]*eff_pixel_size
         self._logger.debug(f'cross_sectional_dim = {cross_sectional_dim}')
@@ -875,15 +878,16 @@
                     raise ValueError(
                         f'Invalid parameter center_rows ({center_rows})')
         t0 = time()
         lower_center_offset = self._find_center_one_plane(
             nxentry.reduced_data.data.tomo_fields[
                 center_stack_index,:,lower_row,:],
             lower_row, thetas, eff_pixel_size, cross_sectional_dim,
-            path=self._output_folder, num_core=self._num_core)
+            path=self._output_folder, num_core=self._num_core,
+            gaussian_sigma=gaussian_sigma, ring_width=ring_width)
         self._logger.info(f'Finding center took {time()-t0:.2f} seconds')
         self._logger.debug(f'lower_row = {lower_row:.2f}')
         self._logger.debug(f'lower_center_offset = {lower_center_offset:.2f}')
 
         # Upper row center
         if self._test_mode:
             upper_row = self._test_config['upper_row']
@@ -914,40 +918,41 @@
                     raise ValueError(
                         f'Invalid parameter center_rows ({center_rows})')
         t0 = time()
         upper_center_offset = self._find_center_one_plane(
             nxentry.reduced_data.data.tomo_fields[
                 center_stack_index,:,upper_row,:],
             upper_row, thetas, eff_pixel_size, cross_sectional_dim,
-            path=self._output_folder, num_core=self._num_core)
+            path=self._output_folder, num_core=self._num_core,
+            gaussian_sigma=gaussian_sigma, ring_width=ring_width)
         self._logger.info(f'Finding center took {time()-t0:.2f} seconds')
         self._logger.debug(f'upper_row = {upper_row:.2f}')
         self._logger.debug(f'upper_center_offset = {upper_center_offset:.2f}')
 
         center_config = {
             'lower_row': lower_row,
             'lower_center_offset': lower_center_offset,
             'upper_row': upper_row,
             'upper_center_offset': upper_center_offset,
         }
         if num_tomo_stacks > 1:
-            # Save as offset 1
-            center_config['center_stack_index'] = center_stack_index+1
+            center_config['center_stack_index'] = center_stack_index
 
         # Save test data to file
         if self._test_mode:
             with open(f'{self._output_folder}/center_config.yaml', 'w',
                       encoding='utf8') as f:
                 safe_dump(center_config, f)
 
         return center_config
 
     def reconstruct_data(
             self, nxroot, center_info, x_bounds=None, y_bounds=None,
-            z_bounds=None):
+            z_bounds=None, secondary_iters=0, remove_stripe_sigma=None,
+            ring_width=None):
         """
         Reconstruct the tomography data.
 
         :param nxroot: Reduced data
         :type data: nexusformat.nexus.NXroot
         :param center_info: Calibrated center axis info
         :type center_info: dict
@@ -1031,35 +1036,37 @@
         tomo_recon_stacks = num_tomo_stacks*[np.array([])]
         for i in range(num_tomo_stacks):
             # Convert reduced data stack from theta,row,column to
             #     row,theta,column
             t0 = time()
             tomo_stack = np.asarray(nxentry.reduced_data.data.tomo_fields[i])
             self._logger.info(
-                f'Reading reduced data stack {i+1} took {time()-t0:.2f} '
+                f'Reading reduced data stack {i} took {time()-t0:.2f} '
                 + 'seconds')
             if (len(tomo_stack.shape) != 3
                     or any(True for dim in tomo_stack.shape if not dim)):
                 raise RuntimeError(
-                    f'Unable to load tomography stack {i+1} for '
+                    f'Unable to load tomography stack {i} for '
                     + 'reconstruction')
             tomo_stack = np.swapaxes(tomo_stack, 0, 1)
             assert len(thetas) == tomo_stack.shape[1]
             assert 0 <= lower_row < upper_row < tomo_stack.shape[0]
             center_offsets = [
                 lower_center_offset-lower_row*center_slope,
                 upper_center_offset + center_slope * (
                     tomo_stack.shape[0]-1-upper_row),
             ]
             t0 = time()
             tomo_recon_stack = self._reconstruct_one_tomo_stack(
                 tomo_stack, thetas, center_offsets=center_offsets,
-                num_core=self._num_core, algorithm='gridrec')
+                num_core=self._num_core, algorithm='gridrec',
+                secondary_iters=secondary_iters,
+                remove_stripe_sigma=remove_stripe_sigma, ring_width=ring_width)
             self._logger.info(
-                f'Reconstruction of stack {i+1} took {time()-t0:.2f} seconds')
+                f'Reconstruction of stack {i} took {time()-t0:.2f} seconds')
 
             # Combine stacks
             tomo_recon_stacks[i] = tomo_recon_stack
 
         # Resize the reconstructed tomography data
         #     reconstructed data order in each stack: row/z,x,y
         if self._test_mode:
@@ -1067,20 +1074,24 @@
             y_bounds = tuple(self._test_config.get('y_bounds'))
             z_bounds = None
         elif self._interactive:
             x_bounds, y_bounds, z_bounds = self._resize_reconstructed_data(
                 tomo_recon_stacks, x_bounds=x_bounds, y_bounds=y_bounds,
                 z_bounds=z_bounds)
         else:
+            if x_bounds == (-1, -1):
+                x_bounds = None
             if x_bounds is None:
                 self._logger.warning(
                     'x_bounds unspecified, reconstruct data for full x-range')
             elif not is_int_pair(x_bounds, ge=0,
                                  lt=tomo_recon_stacks[0].shape[1]):
                 raise ValueError(f'Invalid parameter x_bounds ({x_bounds})')
+            if y_bounds == (-1, -1):
+                y_bounds = None
             if y_bounds is None:
                 self._logger.warning(
                     'y_bounds unspecified, reconstruct data for full y-range')
             elif not is_int_pair(
                     y_bounds, ge=0, lt=tomo_recon_stacks[0].shape[2]):
                 raise ValueError(f'Invalid parameter y_bounds ({y_bounds})')
             z_bounds = None
@@ -1105,15 +1116,15 @@
 
         # Plot a few reconstructed image slices
         if self._save_figs:
             for i, stack in enumerate(tomo_recon_stacks):
                 if num_tomo_stacks == 1:
                     basetitle = 'recon'
                 else:
-                    basetitle = f'recon stack {i+1}'
+                    basetitle = f'recon stack {i}'
                 title = f'{basetitle} {res_title} xslice{x_slice}'
                 quick_imshow(
                     stack[z_range[0]:z_range[1],x_slice,y_range[0]:y_range[1]],
                     title=title, path=self._output_folder, save_fig=True,
                     save_only=True)
                 title = f'{basetitle} {res_title} yslice{y_slice}'
                 quick_imshow(
@@ -1127,15 +1138,15 @@
                     save_only=True)
 
         # Save test data to file
         #     reconstructed data order in each stack: row/z,x,y
         if self._test_mode:
             for i, stack in enumerate(tomo_recon_stacks):
                 np.savetxt(
-                    f'{self._output_folder}/recon_stack_{i+1}.txt',
+                    f'{self._output_folder}/recon_stack_{i}.txt',
                     stack[z_slice,x_range[0]:x_range[1],y_range[0]:y_range[1]],
                     fmt='%.6e')
 
         # Add image reconstruction to reconstructed data NXprocess
         #     reconstructed data order in each stack: row/z,x,y
         nxprocess.data = NXdata()
         nxprocess.attrs['default'] = 'data'
@@ -1374,15 +1385,15 @@
         from CHAP.common.models.map import (
             get_scanparser,
             import_scanparser,
         )
 
         # Get the dark field images
         image_key = nxentry.instrument.detector.get('image_key', None)
-        if image_key and 'data' in nxentry.instrument.detector:
+        if image_key is not None and 'data' in nxentry.instrument.detector:
             field_indices = [
                 index for index, key in enumerate(image_key) if key == 2]
             tdf_stack = nxentry.instrument.detector.data[field_indices,:,:]
             # RV the default NXtomo form does not accomodate dark field
             #     stacks
         else:
             import_scanparser(
@@ -1427,15 +1438,15 @@
                 tdf[tdf > tdf_cutoff] = np.nan
                 self._logger.debug(f'tdf_cutoff = {tdf_cutoff}')
 
         # Remove nans
         tdf_mean = np.nanmean(tdf)
         self._logger.debug(f'tdf_mean = {tdf_mean}')
         np.nan_to_num(
-            tdf, copy=False, nan=tdf_mean, posinf=tdf_mean, neginf=0.0)
+            tdf, copy=False, nan=tdf_mean, posinf=tdf_mean, neginf=0.)
 
         # Plot dark field
         if self._save_figs:
             quick_imshow(
                 tdf, title='dark field', path=self._output_folder,
                 save_fig=True, save_only=True)
 
@@ -1454,15 +1465,15 @@
         from CHAP.common.models.map import (
             get_scanparser,
             import_scanparser,
         )
 
         # Get the bright field images
         image_key = nxentry.instrument.detector.get('image_key', None)
-        if image_key and 'data' in nxentry.instrument.detector:
+        if image_key is not None and 'data' in nxentry.instrument.detector:
             field_indices = [
                 index for index, key in enumerate(image_key) if key == 1]
             tbf_stack = nxentry.instrument.detector.data[field_indices,:,:]
             # RV the default NXtomo form does not accomodate bright
             #     field stacks
         else:
             import_scanparser(
@@ -1526,15 +1537,16 @@
         # Add bright field to reduced data NXprocess
         if 'data' not in reduced_data:
             reduced_data.data = NXdata()
         reduced_data.data['bright_field'] = tbf
 
         return reduced_data
 
-    def _set_detector_bounds(self, nxentry, reduced_data, img_x_bounds=None):
+    def _set_detector_bounds(self, nxentry, reduced_data, theta,
+            img_x_bounds=None):
         """
         Set vertical detector bounds for each image stack.Right now the
         range is the same for each set in the image stack.
         """
         # Local modules
         from CHAP.common.models.map import (
             get_scanparser,
@@ -1542,22 +1554,31 @@
         )
         from CHAP.common.utils.general import is_index_range
 
         if self._test_mode:
             return tuple(self._test_config['img_x_bounds'])
 
         # Get the first tomography image and the reference heights
+        image_mask = reduced_data.get('image_mask')
+        if image_mask is None:
+            first_image_index = 0
+        else:
+            image_mask = np.asarray(image_mask)
+            first_image_index = int(np.argmax(image_mask))
         image_key = nxentry.instrument.detector.get('image_key', None)
-        if image_key and 'data' in nxentry.instrument.detector:
+        if image_key is not None and 'data' in nxentry.instrument.detector:
             field_indices = [
                 index for index, key in enumerate(image_key) if key == 0]
-            first_image = np.asarray(
-                nxentry.instrument.detector.data[field_indices[0],:,:])
-            theta = float(nxentry.sample.rotation_angle[field_indices[0]])
-            z_translation_all = nxentry.sample.z_translation[field_indices]
+            field_indices_masked = field_indices[image_mask]
+            first_image = np.asarray(nxentry.instrument.detector.data[
+                field_indices[first_image_index,:,:]])
+            assert theta == float(nxentry.sample.rotation_angle[
+                field_indices[first_image_index]])
+            z_translation_all = \
+                nxentry.sample.z_translation[field_indices_masked]
             vertical_shifts = sorted(list(set(z_translation_all)))
             num_tomo_stacks = len(vertical_shifts)
         else:
             import_scanparser(
                 nxentry.instrument.source.attrs['station'],
                 nxentry.instrument.source.attrs['experiment_type'])
             tomo_field_scans = nxentry.spec_scans.tomo_fields
@@ -1570,19 +1591,20 @@
                 scanparser = get_scanparser(
                     tomo_field_scans.attrs['spec_file'], scan_number)
                 image_offset = int(
                     nxsubentry[1].instrument.detector.frame_start_number)
                 vertical_shifts.append(nxsubentry[1].sample.z_translation)
                 if i == center_stack_index:
                     first_image = scanparser.get_detector_data(
-                        detector_prefix, image_offset)
-                    theta = float(nxsubentry[1].sample.rotation_angle[0])
+                        detector_prefix, image_offset+first_image_index)
+                    assert theta == float(
+                        nxsubentry[1].sample.rotation_angle[first_image_index])
 
         # Select image bounds
-        title = f'tomography image at theta = {round(theta, 2)+0}'
+        title = f'tomography image at theta={round(theta, 2)+0}'
         if img_x_bounds == (-1, -1):
             img_x_bounds = None
         if img_x_bounds is not None:
             if is_index_range(img_x_bounds, ge=0, le=first_image.shape[0]):
                 return img_x_bounds
             if self._interactive:
                 self._logger.warning(
@@ -1623,25 +1645,25 @@
                     # Set the default range to enclose the full fitted
                     #     window
                     x_low = int(x_low_fit)
                     x_upp = int(x_upp_fit)
                 else:
                     # Center a default range of 1 mm
                     # RV can we get this from the slits?
-                    num_x_min = int((1.0 - 0.5*pixel_size) / pixel_size)
+                    num_x_min = int((1. + 0.5*pixel_size) / pixel_size)
                     x_low = int((tbf_shape[0]-num_x_min) / 2)
                     x_upp = x_low+num_x_min
             else:
                 # Get the default range from the reference heights
                 delta_z = vertical_shifts[1]-vertical_shifts[0]
                 for i in range(2, num_tomo_stacks):
                     delta_z = min(
                         delta_z, vertical_shifts[i]-vertical_shifts[i-1])
                 self._logger.debug(f'delta_z = {delta_z}')
-                num_x_min = int((delta_z - 0.5*pixel_size) / pixel_size)
+                num_x_min = int((delta_z + 0.5*pixel_size) / pixel_size)
                 self._logger.debug(f'num_x_min = {num_x_min}')
                 if num_x_min > tbf_shape[0]:
                     self._logger.warning(
                         'Image bounds and pixel size prevent seamless '
                         + 'stacking')
                 if have_fit:
                     # Center the default range relative to the fitted
@@ -1679,22 +1701,22 @@
                 clear_plot('sum over theta and y')
                 if accept:
                     img_x_bounds = (x_low, x_upp)
                 else:
                     while True:
                         _, img_x_bounds = draw_mask_1d(
                             x_sum, title='select x data range',
-                            legend='sum over theta and y')
+                            ylabel='sum over theta and y')
                         if len(img_x_bounds) == 1:
                             break
                         print('Choose a single connected data range')
                     img_x_bounds = tuple(img_x_bounds[0])
             if (num_tomo_stacks > 1
                     and (img_x_bounds[1]-img_x_bounds[0]+1)
-                    < int((delta_z - 0.5*pixel_size) / pixel_size)):
+                         < int((delta_z - 0.5*pixel_size) / pixel_size)):
                 self._logger.warning(
                     'Image bounds and pixel size prevent seamless stacking')
         else:
             if num_tomo_stacks > 1:
                 raise NotImplementedError(
                     'Selecting image bounds for multiple stacks on FMB')
             # For FMB: use the first tomography image to select range
@@ -1733,40 +1755,98 @@
                 ([x_upp, x_upp], [x_sum_min, x_sum_max], 'r-'),
                 title='sum over theta and y', path=self._output_folder,
                 save_fig=True, save_only=True)
             del tmp
 
         return img_x_bounds
 
-    def _set_zoom_or_skip(self):
+    def _gen_thetas(self, nxentry):
+        """Get the rotation angles for the image stacks."""
+
+        # Get the rotation angles
+        image_key = nxentry.instrument.detector.get('image_key', None)
+        if image_key is not None and 'data' in nxentry.instrument.detector:
+            field_indices_all = [
+                index for index, key in enumerate(image_key) if key == 0]
+            z_translation_all = nxentry.sample.z_translation[field_indices_all]
+            z_translation_levels = sorted(list(set(z_translation_all)))
+            thetas = None
+            for i, z_translation in enumerate(z_translation_levels):
+                field_indices = [
+                    field_indices_all[index]
+                    for index, z in enumerate(z_translation_all)
+                    if z == z_translation]
+                sequence_numbers = \
+                    nxentry.instrument.detector.sequence_number[field_indices]
+                assert (list(sequence_numbers)
+                        == list(range((len(sequence_numbers)))))
+                if thetas is None:
+                    thetas = np.asarray(
+                        nxentry.sample.rotation_angle[
+                            field_indices])[sequence_numbers]
+                else:
+                    assert all(
+                        thetas[i] == nxentry.sample.rotation_angle[
+                            field_indices[index]]
+                        for i, index in enumerate(sequence_numbers))
+        else:
+            tomo_field_scans = nxentry.spec_scans.tomo_fields
+            thetas = None
+            for nxsubentry_name, nxsubentry in tomo_field_scans.items():
+                if thetas is None:
+                    thetas = np.asarray(nxsubentry.sample.rotation_angle)
+                else:
+                    assert all(
+                        thetas[i] == theta for i, theta
+                            in enumerate(nxsubentry.sample.rotation_angle))
+
+        return thetas
+
+    def _set_zoom_or_delta_theta(self, thetas, delta_theta=None):
         """
-        Set zoom and/or theta skip to reduce memory the requirement
+        Set zoom and/or delta theta to reduce memory the requirement
         for the analysis.
         """
+        # Local modules
+        from CHAP.common.utils.general import index_nearest
+
+        if self._test_mode:
+            return tuple(self._test_config['delta_theta'])
+
 #        if input_yesno(
 #                '\nDo you want to zoom in to reduce memory '
 #                + 'requirement (y/n)?', 'n'):
 #            zoom_perc = input_int(
 #                '    Enter zoom percentage', ge=1, le=100)
 #        else:
 #            zoom_perc = None
         zoom_perc = None
-#        if input_yesno(
-#                'Do you want to skip thetas to reduce memory '
-#                + 'requirement (y/n)?', 'n'):
-#            num_theta_skip = input_int(
-#                '    Enter the number skip theta interval',
-#                ge=0, lt=num_theta)
-#        else:
-#            num_theta_skip = None
-        num_theta_skip = None
-        self._logger.debug(f'zoom_perc = {zoom_perc}')
-        self._logger.debug(f'num_theta_skip = {num_theta_skip}')
 
-        return zoom_perc, num_theta_skip
+        if delta_theta is not None and not is_num(delta_theta, gt=0):
+            self._logger.warning(
+                f'Invalid parameter delta_theta ({delta_theta}), '
+                + 'ignoring delta_theta')
+            delta_theta = None
+        if self._interactive:
+            if delta_theta is None:
+                delta_theta = thetas[1]-thetas[0]
+            print(f'Available theta range: [{thetas[0]}, {thetas[-1]}]')
+            print(f'Current theta interval: {delta_theta}')
+            if input_yesno(
+                    'Do you want to change the theta interval to reduce the '
+                    + 'memory requirement (y/n)?', 'n'):
+                delta_theta = input_num(
+                    '    Enter the desired theta interval',
+                    ge=thetas[1]-thetas[0], lt=(thetas[-1]-thetas[0])/2)
+        if delta_theta is not None:
+            delta_theta = index_nearest(thetas, thetas[0]+delta_theta)
+            if delta_theta <= 1:
+                delta_theta = None
+
+        return zoom_perc, delta_theta
 
     def _gen_tomo(self, nxentry, reduced_data):
         """Generate tomography fields."""
         # Third party modules
         from numexpr import evaluate
         from scipy.ndimage import zoom
 
@@ -1783,113 +1863,120 @@
         # Get image bounds
         img_x_bounds = tuple(
             reduced_data.get('img_x_bounds', (0, tbf_shape[0])))
         img_y_bounds = tuple(
             reduced_data.get('img_y_bounds', (0, tbf_shape[1])))
 
         # Get resized dark field
-#        if 'dark_field' in data:
-#            tbf = np.asarray(
-#                reduced_data.data.dark_field[
-#                    img_x_bounds[0]:img_x_bounds[1],
-#                    img_y_bounds[0]:img_y_bounds[1]])
-#        else:
-#            self._logger.warning('Dark field unavailable')
-#            tdf = None
-        tdf = None
+        if 'dark_field' in reduced_data.data:
+            tdf = np.asarray(
+                reduced_data.data.dark_field[
+                    img_x_bounds[0]:img_x_bounds[1],
+                    img_y_bounds[0]:img_y_bounds[1]])
+        else:
+            self._logger.warning('Dark field unavailable')
+            tdf = None
 
         # Resize bright field
         if (img_x_bounds != (0, tbf.shape[0])
                 or img_y_bounds != (0, tbf.shape[1])):
             tbf = tbf[
                 img_x_bounds[0]:img_x_bounds[1],
                 img_y_bounds[0]:img_y_bounds[1]]
 
+        # Get thetas (in degrees)
+        thetas = np.asarray(reduced_data.rotation_angle)
+
+        # Get or create image mask
+        image_mask = reduced_data.get('image_mask')
+        if image_mask is None:
+            image_mask = np.ones(len(thetas), dtype=bool)
+        else:
+            image_mask = np.asarray(image_mask)
+#        exit(f'image_mask {type(image_mask)} {len(image_mask)}: {image_mask}')
+
         # Get the tomography images
         image_key = nxentry.instrument.detector.get('image_key', None)
-        if image_key and 'data' in nxentry.instrument.detector:
+        if image_key is not None and 'data' in nxentry.instrument.detector:
             field_indices_all = [
                 index for index, key in enumerate(image_key) if key == 0]
             z_translation_all = nxentry.sample.z_translation[field_indices_all]
             z_translation_levels = sorted(list(set(z_translation_all)))
             num_tomo_stacks = len(z_translation_levels)
             tomo_stacks = num_tomo_stacks*[np.array([])]
             horizontal_shifts = []
             vertical_shifts = []
-            thetas = None
             tomo_stacks = []
             for i, z_translation in enumerate(z_translation_levels):
                 field_indices = [
                     field_indices_all[index]
                     for index, z in enumerate(z_translation_all)
                     if z == z_translation]
-                horizontal_shift = list(
-                    set(nxentry.sample.x_translation[field_indices]))
+                field_indices_masked = field_indices[image_mask]
+                horizontal_shift = np.asarray(
+                    set(nxentry.sample.x_translation[field_indices_masked]))
                 assert len(horizontal_shift) == 1
-                horizontal_shifts += horizontal_shift
-                vertical_shift = list(
-                    set(nxentry.sample.z_translation[field_indices]))
+                horizontal_shifts += list(horizontal_shift)
+                vertical_shift = np.asarray(
+                    set(nxentry.sample.z_translation[field_indices_masked]))
                 assert len(vertical_shift) == 1
                 vertical_shifts += vertical_shift
                 sequence_numbers = nxentry.instrument.detector.sequence_number[
                     field_indices]
-                if thetas is None:
-                    thetas = np.asarray(
-                        nxentry.sample.rotation_angle[
-                            field_indices])[sequence_numbers]
-                else:
-                    assert all(
-                        thetas[i] == nxentry.sample.rotation_angle[
-                            field_indices[index]]
-                        for i, index in enumerate(sequence_numbers))
-                assert (list(set(sequence_numbers))
-                        == list(np.arange(0, (len(sequence_numbers)))))
                 if (list(sequence_numbers)
-                        == list(np.arange(0, (len(sequence_numbers))))):
+                        == list(range((len(sequence_numbers))))):
                     tomo_stack = np.asarray(
-                        nxentry.instrument.detector.data[field_indices])
+                        nxentry.instrument.detector.data[
+                            field_indices_masked])
                 else:
                     raise RuntimeError('Unable to load the tomography images')
                 tomo_stacks.append(tomo_stack)
         else:
             import_scanparser(
                 nxentry.instrument.source.attrs['station'],
                 nxentry.instrument.source.attrs['experiment_type'])
             tomo_field_scans = nxentry.spec_scans.tomo_fields
             num_tomo_stacks = len(tomo_field_scans.keys())
             detector_prefix = str(nxentry.instrument.detector.local_name)
-            thetas = None
             tomo_stacks = []
             horizontal_shifts = []
             vertical_shifts = []
             for nxsubentry_name, nxsubentry in tomo_field_scans.items():
                 scan_number = int(nxsubentry_name.split('_')[-1])
                 scanparser = get_scanparser(
                     tomo_field_scans.attrs['spec_file'], scan_number)
                 image_offset = int(
                     nxsubentry.instrument.detector.frame_start_number)
-                if thetas is None:
-                    thetas = np.asarray(nxsubentry.sample.rotation_angle)
-                num_image = len(thetas)
-                tomo_stacks.append(
-                    scanparser.get_detector_data(
-                        detector_prefix,
-                        (image_offset, image_offset+num_image)))
-                horizontal_shifts.append(nxsubentry.sample.x_translation)
-                vertical_shifts.append(nxsubentry.sample.z_translation)
+                tomo_stack = []
+                n = 0
+                for i in range(image_mask.size):
+                    if image_mask[i]:
+                        tomo_stack.append(
+                            scanparser.get_detector_data(
+                                detector_prefix, image_offset+n))
+                        n += 1
+                tomo_stacks.append(np.asarray(tomo_stack))
+                horizontal_shift = float(nxsubentry.sample.x_translation)
+                horizontal_shifts.append(horizontal_shift)
+                vertical_shift = float(nxsubentry.sample.z_translation)
+                vertical_shifts.append(vertical_shift)
 
         reduced_tomo_stacks = []
         for i, tomo_stack in enumerate(tomo_stacks):
             # Resize the tomography images
             # Right now the range is the same for each set in the stack
-            if (img_x_bounds != (0, tbf.shape[0])
-                    or img_y_bounds != (0, tbf.shape[1])):
+            assert len(thetas) == tomo_stack.shape[0]
+            if (img_x_bounds == (0, tbf.shape[0])
+                    and img_y_bounds == (0, tbf.shape[1])):
+                tomo_stack = tomo_stack.astype('float64', copy=False)
+            else:
                 tomo_stack = tomo_stack[
                     :,img_x_bounds[0]:img_x_bounds[1],
-                    img_y_bounds[0]:img_y_bounds[1]].astype('float64')
+                    img_y_bounds[0]:img_y_bounds[1]].astype(
+                        'float64', copy=False)
 
             # Subtract dark field
             if tdf is not None:
                 try:
                     with SetNumexprThreads(self._num_core):
                         evaluate('tomo_stack-tdf', out=tomo_stack)
                 except TypeError as e:
@@ -1921,21 +2008,20 @@
             with SetNumexprThreads(self._num_core):
                 evaluate('-log(tomo_stack)', out=tomo_stack)
 
             # Get rid of nans/infs that may be introduced by normalization
             np.where(np.isfinite(tomo_stack), tomo_stack, 0.)
 
             # Downsize tomography stack to smaller size
-            # RV use theta_skip as well
-            tomo_stack = tomo_stack.astype('float32')
+            tomo_stack = tomo_stack.astype('float32', copy=False)
             if not self._test_mode:
                 if len(tomo_stacks) == 1:
                     title = f'red fullres theta {round(thetas[0], 2)+0}'
                 else:
-                    title = f'red stack {i+1} fullres theta ' \
+                    title = f'red stack {i} fullres theta ' \
                         + f'{round(thetas[0], 2)+0}'
                 quick_imshow(
                     tomo_stack[0,:,:], title=title, path=self._output_folder,
                     save_fig=self._save_figs, save_only=self._save_only,
                     block=self._block)
 #                if not self._block:
 #                    clear_imshow(title)
@@ -1960,45 +2046,51 @@
 #                    if not self._block:
 #                        clear_imshow(title)
 
             # Save test data to file
             if self._test_mode:
                 row_index = int(tomo_stack.shape[1]/2)
                 np.savetxt(
-                    f'{self._output_folder}/red_stack_{i+1}.txt',
+                    f'{self._output_folder}/red_stack_{i}.txt',
                     tomo_stack[:,row_index,:], fmt='%.6e')
 
             # Combine resized stacks
             reduced_tomo_stacks.append(tomo_stack)
 
         # Add tomo field info to reduced data NXprocess
-        reduced_data['rotation_angle'] = thetas
         reduced_data['x_translation'] = np.asarray(horizontal_shifts)
         reduced_data['z_translation'] = np.asarray(vertical_shifts)
         reduced_data.data['tomo_fields'] = np.asarray(reduced_tomo_stacks)
 
         if tdf is not None:
             del tdf
         del tbf
 
         return reduced_data
 
     def _find_center_one_plane(
             self, sinogram, row, thetas, eff_pixel_size, cross_sectional_dim,
-            path=None, num_core=1):  # , tol=0.1):
+            path=None, num_core=1, gaussian_sigma=None, ring_width=None):
         """Find center for a single tomography plane."""
+        # Third party modules
         from tomopy import find_center_vo
 
         # Try automatic center finding routines for initial value
         # sinogram index order: theta,column
         # need column,theta for iradon, so take transpose
         sinogram = np.asarray(sinogram)
         sinogram_t = sinogram.T
         center = sinogram.shape[1]/2
 
+#        quick_imshow(
+#            sinogram_t, f'sinogram row{row}',
+#            aspect='auto', path=self._output_folder,
+#            save_fig=self._save_figs, save_only=self._save_only,
+#            block=self._block)
+
         # Try using Nghia Vo’s method
         t0 = time()
         if num_core > NUM_CORE_TOMOPY_LIMIT:
             self._logger.debug(
                 f'Running find_center_vo on {NUM_CORE_TOMOPY_LIMIT} cores ...')
             tomo_center = find_center_vo(
                 sinogram, ncore=NUM_CORE_TOMOPY_LIMIT)
@@ -2010,20 +2102,21 @@
         center_offset_vo = tomo_center-center
         self._logger.info(
             f'Center at row {row} using Nghia Vo’s method = '
             + f'{center_offset_vo:.2f}')
         t0 = time()
         recon_plane = self._reconstruct_one_plane(
             sinogram_t, tomo_center, thetas, eff_pixel_size,
-            cross_sectional_dim, False, num_core)
+            cross_sectional_dim, False, num_core, gaussian_sigma, ring_width)
         self._logger.info(
             f'Reconstructing row {row} took {time()-t0:.2f} seconds')
 
-        title = f'edges row{row} center offset{center_offset_vo:.2f} Vo'
-        self._plot_edges_one_plane(recon_plane, title, path=path)
+        if self._save_figs:
+            title = f'edges row{row} center offset{center_offset_vo:.2f} Vo'
+            self._plot_edges_one_plane(recon_plane, title, path=path)
 
         # Try using phase correlation method
 #        if input_yesno('
 #                Try finding center using phase correlation (y/n)?',
 #                'n'):
 #            t0 = time()
 #            tomo_center = find_center_pc(
@@ -2040,15 +2133,15 @@
 #            center_offset = tomo_center-center
 #            print(
 #                f'Center at row {row} using phase correlation = '
 #                + f'{center_offset:.2f}')
 #            t0 = time()
 #            recon_plane = self._reconstruct_one_plane(
 #                sinogram_t, tomo_center, thetas, eff_pixel_size,
-#                cross_sectional_dim, False, num_core)
+#                cross_sectional_dim, False, num_core, gaussian_sigma, ring_width)
 #            self._logger.info(
 #                f'Reconstructing row {row} took {time()-t0:.2f} seconds')
 #
 #            title = \
 #                f'edges row{row} center_offset{center_offset:.2f} PC'
 #            self._plot_edges_one_plane(recon_plane, title, path=path)
 
@@ -2079,15 +2172,15 @@
 #                center_offset_low, center_offset_upp, num_center_offset)
 #            for center_offset in center_offsets:
 #                if center_offset == center_offset_vo:
 #                    continue
 #                t0 = time()
 #                recon_plane = self._reconstruct_one_plane(
 #                    sinogram_t, center_offset+center, thetas, eff_pixel_size,
-#                    cross_sectional_dim, False, num_core)
+#                    cross_sectional_dim, False, num_core, gaussian_sigma, ring_width)
 #                self._logger.info(
 #                    f'Reconstructing center_offset {center_offset} took '
 #                    + 'f{time()-t0:.2f} seconds')
 #                title = f'edges row{row} center_offset{center_offset:.2f}'
 #                self._plot_edges_one_plane(recon_plane, title, path=path)
 #            if input_int('\nContinue (0) or end the search (1)', ge=0, le=1):
 #                break
@@ -2098,31 +2191,33 @@
 #            '    Enter chosen center offset', ge=-center, le=center)
         center_offset = center_offset_vo
 
         return float(center_offset)
 
     def _reconstruct_one_plane(
             self, tomo_plane_t, center, thetas, eff_pixel_size,
-            cross_sectional_dim, plot_sinogram=True, num_core=1):
+            cross_sectional_dim, plot_sinogram=True, num_core=1,
+            gaussian_sigma=None, ring_width=None):
         """Invert the sinogram for a single tomography plane."""
+        # Third party modules
         from scipy.ndimage import gaussian_filter
         from skimage.transform import iradon
         from tomopy import misc
 
         # tomo_plane_t index order: column,theta
         assert 0 <= center < tomo_plane_t.shape[0]
         center_offset = center-tomo_plane_t.shape[0]/2
         two_offset = 2 * int(np.round(center_offset))
         two_offset_abs = np.abs(two_offset)
         # Add 10% slack to max_rad to avoid edge effects
         max_rad = int(0.55 * (cross_sectional_dim/eff_pixel_size))
         if max_rad > 0.5*tomo_plane_t.shape[0]:
             max_rad = 0.5*tomo_plane_t.shape[0]
         dist_from_edge = max(1, int(np.floor(
-            (tomo_plane_t.shape[0] - two_offset_abs) / 2.0) - max_rad))
+            (tomo_plane_t.shape[0] - two_offset_abs) / 2.) - max_rad))
         if two_offset >= 0:
             self._logger.debug(
                 f'sinogram range = [{two_offset+dist_from_edge}, '
                 + f'{-dist_from_edge}]')
             sinogram = tomo_plane_t[
                 two_offset+dist_from_edge:-dist_from_edge,:]
         else:
@@ -2140,53 +2235,39 @@
         # Inverting sinogram
         t0 = time()
         recon_sinogram = iradon(sinogram, theta=thetas, circle=True)
         self._logger.info(f'Inverting sinogram took {time()-t0:.2f} seconds')
         del sinogram
 
         # Performing Gaussian filtering and removing ring artifacts
-        recon_parameters = None  # self._config.get('recon_parameters')
-        if recon_parameters is None:
-            sigma = 1.0
-            ring_width = 15
-        else:
-            sigma = recon_parameters.get('gaussian_sigma', 1.0)
-            if not is_num(sigma, ge=0.0):
-                self._logger.warning(
-                    f'Invalid gaussian_sigma ({sigma}) in '
-                    + '_reconstruct_one_plane, set to a default of 1.0')
-                sigma = 1.0
-            ring_width = recon_parameters.get('ring_width', 15)
-            if not isinstance(ring_width, int) or ring_width < 0:
-                self._logger.warning(
-                    f'Invalid ring_width ({ring_width}) in '
-                    + '_reconstruct_one_plane, set to a default of 15')
-                ring_width = 15
-        recon_sinogram = gaussian_filter(
-            recon_sinogram, sigma, mode='nearest')
+        if gaussian_sigma is not None:
+            recon_sinogram = gaussian_filter(
+                recon_sinogram, gaussian_sigma, mode='nearest')
         recon_clean = np.expand_dims(recon_sinogram, axis=0)
         del recon_sinogram
-        recon_clean = misc.corr.remove_ring(
-            recon_clean, rwidth=ring_width, ncore=num_core)
+        if ring_width is not None:
+            recon_clean = misc.corr.remove_ring(
+                recon_clean, rwidth=ring_width, ncore=num_core)
 
         return recon_clean
 
     def _plot_edges_one_plane(self, recon_plane, title, path=None):
         """
         Create an "edges plot" for a singled reconstructed tomography
         data plane.
         """
+        # Third party modules
         from skimage.restoration import denoise_tv_chambolle
 
         vis_parameters = None  # self._config.get('vis_parameters')
         if vis_parameters is None:
             weight = 0.1
         else:
             weight = vis_parameters.get('denoise_weight', 0.1)
-            if not is_num(weight, ge=0.0):
+            if not is_num(weight, ge=0.):
                 self._logger.warning(
                     f'Invalid weight ({weight}) in _plot_edges_one_plane, '
                     + 'set to a default of 0.1')
                 weight = 0.1
         edges = denoise_tv_chambolle(recon_plane, weight=weight)
         vmax = np.max(edges[0,:,:])
         vmin = -vmax
@@ -2200,15 +2281,16 @@
             edges[0,:,:], f'{title} gray', path=path, cmap='gray', vmin=vmin,
             vmax=vmax, save_fig=self._save_figs, save_only=self._save_only,
             block=self._block)
         del edges
 
     def _reconstruct_one_tomo_stack(
             self, tomo_stack, thetas, center_offsets=None, num_core=1,
-            algorithm='gridrec'):
+            algorithm='gridrec', secondary_iters=0, remove_stripe_sigma=None,
+            ring_width=None):
         """Reconstruct a single tomography stack."""
         # Third party modules
         from tomopy import (
             astra,
             misc,
             prep,
             recon,
@@ -2233,48 +2315,23 @@
             if center_offsets.size != tomo_stack.shape[0]:
                 raise RuntimeError(
                     'center_offsets dimension mismatch in '
                     + 'reconstruct_one_tomo_stack')
             centers = center_offsets
         centers += tomo_stack.shape[2]/2
 
-        # Get reconstruction parameters
-        recon_parameters = None  # self._config.get('recon_parameters')
-        if recon_parameters is None:
-            sigma = 2.0
-            secondary_iters = 0
-            ring_width = 15
-        else:
-            sigma = recon_parameters.get('stripe_fw_sigma', 2.0)
-            if not is_num(sigma, ge=0):
-                self._logger.warning(
-                    f'Invalid stripe_fw_sigma ({sigma}) in '
-                    + '_reconstruct_one_tomo_stack, set to a default of 2.0')
-                ring_width = 15
-            secondary_iters = recon_parameters.get('secondary_iters', 0)
-            if not isinstance(secondary_iters, int) or secondary_iters < 0:
-                self._logger.warning(
-                    f'Invalid secondary_iters ({secondary_iters}) in '
-                    + '_reconstruct_one_tomo_stack, set to a default of 0 '
-                    + '(i.e., skip them)')
-                ring_width = 0
-            ring_width = recon_parameters.get('ring_width', 15)
-            if not isinstance(ring_width, int) or ring_width < 0:
-                self._logger.warning(
-                    f'Invalid ring_width ({ring_width}) in '
-                    + '_reconstruct_one_plane, set to a default of 15')
-                ring_width = 15
-
         # Remove horizontal stripe
-        if num_core > NUM_CORE_TOMOPY_LIMIT:
-            tomo_stack = prep.stripe.remove_stripe_fw(
-                tomo_stack, sigma=sigma, ncore=NUM_CORE_TOMOPY_LIMIT)
-        else:
-            tomo_stack = prep.stripe.remove_stripe_fw(
-                tomo_stack, sigma=sigma, ncore=num_core)
+        if remove_stripe_sigma is not None:
+            if num_core > NUM_CORE_TOMOPY_LIMIT:
+                tomo_stack = prep.stripe.remove_stripe_fw(
+                    tomo_stack, sigma=remove_stripe_sigma,
+                    ncore=NUM_CORE_TOMOPY_LIMIT)
+            else:
+                tomo_stack = prep.stripe.remove_stripe_fw(
+                    tomo_stack, sigma=remove_stripe_sigma, ncore=num_core)
 
         # Perform initial image reconstruction
         self._logger.debug('Performing initial image reconstruction')
         t0 = time()
         tomo_recon_stack = recon(
             tomo_stack, np.radians(thetas), centers, sinogram_order=True,
             algorithm=algorithm, ncore=num_core)
@@ -2318,17 +2375,18 @@
                 init_recon=tomo_recon_stack, options=options,
                 sinogram_order=True, algorithm=astra, ncore=num_core)
             self._logger.info(
                 f'Performing secondary iterations took {time()-t0:.2f} '
                 + 'seconds')
 
         # Remove ring artifacts
-        misc.corr.remove_ring(
-            tomo_recon_stack, rwidth=ring_width, out=tomo_recon_stack,
-            ncore=num_core)
+        if ring_width is not None:
+            misc.corr.remove_ring(
+                tomo_recon_stack, rwidth=ring_width, out=tomo_recon_stack,
+                ncore=num_core)
 
         return tomo_recon_stack
 
     def _resize_reconstructed_data(
             self, data, x_bounds=None, y_bounds=None, z_bounds=None,
             z_only=False):
         """Resize the reconstructed tomography data."""
@@ -2357,20 +2415,20 @@
             else:
                 accept = False
                 index_ranges = None
                 while not accept:
                     _, x_bounds = draw_mask_1d(
                         tomosum, current_index_ranges=index_ranges,
                         title='select x data range',
-                        legend='recon stack sum yz')
+                        ylabel='sum yz')
                     while len(x_bounds) != 1:
                         print('Please select exactly one continuous range')
                         _, x_bounds = draw_mask_1d(
                             tomosum, title='select x data range',
-                            legend='recon stack sum yz')
+                            ylabel='sum yz')
                     x_bounds = x_bounds[0]
                     accept = True
             self._logger.debug(f'x_bounds = {x_bounds}')
 
         if y_bounds == (-1, -1):
             y_bounds = None
         elif not z_only and y_bounds is None:
@@ -2385,20 +2443,20 @@
             else:
                 accept = False
                 index_ranges = None
                 while not accept:
                     _, y_bounds = draw_mask_1d(
                         tomosum, current_index_ranges=index_ranges,
                         title='select x data range',
-                        legend='recon stack sum xz')
+                        ylabel='sum xz')
                     while len(y_bounds) != 1:
                         print('Please select exactly one continuous range')
                         _, y_bounds = draw_mask_1d(
                             tomosum, title='select x data range',
-                            legend='recon stack sum xz')
+                            ylabel='sum xz')
                     y_bounds = y_bounds[0]
                     accept = True
             self._logger.debug(f'y_bounds = {y_bounds}')
 
         # Selecting z bounds (in xy-plane)
         # (only valid for a single image stack)
         if z_bounds == (-1, -1):
@@ -2414,22 +2472,709 @@
             else:
                 accept = False
                 index_ranges = None
                 while not accept:
                     _, z_bounds = draw_mask_1d(
                         tomosum, current_index_ranges=index_ranges,
                         title='select x data range',
-                        legend='recon stack sum xy')
+                        ylabel='sum xy')
                     while len(z_bounds) != 1:
                         print('Please select exactly one continuous range')
                         _, z_bounds = draw_mask_1d(
                             tomosum, title='select x data range',
-                            legend='recon stack sum xy')
+                            ylabel='sum xy')
                     z_bounds = z_bounds[0]
                     accept = True
             self._logger.debug(f'z_bounds = {z_bounds}')
 
         return x_bounds, y_bounds, z_bounds
 
 
+class TomoSimFieldProcessor(Processor):
+    """
+    Class representing the process to create a simulated tomography
+    data set returning a `nexusformat.nexus.NXroot` object containing
+    the simulated tomography detector images.
+    """
+
+    def process(self, data, **kwargs):
+        # Third party modules
+        from nexusformat.nexus import (
+            NXdetector,
+            NXentry,
+            NXinstrument,
+            NXroot,
+            NXsample,
+            NXsource,
+        )
+
+        # Get and validate the relevant configuration object in data
+        config = self.get_configs(data)
+
+        station = config.station
+        sample_type = config.sample_type
+        sample_size = config.sample_size
+        if len(sample_size) == 1:
+            sample_size = (sample_size[0], sample_size[0])
+        wall_thickness = config.wall_thickness
+        mu = config.mu
+        theta_step = config.theta_step
+        beam_intensity = config.beam_intensity
+        background_intensity = config.background_intensity
+        slit_size = config.slit_size
+        pixel_size = config.detector.pixel_size
+        if len(pixel_size) == 1:
+            pixel_size = (
+                pixel_size[0]/config.detector.lens_magnification,
+                pixel_size[0]/config.detector.lens_magnification,
+            )
+        else:
+            pixel_size = (
+                pixel_size[0]/config.detector.lens_magnification,
+                pixel_size[1]/config.detector.lens_magnification,
+            )
+        detector_size = (config.detector.rows, config.detector.columns)
+        if slit_size-0.5*pixel_size[0] > detector_size[0]*pixel_size[0]:
+            raise ValueError(
+                f'Slit size ({slit_size}) larger than detector height '
+                f'({detector_size[0]*pixel_size[0]})')
+
+        # Get the rotation angles (start at a arbitrarily choose angle
+        #    and add thetas for a full 360 degrees rotation series)
+        if station in ('id1a3', 'id3a'):
+            theta_start = 0.
+        else:
+            theta_start = -17
+        theta_end = theta_start + 360.
+        thetas = list(
+            np.arange(theta_start, theta_end+0.5*theta_step, theta_step))
+
+        # Get the number of horizontal stacks bases on the diagonal
+        #     of the square and for now don't allow more than one
+        num_tomo_stack = 1 + int((sample_size[1]*np.sqrt(2)-pixel_size[1])
+                                 / (detector_size[1]*pixel_size[1]))
+        if num_tomo_stack > 1:
+            raise ValueError('Sample is too wide for the detector')
+
+        # Create the x-ray path length through a solid square
+        #     crosssection for a set of rotation angles.
+        path_lengths_solid = self._create_pathlength_solid_square(
+                sample_size[1], thetas, pixel_size[1], detector_size[1])
+
+        # Create the x-ray path length through a hollow square
+        #     crosssection for a set of rotation angles.
+        path_lengths_hollow = None
+        if sample_type in ('square_pipe', 'hollow_cube', 'hollow_brick'):
+            path_lengths_hollow = path_lengths_solid \
+                - self._create_pathlength_solid_square(
+                    sample_size[1] - 2*wall_thickness, thetas,
+                    pixel_size[1], detector_size[1])
+
+        # Get the number of stacks
+        num_tomo_stack = 1 + int((sample_size[0]-pixel_size[0])/slit_size)
+        if num_tomo_stack > 1 and station == 'id3b':
+            raise ValueError('Sample is to tall for the detector')
+
+        # Get the column coordinates
+        img_x_offset = -0.5 * (detector_size[0]*pixel_size[0]
+                               + slit_size * (num_tomo_stack-1))
+        img_x_coords = (img_x_offset
+            + pixel_size[0] * (0.5 + np.asarray(range(int(detector_size[0])))))
+
+        # Get the transmitted intensities
+        num_theta = len(thetas)
+        vertical_shifts = []
+        tomo_fields_stack = []
+        img_dim = (len(img_x_coords), path_lengths_solid.shape[1])
+        intensities_solid = None
+        intensities_hollow = None
+        for n in range(num_tomo_stack):
+            vertical_shifts.append(img_x_offset + n*slit_size)
+            tomo_field = beam_intensity * np.ones((num_theta, *img_dim))
+            if sample_type == 'square_rod':
+                intensities_solid = \
+                    beam_intensity * np.exp(-mu*path_lengths_solid)
+                for n in range(num_theta):
+                    tomo_field[n,:,:] = intensities_solid[n]
+            elif sample_type == 'square_pipe':
+                intensities_hollow = \
+                    beam_intensity * np.exp(-mu*path_lengths_hollow)
+                for n in range(num_theta):
+                    tomo_field[n,:,:] = intensities_hollow[n]
+            else:
+                intensities_solid = \
+                    beam_intensity * np.exp(-mu*path_lengths_solid)
+                intensities_hollow = \
+                    beam_intensity * np.exp(-mu*path_lengths_hollow)
+                outer_indices = \
+                    np.where(abs(img_x_coords) <= sample_size[0]/2)[0]
+                inner_indices = np.where(
+                    abs(img_x_coords) < sample_size[0]/2 - wall_thickness)[0]
+                wall_indices = list(set(outer_indices)-set(inner_indices))
+                for i in wall_indices:
+                    for n in range(num_theta):
+                        tomo_field[n,i] = intensities_solid[n]
+                for i in inner_indices:
+                    for n in range(num_theta):
+                        tomo_field[n,i] = intensities_hollow[n]
+            tomo_field += background_intensity
+            tomo_fields_stack.append(tomo_field.astype(np.int64))
+            if num_tomo_stack > 1:
+                img_x_coords += slit_size
+            
+        # Add dummy snapshots at each end to mimic FMB/SMB
+        if station in ('id1a3', 'id3a'):
+            num_theta_dummy_start = 5
+            num_theta_dummy_end = 0
+        else:
+            num_theta_dummy_start = 1
+            num_theta_dummy_end = 1
+        thetas = [theta_start-n*theta_step
+            for n in range(num_theta_dummy_start, 0, -1)] + thetas
+        thetas += [theta_end+n*theta_step
+            for n in range(1, num_theta_dummy_end+1)]
+        if num_theta_dummy_start:
+            dummy_fields = background_intensity * np.ones(
+                (num_theta_dummy_start, *img_dim), dtype=np.int64)
+            for n, tomo_field in enumerate(tomo_fields_stack):
+                tomo_fields_stack[n] = np.concatenate(
+                    (dummy_fields, tomo_field))
+        if num_theta_dummy_end:
+            dummy_fields = background_intensity * np.ones(
+                (num_theta_dummy_end, *img_dim), dtype=np.int64)
+            for n, tomo_field in enumerate(tomo_fields_stack):
+                tomo_fields_stack[n] = np.concatenate(
+                    (tomo_field, dummy_fields))
+        if num_tomo_stack == 1:
+            tomo_fields_stack = tomo_fields_stack[0]
+
+        # Create Nexus object and write to file
+        nxroot = NXroot()
+        nxroot.entry = NXentry()
+        nxroot.entry.sample = NXsample()
+        nxroot.entry.sample.sample_type = sample_type
+        nxroot.entry.sample.sample_size = sample_size
+        if wall_thickness is not None:
+            nxroot.entry.sample.wall_thickness = wall_thickness
+        nxroot.entry.sample.mu = mu
+        nxinstrument = NXinstrument()
+        nxroot.entry.instrument = nxinstrument
+        nxinstrument.source = NXsource()
+        nxinstrument.source.attrs['station'] = station
+        nxinstrument.source.type = 'Synchrotron X-ray Source'
+        nxinstrument.source.name = 'Tomography Simulator'
+        nxinstrument.source.probe = 'x-ray'
+        nxinstrument.source.background_intensity = background_intensity
+        nxinstrument.source.beam_intensity = beam_intensity
+        nxinstrument.source.slit_size = slit_size
+        nxdetector = NXdetector()
+        nxinstrument.detector = nxdetector
+        nxdetector.local_name = config.detector.prefix
+        nxdetector.x_pixel_size = pixel_size[0]
+        nxdetector.y_pixel_size = pixel_size[1]
+        nxdetector.x_pixel_size.attrs['units'] = 'mm'
+        nxdetector.y_pixel_size.attrs['units'] = 'mm'
+        nxdetector.data = tomo_fields_stack
+        nxdetector.thetas = thetas
+        nxdetector.z_translation = vertical_shifts
+        nxdetector.frame_start_number = num_theta_dummy_start
+#        nxdetector.path_lengths_solid = path_lengths_solid
+#        nxdetector.path_lengths_hollow = path_lengths_hollow
+#        nxdetector.intensities_solid = intensities_solid
+#        nxdetector.intensities_hollow = intensities_hollow
+
+        return nxroot
+
+    def get_configs(self, data):
+        """
+        Get instances of the configuration objects needed by this
+        `Processor` from a returned value of `Reader.read`
+
+        :param data: Result of `Reader.read` where at least one item
+            has `'TomoReduceConfig'` for the `'schema'` key, and at
+            least one item has `'TomoSimConfig'` for the `'schema'` key.
+        :type data: list[dict[str,object]]
+        :raises Exception: If valid config objects cannot be constructed
+            from `data`.
+        :return: valid instance of the configuration object with field
+            values taken from `data`.
+        :rtype: TomoSimConfig
+        """
+        # Local modules
+        from CHAP.tomo.models import TomoSimConfig
+
+        tomo_sim_data = None
+        if isinstance(data, list):
+            for item in data:
+                if (isinstance(item, dict) and item.get('data') is not None
+                        and item.get('schema') == 'TomoSimConfig'):
+                    tomo_sim_data = item.get('data')
+        if tomo_sim_data is None:
+            raise ValueError(f'Invalid parameter data ({data})')
+
+        return TomoSimConfig(**tomo_sim_data)
+
+    def _create_pathlength_solid_square(self, dim, thetas, pixel_size,
+            detector_size):
+        """
+        Create the x-ray path length through a solid square
+        crosssection for a set of rotation angles.
+        """
+
+        # Get the column coordinates
+        img_y_coords = pixel_size * (0.5 * (1 - detector_size%2)
+            + np.asarray(range(int(0.5 * (detector_size+1)))))
+
+        # Get the path lenghts for position column coordinates
+        lengths = np.zeros((len(thetas), len(img_y_coords)), dtype=np.float64)
+        for i, theta in enumerate(thetas):
+            dummy = theta
+            theta = theta - 90.*np.floor(theta/90.)
+            if 45. < theta <= 90.:
+                theta = 90.-theta
+            theta_rad = theta*np.pi/180.
+            len_ab = dim/np.cos(theta_rad)
+            len_oc = dim*np.cos(theta_rad+0.25*np.pi)/np.sqrt(2.)
+            len_ce = dim*np.sin(theta_rad)
+            index1 = int(np.argmin(np.abs(img_y_coords-len_oc)))
+            if len_oc < img_y_coords[index1] and index1 > 0:
+                index1 -= 1
+            index2 = int(np.argmin(np.abs(img_y_coords-len_oc-len_ce)))
+            if len_oc+len_ce < img_y_coords[index2]:
+                index2 -= 1
+            index1 += 1
+            index2 += 1
+            for j in range(index1):
+                lengths[i,j] = len_ab
+            for j, column in enumerate(img_y_coords[index1:index2]):
+                lengths[i,j+index1] = len_ab*(len_oc+len_ce-column)/len_ce
+
+        # Add the mirror image for negative column coordinates
+        if len(img_y_coords)%2:
+            lengths = np.concatenate(
+                (np.fliplr(lengths[:,1:]), lengths), axis=1)
+        else:
+            lengths = np.concatenate((np.fliplr(lengths), lengths), axis=1)
+
+        return lengths
+
+
+class TomoDarkFieldProcessor(Processor):
+    """
+    Class representing the process to create a dark field associated
+    with a simulated tomography data set created by TomoSimProcessor
+    returning a `nexusformat.nexus.NXroot` object containing the
+    dark field tomography detector images.
+    """
+
+    def process(self, data, num_image=5, **kwargs):
+        # Third party modules
+        from nexusformat.nexus import (
+            NXroot,
+            NXentry,
+            NXinstrument,
+            NXdetector,
+        )
+
+        # Get the TomoSimField configuration object in data
+        nxroot = self.get_config(data)
+        source = nxroot.entry.instrument.source
+        detector = nxroot.entry.instrument.detector
+        background_intensity = source.background_intensity
+        detector_size = detector.data.shape[-2:]
+
+        # Add dummy snapshots at start to mimic SMB
+        if source.station in ('id1a3', 'id3a'):
+            num_theta_dummy_start = 5
+        else:
+            num_theta_dummy_start = 0
+        num_image += num_theta_dummy_start
+
+        # Create the dark field
+        dark_field = int(background_intensity) * np.ones(
+            (num_image, detector_size[0], detector_size[1]), dtype=np.int64)
+
+        # Create Nexus object and write to file
+        nxdark = NXroot()
+        nxdark.entry = NXentry()
+        nxdark.entry.sample = nxroot.entry.sample
+        nxinstrument = NXinstrument()
+        nxdark.entry.instrument = nxinstrument
+        nxinstrument.source = nxroot.entry.instrument.source
+        nxdetector = NXdetector()
+        nxinstrument.detector = nxdetector
+        nxdetector.local_name = detector.local_name
+        nxdetector.x_pixel_size = detector.x_pixel_size
+        nxdetector.y_pixel_size = detector.y_pixel_size
+        nxdetector.data = dark_field
+        nxdetector.thetas = np.asarray(num_image*[0])
+        nxdetector.frame_start_number = num_theta_dummy_start
+
+        return nxdark
+
+    def get_config(self, data):
+        """Get an instance of the configuration object needed by this
+        `Processor` from a returned value of `Reader.read`
+
+        :param data: Result of `Reader.read` where at least one item
+            has the value `'TomoSimField'` for the `'schema'` key.
+        :type data: list[dict[str,object]]
+        :raises Exception: If a valid config object cannot be
+            constructed from `data`.
+        :return: a valid instance of a configuration object with field
+            values taken from `data`.
+        :rtype: nexusformat.nexus.NXroot
+        """
+        nxroot = None
+        if isinstance(data, list):
+            for item in data:
+                if isinstance(item, dict):
+                    if item.get('schema') == 'TomoSimField':
+                        nxroot = item.get('data')
+                        break
+        if nxroot is None:
+            raise ValueError(
+                'No tomography data set found in input data')
+
+        return nxroot
+
+
+class TomoBrightFieldProcessor(Processor):
+    """
+    Class representing the process to create a bright field associated
+    with a simulated tomography data set created by TomoSimProcessor
+    returning a `nexusformat.nexus.NXroot` object containing the
+    bright field tomography detector images.
+    """
+
+    def process(self, data, num_image=5, **kwargs):
+        # Third party modules
+        from nexusformat.nexus import (
+            NeXusError,
+            NXroot,
+            NXentry,
+            NXinstrument,
+            NXdetector,
+        )
+
+        # Get and validate the TomoSimField configuration object in data
+        nxroot = self.get_config(data)
+        source = nxroot.entry.instrument.source
+        detector = nxroot.entry.instrument.detector
+        beam_intensity = source.beam_intensity
+        background_intensity = source.background_intensity
+        detector_size = detector.data.shape[-2:]
+
+        # Add dummy snapshots at start to mimic SMB
+        if source.station in ('id1a3', 'id3a'):
+            num_theta_dummy_start = 5
+        else:
+            num_theta_dummy_start = 0
+        num_image += num_theta_dummy_start
+
+        # Create the bright field
+        bright_field = int(background_intensity+beam_intensity) * np.ones(
+            (num_image, detector_size[0], detector_size[1]), dtype=np.int64)
+        # Add 10% to slit size to make the bright beam slightly taller
+        #     than the vertical displacements between stacks
+        slit_size = 1.10*source.slit_size
+        if slit_size < detector.x_pixel_size*detector_size[0]:
+            img_x_coords = detector.x_pixel_size \
+                * (0.5 + np.asarray(range(int(detector_size[0])))
+                   - 0.5*detector_size[0])
+            outer_indices = np.where(abs(img_x_coords) > slit_size/2)[0]
+            bright_field[:,outer_indices,:] = 0
+
+        # Create Nexus object and write to file
+        nxbright = NXroot()
+        nxbright.entry = NXentry()
+        nxbright.entry.sample = nxroot.entry.sample
+        nxinstrument = NXinstrument()
+        nxbright.entry.instrument = nxinstrument
+        nxinstrument.source = nxroot.entry.instrument.source
+        nxdetector = NXdetector()
+        nxinstrument.detector = nxdetector
+        nxdetector.local_name = detector.local_name
+        nxdetector.x_pixel_size = detector.x_pixel_size
+        nxdetector.y_pixel_size = detector.y_pixel_size
+        nxdetector.data = bright_field
+        nxdetector.thetas = np.asarray(num_image*[0])
+        nxdetector.frame_start_number = num_theta_dummy_start
+
+        return nxbright
+
+    def get_config(self, data):
+        """Get an instance of the configuration object needed by this
+        `Processor` from a returned value of `Reader.read`
+
+        :param data: Result of `Reader.read` where at least one item
+            has the value `'TomoSimField'` for the `'schema'` key.
+        :type data: list[dict[str,object]]
+        :raises Exception: If a valid config object cannot be
+            constructed from `data`.
+        :return: a valid instance of a configuration object with field
+            values taken from `data`.
+        :rtype: nexusformat.nexus.NXroot
+        """
+        nxroot = None
+        if isinstance(data, list):
+            for item in data:
+                if isinstance(item, dict):
+                    if item.get('schema') == 'TomoSimField':
+                        nxroot = item.get('data')
+                        break
+        if nxroot is None:
+            raise ValueError(
+                'No tomography data set found in input data')
+
+        return nxroot
+
+
+class TomoSpecProcessor(Processor):
+    """
+    Class representing the process to create a tomography SPEC file
+    associated with a simulated tomography data set created by
+    TomoSimProcessor returning a plain text object containing the
+    tomography SPEC file.
+    """
+
+    def process(self, data, spec_folder='.', scan_numbers=[1], **kwargs):
+        # System modules
+        from json import dump
+        from datetime import datetime
+
+        # Third party modules
+        from nexusformat.nexus import NeXusError
+
+        # Get and validate the TomoSimField, TomoDarkField, or
+        #     TomoBrightField configuration object in data
+        scan_numbers = list(set(scan_numbers))
+        configs = self.get_config(data)
+        station = None
+        sample_type = None
+        num_scan = 0
+        for schema, nxroot in configs.items():
+            source = nxroot.entry.instrument.source
+            if station is None:
+                station = source.attrs.get('station')
+            else:
+                if station != source.attrs.get('station'):
+                    raise ValueError('Inconsistent station among scans')
+            if sample_type is None:
+                sample_type = nxroot.entry.sample.sample_type
+            else:
+                if sample_type != nxroot.entry.sample.sample_type:
+                    raise ValueError('Inconsistent sample_type among scans')
+            detector = nxroot.entry.instrument.detector
+            if 'z_translation' in detector:
+                num_stack = np.asarray(detector.z_translation).size
+            else:
+                num_stack = 1
+            data_shape = detector.data.shape
+            if len(data_shape) == 3:
+                if num_stack != 1:
+                    raise ValueError(
+                        'Inconsistent z_translation and data dimensions'
+                        f'({num_stack} vs {1})')
+            elif len(data_shape) == 4:
+                if num_stack != data_shape[0]:
+                    raise ValueError(
+                        'Inconsistent z_translation dimension and data shape '
+                        f'({num_stack} vs {data_shape[0]})')
+            else:
+                raise ValueError(f'Invalid data shape ({data_shape})')
+            num_scan += num_stack
+        if len(scan_numbers) != num_scan:
+            raise ValueError(
+                f'Inconsistent number of scans ({num_scan}), '
+                f'len(scan_numbers) = {len(scan_numbers)})')
+
+        # Create the SPEC output folder if needed
+        spec_folder = os_path.abspath(spec_folder)
+        if not os_path.isdir(spec_folder):
+            mkdir(spec_folder)
+
+        # Create the SPEC file header
+        spec_file = [f'#F {sample_type}']
+        spec_file.append('#E 0')
+        spec_file.append(
+            f'#D {datetime.now().strftime("%a %b %d %I:%M:%S %Y")}')
+        spec_file.append(f'#C spec  User = chess_{station}\n')
+        if station in ('id1a3', 'id3a'):
+            spec_file.append('#O0 ramsx  ramsz')
+        else:
+            #RV Fix main code to use independent dim info
+            spec_file.append('#O0 GI_samx  GI_samz  GI_samphi')
+            spec_file.append('#o0 samx samz samphi') #RV do I need this line?
+        spec_file.append('')
+
+        # Create the SPEC file scan info (and image and parfile data for SMB)
+        par_file = []
+        image_sets = []
+        num_scan = 0
+        count_time = 1
+        for schema, nxroot in configs.items():
+            detector = nxroot.entry.instrument.detector
+            if 'z_translation' in detector:
+                z_translations = list(np.asarray(detector.z_translation))
+            else:
+                z_translations = [0.]
+            frame_start_number = int(detector.frame_start_number)
+            thetas = np.asarray(detector.thetas)[frame_start_number:]
+            num_theta = thetas.size
+            if schema == 'TomoDarkField':
+                if station in ('id1a3', 'id3a'):
+                    macro = f'slew_ome {thetas[0]} {thetas[-1]} ' \
+                        f'{num_theta} {count_time} darkfield'
+                    scan_type = 'df1'
+                else:
+                    macro = f'flyscan {num_theta} {count_time}'
+            elif schema == 'TomoBrightField':
+                if station in ('id1a3', 'id3a'):
+                    macro = f'slew_ome {thetas[0]} {thetas[-1]} ' \
+                        f'{num_theta} {count_time}'
+                    scan_type = 'bf1'
+                else:
+                    macro = f'flyscan {num_theta} {count_time}'
+            elif schema == 'TomoSimField':
+                if station in ('id1a3', 'id3a'):
+                    macro = f'slew_ome {thetas[0]} {thetas[-1]} ' \
+                        f'{num_theta} {count_time}'
+                    scan_type = 'ts1'
+                else:
+                    macro = f'flyscan samphi {thetas[0]} ' \
+                        f'{thetas[-1]} {num_theta-1} {count_time}'
+            for  n, z_translation in enumerate(z_translations):
+                spec_file.append(f'#S {scan_numbers[num_scan]}  {macro}')
+                spec_file.append(
+                    f'#D {datetime.now().strftime("%a %b %d %I:%M:%S %Y")}')
+                if station in ('id1a3', 'id3a'):
+                    spec_file.append(f'#P0 0.0 {z_translation}')
+                    spec_file.append('#N 1')
+                    spec_file.append('#L  ome')
+                    if scan_type == 'ts1':
+                        image_sets.append(detector.data[n])
+                    else:
+                        image_sets.append(detector.data)
+                    par_file.append(
+                        f'{datetime.now().strftime("%Y%m%d")} '
+                        f'{datetime.now().strftime("%H%M%S")} '
+                        f'{scan_numbers[num_scan]} '
+#                        '2.0 '
+#                        '1.0 '
+                        '0 '
+                        f'{frame_start_number} '
+                        '0.0 '
+                        f'{z_translation} '
+                        f'{thetas[0]} '
+                        f'{thetas[-1]} '
+                        f'{num_theta} '
+                        f'{count_time} '
+                        f'{scan_type}')
+                else:
+                    spec_file.append(f'#P0 0.0 {z_translation} 0.0')
+                    spec_file.append('#N 1')
+                    if schema in ('TomoDarkField', 'TomoBrightField'):
+                        spec_file.append('#L Time')
+                        spec_file += [str(count_time*time)
+                            for time in range(num_theta)]
+                    elif schema == 'TomoSimField':
+                        spec_file.append('#L GI_samphi')
+                        spec_file += [str(theta) for theta in thetas]
+                spec_file.append('')
+                num_scan += 1
+        
+        if station in ('id1a3', 'id3a'):
+
+            # Write the SPEC file
+            self.write_txt(spec_file, os_path.join(spec_folder, 'spec.log'))
+
+            # Write the JSON file
+            parfile_header = {
+                '0': 'date',
+                '1': 'time',
+                '2': 'SCAN_N',
+#                '3': 'beam_width',
+#                '4': 'beam_height',
+                '3': 'junkstart',
+                '4': 'goodstart',
+                '5': 'ramsx',
+                '6': 'ramsz',
+                '7': 'ome_start_real',
+                '8': 'ome_end_real',
+                '9': 'nframes_real',
+                '10': 'count_time',
+                '11': 'tomotype',
+            }
+            json_filename = os_path.join(
+                spec_folder,
+                f'{station}-tomo_sim-{os_path.basename(spec_folder)}.json')
+            with open(json_filename, 'w') as f:
+                dump(parfile_header, f)
+        
+            # Write the par file
+            par_filename = os_path.join(
+                spec_folder,
+                f'{station}-tomo_sim-{os_path.basename(spec_folder)}.par')
+            self.write_txt(par_file, par_filename)
+
+            # Write image files as individual tiffs
+            for scan_number, image_set in zip(scan_numbers, image_sets):
+                image_folder = os_path.join(spec_folder, str(scan_number))
+                if not os_path.isdir(image_folder):
+                    mkdir(image_folder)
+                image_folder = os_path.join(image_folder, 'nf')
+                if not os_path.isdir(image_folder):
+                    mkdir(image_folder)
+                self.write_tiffs(image_set, image_folder)
+
+        return spec_file
+
+    def get_config(self, data):
+        """Get an instance of the configuration object needed by this
+        `Processor` from a returned value of `Reader.read`
+
+        :param data: Result of `Reader.read` where at least one item
+            has the value `'TomoSimField'` for the `'schema'` key.
+        :type data: list[dict[str,object]]
+        :raises Exception: If a valid config object cannot be
+            constructed from `data`.
+        :return: a valid instance of a configuration object with field
+            values taken from `data`.
+        :rtype: nexusformat.nexus.NXroot
+        """
+        configs = {}
+        if isinstance(data, list):
+            for item in data:
+                if isinstance(item, dict):
+                    schema = item.get('schema')
+                    if schema == 'TomoDarkField':
+                        configs[schema] = item.get('data')
+                    elif schema == 'TomoBrightField':
+                        configs[schema] = item.get('data')
+                    elif schema == 'TomoSimField':
+                        configs[schema] = item.get('data')
+        if not len(configs):
+            raise ValueError(
+                'No tomography data set found in input data')
+
+        return configs
+
+    def write_tiffs(self, data, image_folder):
+        # Third party modules
+        from imageio import imwrite
+        for n in range(data.shape[0]):
+            imwrite(
+                os_path.join(image_folder, f'nf_{n:06d}.tif'), data[n])
+
+    def write_txt(self, data, filepath, force_overwrite=True):
+        # Local modules
+        from CHAP.common import TXTWriter
+        from CHAP.pipeline import PipelineData
+        writer = TXTWriter()
+        writer.write(
+            [PipelineData(data=data)], filepath,
+            force_overwrite=force_overwrite)
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `ChessAnalysisPipeline-0.0.7/CHAP/writer.py` & `ChessAnalysisPipeline-0.0.8/CHAP/writer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,48 @@
 #!/usr/bin/env python
 """
 File       : writer.py
 Author     : Valentin Kuznetsov <vkuznet AT gmail dot com>
 Description: generic Writer module
+
+Define a generic `Writer` object.
 """
 
 # system modules
 import argparse
 from inspect import getfullargspec
 import logging
 from sys import modules
 from time import time
 
+# local modules
+from CHAP.pipeline import PipelineItem
+
 
-class Writer():
-    """Writer represent generic file writer"""
+class Writer(PipelineItem):
+    """Generic file writer
 
-    def __init__(self):
-        """Constructor of Writer class"""
-        self.__name__ = self.__class__.__name__
-        self.logger = logging.getLogger(self.__name__)
-        self.logger.propagate = False
+    The job of any `Writer` in a `Pipeline` is to receive input
+    returned by a previous `PipelineItem`, write its data to a
+    particular file format, then return the same data unaltered so it
+    can be used by a successive `PipelineItem`.
+    """
 
-    def write(self, data, filename, **_write_kwargs):
-        """write API
+    def write(self, data, filename):
+        """Write the input data as text to a file.
 
+        :param data: input data
+        :type data: list[PipelineData]
         :param filename: Name of file to write to
-        :param data: data to write to file
-        :return: data written to file
+        :type filename: str
+        :return: contents of the input data
+        :rtype: object
         """
 
-        t0 = time()
-        self.logger.info(f'Executing "write" with filename={filename}, '
-                         f'type(data)={type(data)}, kwargs={_write_kwargs}')
-
-        _valid_write_args = {}
-        allowed_args = getfullargspec(self._write).args \
-            + getfullargspec(self._write).kwonlyargs
-        for k, v in _write_kwargs.items():
-            if k in allowed_args:
-                _valid_write_args[k] = v
-            else:
-                self.logger.warning(f'Ignoring invalid arg to _write: {k}')
-
-        data = self._write(data, filename, **_valid_write_args)
-
-        self.logger.info(f'Finished "write" in {time()-t0:.3f} seconds\n')
-
-        return data
-
-    def _write(self, data, filename):
+        data = self.unwrap_pipelinedata(data)
         with open(filename, 'a') as file:
             file.write(data)
         return data
 
 
 class OptionParser():
     """User based option parser"""
```

### Comparing `ChessAnalysisPipeline-0.0.7/ChessAnalysisPipeline.egg-info/PKG-INFO` & `ChessAnalysisPipeline-0.0.8/ChessAnalysisPipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChessAnalysisPipeline
-Version: 0.0.7
+Version: 0.0.8
 Summary: CHESS analysis pipeline framework
 Home-page: https://github.com/CHESSComputing/ChessAnalysisPipeline
 Author: Keara Soloway, Rolf Verberg, Valentin Kuznetsov
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ChessAnalysisPipeline-0.0.7/ChessAnalysisPipeline.egg-info/SOURCES.txt` & `ChessAnalysisPipeline-0.0.8/ChessAnalysisPipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.7/LICENSE` & `ChessAnalysisPipeline-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.7/MLaaS/ktrain.py` & `ChessAnalysisPipeline-0.0.8/MLaaS/ktrain.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.7/MLaaS/mnist_img.py` & `ChessAnalysisPipeline-0.0.8/MLaaS/mnist_img.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.7/MLaaS/tfaas_client.py` & `ChessAnalysisPipeline-0.0.8/MLaaS/tfaas_client.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.7/PKG-INFO` & `ChessAnalysisPipeline-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChessAnalysisPipeline
-Version: 0.0.7
+Version: 0.0.8
 Summary: CHESS analysis pipeline framework
 Home-page: https://github.com/CHESSComputing/ChessAnalysisPipeline
 Author: Keara Soloway, Rolf Verberg, Valentin Kuznetsov
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ChessAnalysisPipeline-0.0.7/README.md` & `ChessAnalysisPipeline-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.7/setup.py` & `ChessAnalysisPipeline-0.0.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+#!/usr/bin/env python
 """
 Standard python setup.py file
 to build     : python setup.py build
 to install   : python setup.py install --prefix=<some dir>
 to clean     : python setup.py clean
 to build doc : python setup.py doc
 to run tests : python setup.py test
 """
 
 import os
 import setuptools
 
-version = 'v0.0.7'
+# [set version]
+version = 'v0.0.8'
+# [version set]
 
 def datafiles(idir, pattern=None):
     """Return list of data files in provided relative dir"""
     files = []
     for dirname, dirnames, filenames in os.walk(idir):
         for subdirname in dirnames:
             files.append(os.path.join(dirname, subdirname))
```

