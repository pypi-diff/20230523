# Comparing `tmp/autoscale_queue_celery-0.1.1.tar.gz` & `tmp/autoscale_queue_celery-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoscale_queue_celery-0.1.1.tar", max compression
+gzip compressed data, was "autoscale_queue_celery-0.2.0.tar", max compression
```

## Comparing `autoscale_queue_celery-0.1.1.tar` & `autoscale_queue_celery-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1081 2023-04-23 13:47:43.044600 autoscale_queue_celery-0.1.1/LICENSE
--rw-r--r--   0        0        0      807 2023-04-23 13:47:43.044600 autoscale_queue_celery-0.1.1/README.md
--rw-r--r--   0        0        0     4195 2023-04-23 13:47:43.044600 autoscale_queue_celery-0.1.1/autoscale_queue_celery/__init__.py
--rw-r--r--   0        0        0     1203 2023-04-23 13:47:43.044600 autoscale_queue_celery-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1999 1970-01-01 00:00:00.000000 autoscale_queue_celery-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-23 14:50:26.629552 autoscale_queue_celery-0.2.0/LICENSE
+-rw-r--r--   0        0        0      807 2023-05-23 14:50:26.629552 autoscale_queue_celery-0.2.0/README.md
+-rw-r--r--   0        0        0     4414 2023-05-23 14:50:26.629552 autoscale_queue_celery-0.2.0/autoscale_queue_celery/__init__.py
+-rw-r--r--   0        0        0     1203 2023-05-23 14:50:26.629552 autoscale_queue_celery-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1749 1970-01-01 00:00:00.000000 autoscale_queue_celery-0.2.0/PKG-INFO
```

### Comparing `autoscale_queue_celery-0.1.1/LICENSE` & `autoscale_queue_celery-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autoscale_queue_celery-0.1.1/README.md` & `autoscale_queue_celery-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `autoscale_queue_celery-0.1.1/autoscale_queue_celery/__init__.py` & `autoscale_queue_celery-0.2.0/autoscale_queue_celery/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import os
 from datetime import datetime, timezone
 
 from celery import signals
 from kombu.serialization import loads
 from redis import Redis
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 __author__ = "Michael R. van Rooijen"
 __contact__ = "support@autoscale.app"
 __homepage__ = "https://autoscale.app"
 __docformat__ = "restructuredtext"
 __keywords__ = "python queue worker autoscale celery"
 
 
-def latency(queue_names, redis_url=None):
+def job_queue_time(queue_names, redis_url=None):
     """
-    Calculates the maximum latency across multiple queues in Redis.
+    Calculates the maximum job queue time across multiple queues in Redis.
 
     Parameters:
     - queue_names (list): A list of queue names to query.
     - redis_url (str): A Redis connection URL. If not provided, the REDIS_URL environment variable
         will be used. If the environment variable is not set, a ValueError will be raised.
 
     Returns:
-    - The maximum latency (float) in seconds across all the provided queues. Returns 0 if no tasks can be found.
+    - The maximum job queue time (float) in seconds across all the provided queues. Returns 0 if no tasks can be found.
 
     This function retrieves the tail of the queue (the task that would be processed next by a worker)
-    for each provided queue name using a single Redis transaction, and then calculates the latency
+    for each provided queue name using a single Redis transaction, and then calculates the job queue time
     of the tail task for each queue, taking into account the 'eta', 'expires', and 'enqueued_at'
-    timestamp attributes. The maximum latency across all the provided queues is then returned.
+    timestamp attributes. The maximum job queue time across all the provided queues is then returned.
 
     If a task has an 'expires' attribute, it checks whether the task has expired. If it has, the task
-    is skipped, and its latency is not considered. If the task has an 'eta' attribute and the current
-    time is greater than or equal to the 'eta', the latency is calculated as the difference between
-    the current time and 'eta'. If the task does not have an 'eta' attribute, the latency is calculated
+    is skipped, and its job queue time is not considered. If the task has an 'eta' attribute and the current
+    time is greater than or equal to the 'eta', the job queue time is calculated as the difference between
+    the current time and 'eta'. If the task does not have an 'eta' attribute, the job queue time is calculated
     as the difference between the current time and 'enqueued_at'.
 
     The enqueued_at header is added to each task before it's sent to the broker using the
     'add_enqueued_at_header' function. It is not added by default by Celery, so this function must be
     called before any tasks are sent to the broker.
     """
     if not queue_names:
@@ -56,47 +56,51 @@
     try:
         with redis_conn.pipeline(transaction=True) as pipe:
             for queue_name in queue_names:
                 pipe.lindex(queue_name, -1)
 
             serialized_tasks = pipe.execute()
 
-        max_latency = 0
+        max_job_queue_time = 0
 
         for serialized_task in serialized_tasks:
             if serialized_task:
                 task = loads(
                     serialized_task,
                     content_type="application/json",
                     content_encoding="utf-8",
                 )
                 current_time = datetime.now(timezone.utc)
-                latency_seconds = 0
+                job_queue_time_seconds = 0
 
                 if task["headers"]["expires"]:
                     expires_time = datetime.fromisoformat(
                         task["headers"]["expires"]
                     ).replace(tzinfo=timezone.utc)
                     if current_time >= expires_time:
                         continue
 
                 if task["headers"]["eta"]:
                     eta_time = datetime.fromisoformat(task["headers"]["eta"]).replace(
                         tzinfo=timezone.utc
                     )
                     if current_time >= eta_time:
-                        latency_seconds = (current_time - eta_time).total_seconds()
+                        job_queue_time_seconds = (
+                            current_time - eta_time
+                        ).total_seconds()
                 else:
                     enqueued_at = datetime.fromisoformat(task["headers"]["enqueued_at"])
-                    latency_seconds = (current_time - enqueued_at).total_seconds()
+                    job_queue_time_seconds = (
+                        current_time - enqueued_at
+                    ).total_seconds()
 
-                if latency_seconds > max_latency:
-                    max_latency = latency_seconds
+                if job_queue_time_seconds > max_job_queue_time:
+                    max_job_queue_time = job_queue_time_seconds
 
-        return max_latency
+        return max_job_queue_time
     finally:
         redis_conn.connection_pool.disconnect()
 
 
 @signals.before_task_publish.connect
 def add_enqueued_at_header(sender=None, headers=None, **kwargs):
     """
```

### Comparing `autoscale_queue_celery-0.1.1/pyproject.toml` & `autoscale_queue_celery-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoscale-queue-celery"
-version = "0.1.1"
+version = "0.2.0"
 description = "Produces Celery queue metrics for the Autoscale.app Agent"
 authors = ["Michael R. van Rooijen <support@autoscale.app>"]
 license = "MIT"
 repository = "https://github.com/autoscale-app/python-queue-celery"
 readme = "README.md"
 homepage = "https://autoscale.app"
 keywords = ["python", "queue", "worker", "autoscale", "celery"]
```

### Comparing `autoscale_queue_celery-0.1.1/PKG-INFO` & `autoscale_queue_celery-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoscale-queue-celery
-Version: 0.1.1
+Version: 0.2.0
 Summary: Produces Celery queue metrics for the Autoscale.app Agent
 Home-page: https://autoscale.app
 License: MIT
 Keywords: python,queue,worker,autoscale,celery
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
 Requires-Dist: celery (>=5.0,<6)
 Requires-Dist: redis (>=4.1,<6)
 Project-URL: Repository, https://github.com/autoscale-app/python-queue-celery
 Description-Content-Type: text/markdown
 
 # Python Queue Celery (Autoscale.app)
```

