# Comparing `tmp/autoscale_queue_rq-0.1.1.tar.gz` & `tmp/autoscale_queue_rq-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoscale_queue_rq-0.1.1.tar", max compression
+gzip compressed data, was "autoscale_queue_rq-0.2.0.tar", max compression
```

## Comparing `autoscale_queue_rq-0.1.1.tar` & `autoscale_queue_rq-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1081 2023-04-23 13:49:03.717091 autoscale_queue_rq-0.1.1/LICENSE
--rw-r--r--   0        0        0      773 2023-04-23 13:49:03.717091 autoscale_queue_rq-0.1.1/README.md
--rw-r--r--   0        0        0     2753 2023-04-23 13:49:03.717091 autoscale_queue_rq-0.1.1/autoscale_queue_rq/__init__.py
--rw-r--r--   0        0        0     1171 2023-04-23 13:49:03.717091 autoscale_queue_rq-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 autoscale_queue_rq-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-23 15:05:53.693998 autoscale_queue_rq-0.2.0/LICENSE
+-rw-r--r--   0        0        0      773 2023-05-23 15:05:53.693998 autoscale_queue_rq-0.2.0/README.md
+-rw-r--r--   0        0        0     2802 2023-05-23 15:05:53.693998 autoscale_queue_rq-0.2.0/autoscale_queue_rq/__init__.py
+-rw-r--r--   0        0        0     1171 2023-05-23 15:05:53.693998 autoscale_queue_rq-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1668 1970-01-01 00:00:00.000000 autoscale_queue_rq-0.2.0/PKG-INFO
```

### Comparing `autoscale_queue_rq-0.1.1/LICENSE` & `autoscale_queue_rq-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autoscale_queue_rq-0.1.1/README.md` & `autoscale_queue_rq-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `autoscale_queue_rq-0.1.1/autoscale_queue_rq/__init__.py` & `autoscale_queue_rq-0.2.0/autoscale_queue_rq/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import os
 from datetime import datetime, timezone
 
 import redis
 from rq import Queue
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 __author__ = "Michael R. van Rooijen"
 __contact__ = "support@autoscale.app"
 __homepage__ = "https://autoscale.app"
 __docformat__ = "restructuredtext"
 __keywords__ = "python queue worker autoscale rq"
 
 
-def latency(queue_names, redis_url=None):
+def job_queue_time(queue_names, redis_url=None):
     """
-    Calculate the maximum latency in seconds of the given RQ queues.
+    Calculate the maximum job queue time in seconds of the given RQ queues.
 
-    This function calculates the latency of the provided queues by measuring the time
-    elapsed since the oldest job was enqueued in each queue. The maximum latency among
+    This function calculates the job queue time of the provided queues by measuring the time
+    elapsed since the oldest job was enqueued in each queue. The maximum job queue time among
     all the queues is returned.
 
     Args:
-        queue_names (list[str]): A list of RQ queue names for which to calculate latency.
+        queue_names (list[str]): A list of RQ queue names for which to calculate job queue time.
         redis_url (str, optional): The URL of the Redis server used by RQ. Defaults to None,
             in which case the value will be read from the REDIS_URL environment variable.
 
     Raises:
         ValueError: If no queue names are provided or if a Redis URL is not provided and
             not found in the environment variables.
 
         redis.exceptions.ConnectionError: If the provided Redis URL is not valid.
 
     Returns:
-        float: The maximum latency in seconds among all the given queues. If a queue has no
-            jobs, its latency is considered as 0.
+        float: The maximum job queue time in seconds among all the given queues. If a queue has no
+            jobs, its job queue time is considered as 0.
     """
     if not queue_names:
         raise ValueError("At least one queue name must be provided")
 
     if not redis_url:
         redis_url = os.getenv("REDIS_URL")
```

### Comparing `autoscale_queue_rq-0.1.1/pyproject.toml` & `autoscale_queue_rq-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoscale-queue-rq"
-version = "0.1.1"
+version = "0.2.0"
 description = "Produces RQ queue metrics for the Autoscale.app Agent"
 authors = ["Michael R. van Rooijen <support@autoscale.app>"]
 license = "MIT"
 repository = "https://github.com/autoscale-app/python-queue-rq"
 readme = "README.md"
 homepage = "https://autoscale.app"
 keywords = ["python", "queue", "worker", "autoscale", "rq"]
```

### Comparing `autoscale_queue_rq-0.1.1/PKG-INFO` & `autoscale_queue_rq-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoscale-queue-rq
-Version: 0.1.1
+Version: 0.2.0
 Summary: Produces RQ queue metrics for the Autoscale.app Agent
 Home-page: https://autoscale.app
 License: MIT
 Keywords: python,queue,worker,autoscale,rq
 Author: Michael R. van Rooijen
 Author-email: support@autoscale.app
 Requires-Python: >=3.8,<3.12
@@ -13,19 +13,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: rq (>=1.10.1,<2.0)
 Project-URL: Repository, https://github.com/autoscale-app/python-queue-rq
 Description-Content-Type: text/markdown
 
 # Python Queue RQ (Autoscale.app)
 
 Produces [RQ] queue metrics for the [Autoscale.app] [Agent].
```

