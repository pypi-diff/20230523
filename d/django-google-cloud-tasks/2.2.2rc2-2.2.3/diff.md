# Comparing `tmp/django_google_cloud_tasks-2.2.2rc2.tar.gz` & `tmp/django_google_cloud_tasks-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_google_cloud_tasks-2.2.2rc2.tar", max compression
+gzip compressed data, was "django_google_cloud_tasks-2.2.3.tar", max compression
```

## Comparing `django_google_cloud_tasks-2.2.2rc2.tar` & `django_google_cloud_tasks-2.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11358 2022-07-24 16:19:35.292566 django_google_cloud_tasks-2.2.2rc2/LICENSE.md
--rw-r--r--   0        0        0      153 2023-04-05 13:39:44.250424 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/__init__.py
--rw-r--r--   0        0        0     6245 2023-04-05 13:39:44.250645 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/apps.py
--rw-r--r--   0        0        0      446 2023-04-05 13:39:44.250738 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/context.py
--rw-r--r--   0        0        0      373 2023-04-05 13:39:44.250892 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/exceptions.py
--rw-r--r--   0        0        0     1389 2023-04-05 13:39:44.250988 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/field.py
--rw-r--r--   0        0        0        0 2022-07-24 16:19:35.293209 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/management/__init__.py
--rw-r--r--   0        0        0      860 2023-04-05 13:39:44.251171 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/management/commands/__init__.py
--rw-r--r--   0        0        0      490 2023-04-05 13:39:44.251329 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/management/commands/initialize_subscribers.py
--rw-r--r--   0        0        0      394 2022-07-24 16:19:35.294227 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/management/commands/initialize_tasks.py
--rw-r--r--   0        0        0      501 2023-03-12 12:43:20.381324 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/management/commands/schedule_tasks.py
--rw-r--r--   0        0        0      252 2023-04-05 13:39:44.251483 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/middleware/__init__.py
--rw-r--r--   0        0        0     1179 2023-04-05 13:39:44.251578 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/middleware/headers_context_middlware.py
--rw-r--r--   0        0        0     1870 2023-05-18 17:35:04.723809 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/middleware/pubsub_headers_middleware.py
--rw-r--r--   0        0        0     3888 2023-04-05 13:39:44.251981 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/migrations/0001_initial.py
--rw-r--r--   0        0        0     1024 2023-04-05 13:39:44.252082 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py
--rw-r--r--   0        0        0        0 2022-07-24 16:19:35.294840 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/migrations/__init__.py
--rw-r--r--   0        0        0     4421 2023-05-18 17:35:05.512244 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/models.py
--rw-r--r--   0        0        0      925 2022-07-24 16:19:35.295438 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/serializers.py
--rw-r--r--   0        0        0     2693 2023-05-18 17:35:05.512575 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/signals.py
--rw-r--r--   0        0        0      667 2023-04-05 13:39:44.252578 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/__init__.py
--rw-r--r--   0        0        0     1118 2023-04-05 13:39:44.252714 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/periodic_task.py
--rw-r--r--   0        0        0     4775 2023-04-05 13:39:44.252856 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/publisher_task.py
--rw-r--r--   0        0        0     2700 2023-05-18 17:35:05.512881 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/routine_task.py
--rw-r--r--   0        0        0     2610 2023-05-18 17:35:04.724509 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/subscriber_task.py
--rw-r--r--   0        0        0     9178 2023-05-18 17:35:04.724808 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/task.py
--rw-r--r--   0        0        0        0 2022-07-24 16:19:35.296011 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tests/__init__.py
--rw-r--r--   0        0        0      985 2023-04-05 13:39:44.253503 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tests/factories.py
--rw-r--r--   0        0        0      871 2023-04-05 13:39:44.253865 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tests/tests_base.py
--rw-r--r--   0        0        0      291 2022-07-24 16:19:35.296184 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/urls.py
--rw-r--r--   0        0        0     3014 2023-05-18 17:35:04.725038 django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/views.py
--rw-r--r--   0        0        0      795 2023-05-18 17:35:05.514474 django_google_cloud_tasks-2.2.2rc2/pyproject.toml
--rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 django_google_cloud_tasks-2.2.2rc2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/LICENSE.md
+-rw-r--r--   0        0        0      153 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/__init__.py
+-rw-r--r--   0        0        0     6245 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/apps.py
+-rw-r--r--   0        0        0      446 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/context.py
+-rw-r--r--   0        0        0      373 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/exceptions.py
+-rw-r--r--   0        0        0     1389 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/field.py
+-rw-r--r--   0        0        0        0 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/management/__init__.py
+-rw-r--r--   0        0        0      860 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/management/commands/__init__.py
+-rw-r--r--   0        0        0      490 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/management/commands/initialize_subscribers.py
+-rw-r--r--   0        0        0      394 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/management/commands/initialize_tasks.py
+-rw-r--r--   0        0        0      501 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/management/commands/schedule_tasks.py
+-rw-r--r--   0        0        0      252 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/middleware/__init__.py
+-rw-r--r--   0        0        0     1179 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/middleware/headers_context_middlware.py
+-rw-r--r--   0        0        0     1870 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/middleware/pubsub_headers_middleware.py
+-rw-r--r--   0        0        0     3888 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1024 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py
+-rw-r--r--   0        0        0        0 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/migrations/__init__.py
+-rw-r--r--   0        0        0     4364 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/models.py
+-rw-r--r--   0        0        0      925 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/serializers.py
+-rw-r--r--   0        0        0     2704 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/signals.py
+-rw-r--r--   0        0        0      667 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/__init__.py
+-rw-r--r--   0        0        0     1118 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/periodic_task.py
+-rw-r--r--   0        0        0     4775 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/publisher_task.py
+-rw-r--r--   0        0        0     2522 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/routine_task.py
+-rw-r--r--   0        0        0     2610 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/subscriber_task.py
+-rw-r--r--   0        0        0    10404 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/task.py
+-rw-r--r--   0        0        0        0 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/tests/__init__.py
+-rw-r--r--   0        0        0      985 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/tests/factories.py
+-rw-r--r--   0        0        0      871 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/tests/tests_base.py
+-rw-r--r--   0        0        0      291 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/urls.py
+-rw-r--r--   0        0        0     3014 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/views.py
+-rw-r--r--   0        0        0      772 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 django_google_cloud_tasks-2.2.3/PKG-INFO
```

### Comparing `django_google_cloud_tasks-2.2.2rc2/LICENSE.md` & `django_google_cloud_tasks-2.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/apps.py` & `django_google_cloud_tasks-2.2.3/django_cloud_tasks/apps.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/field.py` & `django_google_cloud_tasks-2.2.3/django_cloud_tasks/field.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/management/commands/__init__.py` & `django_google_cloud_tasks-2.2.3/django_cloud_tasks/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/middleware/headers_context_middlware.py` & `django_google_cloud_tasks-2.2.3/django_cloud_tasks/middleware/headers_context_middlware.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/middleware/pubsub_headers_middleware.py` & `django_google_cloud_tasks-2.2.3/django_cloud_tasks/middleware/pubsub_headers_middleware.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/migrations/0001_initial.py` & `django_google_cloud_tasks-2.2.3/django_cloud_tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py` & `django_google_cloud_tasks-2.2.3/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/models.py` & `django_google_cloud_tasks-2.2.3/django_cloud_tasks/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Self
 
 from django.db import models, transaction
 from django.utils import timezone
-from drf_kit.models import ModelDiffMixin
+
 from django_cloud_tasks import serializers
 from django_cloud_tasks.field import TaskField
 
 
 class Pipeline(models.Model):
     name = models.CharField(max_length=100)
 
@@ -26,15 +26,15 @@
         for routine in routines:
             routine.revert()
 
     def add_routine(self, routine: dict) -> "Routine":
         return self.routines.create(**routine)
 
 
-class Routine(models.Model, ModelDiffMixin):
+class Routine(models.Model):
     class Statuses(models.TextChoices):
         PENDING = ("pending", "Pending")
         SCHEDULED = ("scheduled", "Scheduled")
         RUNNING = ("running", "Running")
         COMPLETED = ("completed", "Completed")
         FAILED = ("failed", "Failed")
         REVERTING = ("reverting", "Reverting")
```

### Comparing `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/serializers.py` & `django_google_cloud_tasks-2.2.3/django_cloud_tasks/serializers.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/signals.py` & `django_google_cloud_tasks-2.2.3/django_cloud_tasks/signals.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from django.core.exceptions import ValidationError
-from django.db.models import Model
-from django.db.models.signals import post_save, pre_save
+from django.db.models.signals import pre_save
 from django.dispatch import receiver
 
 from django_cloud_tasks import models
 
 
-def _is_status_changing(instance: Model) -> bool:
-    previous_status, current_status = instance._diff.get("status", (None, None))
-    return previous_status != current_status
+def _is_status_changing(instance: models.Routine) -> bool:
+    if not instance.pk:
+        return False
+
+    current_routine = models.Routine.objects.get(pk=instance.pk)
+    return current_routine.status != instance.status
 
 
 def enqueue_next_routines(instance: models.Routine):
     for routine in instance.next_routines.all():
         routine.enqueue()
 
 
@@ -37,15 +39,15 @@
     models.Routine.Statuses.COMPLETED: enqueue_next_routines,
     models.Routine.Statuses.REVERTED: revert_previous_routines,
     models.Routine.Statuses.SCHEDULED: enqueue_routine_scheduled,
     models.Routine.Statuses.REVERTING: enqueue_revert_task,
 }
 
 
-@receiver(post_save, sender=models.Routine)
+@receiver(pre_save, sender=models.Routine)
 def handle_status_changed(sender, instance: models.Routine, **kwargs):
     if not _is_status_changing(instance=instance):
         return
 
     if action := STATUS_ACTION.get(instance.status):
         action(instance=instance)
 
@@ -54,23 +56,23 @@
 def ensure_status_machine(sender, instance: models.Routine, **kwargs):
     if not instance.pk and instance.status != models.Routine.Statuses.PENDING:
         raise ValidationError(f"The initial routine's status must be 'pending' not '{instance.status}'")
 
     if not _is_status_changing(instance=instance):
         return
 
-    previous_status, _ = instance._diff.get("status", (None, None))
+    current_routine = models.Routine.objects.get(pk=instance.pk)
 
     statuses = models.Routine.Statuses
     machine_statuses = {
         statuses.PENDING: [None],
         statuses.SCHEDULED: [statuses.PENDING, statuses.FAILED],
         statuses.RUNNING: [statuses.SCHEDULED],
         statuses.COMPLETED: [statuses.RUNNING],
         statuses.FAILED: [statuses.RUNNING, statuses.SCHEDULED],
         statuses.REVERTING: [statuses.COMPLETED, statuses.PENDING, statuses.SCHEDULED, statuses.FAILED],
         statuses.REVERTED: [statuses.REVERTING],
     }
     available_statuses = machine_statuses[instance.status]
 
-    if previous_status not in available_statuses:
-        raise ValidationError(f"Status update from '{previous_status}' to '{instance.status}' is not allowed")
+    if current_routine.status not in available_statuses:
+        raise ValidationError(f"Status update from '{current_routine.status}' to '{instance.status}' is not allowed")
```

### Comparing `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/__init__.py` & `django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/periodic_task.py` & `django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/periodic_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/publisher_task.py` & `django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/publisher_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/routine_task.py` & `django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/routine_task.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 
 from django.core.cache import cache
 
 from django_cloud_tasks import models
 from django_cloud_tasks.tasks.task import Task
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger()
 
 
 class RoutineTask(Task, abc.ABC):
     @classmethod
     @abc.abstractmethod
     def revert(cls, data: dict):
         raise NotImplementedError()
@@ -52,25 +52,19 @@
             routine.pipeline.revert()
             return
 
         routine.attempt_count += 1
         routine.status = models.Routine.Statuses.RUNNING
         routine.save(update_fields=("attempt_count", "status", "updated_at"))
 
-        logger.info(f"Running ruotine: {routine._dict}")
-
-        routine = models.Routine(**routine._dict)
-
         try:
             logger.info(f"Routine #{routine.pk} is running")
             task_response = routine.task_class(metadata=self._metadata).sync(**routine.body)
         except Exception as error:
             logger.info(f"Routine #{routine.pk} has failed")
             routine.fail(output={"error": str(error)})
             routine.enqueue()
             logger.info(f"Routine #{routine.pk} has been enqueued for retry")
             return
 
-        logger.info(f"Completing ruotine: {routine._dict}")
-
         routine.complete(output=task_response)
         logger.info(f"Routine #{routine.pk} just completed")
```

### Comparing `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/subscriber_task.py` & `django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/subscriber_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tasks/task.py` & `django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/task.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import abc
 import inspect
-from dataclasses import dataclass
+from dataclasses import dataclass, fields
 from datetime import datetime, timedelta, timezone
 from functools import lru_cache
 from random import randint
 from typing import Any, Self
 from urllib.parse import urljoin
 
 from django.apps import apps
@@ -41,20 +41,20 @@
         self.custom_headers = get_current_headers()
 
     @classmethod
     def from_headers(cls, headers: dict) -> Self:
         # Available data: https://cloud.google.com/tasks/docs/creating-http-target-tasks#handler
         cloud_tasks_prefix = "X-Cloudtasks-"
 
-        if attempt_str := headers.get(f"{cloud_tasks_prefix}Taskexecutioncount"):
+        if (attempt_str := headers.get(f"{cloud_tasks_prefix}Taskexecutioncount")) is not None:
             execution_number = int(attempt_str)
         else:
             execution_number = None
 
-        if retry_str := headers.get(f"{cloud_tasks_prefix}Taskretrycount"):
+        if (retry_str := headers.get(f"{cloud_tasks_prefix}Taskretrycount")) is not None:
             dispatch_number = int(retry_str)
         else:
             dispatch_number = None
 
         if eta_epoch := headers.get(f"{cloud_tasks_prefix}Tasketa"):
             eta = datetime.fromtimestamp(int(eta_epoch.split(".")[0]), tz=timezone.utc)
         else:
@@ -67,14 +67,27 @@
             dispatch_number=dispatch_number,
             execution_number=execution_number,
             eta=eta,
             previous_response=headers.get(f"{cloud_tasks_prefix}TaskPreviousResponse"),
             previous_failure=headers.get(f"{cloud_tasks_prefix}TaskRetryReason"),
         )
 
+    def to_headers(self) -> dict:
+        cloud_tasks_prefix = "X-Cloudtasks-"
+        return {
+            f"{cloud_tasks_prefix}Taskname": self.task_id,
+            f"{cloud_tasks_prefix}Queuename": self.queue_name,
+            f"{cloud_tasks_prefix}Projectname": self.project_id,
+            f"{cloud_tasks_prefix}Taskexecutioncount": str(self.execution_number),
+            f"{cloud_tasks_prefix}Taskretrycount": str(self.dispatch_number),
+            f"{cloud_tasks_prefix}Tasketa": str(int(self.eta.timestamp())),
+            f"{cloud_tasks_prefix}TaskPreviousResponse": self.previous_response,
+            f"{cloud_tasks_prefix}TaskRetryReason": self.previous_failure,
+        }
+
     @classmethod
     def from_task_obj(cls, task_obj: GoogleCloudTask) -> Self:
         _, project_id, _, _, _, queue_name, _, task_id = task_obj.name.split("/")  # TODO: use regex
         return cls(
             project_id=project_id,
             queue_name=queue_name,
             task_id=task_id,
@@ -116,14 +129,29 @@
     def last_attempt(self) -> bool:
         return self.attempt_number == self.max_retries
 
     @property
     def eager(self) -> bool:
         return self.task_id == "--SYNC--"
 
+    def __eq__(self, other) -> bool:
+        if not isinstance(other, TaskMetadata):
+            return False
+
+        check_fields = [field.name for field in fields(TaskMetadata)]
+        for field in check_fields:
+            try:
+                value = getattr(self, field)
+                other_value = getattr(other, field)
+                if value != other_value:
+                    return False
+            except (AttributeError, ValueError):
+                return False
+        return True
+
 
 class TaskMeta(type):
     def __new__(cls, name, bases, attrs):
         klass = type.__new__(cls, name, bases, attrs)
         if not inspect.isabstract(klass) and abc.ABC not in bases:
             register(task_class=klass)
         return klass
```

### Comparing `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tests/factories.py` & `django_google_cloud_tasks-2.2.3/django_cloud_tasks/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/tests/tests_base.py` & `django_google_cloud_tasks-2.2.3/django_cloud_tasks/tests/tests_base.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc2/django_cloud_tasks/views.py` & `django_google_cloud_tasks-2.2.3/django_cloud_tasks/views.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.2rc2/pyproject.toml` & `django_google_cloud_tasks-2.2.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "django-google-cloud-tasks"
-version = "2.2.2rc2"
+version = "2.2.3"
 description = "Async Tasks with HTTP endpoints"
 authors = ["Joao Daher <joao@daher.dev>"]
 packages = [
     { include = "django_cloud_tasks" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 django = ">=4,<5"
 gcp-pilot = {version = "*", extras = ["tasks", "pubsub"]}
-drf-kit = "^1.21.6"
 
 
 [tool.poetry.dev-dependencies]
 ruff = "*"
 black = "*"
 coverage = "*"
 factory-boy = "*"
```

