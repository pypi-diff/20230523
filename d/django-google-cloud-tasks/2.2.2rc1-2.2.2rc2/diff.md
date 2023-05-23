# Comparing `tmp/django_google_cloud_tasks-2.2.2rc1.tar.gz` & `tmp/django_google_cloud_tasks-2.2.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_google_cloud_tasks-2.2.2rc1.tar", max compression
+gzip compressed data, was "django_google_cloud_tasks-2.2.2rc2.tar", max compression
```

## Comparing `django_google_cloud_tasks-2.2.2rc1.tar` & `django_google_cloud_tasks-2.2.2rc2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11358 2022-11-21 14:22:47.501421 django_google_cloud_tasks-2.2.2rc1/LICENSE.md
--rw-r--r--   0        0        0      153 2023-03-15 20:17:34.011359 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/__init__.py
--rw-r--r--   0        0        0     6245 2023-03-22 17:43:19.343899 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/apps.py
--rw-r--r--   0        0        0      446 2023-03-22 18:41:55.809147 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/context.py
--rw-r--r--   0        0        0      373 2023-03-15 20:17:34.220121 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/exceptions.py
--rw-r--r--   0        0        0     1389 2023-03-15 20:17:33.764578 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/field.py
--rw-r--r--   0        0        0        0 2022-11-21 14:22:47.495972 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/management/__init__.py
--rw-r--r--   0        0        0      860 2023-03-15 20:17:33.597653 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/management/commands/__init__.py
--rw-r--r--   0        0        0      490 2023-03-22 17:43:19.019827 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/management/commands/initialize_subscribers.py
--rw-r--r--   0        0        0      394 2022-11-21 14:22:47.497092 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/management/commands/initialize_tasks.py
--rw-r--r--   0        0        0      501 2022-11-21 14:22:47.497226 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/management/commands/schedule_tasks.py
--rw-r--r--   0        0        0      252 2023-03-22 17:43:19.344171 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/middleware/__init__.py
--rw-r--r--   0        0        0     1179 2023-03-22 17:43:18.952608 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/middleware/headers_context_middlware.py
--rw-r--r--   0        0        0     1870 2023-04-12 23:12:38.891213 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/middleware/pubsub_headers_middleware.py
--rw-r--r--   0        0        0     3888 2023-03-15 20:17:33.597800 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/migrations/0001_initial.py
--rw-r--r--   0        0        0     1024 2023-03-15 20:17:33.764958 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py
--rw-r--r--   0        0        0        0 2022-11-21 14:22:47.496709 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/migrations/__init__.py
--rw-r--r--   0        0        0     4421 2023-05-18 12:54:13.349917 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/models.py
--rw-r--r--   0        0        0      925 2022-11-21 14:22:47.497904 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/serializers.py
--rw-r--r--   0        0        0     2693 2023-05-18 12:54:13.349995 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/signals.py
--rw-r--r--   0        0        0      667 2023-03-15 20:17:34.347222 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/tasks/__init__.py
--rw-r--r--   0        0        0     1118 2023-03-15 20:17:34.101243 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/tasks/periodic_task.py
--rw-r--r--   0        0        0     4775 2023-03-22 18:15:18.921786 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/tasks/publisher_task.py
--rw-r--r--   0        0        0     2522 2023-03-15 20:17:34.143566 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/tasks/routine_task.py
--rw-r--r--   0        0        0     2610 2023-04-12 23:12:38.881460 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/tasks/subscriber_task.py
--rw-r--r--   0        0        0     9178 2023-05-18 12:54:13.352192 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/tasks/task.py
--rw-r--r--   0        0        0        0 2023-03-13 22:03:16.402866 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/tests/__init__.py
--rw-r--r--   0        0        0      985 2023-03-15 20:17:34.384480 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/tests/factories.py
--rw-r--r--   0        0        0      871 2023-03-15 20:17:34.384727 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/tests/tests_base.py
--rw-r--r--   0        0        0      291 2022-11-21 14:22:47.500083 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/urls.py
--rw-r--r--   0        0        0     3014 2023-04-12 23:17:48.891352 django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/views.py
--rw-r--r--   0        0        0      795 2023-05-18 12:54:13.352527 django_google_cloud_tasks-2.2.2rc1/pyproject.toml
--rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 django_google_cloud_tasks-2.2.2rc1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-07-24 16:19:35.292566 django_google_cloud_tasks-2.2.2rc2/LICENSE.md
+-rw-r--r--   0        0        0      153 2023-04-05 13:39:44.250424 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/__init__.py
+-rw-r--r--   0        0        0     6245 2023-04-05 13:39:44.250645 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/apps.py
+-rw-r--r--   0        0        0      446 2023-04-05 13:39:44.250738 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/context.py
+-rw-r--r--   0        0        0      373 2023-04-05 13:39:44.250892 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/exceptions.py
+-rw-r--r--   0        0        0     1389 2023-04-05 13:39:44.250988 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/field.py
+-rw-r--r--   0        0        0        0 2022-07-24 16:19:35.293209 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/management/__init__.py
+-rw-r--r--   0        0        0      860 2023-04-05 13:39:44.251171 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/management/commands/__init__.py
+-rw-r--r--   0        0        0      490 2023-04-05 13:39:44.251329 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/management/commands/initialize_subscribers.py
+-rw-r--r--   0        0        0      394 2022-07-24 16:19:35.294227 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/management/commands/initialize_tasks.py
+-rw-r--r--   0        0        0      501 2023-03-12 12:43:20.381324 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/management/commands/schedule_tasks.py
+-rw-r--r--   0        0        0      252 2023-04-05 13:39:44.251483 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/middleware/__init__.py
+-rw-r--r--   0        0        0     1179 2023-04-05 13:39:44.251578 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/middleware/headers_context_middlware.py
+-rw-r--r--   0        0        0     1870 2023-05-18 17:35:04.723809 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/middleware/pubsub_headers_middleware.py
+-rw-r--r--   0        0        0     3888 2023-04-05 13:39:44.251981 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1024 2023-04-05 13:39:44.252082 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py
+-rw-r--r--   0        0        0        0 2022-07-24 16:19:35.294840 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/migrations/__init__.py
+-rw-r--r--   0        0        0     4421 2023-05-18 17:35:05.512244 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/models.py
+-rw-r--r--   0        0        0      925 2022-07-24 16:19:35.295438 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/serializers.py
+-rw-r--r--   0        0        0     2693 2023-05-18 17:35:05.512575 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/signals.py
+-rw-r--r--   0        0        0      667 2023-04-05 13:39:44.252578 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/__init__.py
+-rw-r--r--   0        0        0     1118 2023-04-05 13:39:44.252714 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/periodic_task.py
+-rw-r--r--   0        0        0     4775 2023-04-05 13:39:44.252856 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/publisher_task.py
+-rw-r--r--   0        0        0     2700 2023-05-18 17:35:05.512881 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/routine_task.py
+-rw-r--r--   0        0        0     2610 2023-05-18 17:35:04.724509 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/subscriber_task.py
+-rw-r--r--   0        0        0     9178 2023-05-18 17:35:04.724808 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/task.py
+-rw-r--r--   0        0        0        0 2022-07-24 16:19:35.296011 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tests/__init__.py
+-rw-r--r--   0        0        0      985 2023-04-05 13:39:44.253503 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tests/factories.py
+-rw-r--r--   0        0        0      871 2023-04-05 13:39:44.253865 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tests/tests_base.py
+-rw-r--r--   0        0        0      291 2022-07-24 16:19:35.296184 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/urls.py
+-rw-r--r--   0        0        0     3014 2023-05-18 17:35:04.725038 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/views.py
+-rw-r--r--   0        0        0      795 2023-05-18 17:35:05.514474 django_google_cloud_tasks-2.2.2rc2/pyproject.toml
+-rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 django_google_cloud_tasks-2.2.2rc2/PKG-INFO
```

### Comparing `django_google_cloud_tasks-2.2.2rc1/LICENSE.md` & `django_google_cloud_tasks-2.2.2rc2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/apps.py` & `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/apps.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/field.py` & `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/field.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/management/commands/__init__.py` & `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/middleware/headers_context_middlware.py` & `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/middleware/headers_context_middlware.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/middleware/pubsub_headers_middleware.py` & `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/middleware/pubsub_headers_middleware.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/migrations/0001_initial.py` & `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py` & `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/models.py` & `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/models.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/serializers.py` & `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/serializers.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/signals.py` & `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/signals.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/tasks/__init__.py` & `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/tasks/periodic_task.py` & `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/periodic_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/tasks/publisher_task.py` & `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/publisher_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/tasks/routine_task.py` & `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/routine_task.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 
 from django.core.cache import cache
 
 from django_cloud_tasks import models
 from django_cloud_tasks.tasks.task import Task
 
-logger = logging.getLogger()
+logger = logging.getLogger(__name__)
 
 
 class RoutineTask(Task, abc.ABC):
     @classmethod
     @abc.abstractmethod
     def revert(cls, data: dict):
         raise NotImplementedError()
@@ -52,19 +52,25 @@
             routine.pipeline.revert()
             return
 
         routine.attempt_count += 1
         routine.status = models.Routine.Statuses.RUNNING
         routine.save(update_fields=("attempt_count", "status", "updated_at"))
 
+        logger.info(f"Running ruotine: {routine._dict}")
+
+        routine = models.Routine(**routine._dict)
+
         try:
             logger.info(f"Routine #{routine.pk} is running")
             task_response = routine.task_class(metadata=self._metadata).sync(**routine.body)
         except Exception as error:
             logger.info(f"Routine #{routine.pk} has failed")
             routine.fail(output={"error": str(error)})
             routine.enqueue()
             logger.info(f"Routine #{routine.pk} has been enqueued for retry")
             return
 
+        logger.info(f"Completing ruotine: {routine._dict}")
+
         routine.complete(output=task_response)
         logger.info(f"Routine #{routine.pk} just completed")
```

### Comparing `django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/tasks/subscriber_task.py` & `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/subscriber_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/tasks/task.py` & `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/tests/factories.py` & `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/tests/tests_base.py` & `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tests/tests_base.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc1/django_cloud_tasks/views.py` & `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/views.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc1/pyproject.toml` & `django_google_cloud_tasks-2.2.2rc2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-google-cloud-tasks"
-version = "2.2.2rc1"
+version = "2.2.2rc2"
 description = "Async Tasks with HTTP endpoints"
 authors = ["Joao Daher <joao@daher.dev>"]
 packages = [
     { include = "django_cloud_tasks" },
 ]
 
 [tool.poetry.dependencies]
```

