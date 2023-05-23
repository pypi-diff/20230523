# Comparing `tmp/matter_task_queue-1.2.0-py3-none-any.whl.zip` & `tmp/matter_task_queue-1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8758 bytes, number of entries: 10
+Zip file size: 8756 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      134 b- defN 20-Feb-02 00:00 matter_task_queue/__about__.py
 -rw-r--r--  2.0 unx      327 b- defN 20-Feb-02 00:00 matter_task_queue/__init__.py
 -rw-r--r--  2.0 unx     1228 b- defN 20-Feb-02 00:00 matter_task_queue/base_task.py
 -rw-r--r--  2.0 unx     3829 b- defN 20-Feb-02 00:00 matter_task_queue/celery_config.py
 -rw-r--r--  2.0 unx      941 b- defN 20-Feb-02 00:00 matter_task_queue/config.py
 -rw-r--r--  2.0 unx     3232 b- defN 20-Feb-02 00:00 matter_task_queue/utils.py
-?rw-r--r--  2.0 unx     4757 b- defN 20-Feb-02 00:00 matter_task_queue-1.2.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_task_queue-1.2.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_task_queue-1.2.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      858 b- defN 20-Feb-02 00:00 matter_task_queue-1.2.0.dist-info/RECORD
-10 files, 16461 bytes uncompressed, 7282 bytes compressed:  55.8%
+?rw-r--r--  2.0 unx     4757 b- defN 20-Feb-02 00:00 matter_task_queue-1.2.1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_task_queue-1.2.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_task_queue-1.2.1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      858 b- defN 20-Feb-02 00:00 matter_task_queue-1.2.1.dist-info/RECORD
+10 files, 16461 bytes uncompressed, 7280 bytes compressed:  55.8%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: matter_task_queue/config.py
 Comment: 
 
 Filename: matter_task_queue/utils.py
 Comment: 
 
-Filename: matter_task_queue-1.2.0.dist-info/METADATA
+Filename: matter_task_queue-1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: matter_task_queue-1.2.0.dist-info/WHEEL
+Filename: matter_task_queue-1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: matter_task_queue-1.2.0.dist-info/licenses/LICENSE
+Filename: matter_task_queue-1.2.1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: matter_task_queue-1.2.0.dist-info/RECORD
+Filename: matter_task_queue-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## matter_task_queue/__about__.py

```diff
@@ -1,4 +1,4 @@
 # SPDX-FileCopyrightText: 2023-present Rômulo Jales <romulo@thisismatter.com>
 #
 # SPDX-License-Identifier: MIT
-__version__ = "1.2.0"
+__version__ = "1.2.1"
```

## Comparing `matter_task_queue-1.2.0.dist-info/METADATA` & `matter_task_queue-1.2.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matter-task-queue
-Version: 1.2.0
+Version: 1.2.1
 Summary: A template for new Matter's library
 Project-URL: Documentation, https://github.com/Matter-Tech/matter-task-queue#readme
 Project-URL: Issues, https://github.com/Matter-Tech/matter-task-queue/issues
 Project-URL: Source, https://github.com/Matter-Tech/matter-task-queue
 Author-email: Tomer Sasson <tomer@thisismatter.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -13,17 +13,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: celery[sqs]==5.2.7
 Requires-Dist: kombu==5.2.4
-Requires-Dist: matter-exceptions==1.1.0
+Requires-Dist: matter-exceptions>=1.1.0
 Provides-Extra: sentry
-Requires-Dist: sentry-sdk==1.19.1; extra == 'sentry'
+Requires-Dist: sentry-sdk==1.23.1; extra == 'sentry'
 Description-Content-Type: text/markdown
 
 # matter-task-queue
 
 The Task Queue Library is a Python library that provides functionality for managing queues and integrates Celery into FastAPI apps. It enables a seamless integration that unlocks all of Celery's capabilities and allows for easy queue management and task execution.
 
 Celery is an open-source, distributed task queue that is widely used in Python-based applications for processing and executing background tasks or long-running processes asynchronously. It was created in 2009 and has since grown into a mature and powerful library that provides a robust and scalable solution for managing task queues.
```

## Comparing `matter_task_queue-1.2.0.dist-info/licenses/LICENSE` & `matter_task_queue-1.2.1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `matter_task_queue-1.2.0.dist-info/RECORD` & `matter_task_queue-1.2.1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-matter_task_queue/__about__.py,sha256=bJZ4QuVO53FpCQDaei3XZ3hp7NNjLm1SJ-DBD3aFyc8,134
+matter_task_queue/__about__.py,sha256=qHh4wMavjsGdNUHpHyFu2j5Kksk6ZgisOQYTZgeEPSU,134
 matter_task_queue/__init__.py,sha256=ZFkdbgwBSqy_H99nGWgV3FPvA4_qn3SjQ0jFyBDa7q0,327
 matter_task_queue/base_task.py,sha256=6J-CkaNo3PoERYwfcq2N6WKvUkm7eE1ZtGqqv9ms7nk,1228
 matter_task_queue/celery_config.py,sha256=aIe-i7riee3C7fH9LCcmFrBQarc_UJCzRWe1JcPZib0,3829
 matter_task_queue/config.py,sha256=MviXOQN378CSGMphlOUSdXUkblIb49w2armMnb4Xg7E,941
 matter_task_queue/utils.py,sha256=V5vlCW39lRJvorJka7kAAt2IRSebgmAGVXydOYHwdQ0,3232
-matter_task_queue-1.2.0.dist-info/METADATA,sha256=rbRwmPr-4Lde6qBVtJawjRg2XQ6D32Bwova6WvQ9slg,4757
-matter_task_queue-1.2.0.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
-matter_task_queue-1.2.0.dist-info/licenses/LICENSE,sha256=bqRY4B_u4xSKzKFb3ML8l0nCWvMXyzEGwY2B2hteV8g,1068
-matter_task_queue-1.2.0.dist-info/RECORD,,
+matter_task_queue-1.2.1.dist-info/METADATA,sha256=JCo2mXed_fJ_TFQTbMvzytDyFH7BpdarKfeFdAiXRCc,4757
+matter_task_queue-1.2.1.dist-info/WHEEL,sha256=y1bSCq4r5i4nMmpXeUJMqs3ipKvkZObrIXSvJHm1qCI,87
+matter_task_queue-1.2.1.dist-info/licenses/LICENSE,sha256=bqRY4B_u4xSKzKFb3ML8l0nCWvMXyzEGwY2B2hteV8g,1068
+matter_task_queue-1.2.1.dist-info/RECORD,,
```

