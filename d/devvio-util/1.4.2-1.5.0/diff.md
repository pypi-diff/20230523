# Comparing `tmp/devvio_util-1.4.2.tar.gz` & `tmp/devvio_util-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devvio_util-1.4.2.tar", last modified: Thu Apr 27 17:02:14 2023, max compression
+gzip compressed data, was "devvio_util-1.5.0.tar", last modified: Tue May 23 18:47:29 2023, max compression
```

## Comparing `devvio_util-1.4.2.tar` & `devvio_util-1.5.0.tar`

### file list

```diff
@@ -1,16 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:14.544627 devvio_util-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-27 17:02:14.544627 devvio_util-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:01.000000 devvio_util-1.4.2/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:14.540627 devvio_util-1.4.2/devvio_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:01.000000 devvio_util-1.4.2/devvio_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-27 17:02:01.000000 devvio_util-1.4.2/devvio_util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-27 17:02:01.000000 devvio_util-1.4.2/devvio_util/lib_creds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-27 17:02:01.000000 devvio_util-1.4.2/devvio_util/psql_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:14.540627 devvio_util-1.4.2/devvio_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-27 17:02:14.000000 devvio_util-1.4.2/devvio_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-27 17:02:14.000000 devvio_util-1.4.2/devvio_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:02:14.000000 devvio_util-1.4.2/devvio_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:02:14.000000 devvio_util-1.4.2/devvio_util.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 17:02:14.000000 devvio_util-1.4.2/devvio_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 17:02:14.544627 devvio_util-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-27 17:02:01.000000 devvio_util-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:47:29.909786 devvio_util-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-23 18:47:29.909786 devvio_util-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:47:22.000000 devvio_util-1.5.0/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:47:29.905786 devvio_util-1.5.0/devvio_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:47:22.000000 devvio_util-1.5.0/devvio_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-23 18:47:22.000000 devvio_util-1.5.0/devvio_util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-05-23 18:47:22.000000 devvio_util-1.5.0/devvio_util/lib_creds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:47:29.909786 devvio_util-1.5.0/devvio_util/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:47:22.000000 devvio_util-1.5.0/devvio_util/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-23 18:47:22.000000 devvio_util-1.5.0/devvio_util/primitives/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-23 18:47:22.000000 devvio_util-1.5.0/devvio_util/primitives/atomic_transaction_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-23 18:47:22.000000 devvio_util-1.5.0/devvio_util/primitives/chainstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-23 18:47:22.000000 devvio_util-1.5.0/devvio_util/primitives/devv_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-23 18:47:22.000000 devvio_util-1.5.0/devvio_util/primitives/final_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-23 18:47:22.000000 devvio_util-1.5.0/devvio_util/primitives/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-23 18:47:22.000000 devvio_util-1.5.0/devvio_util/primitives/smart_coin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-05-23 18:47:22.000000 devvio_util-1.5.0/devvio_util/primitives/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-05-23 18:47:22.000000 devvio_util-1.5.0/devvio_util/primitives/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-23 18:47:22.000000 devvio_util-1.5.0/devvio_util/primitives/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-23 18:47:22.000000 devvio_util-1.5.0/devvio_util/primitives/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-23 18:47:22.000000 devvio_util-1.5.0/devvio_util/primitives/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-23 18:47:22.000000 devvio_util-1.5.0/devvio_util/psql_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:47:29.909786 devvio_util-1.5.0/devvio_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-23 18:47:29.000000 devvio_util-1.5.0/devvio_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-23 18:47:29.000000 devvio_util-1.5.0/devvio_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:47:29.000000 devvio_util-1.5.0/devvio_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:47:29.000000 devvio_util-1.5.0/devvio_util.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-23 18:47:29.000000 devvio_util-1.5.0/devvio_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 18:47:29.909786 devvio_util-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-23 18:47:22.000000 devvio_util-1.5.0/setup.py
```

### Comparing `devvio_util-1.4.2/devvio_util/config.py` & `devvio_util-1.5.0/devvio_util/config.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.4.2/devvio_util/lib_creds.py` & `devvio_util-1.5.0/devvio_util/lib_creds.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-#!/usr/bin/env python
-# encoding: utf-8
-import os
-
 # reload(sys)
 # sys.setdefaultencoding('utf-8')
 import json
 import boto3
 import base64
 from botocore.exceptions import ClientError
-import base64
 from abc import ABC
 
 
 class Loader(ABC):
     def __init__(self, *args, **kwargs):
         """
         :param credentials: AWS credentials (AWS_ACCESS_KEY_ID, AWS_REGION, AWS_SECRET_ACCESS_KEY)
```

### Comparing `devvio_util-1.4.2/devvio_util/psql_mixin.py` & `devvio_util-1.5.0/devvio_util/psql_mixin.py`

 * *Files identical despite different names*

