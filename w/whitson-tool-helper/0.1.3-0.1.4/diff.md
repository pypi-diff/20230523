# Comparing `tmp/whitson_tool_helper-0.1.3.tar.gz` & `tmp/whitson_tool_helper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whitson_tool_helper-0.1.3.tar", last modified: Tue May  2 11:39:10 2023, max compression
+gzip compressed data, was "whitson_tool_helper-0.1.4.tar", last modified: Tue May 23 14:40:52 2023, max compression
```

## Comparing `whitson_tool_helper-0.1.3.tar` & `whitson_tool_helper-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-05-02 11:39:10.140303 whitson_tool_helper-0.1.3/
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      404 2023-05-02 11:39:10.140303 whitson_tool_helper-0.1.3/PKG-INFO
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      705 2023-05-02 11:39:04.000000 whitson_tool_helper-0.1.3/pyproject.toml
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       38 2023-05-02 11:39:10.140303 whitson_tool_helper-0.1.3/setup.cfg
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-05-02 11:39:10.140303 whitson_tool_helper-0.1.3/src/
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-05-02 11:39:10.140303 whitson_tool_helper-0.1.3/src/whitson_tool_helper/
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      107 2023-04-26 09:24:26.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper/__init__.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       66 2023-04-26 13:22:55.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper/logger.py
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-05-02 11:39:10.140303 whitson_tool_helper-0.1.3/src/whitson_tool_helper/messaging/
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      370 2023-04-26 13:32:24.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper/messaging/aux.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     2738 2023-05-02 09:42:15.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper/messaging/main.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     4382 2023-05-02 09:41:25.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper/messaging/pubsub.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     3725 2023-05-02 11:17:35.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper/messaging/rabbitmq.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      574 2023-04-26 07:15:11.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper/timeout.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      704 2023-04-26 12:52:42.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper/whitson_exceptions.py
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-05-02 11:39:10.140303 whitson_tool_helper-0.1.3/src/whitson_tool_helper.egg-info/
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      404 2023-05-02 11:39:10.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper.egg-info/PKG-INFO
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      572 2023-05-02 11:39:10.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper.egg-info/SOURCES.txt
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)        1 2023-05-02 11:39:10.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper.egg-info/dependency_links.txt
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      116 2023-05-02 11:39:10.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper.egg-info/requires.txt
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       20 2023-05-02 11:39:10.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper.egg-info/top_level.txt
+drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-05-23 14:40:52.899701 whitson_tool_helper-0.1.4/
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      404 2023-05-23 14:40:52.899701 whitson_tool_helper-0.1.4/PKG-INFO
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      705 2023-05-23 14:40:47.000000 whitson_tool_helper-0.1.4/pyproject.toml
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       38 2023-05-23 14:40:52.899701 whitson_tool_helper-0.1.4/setup.cfg
+drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-05-23 14:40:52.899701 whitson_tool_helper-0.1.4/src/
+drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-05-23 14:40:52.899701 whitson_tool_helper-0.1.4/src/whitson_tool_helper/
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      107 2023-04-26 09:24:26.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper/__init__.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       66 2023-04-26 13:22:55.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper/logger.py
+drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-05-23 14:40:52.899701 whitson_tool_helper-0.1.4/src/whitson_tool_helper/messaging/
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      370 2023-04-26 13:32:24.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper/messaging/helper.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     2738 2023-05-02 09:42:15.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper/messaging/main.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     4385 2023-05-23 14:38:25.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper/messaging/pubsub.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     3728 2023-05-23 14:38:30.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper/messaging/rabbitmq.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      574 2023-04-26 07:15:11.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper/timeout.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      704 2023-04-26 12:52:42.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper/whitson_exceptions.py
+drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-05-23 14:40:52.899701 whitson_tool_helper-0.1.4/src/whitson_tool_helper.egg-info/
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      404 2023-05-23 14:40:52.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper.egg-info/PKG-INFO
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      575 2023-05-23 14:40:52.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)        1 2023-05-23 14:40:52.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      116 2023-05-23 14:40:52.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper.egg-info/requires.txt
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       20 2023-05-23 14:40:52.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper.egg-info/top_level.txt
```

### Comparing `whitson_tool_helper-0.1.3/pyproject.toml` & `whitson_tool_helper-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whitson_tool_helper"
-version =  "0.1.3"
+version =  "0.1.4"
 authors = [
   { name="Markus Blytt", email="blytt@whitson.com" },
   { name="Jason Hu", email="jason@whitson.com" },
   { name="Arnaud Hoffmann", email="arnaud@whitson.com" },
 ]
 description = "A Toolbox for whitson cloud software solutions"
 dependencies = ["pika==1.3.1", "google-auth==2.16.0","google-cloud-pubsub==2.14.0", "google-cloud-storage==2.7.0","google-cloud-logging==3.5.0"]
```

### Comparing `whitson_tool_helper-0.1.3/src/whitson_tool_helper/messaging/main.py` & `whitson_tool_helper-0.1.4/src/whitson_tool_helper/messaging/main.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.1.3/src/whitson_tool_helper/messaging/pubsub.py` & `whitson_tool_helper-0.1.4/src/whitson_tool_helper/messaging/pubsub.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 import json
 import traceback
 from typing import List
 import time
 from concurrent import futures
 
-from whitson_tool_helper.messaging.aux import check_environment_variables
+from whitson_tool_helper.messaging.helper import check_environment_variables
 from whitson_tool_helper.logger import LOGGER
 
 
 class PubsubConsumer:
     def __init__(self, process_func, to_dict=False):
         check_environment_variables(
             [
```

### Comparing `whitson_tool_helper-0.1.3/src/whitson_tool_helper/messaging/rabbitmq.py` & `whitson_tool_helper-0.1.4/src/whitson_tool_helper/messaging/rabbitmq.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pika
 import os
 from typing import List
 import json
 
-from whitson_tool_helper.messaging.aux import check_environment_variables
+from whitson_tool_helper.messaging.helper import check_environment_variables
 from whitson_tool_helper.logger import LOGGER
 
 
 def get_rabbitmq_params():
     check_environment_variables(
         [
             "RABBITMQ_USER",
```

### Comparing `whitson_tool_helper-0.1.3/src/whitson_tool_helper/timeout.py` & `whitson_tool_helper-0.1.4/src/whitson_tool_helper/timeout.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.1.3/src/whitson_tool_helper/whitson_exceptions.py` & `whitson_tool_helper-0.1.4/src/whitson_tool_helper/whitson_exceptions.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.1.3/src/whitson_tool_helper.egg-info/SOURCES.txt` & `whitson_tool_helper-0.1.4/src/whitson_tool_helper.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,11 +4,11 @@
 src/whitson_tool_helper/timeout.py
 src/whitson_tool_helper/whitson_exceptions.py
 src/whitson_tool_helper.egg-info/PKG-INFO
 src/whitson_tool_helper.egg-info/SOURCES.txt
 src/whitson_tool_helper.egg-info/dependency_links.txt
 src/whitson_tool_helper.egg-info/requires.txt
 src/whitson_tool_helper.egg-info/top_level.txt
-src/whitson_tool_helper/messaging/aux.py
+src/whitson_tool_helper/messaging/helper.py
 src/whitson_tool_helper/messaging/main.py
 src/whitson_tool_helper/messaging/pubsub.py
 src/whitson_tool_helper/messaging/rabbitmq.py
```

