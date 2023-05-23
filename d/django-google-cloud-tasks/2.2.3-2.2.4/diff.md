# Comparing `tmp/django_google_cloud_tasks-2.2.3.tar.gz` & `tmp/django_google_cloud_tasks-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_google_cloud_tasks-2.2.3.tar", max compression
+gzip compressed data, was "django_google_cloud_tasks-2.2.4.tar", max compression
```

## Comparing `django_google_cloud_tasks-2.2.3.tar` & `django_google_cloud_tasks-2.2.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11358 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/LICENSE.md
--rw-r--r--   0        0        0      153 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/__init__.py
--rw-r--r--   0        0        0     6245 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/apps.py
--rw-r--r--   0        0        0      446 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/context.py
--rw-r--r--   0        0        0      373 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/exceptions.py
--rw-r--r--   0        0        0     1389 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/field.py
--rw-r--r--   0        0        0        0 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/management/__init__.py
--rw-r--r--   0        0        0      860 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/management/commands/__init__.py
--rw-r--r--   0        0        0      490 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/management/commands/initialize_subscribers.py
--rw-r--r--   0        0        0      394 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/management/commands/initialize_tasks.py
--rw-r--r--   0        0        0      501 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/management/commands/schedule_tasks.py
--rw-r--r--   0        0        0      252 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/middleware/__init__.py
--rw-r--r--   0        0        0     1179 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/middleware/headers_context_middlware.py
--rw-r--r--   0        0        0     1870 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/middleware/pubsub_headers_middleware.py
--rw-r--r--   0        0        0     3888 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/migrations/0001_initial.py
--rw-r--r--   0        0        0     1024 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py
--rw-r--r--   0        0        0        0 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/migrations/__init__.py
--rw-r--r--   0        0        0     4364 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/models.py
--rw-r--r--   0        0        0      925 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/serializers.py
--rw-r--r--   0        0        0     2704 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/signals.py
--rw-r--r--   0        0        0      667 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/__init__.py
--rw-r--r--   0        0        0     1118 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/periodic_task.py
--rw-r--r--   0        0        0     4775 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/publisher_task.py
--rw-r--r--   0        0        0     2522 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/routine_task.py
--rw-r--r--   0        0        0     2610 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/subscriber_task.py
--rw-r--r--   0        0        0    10404 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/task.py
--rw-r--r--   0        0        0        0 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/tests/__init__.py
--rw-r--r--   0        0        0      985 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/tests/factories.py
--rw-r--r--   0        0        0      871 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/tests/tests_base.py
--rw-r--r--   0        0        0      291 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/urls.py
--rw-r--r--   0        0        0     3014 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/django_cloud_tasks/views.py
--rw-r--r--   0        0        0      772 2023-05-23 20:09:23.904735 django_google_cloud_tasks-2.2.3/pyproject.toml
--rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 django_google_cloud_tasks-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-11-21 14:22:47.501421 django_google_cloud_tasks-2.2.4/LICENSE.md
+-rw-r--r--   0        0        0      153 2023-03-15 20:17:34.011359 django_google_cloud_tasks-2.2.4/django_cloud_tasks/__init__.py
+-rw-r--r--   0        0        0     6245 2023-03-22 17:43:19.343899 django_google_cloud_tasks-2.2.4/django_cloud_tasks/apps.py
+-rw-r--r--   0        0        0      446 2023-03-22 18:41:55.809147 django_google_cloud_tasks-2.2.4/django_cloud_tasks/context.py
+-rw-r--r--   0        0        0      373 2023-03-15 20:17:34.220121 django_google_cloud_tasks-2.2.4/django_cloud_tasks/exceptions.py
+-rw-r--r--   0        0        0     1389 2023-03-15 20:17:33.764578 django_google_cloud_tasks-2.2.4/django_cloud_tasks/field.py
+-rw-r--r--   0        0        0        0 2022-11-21 14:22:47.495972 django_google_cloud_tasks-2.2.4/django_cloud_tasks/management/__init__.py
+-rw-r--r--   0        0        0      860 2023-03-15 20:17:33.597653 django_google_cloud_tasks-2.2.4/django_cloud_tasks/management/commands/__init__.py
+-rw-r--r--   0        0        0      490 2023-03-22 17:43:19.019827 django_google_cloud_tasks-2.2.4/django_cloud_tasks/management/commands/initialize_subscribers.py
+-rw-r--r--   0        0        0      394 2022-11-21 14:22:47.497092 django_google_cloud_tasks-2.2.4/django_cloud_tasks/management/commands/initialize_tasks.py
+-rw-r--r--   0        0        0      501 2022-11-21 14:22:47.497226 django_google_cloud_tasks-2.2.4/django_cloud_tasks/management/commands/schedule_tasks.py
+-rw-r--r--   0        0        0      252 2023-03-22 17:43:19.344171 django_google_cloud_tasks-2.2.4/django_cloud_tasks/middleware/__init__.py
+-rw-r--r--   0        0        0     1179 2023-03-22 17:43:18.952608 django_google_cloud_tasks-2.2.4/django_cloud_tasks/middleware/headers_context_middlware.py
+-rw-r--r--   0        0        0     1870 2023-04-12 23:12:38.891213 django_google_cloud_tasks-2.2.4/django_cloud_tasks/middleware/pubsub_headers_middleware.py
+-rw-r--r--   0        0        0     3888 2023-03-15 20:17:33.597800 django_google_cloud_tasks-2.2.4/django_cloud_tasks/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1024 2023-03-15 20:17:33.764958 django_google_cloud_tasks-2.2.4/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py
+-rw-r--r--   0        0        0        0 2022-11-21 14:22:47.496709 django_google_cloud_tasks-2.2.4/django_cloud_tasks/migrations/__init__.py
+-rw-r--r--   0        0        0     4364 2023-05-23 19:53:58.588811 django_google_cloud_tasks-2.2.4/django_cloud_tasks/models.py
+-rw-r--r--   0        0        0      925 2022-11-21 14:22:47.497904 django_google_cloud_tasks-2.2.4/django_cloud_tasks/serializers.py
+-rw-r--r--   0        0        0     2704 2023-05-23 19:53:58.588930 django_google_cloud_tasks-2.2.4/django_cloud_tasks/signals.py
+-rw-r--r--   0        0        0      667 2023-03-15 20:17:34.347222 django_google_cloud_tasks-2.2.4/django_cloud_tasks/tasks/__init__.py
+-rw-r--r--   0        0        0     1118 2023-03-15 20:17:34.101243 django_google_cloud_tasks-2.2.4/django_cloud_tasks/tasks/periodic_task.py
+-rw-r--r--   0        0        0     4775 2023-03-22 18:15:18.921786 django_google_cloud_tasks-2.2.4/django_cloud_tasks/tasks/publisher_task.py
+-rw-r--r--   0        0        0     2522 2023-03-15 20:17:34.143566 django_google_cloud_tasks-2.2.4/django_cloud_tasks/tasks/routine_task.py
+-rw-r--r--   0        0        0     2610 2023-04-12 23:12:38.881460 django_google_cloud_tasks-2.2.4/django_cloud_tasks/tasks/subscriber_task.py
+-rw-r--r--   0        0        0    10404 2023-05-23 20:07:52.385717 django_google_cloud_tasks-2.2.4/django_cloud_tasks/tasks/task.py
+-rw-r--r--   0        0        0        0 2023-03-13 22:03:16.402866 django_google_cloud_tasks-2.2.4/django_cloud_tasks/tests/__init__.py
+-rw-r--r--   0        0        0      985 2023-03-15 20:17:34.384480 django_google_cloud_tasks-2.2.4/django_cloud_tasks/tests/factories.py
+-rw-r--r--   0        0        0      871 2023-03-15 20:17:34.384727 django_google_cloud_tasks-2.2.4/django_cloud_tasks/tests/tests_base.py
+-rw-r--r--   0        0        0      291 2022-11-21 14:22:47.500083 django_google_cloud_tasks-2.2.4/django_cloud_tasks/urls.py
+-rw-r--r--   0        0        0     3014 2023-04-12 23:17:48.891352 django_google_cloud_tasks-2.2.4/django_cloud_tasks/views.py
+-rw-r--r--   0        0        0      772 2023-05-23 21:02:16.421779 django_google_cloud_tasks-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 django_google_cloud_tasks-2.2.4/PKG-INFO
```

### Comparing `django_google_cloud_tasks-2.2.3/LICENSE.md` & `django_google_cloud_tasks-2.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.3/django_cloud_tasks/apps.py` & `django_google_cloud_tasks-2.2.4/django_cloud_tasks/apps.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.3/django_cloud_tasks/field.py` & `django_google_cloud_tasks-2.2.4/django_cloud_tasks/field.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.3/django_cloud_tasks/management/commands/__init__.py` & `django_google_cloud_tasks-2.2.4/django_cloud_tasks/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.3/django_cloud_tasks/middleware/headers_context_middlware.py` & `django_google_cloud_tasks-2.2.4/django_cloud_tasks/middleware/headers_context_middlware.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.3/django_cloud_tasks/middleware/pubsub_headers_middleware.py` & `django_google_cloud_tasks-2.2.4/django_cloud_tasks/middleware/pubsub_headers_middleware.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.3/django_cloud_tasks/migrations/0001_initial.py` & `django_google_cloud_tasks-2.2.4/django_cloud_tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.3/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py` & `django_google_cloud_tasks-2.2.4/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.3/django_cloud_tasks/models.py` & `django_google_cloud_tasks-2.2.4/django_cloud_tasks/models.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.3/django_cloud_tasks/serializers.py` & `django_google_cloud_tasks-2.2.4/django_cloud_tasks/serializers.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.3/django_cloud_tasks/signals.py` & `django_google_cloud_tasks-2.2.4/django_cloud_tasks/signals.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/__init__.py` & `django_google_cloud_tasks-2.2.4/django_cloud_tasks/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/periodic_task.py` & `django_google_cloud_tasks-2.2.4/django_cloud_tasks/tasks/periodic_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/publisher_task.py` & `django_google_cloud_tasks-2.2.4/django_cloud_tasks/tasks/publisher_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/routine_task.py` & `django_google_cloud_tasks-2.2.4/django_cloud_tasks/tasks/routine_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/subscriber_task.py` & `django_google_cloud_tasks-2.2.4/django_cloud_tasks/tasks/subscriber_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.3/django_cloud_tasks/tasks/task.py` & `django_google_cloud_tasks-2.2.4/django_cloud_tasks/tasks/task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.3/django_cloud_tasks/tests/factories.py` & `django_google_cloud_tasks-2.2.4/django_cloud_tasks/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.3/django_cloud_tasks/tests/tests_base.py` & `django_google_cloud_tasks-2.2.4/django_cloud_tasks/tests/tests_base.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.3/django_cloud_tasks/views.py` & `django_google_cloud_tasks-2.2.4/django_cloud_tasks/views.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.2.3/pyproject.toml` & `django_google_cloud_tasks-2.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-google-cloud-tasks"
-version = "2.2.3"
+version = "2.2.4"
 description = "Async Tasks with HTTP endpoints"
 authors = ["Joao Daher <joao@daher.dev>"]
 packages = [
     { include = "django_cloud_tasks" },
 ]
 
 [tool.poetry.dependencies]
```

