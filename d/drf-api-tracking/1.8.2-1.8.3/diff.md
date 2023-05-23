# Comparing `tmp/drf-api-tracking-1.8.2.tar.gz` & `tmp/drf-api-tracking-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-api-tracking-1.8.2.tar", last modified: Thu May 11 19:07:17 2023, max compression
+gzip compressed data, was "drf-api-tracking-1.8.3.tar", last modified: Tue May 23 19:20:38 2023, max compression
```

## Comparing `drf-api-tracking-1.8.2.tar` & `drf-api-tracking-1.8.3.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 ling      (1000) ling      (1000)        0 2023-05-11 19:07:17.519522 drf-api-tracking-1.8.2/
--rw-rw-r--   0 ling      (1000) ling      (1000)       61 2020-02-21 11:51:40.000000 drf-api-tracking-1.8.2/MANIFEST.in
--rw-r--r--   0 ling      (1000) ling      (1000)    12265 2023-05-11 19:07:17.519522 drf-api-tracking-1.8.2/PKG-INFO
--rw-r--r--   0 ling      (1000) ling      (1000)     9092 2023-05-11 19:05:54.000000 drf-api-tracking-1.8.2/README.md
-drwxr-xr-x   0 ling      (1000) ling      (1000)        0 2023-05-11 19:07:17.516188 drf-api-tracking-1.8.2/drf_api_tracking.egg-info/
--rw-rw-r--   0 ling      (1000) ling      (1000)    12265 2023-05-11 19:07:17.000000 drf-api-tracking-1.8.2/drf_api_tracking.egg-info/PKG-INFO
--rw-rw-r--   0 ling      (1000) ling      (1000)     1522 2023-05-11 19:07:17.000000 drf-api-tracking-1.8.2/drf_api_tracking.egg-info/SOURCES.txt
--rw-rw-r--   0 ling      (1000) ling      (1000)        1 2023-05-11 19:07:17.000000 drf-api-tracking-1.8.2/drf_api_tracking.egg-info/dependency_links.txt
--rw-rw-r--   0 ling      (1000) ling      (1000)       40 2023-05-11 19:07:17.000000 drf-api-tracking-1.8.2/drf_api_tracking.egg-info/requires.txt
--rw-rw-r--   0 ling      (1000) ling      (1000)       59 2023-05-11 19:07:17.000000 drf-api-tracking-1.8.2/drf_api_tracking.egg-info/top_level.txt
--rw-r--r--   0 ling      (1000) ling      (1000)      463 2021-05-03 10:30:46.000000 drf-api-tracking-1.8.2/pyproject.toml
-drwxr-xr-x   0 ling      (1000) ling      (1000)        0 2023-05-11 19:07:17.516188 drf-api-tracking-1.8.2/rest_framework_tracking/
--rw-r--r--   0 ling      (1000) ling      (1000)      149 2023-05-11 19:06:59.000000 drf-api-tracking-1.8.2/rest_framework_tracking/__init__.py
--rw-r--r--   0 ling      (1000) ling      (1000)     2982 2023-05-11 19:05:54.000000 drf-api-tracking-1.8.2/rest_framework_tracking/admin.py
--rw-r--r--   0 ling      (1000) ling      (1000)     1064 2023-05-11 18:58:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/app_settings.py
--rw-r--r--   0 ling      (1000) ling      (1000)      164 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/apps.py
--rw-r--r--   0 ling      (1000) ling      (1000)     8359 2023-05-11 19:05:54.000000 drf-api-tracking-1.8.2/rest_framework_tracking/base_mixins.py
--rw-r--r--   0 ling      (1000) ling      (1000)     1851 2023-05-11 19:05:54.000000 drf-api-tracking-1.8.2/rest_framework_tracking/base_models.py
-drwxr-xr-x   0 ling      (1000) ling      (1000)        0 2023-05-11 19:07:17.516188 drf-api-tracking-1.8.2/rest_framework_tracking/management/
-drwxr-xr-x   0 ling      (1000) ling      (1000)        0 2023-05-11 19:07:17.519522 drf-api-tracking-1.8.2/rest_framework_tracking/management/commands/
--rw-r--r--   0 ling      (1000) ling      (1000)     1238 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/management/commands/clearapilogs.py
--rw-r--r--   0 ling      (1000) ling      (1000)      188 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/managers.py
-drwxr-xr-x   0 ling      (1000) ling      (1000)        0 2023-05-11 19:07:17.519522 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/
--rw-r--r--   0 ling      (1000) ling      (1000)     1886 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0001_initial.py
--rw-r--r--   0 ling      (1000) ling      (1000)      749 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0002_auto_20170118_1713.py
--rw-r--r--   0 ling      (1000) ling      (1000)      409 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0003_add_errors.py
--rw-r--r--   0 ling      (1000) ling      (1000)      438 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0004_add_verbose_name.py
--rw-r--r--   0 ling      (1000) ling      (1000)      698 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0005_auto_20171219_1537.py
--rw-r--r--   0 ling      (1000) ling      (1000)      702 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0006_auto_20180315_1442.py
--rw-r--r--   0 ling      (1000) ling      (1000)      745 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0006_view_and_view_method_nullable.py
--rw-r--r--   0 ling      (1000) ling      (1000)      335 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0007_merge_20180419_1646.py
--rw-r--r--   0 ling      (1000) ling      (1000)      521 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0008_auto_20200201_2048.py
--rw-r--r--   0 ling      (1000) ling      (1000)      549 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0009_view_method_max_length_200.py
--rw-r--r--   0 ling      (1000) ling      (1000)      986 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0010_auto_20200609_1404.py
--rw-r--r--   0 ling      (1000) ling      (1000)      449 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0011_auto_20201117_2016.py
--rw-rw-r--   0 ling      (1000) ling      (1000)        0 2020-02-21 11:51:40.000000 drf-api-tracking-1.8.2/rest_framework_tracking/migrations/__init__.py
--rw-rw-r--   0 ling      (1000) ling      (1000)      472 2020-02-21 11:51:40.000000 drf-api-tracking-1.8.2/rest_framework_tracking/mixins.py
--rw-rw-r--   0 ling      (1000) ling      (1000)       94 2020-02-21 11:51:40.000000 drf-api-tracking-1.8.2/rest_framework_tracking/models.py
-drwxr-xr-x   0 ling      (1000) ling      (1000)        0 2023-05-11 19:07:17.516188 drf-api-tracking-1.8.2/rest_framework_tracking/templates/
-drwxr-xr-x   0 ling      (1000) ling      (1000)        0 2023-05-11 19:07:17.516188 drf-api-tracking-1.8.2/rest_framework_tracking/templates/admin/
-drwxr-xr-x   0 ling      (1000) ling      (1000)        0 2023-05-11 19:07:17.516188 drf-api-tracking-1.8.2/rest_framework_tracking/templates/admin/rest_framework_tracking/
-drwxr-xr-x   0 ling      (1000) ling      (1000)        0 2023-05-11 19:07:17.519522 drf-api-tracking-1.8.2/rest_framework_tracking/templates/admin/rest_framework_tracking/apirequestlog/
--rw-r--r--   0 ling      (1000) ling      (1000)     4699 2023-05-11 19:05:54.000000 drf-api-tracking-1.8.2/rest_framework_tracking/templates/admin/rest_framework_tracking/apirequestlog/change_list.html
--rw-rw-r--   0 ling      (1000) ling      (1000)       61 2023-05-11 19:07:17.519522 drf-api-tracking-1.8.2/setup.cfg
--rw-r--r--   0 ling      (1000) ling      (1000)     3625 2021-05-02 12:20:56.000000 drf-api-tracking-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:38.723967 drf-api-tracking-1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-05-23 19:20:38.727967 drf-api-tracking-1.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:38.723967 drf-api-tracking-1.8.3/drf_api_tracking.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-05-23 19:20:38.000000 drf-api-tracking-1.8.3/drf_api_tracking.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-23 19:20:38.000000 drf-api-tracking-1.8.3/drf_api_tracking.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 19:20:38.000000 drf-api-tracking-1.8.3/drf_api_tracking.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-23 19:20:38.000000 drf-api-tracking-1.8.3/drf_api_tracking.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-23 19:20:38.000000 drf-api-tracking-1.8.3/drf_api_tracking.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:38.723967 drf-api-tracking-1.8.3/rest_framework_tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/base_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/base_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:38.723967 drf-api-tracking-1.8.3/rest_framework_tracking/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:38.723967 drf-api-tracking-1.8.3/rest_framework_tracking/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/management/commands/clearapilogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:38.723967 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0002_auto_20170118_1713.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0003_add_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0004_add_verbose_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0005_auto_20171219_1537.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0006_auto_20180315_1442.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0006_view_and_view_method_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0007_merge_20180419_1646.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0008_auto_20200201_2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0009_view_method_max_length_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0010_auto_20200609_1404.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0011_auto_20201117_2016.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0012_auto_20210930_0713.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:38.723967 drf-api-tracking-1.8.3/rest_framework_tracking/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:38.723967 drf-api-tracking-1.8.3/rest_framework_tracking/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:38.723967 drf-api-tracking-1.8.3/rest_framework_tracking/templates/admin/rest_framework_tracking/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:20:38.723967 drf-api-tracking-1.8.3/rest_framework_tracking/templates/admin/rest_framework_tracking/apirequestlog/
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/rest_framework_tracking/templates/admin/rest_framework_tracking/apirequestlog/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-23 19:20:38.727967 drf-api-tracking-1.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-23 19:20:27.000000 drf-api-tracking-1.8.3/setup.py
```

### Comparing `drf-api-tracking-1.8.2/PKG-INFO` & `drf-api-tracking-1.8.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,266 +1,15 @@
 Metadata-Version: 2.1
 Name: drf-api-tracking
-Version: 1.8.2
+Version: 1.8.3
 Summary: Utils to log Django Rest Framework requests to the database
 Home-page: https://github.com/lingster/drf-api-tracking
 Author: Anna Schneider
 Author-email: anna@WattTime.org
 License: BSD
-Description: # drf-api-tracking
-        
-        [![build-status-image]][travis]
-        [![pypi-version]][pypi]
-        [![Requirements Status](https://requires.io/github/lingster/drf-api-tracking/requirements.svg?branch=master)](https://requires.io/github/lingster/drf-api-tracking/requirements/?branch=master)
-        [![Coverage Status](https://coveralls.io/repos/github/lingster/drf-api-tracking/badge.svg?branch=master)](https://coveralls.io/github/lingster/drf-api-tracking?branch=master)
-        
-        ## Overview
-        
-        drf-api-tracking provides a Django model and DRF view mixin that work together to log Django Rest Framework requests to the database. You'll get these attributes for every request/response cycle to a view that uses the mixin:
-        
-        
-         Model field name | Description | Model field type
-        ------------------|-------------|-----------------
-        `user` | User if authenticated, None if not | Foreign Key
-        `username_persistent` | Static field that persists the username even if the User model object is deleted | CharField
-        `requested_at` | Date-time that the request was made | DateTimeField
-        `response_ms` | Number of milliseconds spent in view code | PositiveIntegerField
-        `path` | Target URI of the request, e.g., `"/api/"` | CharField
-        `view` | Target VIEW of the request, e.g., `"views.api.ApiView"` | CharField
-        `view_method` | Target METHOD of the VIEW of the request, e.g., `"get"` | CharField
-        `remote_addr` | IP address where the request originated (X_FORWARDED_FOR if available, REMOTE_ADDR if not), e.g., `"127.0.0.1"` | GenericIPAddressField
-        `host` | Originating host of the request, e.g., `"example.com"` | URLField
-        `method` | HTTP method, e.g., `"GET"` | CharField
-        `query_params` | Dictionary of request query parameters, as text | TextField
-        `data` | Dictionary of POST data (JSON or form), as text | TextField
-        `response` | JSON response data | TextField
-        `status_code` | HTTP status code, e.g., `200` or `404` | PositiveIntegerField
-        
-        
-        ## Requirements
-        
-        * Django 1.11, 2.0, 2.1, 2.2, 3.0
-        * Django REST Framework and Python release supporting the version of Django you are using
-        
-        Django | Python | DRF
-        -------|--------|----
-        1.11 | 2.7, 3.5, 3.6 | 3.5, 3.6, 3.7, 3.8, 3.9
-        2.0 | 3.5, 3.6, 3.7 | 3.7, 3.8, 3.9
-        2.1 | 3.5, 3.6, 3.7, 3.8 | 3.7, 3.8, 3.9
-        2.2 | 3.5, 3.6, 3.7, 3.8 | 3.7, 3.8, 3.9
-        3.0 | 3.5, 3.6, 3.7, 3.8 | 3.7, 3.8, 3.9
-        
-        ## Installation
-        
-        Install using `pip`...
-        
-        ``` bash
-        $ pip install drf-api-tracking
-        ```
-        
-        Register with your Django project by adding `rest_framework_tracking`
-        to the `INSTALLED_APPS` list in your project's `settings.py` file.
-        Then run the migrations for the `APIRequestLog` model:
-        
-        ``` bash
-        $ python manage.py migrate
-        ```
-        
-        ## Usage
-        
-        Add the `rest_framework_tracking.mixins.LoggingMixin` to any DRF view
-        to create an instance of `APIRequestLog` every time the view is called.
-        
-        For instance:
-        ``` python
-        # views.py
-        from rest_framework import generics
-        from rest_framework.response import Response
-        from rest_framework_tracking.mixins import LoggingMixin
-        
-        class LoggingView(LoggingMixin, generics.GenericAPIView):
-            def get(self, request):
-                return Response('with logging')
-        ```
-        
-        For performance enhancement, explicitly choose methods to be logged using `logging_methods` attribute:
-        
-        ``` python
-        class LoggingView(LoggingMixin, generics.CreateModelMixin, generics.GenericAPIView):
-            logging_methods = ['POST', 'PUT']
-            model = ...
-        ```
-        
-        Moreover, you could define your own rules by overriding `should_log` method.
-        If `should_log` evaluates to True a log is created.
-        
-        ``` python
-        class LoggingView(LoggingMixin, generics.GenericAPIView):
-            def should_log(self, request, response):
-                """Log only errors"""
-                return response.status_code >= 400
-        ```
-        
-        At the example above, `logging_methods` attribute will be ignored. If you want to provide some extra rules
-        on top of the http method filtering you should rewrite the `should_log` method.
-        
-        ``` python
-        class LoggingView(LoggingMixin, generics.GenericAPIView):
-            def should_log(self, request, response):
-                """Log only errors with respect on `logging_methods` attributes"""
-                should_log_method = super(LoggingView, self).should_log(request, response)
-                if not should_log_method:
-                    return False
-                return response.status_code >= 400
-        ```
-        
-         A bit simpler.
-        ``` python
-        class LoggingView(LoggingMixin, generics.GenericAPIView):
-            def should_log(self, request, response):
-                """Log only errors with respect on `logging_methods` attributes"""
-                if not request.method in self.logging_methods:
-                    return False
-                return response.status_code >= 400
-        ```
-        
-        Finally, you can also apply your customizations by overriding `handle_log` method.
-        By default, all requests that satisfy `should_log` method are saved on the database.
-        ``` python
-        class LoggingView(LoggingMixin, generics.GenericAPIView):
-            def handle_log(self):
-                # Do some stuff before saving.
-                super(MockCustomLogHandlerView, self).handle_log()
-                # Do some stuff after saving.
-        ```
-        
-        
-        Though, you could define your own handling. For example save on an in-memory data structure store, remote logging system etc.
-        ``` python
-        class LoggingView(LoggingMixin, generics.GenericAPIView):
-        
-            def handle_log(self):
-                cache.set('my_key', self.log, 86400)
-        ```
-        
-        Or you could omit save a request to the database. For example,
-        ``` python
-        class LoggingView(LoggingMixin, generics.GenericAPIView):
-            def handle_log(self):
-                """
-                Save only very slow requests. Requests that took more than a second.
-                """
-                if self.log['response_ms'] > 1000:
-                    super(MockCustomLogHandlerView, self).handle_log()
-        ```
-        
-        If your endpoint accepts large file uploads, drf-api-tracking's default behavior to decode the request body may cause a `RequestDataTooBig` exception. This behavior can be disabled globally by setting `DRF_TRACKING_DECODE_REQUEST_BODY = False` in your `settings.py`file.
-        
-        You can also customize this behavior for individual views by setting the `decode_request_body` attribute:
-        
-        ``` python
-        class LoggingView(LoggingMixin, generics.GenericAPIView):
-            decode_request_body = False
-        ```
-        
-        ## Security
-        
-        By default drf-api-tracking is hiding the values of those fields `{'api', 'token', 'key', 'secret', 'password', 'signature'}`.
-        The default list hast been taken from Django itself ([https://github.com/django/django/blob/stable/1.11.x/django/contrib/auth/__init__.py#L50](https://github.com/django/django/blob/stable/1.11.x/django/contrib/auth/__init__.py#L50)).
-        
-        You can complete this list with your own list by putting the fields you want to be hidden in the `sensitive_fields` parameter of your view.
-        
-        ``` python
-        class LoggingView(LoggingMixin, generics.CreateModelMixin, generics.GenericAPIView):
-            sensitive_fields = {'my_secret_key', 'my_secret_recipe'}
-        ```
-        
-        By default drf-tracking allows API request log entries to be modified from Django admin. This can present a data integrity issue in production environments. In order to change this behavior, you can set `DRF_TRACKING_ADMIN_LOG_READONLY` to `True` in your `settings.py` file.
-        
-        ## Development
-        In the folder there is a sample drf project: `drf_api_sample` if changes are made to this packages models, use this project
-        to help generate new migrations, which should be checked in.
-        
-        ## Testing
-        
-        Install testing requirements.
-        
-        ``` bash
-        $ pip install -r requirements.txt
-        ```
-        
-        Run with runtests.
-        
-        ``` bash
-        $ ./runtests.py
-        ```
-        
-        You can also use the excellent [tox](http://tox.readthedocs.org/en/latest/) testing tool to run the tests against all supported versions of Python and Django. Install tox globally, and then simply run:
-        
-        ``` bash
-        $ tox
-        ```
-        you can also use pyenv to install multiple versions of python and ensure they are found by tox by issuing:
-        ``` bash
-        pyenv install 3.8.4
-        pyenv install 3.7.7
-        pyenv install 3.6.11
-        pyenv local 3.8.4 3.7.7 3.6.11
-        pyenv global 3.8.4 3.7.7 3.6.11
-        ```
-        Also ensure that you don't have a virtualenv activated when you run the tests else you might get the following error, or similar:
-        `
-        ERROR: InterpreterNotFound: python3.6
-        `
-        
-        ## Documentation
-        
-        To build the documentation, you'll need to install `mkdocs`.
-        
-        ``` bash
-        $ pip install mkdocs
-        ```
-        
-        To preview the documentation:
-        
-        ``` bash
-        $ mkdocs serve
-        Running at: http://127.0.0.1:8000/
-        ```
-        
-        To build the documentation:
-        
-        ``` bash
-        $ mkdocs build
-        ```
-        
-        
-        [build-status-image]: https://secure.travis-ci.org/lingster/drf-api-tracking.png?branch=master
-        [travis]: http://travis-ci.org/lingster/drf-api-tracking?branch=master
-        [pypi-version]: https://img.shields.io/pypi/v/drf-api-tracking.svg
-        [pypi]: https://pypi.python.org/pypi/drf-api-tracking
-        
-        
-        # travis
-        Install RVM to have a local user version of ruby/gem:
-        `https://rvm.io/rvm/install`
-        Then install travis like this:
-        `gem install travis`
-        add your secret key as per the link below:
-        `https://docs.travis-ci.com/user/encryption-keys/`
-        
-        pyenv
-        ---
-        using pyenv you can install multiple versions of python so that tox can run tests against all installed versions of python
-        ``` bash
-        pyenv global 3.6.8 3.7.7 3.8.2
-        ```
-        ensure that before running tox you don't have a virtualenv created and tox has been installed globally or via pipx
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
@@ -273,7 +22,273 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Description-Content-Type: text/markdown; charset=UTF-8
+License-File: LICENSE
+
+# drf-api-tracking
+
+[![build-status-image]][travis]
+[![pypi-version]][pypi]
+[![Requirements Status](https://requires.io/github/lingster/drf-api-tracking/requirements.svg?branch=master)](https://requires.io/github/lingster/drf-api-tracking/requirements/?branch=master)
+[![Coverage Status](https://coveralls.io/repos/github/lingster/drf-api-tracking/badge.svg?branch=master)](https://coveralls.io/github/lingster/drf-api-tracking?branch=master)
+
+## Overview
+
+drf-api-tracking provides a Django model and DRF view mixin that work together to log Django Rest Framework requests to the database. You'll get these attributes for every request/response cycle to a view that uses the mixin:
+
+
+ Model field name | Description | Model field type
+------------------|-------------|-----------------
+`user` | User if authenticated, None if not | Foreign Key
+`username_persistent` | Static field that persists the username even if the User model object is deleted | CharField
+`requested_at` | Date-time that the request was made | DateTimeField
+`response_ms` | Number of milliseconds spent in view code | PositiveIntegerField
+`path` | Target URI of the request, e.g., `"/api/"` | CharField
+`view` | Target VIEW of the request, e.g., `"views.api.ApiView"` | CharField
+`view_method` | Target METHOD of the VIEW of the request, e.g., `"get"` | CharField
+`remote_addr` | IP address where the request originated (X_FORWARDED_FOR if available, REMOTE_ADDR if not), e.g., `"127.0.0.1"` | GenericIPAddressField
+`host` | Originating host of the request, e.g., `"example.com"` | URLField
+`method` | HTTP method, e.g., `"GET"` | CharField
+`query_params` | Dictionary of request query parameters, as text | TextField
+`data` | Dictionary of POST data (JSON or form), as text | TextField
+`response` | JSON response data | TextField
+`status_code` | HTTP status code, e.g., `200` or `404` | PositiveIntegerField
+
+
+## Requirements
+
+* Django 1.11, 2.0, 2.1, 2.2, 3.0
+* Django REST Framework and Python release supporting the version of Django you are using
+
+Django | Python | DRF
+-------|--------|----
+1.11 | 2.7, 3.5, 3.6 | 3.5, 3.6, 3.7, 3.8, 3.9
+2.0 | 3.5, 3.6, 3.7 | 3.7, 3.8, 3.9
+2.1 | 3.5, 3.6, 3.7, 3.8 | 3.7, 3.8, 3.9
+2.2 | 3.5, 3.6, 3.7, 3.8 | 3.7, 3.8, 3.9
+3.0 | 3.5, 3.6, 3.7, 3.8 | 3.7, 3.8, 3.9
+
+## Installation
+
+Install using `pip`...
+
+``` bash
+$ pip install drf-api-tracking
+```
+
+Register with your Django project by adding `rest_framework_tracking`
+to the `INSTALLED_APPS` list in your project's `settings.py` file.
+Then run the migrations for the `APIRequestLog` model:
+
+``` bash
+$ python manage.py migrate
+```
+
+## Usage
+
+Add the `rest_framework_tracking.mixins.LoggingMixin` to any DRF view
+to create an instance of `APIRequestLog` every time the view is called.
+
+For instance:
+``` python
+# views.py
+from rest_framework import generics
+from rest_framework.response import Response
+from rest_framework_tracking.mixins import LoggingMixin
+
+class LoggingView(LoggingMixin, generics.GenericAPIView):
+    def get(self, request):
+        return Response('with logging')
+```
+
+For performance enhancement, explicitly choose methods to be logged using `logging_methods` attribute:
+
+``` python
+class LoggingView(LoggingMixin, generics.CreateModelMixin, generics.GenericAPIView):
+    logging_methods = ['POST', 'PUT']
+    model = ...
+```
+
+Moreover, you could define your own rules by overriding `should_log` method.
+If `should_log` evaluates to True a log is created.
+
+``` python
+class LoggingView(LoggingMixin, generics.GenericAPIView):
+    def should_log(self, request, response):
+        """Log only errors"""
+        return response.status_code >= 400
+```
+
+At the example above, `logging_methods` attribute will be ignored. If you want to provide some extra rules
+on top of the http method filtering you should rewrite the `should_log` method.
+
+``` python
+class LoggingView(LoggingMixin, generics.GenericAPIView):
+    def should_log(self, request, response):
+        """Log only errors with respect on `logging_methods` attributes"""
+        should_log_method = super(LoggingView, self).should_log(request, response)
+        if not should_log_method:
+            return False
+        return response.status_code >= 400
+```
+
+ A bit simpler.
+``` python
+class LoggingView(LoggingMixin, generics.GenericAPIView):
+    def should_log(self, request, response):
+        """Log only errors with respect on `logging_methods` attributes"""
+        if not request.method in self.logging_methods:
+            return False
+        return response.status_code >= 400
+```
+
+Finally, you can also apply your customizations by overriding `handle_log` method.
+By default, all requests that satisfy `should_log` method are saved on the database.
+``` python
+class LoggingView(LoggingMixin, generics.GenericAPIView):
+    def handle_log(self):
+        # Do some stuff before saving.
+        super(MockCustomLogHandlerView, self).handle_log()
+        # Do some stuff after saving.
+```
+
+
+Though, you could define your own handling. For example save on an in-memory data structure store, remote logging system etc.
+``` python
+class LoggingView(LoggingMixin, generics.GenericAPIView):
+
+    def handle_log(self):
+        cache.set('my_key', self.log, 86400)
+```
+
+Or you could omit save a request to the database. For example,
+``` python
+class LoggingView(LoggingMixin, generics.GenericAPIView):
+    def handle_log(self):
+        """
+        Save only very slow requests. Requests that took more than a second.
+        """
+        if self.log['response_ms'] > 1000:
+            super(MockCustomLogHandlerView, self).handle_log()
+```
+
+If your endpoint accepts large file uploads, drf-api-tracking's default behavior to decode the request body may cause a `RequestDataTooBig` exception. This behavior can be disabled globally by setting `DRF_TRACKING_DECODE_REQUEST_BODY = False` in your `settings.py`file.
+
+You can also customize this behavior for individual views by setting the `decode_request_body` attribute:
+
+``` python
+class LoggingView(LoggingMixin, generics.GenericAPIView):
+    decode_request_body = False
+```
+
+## Security
+
+By default drf-api-tracking is hiding the values of those fields `{'api', 'token', 'key', 'secret', 'password', 'signature'}`.
+The default list hast been taken from Django itself ([https://github.com/django/django/blob/stable/1.11.x/django/contrib/auth/__init__.py#L50](https://github.com/django/django/blob/stable/1.11.x/django/contrib/auth/__init__.py#L50)).
+
+You can complete this list with your own list by putting the fields you want to be hidden in the `sensitive_fields` parameter of your view.
+
+``` python
+class LoggingView(LoggingMixin, generics.CreateModelMixin, generics.GenericAPIView):
+    sensitive_fields = {'my_secret_key', 'my_secret_recipe'}
+```
+
+By default drf-tracking allows API request log entries to be modified from Django admin. This can present a data integrity issue in production environments. In order to change this behavior, you can set `DRF_TRACKING_ADMIN_LOG_READONLY` to `True` in your `settings.py` file.
+
+## Development
+In the folder there is a sample drf project: `drf_api_sample` if changes are made to this packages models, use this project
+to help generate new migrations, which should be checked in.
+
+## Testing
+
+Install testing requirements.
+
+``` bash
+$ pip install -r requirements.txt
+```
+
+Run with runtests.
+
+``` bash
+$ ./runtests.py
+```
+
+You can also use the excellent [tox](http://tox.readthedocs.org/en/latest/) testing tool to run the tests against all supported versions of Python and Django. Install tox globally, and then simply run:
+
+``` bash
+$ tox
+```
+you can also use pyenv to install multiple versions of python and ensure they are found by tox by issuing:
+``` bash
+pyenv install 3.8.4
+pyenv install 3.7.7
+pyenv install 3.6.11
+pyenv local 3.8.4 3.7.7 3.6.11
+pyenv global 3.8.4 3.7.7 3.6.11
+```
+Also ensure that you don't have a virtualenv activated when you run the tests else you might get the following error, or similar:
+`
+ERROR: InterpreterNotFound: python3.6
+`
+
+## Contributing
+
+In order to make changes to the package itself, providing migrations or something else,
+make sure to install the current package with pip, otherwise using the `drf_api_sample` won't work.
+
+``` bash
+pip install -e .
+```
+
+After this, you can edit models and creating migrations with
+
+``` bash
+python drf_api_sample/manage.py makemigrations
+```
+
+## Documentation
+
+To build the documentation, you'll need to install `mkdocs`.
+
+``` bash
+$ pip install mkdocs
+```
+
+To preview the documentation:
+
+``` bash
+$ mkdocs serve
+Running at: http://127.0.0.1:8000/
+```
+
+To build the documentation:
+
+``` bash
+$ mkdocs build
+```
+
+
+[build-status-image]: https://secure.travis-ci.org/lingster/drf-api-tracking.png?branch=master
+[travis]: http://travis-ci.org/lingster/drf-api-tracking?branch=master
+[pypi-version]: https://img.shields.io/pypi/v/drf-api-tracking.svg
+[pypi]: https://pypi.python.org/pypi/drf-api-tracking
+
+
+# travis
+Install RVM to have a local user version of ruby/gem:
+`https://rvm.io/rvm/install`
+Then install travis like this:
+`gem install travis`
+add your secret key as per the link below:
+`https://docs.travis-ci.com/user/encryption-keys/`
+
+pyenv
+---
+using pyenv you can install multiple versions of python so that tox can run tests against all installed versions of python
+``` bash
+pyenv global 3.6.8 3.7.7 3.8.2
+```
+ensure that before running tox you don't have a virtualenv created and tox has been installed globally or via pipx
```

### Comparing `drf-api-tracking-1.8.2/README.md` & `drf-api-tracking-1.8.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -200,14 +200,29 @@
 pyenv global 3.8.4 3.7.7 3.6.11
 ```
 Also ensure that you don't have a virtualenv activated when you run the tests else you might get the following error, or similar:
 `
 ERROR: InterpreterNotFound: python3.6
 `
 
+## Contributing
+
+In order to make changes to the package itself, providing migrations or something else,
+make sure to install the current package with pip, otherwise using the `drf_api_sample` won't work.
+
+``` bash
+pip install -e .
+```
+
+After this, you can edit models and creating migrations with
+
+``` bash
+python drf_api_sample/manage.py makemigrations
+```
+
 ## Documentation
 
 To build the documentation, you'll need to install `mkdocs`.
 
 ``` bash
 $ pip install mkdocs
 ```
```

### Comparing `drf-api-tracking-1.8.2/drf_api_tracking.egg-info/PKG-INFO` & `drf-api-tracking-1.8.3/drf_api_tracking.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,266 +1,15 @@
 Metadata-Version: 2.1
 Name: drf-api-tracking
-Version: 1.8.2
+Version: 1.8.3
 Summary: Utils to log Django Rest Framework requests to the database
 Home-page: https://github.com/lingster/drf-api-tracking
 Author: Anna Schneider
 Author-email: anna@WattTime.org
 License: BSD
-Description: # drf-api-tracking
-        
-        [![build-status-image]][travis]
-        [![pypi-version]][pypi]
-        [![Requirements Status](https://requires.io/github/lingster/drf-api-tracking/requirements.svg?branch=master)](https://requires.io/github/lingster/drf-api-tracking/requirements/?branch=master)
-        [![Coverage Status](https://coveralls.io/repos/github/lingster/drf-api-tracking/badge.svg?branch=master)](https://coveralls.io/github/lingster/drf-api-tracking?branch=master)
-        
-        ## Overview
-        
-        drf-api-tracking provides a Django model and DRF view mixin that work together to log Django Rest Framework requests to the database. You'll get these attributes for every request/response cycle to a view that uses the mixin:
-        
-        
-         Model field name | Description | Model field type
-        ------------------|-------------|-----------------
-        `user` | User if authenticated, None if not | Foreign Key
-        `username_persistent` | Static field that persists the username even if the User model object is deleted | CharField
-        `requested_at` | Date-time that the request was made | DateTimeField
-        `response_ms` | Number of milliseconds spent in view code | PositiveIntegerField
-        `path` | Target URI of the request, e.g., `"/api/"` | CharField
-        `view` | Target VIEW of the request, e.g., `"views.api.ApiView"` | CharField
-        `view_method` | Target METHOD of the VIEW of the request, e.g., `"get"` | CharField
-        `remote_addr` | IP address where the request originated (X_FORWARDED_FOR if available, REMOTE_ADDR if not), e.g., `"127.0.0.1"` | GenericIPAddressField
-        `host` | Originating host of the request, e.g., `"example.com"` | URLField
-        `method` | HTTP method, e.g., `"GET"` | CharField
-        `query_params` | Dictionary of request query parameters, as text | TextField
-        `data` | Dictionary of POST data (JSON or form), as text | TextField
-        `response` | JSON response data | TextField
-        `status_code` | HTTP status code, e.g., `200` or `404` | PositiveIntegerField
-        
-        
-        ## Requirements
-        
-        * Django 1.11, 2.0, 2.1, 2.2, 3.0
-        * Django REST Framework and Python release supporting the version of Django you are using
-        
-        Django | Python | DRF
-        -------|--------|----
-        1.11 | 2.7, 3.5, 3.6 | 3.5, 3.6, 3.7, 3.8, 3.9
-        2.0 | 3.5, 3.6, 3.7 | 3.7, 3.8, 3.9
-        2.1 | 3.5, 3.6, 3.7, 3.8 | 3.7, 3.8, 3.9
-        2.2 | 3.5, 3.6, 3.7, 3.8 | 3.7, 3.8, 3.9
-        3.0 | 3.5, 3.6, 3.7, 3.8 | 3.7, 3.8, 3.9
-        
-        ## Installation
-        
-        Install using `pip`...
-        
-        ``` bash
-        $ pip install drf-api-tracking
-        ```
-        
-        Register with your Django project by adding `rest_framework_tracking`
-        to the `INSTALLED_APPS` list in your project's `settings.py` file.
-        Then run the migrations for the `APIRequestLog` model:
-        
-        ``` bash
-        $ python manage.py migrate
-        ```
-        
-        ## Usage
-        
-        Add the `rest_framework_tracking.mixins.LoggingMixin` to any DRF view
-        to create an instance of `APIRequestLog` every time the view is called.
-        
-        For instance:
-        ``` python
-        # views.py
-        from rest_framework import generics
-        from rest_framework.response import Response
-        from rest_framework_tracking.mixins import LoggingMixin
-        
-        class LoggingView(LoggingMixin, generics.GenericAPIView):
-            def get(self, request):
-                return Response('with logging')
-        ```
-        
-        For performance enhancement, explicitly choose methods to be logged using `logging_methods` attribute:
-        
-        ``` python
-        class LoggingView(LoggingMixin, generics.CreateModelMixin, generics.GenericAPIView):
-            logging_methods = ['POST', 'PUT']
-            model = ...
-        ```
-        
-        Moreover, you could define your own rules by overriding `should_log` method.
-        If `should_log` evaluates to True a log is created.
-        
-        ``` python
-        class LoggingView(LoggingMixin, generics.GenericAPIView):
-            def should_log(self, request, response):
-                """Log only errors"""
-                return response.status_code >= 400
-        ```
-        
-        At the example above, `logging_methods` attribute will be ignored. If you want to provide some extra rules
-        on top of the http method filtering you should rewrite the `should_log` method.
-        
-        ``` python
-        class LoggingView(LoggingMixin, generics.GenericAPIView):
-            def should_log(self, request, response):
-                """Log only errors with respect on `logging_methods` attributes"""
-                should_log_method = super(LoggingView, self).should_log(request, response)
-                if not should_log_method:
-                    return False
-                return response.status_code >= 400
-        ```
-        
-         A bit simpler.
-        ``` python
-        class LoggingView(LoggingMixin, generics.GenericAPIView):
-            def should_log(self, request, response):
-                """Log only errors with respect on `logging_methods` attributes"""
-                if not request.method in self.logging_methods:
-                    return False
-                return response.status_code >= 400
-        ```
-        
-        Finally, you can also apply your customizations by overriding `handle_log` method.
-        By default, all requests that satisfy `should_log` method are saved on the database.
-        ``` python
-        class LoggingView(LoggingMixin, generics.GenericAPIView):
-            def handle_log(self):
-                # Do some stuff before saving.
-                super(MockCustomLogHandlerView, self).handle_log()
-                # Do some stuff after saving.
-        ```
-        
-        
-        Though, you could define your own handling. For example save on an in-memory data structure store, remote logging system etc.
-        ``` python
-        class LoggingView(LoggingMixin, generics.GenericAPIView):
-        
-            def handle_log(self):
-                cache.set('my_key', self.log, 86400)
-        ```
-        
-        Or you could omit save a request to the database. For example,
-        ``` python
-        class LoggingView(LoggingMixin, generics.GenericAPIView):
-            def handle_log(self):
-                """
-                Save only very slow requests. Requests that took more than a second.
-                """
-                if self.log['response_ms'] > 1000:
-                    super(MockCustomLogHandlerView, self).handle_log()
-        ```
-        
-        If your endpoint accepts large file uploads, drf-api-tracking's default behavior to decode the request body may cause a `RequestDataTooBig` exception. This behavior can be disabled globally by setting `DRF_TRACKING_DECODE_REQUEST_BODY = False` in your `settings.py`file.
-        
-        You can also customize this behavior for individual views by setting the `decode_request_body` attribute:
-        
-        ``` python
-        class LoggingView(LoggingMixin, generics.GenericAPIView):
-            decode_request_body = False
-        ```
-        
-        ## Security
-        
-        By default drf-api-tracking is hiding the values of those fields `{'api', 'token', 'key', 'secret', 'password', 'signature'}`.
-        The default list hast been taken from Django itself ([https://github.com/django/django/blob/stable/1.11.x/django/contrib/auth/__init__.py#L50](https://github.com/django/django/blob/stable/1.11.x/django/contrib/auth/__init__.py#L50)).
-        
-        You can complete this list with your own list by putting the fields you want to be hidden in the `sensitive_fields` parameter of your view.
-        
-        ``` python
-        class LoggingView(LoggingMixin, generics.CreateModelMixin, generics.GenericAPIView):
-            sensitive_fields = {'my_secret_key', 'my_secret_recipe'}
-        ```
-        
-        By default drf-tracking allows API request log entries to be modified from Django admin. This can present a data integrity issue in production environments. In order to change this behavior, you can set `DRF_TRACKING_ADMIN_LOG_READONLY` to `True` in your `settings.py` file.
-        
-        ## Development
-        In the folder there is a sample drf project: `drf_api_sample` if changes are made to this packages models, use this project
-        to help generate new migrations, which should be checked in.
-        
-        ## Testing
-        
-        Install testing requirements.
-        
-        ``` bash
-        $ pip install -r requirements.txt
-        ```
-        
-        Run with runtests.
-        
-        ``` bash
-        $ ./runtests.py
-        ```
-        
-        You can also use the excellent [tox](http://tox.readthedocs.org/en/latest/) testing tool to run the tests against all supported versions of Python and Django. Install tox globally, and then simply run:
-        
-        ``` bash
-        $ tox
-        ```
-        you can also use pyenv to install multiple versions of python and ensure they are found by tox by issuing:
-        ``` bash
-        pyenv install 3.8.4
-        pyenv install 3.7.7
-        pyenv install 3.6.11
-        pyenv local 3.8.4 3.7.7 3.6.11
-        pyenv global 3.8.4 3.7.7 3.6.11
-        ```
-        Also ensure that you don't have a virtualenv activated when you run the tests else you might get the following error, or similar:
-        `
-        ERROR: InterpreterNotFound: python3.6
-        `
-        
-        ## Documentation
-        
-        To build the documentation, you'll need to install `mkdocs`.
-        
-        ``` bash
-        $ pip install mkdocs
-        ```
-        
-        To preview the documentation:
-        
-        ``` bash
-        $ mkdocs serve
-        Running at: http://127.0.0.1:8000/
-        ```
-        
-        To build the documentation:
-        
-        ``` bash
-        $ mkdocs build
-        ```
-        
-        
-        [build-status-image]: https://secure.travis-ci.org/lingster/drf-api-tracking.png?branch=master
-        [travis]: http://travis-ci.org/lingster/drf-api-tracking?branch=master
-        [pypi-version]: https://img.shields.io/pypi/v/drf-api-tracking.svg
-        [pypi]: https://pypi.python.org/pypi/drf-api-tracking
-        
-        
-        # travis
-        Install RVM to have a local user version of ruby/gem:
-        `https://rvm.io/rvm/install`
-        Then install travis like this:
-        `gem install travis`
-        add your secret key as per the link below:
-        `https://docs.travis-ci.com/user/encryption-keys/`
-        
-        pyenv
-        ---
-        using pyenv you can install multiple versions of python so that tox can run tests against all installed versions of python
-        ``` bash
-        pyenv global 3.6.8 3.7.7 3.8.2
-        ```
-        ensure that before running tox you don't have a virtualenv created and tox has been installed globally or via pipx
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
@@ -273,7 +22,273 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Description-Content-Type: text/markdown; charset=UTF-8
+License-File: LICENSE
+
+# drf-api-tracking
+
+[![build-status-image]][travis]
+[![pypi-version]][pypi]
+[![Requirements Status](https://requires.io/github/lingster/drf-api-tracking/requirements.svg?branch=master)](https://requires.io/github/lingster/drf-api-tracking/requirements/?branch=master)
+[![Coverage Status](https://coveralls.io/repos/github/lingster/drf-api-tracking/badge.svg?branch=master)](https://coveralls.io/github/lingster/drf-api-tracking?branch=master)
+
+## Overview
+
+drf-api-tracking provides a Django model and DRF view mixin that work together to log Django Rest Framework requests to the database. You'll get these attributes for every request/response cycle to a view that uses the mixin:
+
+
+ Model field name | Description | Model field type
+------------------|-------------|-----------------
+`user` | User if authenticated, None if not | Foreign Key
+`username_persistent` | Static field that persists the username even if the User model object is deleted | CharField
+`requested_at` | Date-time that the request was made | DateTimeField
+`response_ms` | Number of milliseconds spent in view code | PositiveIntegerField
+`path` | Target URI of the request, e.g., `"/api/"` | CharField
+`view` | Target VIEW of the request, e.g., `"views.api.ApiView"` | CharField
+`view_method` | Target METHOD of the VIEW of the request, e.g., `"get"` | CharField
+`remote_addr` | IP address where the request originated (X_FORWARDED_FOR if available, REMOTE_ADDR if not), e.g., `"127.0.0.1"` | GenericIPAddressField
+`host` | Originating host of the request, e.g., `"example.com"` | URLField
+`method` | HTTP method, e.g., `"GET"` | CharField
+`query_params` | Dictionary of request query parameters, as text | TextField
+`data` | Dictionary of POST data (JSON or form), as text | TextField
+`response` | JSON response data | TextField
+`status_code` | HTTP status code, e.g., `200` or `404` | PositiveIntegerField
+
+
+## Requirements
+
+* Django 1.11, 2.0, 2.1, 2.2, 3.0
+* Django REST Framework and Python release supporting the version of Django you are using
+
+Django | Python | DRF
+-------|--------|----
+1.11 | 2.7, 3.5, 3.6 | 3.5, 3.6, 3.7, 3.8, 3.9
+2.0 | 3.5, 3.6, 3.7 | 3.7, 3.8, 3.9
+2.1 | 3.5, 3.6, 3.7, 3.8 | 3.7, 3.8, 3.9
+2.2 | 3.5, 3.6, 3.7, 3.8 | 3.7, 3.8, 3.9
+3.0 | 3.5, 3.6, 3.7, 3.8 | 3.7, 3.8, 3.9
+
+## Installation
+
+Install using `pip`...
+
+``` bash
+$ pip install drf-api-tracking
+```
+
+Register with your Django project by adding `rest_framework_tracking`
+to the `INSTALLED_APPS` list in your project's `settings.py` file.
+Then run the migrations for the `APIRequestLog` model:
+
+``` bash
+$ python manage.py migrate
+```
+
+## Usage
+
+Add the `rest_framework_tracking.mixins.LoggingMixin` to any DRF view
+to create an instance of `APIRequestLog` every time the view is called.
+
+For instance:
+``` python
+# views.py
+from rest_framework import generics
+from rest_framework.response import Response
+from rest_framework_tracking.mixins import LoggingMixin
+
+class LoggingView(LoggingMixin, generics.GenericAPIView):
+    def get(self, request):
+        return Response('with logging')
+```
+
+For performance enhancement, explicitly choose methods to be logged using `logging_methods` attribute:
+
+``` python
+class LoggingView(LoggingMixin, generics.CreateModelMixin, generics.GenericAPIView):
+    logging_methods = ['POST', 'PUT']
+    model = ...
+```
+
+Moreover, you could define your own rules by overriding `should_log` method.
+If `should_log` evaluates to True a log is created.
+
+``` python
+class LoggingView(LoggingMixin, generics.GenericAPIView):
+    def should_log(self, request, response):
+        """Log only errors"""
+        return response.status_code >= 400
+```
+
+At the example above, `logging_methods` attribute will be ignored. If you want to provide some extra rules
+on top of the http method filtering you should rewrite the `should_log` method.
+
+``` python
+class LoggingView(LoggingMixin, generics.GenericAPIView):
+    def should_log(self, request, response):
+        """Log only errors with respect on `logging_methods` attributes"""
+        should_log_method = super(LoggingView, self).should_log(request, response)
+        if not should_log_method:
+            return False
+        return response.status_code >= 400
+```
+
+ A bit simpler.
+``` python
+class LoggingView(LoggingMixin, generics.GenericAPIView):
+    def should_log(self, request, response):
+        """Log only errors with respect on `logging_methods` attributes"""
+        if not request.method in self.logging_methods:
+            return False
+        return response.status_code >= 400
+```
+
+Finally, you can also apply your customizations by overriding `handle_log` method.
+By default, all requests that satisfy `should_log` method are saved on the database.
+``` python
+class LoggingView(LoggingMixin, generics.GenericAPIView):
+    def handle_log(self):
+        # Do some stuff before saving.
+        super(MockCustomLogHandlerView, self).handle_log()
+        # Do some stuff after saving.
+```
+
+
+Though, you could define your own handling. For example save on an in-memory data structure store, remote logging system etc.
+``` python
+class LoggingView(LoggingMixin, generics.GenericAPIView):
+
+    def handle_log(self):
+        cache.set('my_key', self.log, 86400)
+```
+
+Or you could omit save a request to the database. For example,
+``` python
+class LoggingView(LoggingMixin, generics.GenericAPIView):
+    def handle_log(self):
+        """
+        Save only very slow requests. Requests that took more than a second.
+        """
+        if self.log['response_ms'] > 1000:
+            super(MockCustomLogHandlerView, self).handle_log()
+```
+
+If your endpoint accepts large file uploads, drf-api-tracking's default behavior to decode the request body may cause a `RequestDataTooBig` exception. This behavior can be disabled globally by setting `DRF_TRACKING_DECODE_REQUEST_BODY = False` in your `settings.py`file.
+
+You can also customize this behavior for individual views by setting the `decode_request_body` attribute:
+
+``` python
+class LoggingView(LoggingMixin, generics.GenericAPIView):
+    decode_request_body = False
+```
+
+## Security
+
+By default drf-api-tracking is hiding the values of those fields `{'api', 'token', 'key', 'secret', 'password', 'signature'}`.
+The default list hast been taken from Django itself ([https://github.com/django/django/blob/stable/1.11.x/django/contrib/auth/__init__.py#L50](https://github.com/django/django/blob/stable/1.11.x/django/contrib/auth/__init__.py#L50)).
+
+You can complete this list with your own list by putting the fields you want to be hidden in the `sensitive_fields` parameter of your view.
+
+``` python
+class LoggingView(LoggingMixin, generics.CreateModelMixin, generics.GenericAPIView):
+    sensitive_fields = {'my_secret_key', 'my_secret_recipe'}
+```
+
+By default drf-tracking allows API request log entries to be modified from Django admin. This can present a data integrity issue in production environments. In order to change this behavior, you can set `DRF_TRACKING_ADMIN_LOG_READONLY` to `True` in your `settings.py` file.
+
+## Development
+In the folder there is a sample drf project: `drf_api_sample` if changes are made to this packages models, use this project
+to help generate new migrations, which should be checked in.
+
+## Testing
+
+Install testing requirements.
+
+``` bash
+$ pip install -r requirements.txt
+```
+
+Run with runtests.
+
+``` bash
+$ ./runtests.py
+```
+
+You can also use the excellent [tox](http://tox.readthedocs.org/en/latest/) testing tool to run the tests against all supported versions of Python and Django. Install tox globally, and then simply run:
+
+``` bash
+$ tox
+```
+you can also use pyenv to install multiple versions of python and ensure they are found by tox by issuing:
+``` bash
+pyenv install 3.8.4
+pyenv install 3.7.7
+pyenv install 3.6.11
+pyenv local 3.8.4 3.7.7 3.6.11
+pyenv global 3.8.4 3.7.7 3.6.11
+```
+Also ensure that you don't have a virtualenv activated when you run the tests else you might get the following error, or similar:
+`
+ERROR: InterpreterNotFound: python3.6
+`
+
+## Contributing
+
+In order to make changes to the package itself, providing migrations or something else,
+make sure to install the current package with pip, otherwise using the `drf_api_sample` won't work.
+
+``` bash
+pip install -e .
+```
+
+After this, you can edit models and creating migrations with
+
+``` bash
+python drf_api_sample/manage.py makemigrations
+```
+
+## Documentation
+
+To build the documentation, you'll need to install `mkdocs`.
+
+``` bash
+$ pip install mkdocs
+```
+
+To preview the documentation:
+
+``` bash
+$ mkdocs serve
+Running at: http://127.0.0.1:8000/
+```
+
+To build the documentation:
+
+``` bash
+$ mkdocs build
+```
+
+
+[build-status-image]: https://secure.travis-ci.org/lingster/drf-api-tracking.png?branch=master
+[travis]: http://travis-ci.org/lingster/drf-api-tracking?branch=master
+[pypi-version]: https://img.shields.io/pypi/v/drf-api-tracking.svg
+[pypi]: https://pypi.python.org/pypi/drf-api-tracking
+
+
+# travis
+Install RVM to have a local user version of ruby/gem:
+`https://rvm.io/rvm/install`
+Then install travis like this:
+`gem install travis`
+add your secret key as per the link below:
+`https://docs.travis-ci.com/user/encryption-keys/`
+
+pyenv
+---
+using pyenv you can install multiple versions of python so that tox can run tests against all installed versions of python
+``` bash
+pyenv global 3.6.8 3.7.7 3.8.2
+```
+ensure that before running tox you don't have a virtualenv created and tox has been installed globally or via pipx
```

### Comparing `drf-api-tracking-1.8.2/drf_api_tracking.egg-info/SOURCES.txt` & `drf-api-tracking-1.8.3/drf_api_tracking.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+LICENSE
 MANIFEST.in
 README.md
-pyproject.toml
 setup.cfg
 setup.py
 drf_api_tracking.egg-info/PKG-INFO
 drf_api_tracking.egg-info/SOURCES.txt
 drf_api_tracking.egg-info/dependency_links.txt
 drf_api_tracking.egg-info/requires.txt
 drf_api_tracking.egg-info/top_level.txt
@@ -26,9 +26,10 @@
 rest_framework_tracking/migrations/0006_auto_20180315_1442.py
 rest_framework_tracking/migrations/0006_view_and_view_method_nullable.py
 rest_framework_tracking/migrations/0007_merge_20180419_1646.py
 rest_framework_tracking/migrations/0008_auto_20200201_2048.py
 rest_framework_tracking/migrations/0009_view_method_max_length_200.py
 rest_framework_tracking/migrations/0010_auto_20200609_1404.py
 rest_framework_tracking/migrations/0011_auto_20201117_2016.py
+rest_framework_tracking/migrations/0012_auto_20210930_0713.py
 rest_framework_tracking/migrations/__init__.py
 rest_framework_tracking/templates/admin/rest_framework_tracking/apirequestlog/change_list.html
```

### Comparing `drf-api-tracking-1.8.2/rest_framework_tracking/admin.py` & `drf-api-tracking-1.8.3/rest_framework_tracking/admin.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.2/rest_framework_tracking/app_settings.py` & `drf-api-tracking-1.8.3/rest_framework_tracking/app_settings.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.2/rest_framework_tracking/base_mixins.py` & `drf-api-tracking-1.8.3/rest_framework_tracking/base_mixins.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.2/rest_framework_tracking/base_models.py` & `drf-api-tracking-1.8.3/rest_framework_tracking/base_models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime
 from django.db import models
 from django.conf import settings
 
 from .managers import PrefetchUserManager
 
 
 class BaseAPIRequestLog(models.Model):
@@ -14,15 +15,15 @@
         blank=True,
     )
     username_persistent = models.CharField(
         max_length=getattr(settings, "DRF_TRACKING_USERNAME_LENGTH", 200),
         null=True,
         blank=True,
     )
-    requested_at = models.DateTimeField(db_index=True)
+    requested_at = models.DateTimeField(default=datetime.now, db_index=True)
     response_ms = models.PositiveIntegerField(default=0)
     path = models.CharField(
         max_length=getattr(settings, "DRF_TRACKING_PATH_LENGTH", 200),
         db_index=True,
         help_text="url path",
     )
     view = models.CharField(
@@ -34,15 +35,15 @@
     )
     view_method = models.CharField(
         max_length=getattr(settings, "DRF_TRACKING_VIEW_METHOD_LENGTH", 200),
         null=True,
         blank=True,
         db_index=True,
     )
-    remote_addr = models.GenericIPAddressField()
+    remote_addr = models.GenericIPAddressField(null=True, blank=True)
     host = models.URLField()
     method = models.CharField(max_length=10)
     user_agent = models.CharField(max_length=255, blank=True)
     query_params = models.TextField(null=True, blank=True)
     data = models.TextField(null=True, blank=True)
     response = models.TextField(null=True, blank=True)
     errors = models.TextField(null=True, blank=True)
```

### Comparing `drf-api-tracking-1.8.2/rest_framework_tracking/management/commands/clearapilogs.py` & `drf-api-tracking-1.8.3/rest_framework_tracking/management/commands/clearapilogs.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0001_initial.py` & `drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0002_auto_20170118_1713.py` & `drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0002_auto_20170118_1713.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0005_auto_20171219_1537.py` & `drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0005_auto_20171219_1537.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0006_auto_20180315_1442.py` & `drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0006_auto_20180315_1442.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0006_view_and_view_method_nullable.py` & `drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0006_view_and_view_method_nullable.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0008_auto_20200201_2048.py` & `drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0008_auto_20200201_2048.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0009_view_method_max_length_200.py` & `drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0009_view_method_max_length_200.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.2/rest_framework_tracking/migrations/0010_auto_20200609_1404.py` & `drf-api-tracking-1.8.3/rest_framework_tracking/migrations/0010_auto_20200609_1404.py`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.2/rest_framework_tracking/templates/admin/rest_framework_tracking/apirequestlog/change_list.html` & `drf-api-tracking-1.8.3/rest_framework_tracking/templates/admin/rest_framework_tracking/apirequestlog/change_list.html`

 * *Files identical despite different names*

### Comparing `drf-api-tracking-1.8.2/setup.py` & `drf-api-tracking-1.8.3/setup.py`

 * *Files identical despite different names*

