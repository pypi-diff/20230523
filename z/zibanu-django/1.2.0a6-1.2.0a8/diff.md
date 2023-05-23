# Comparing `tmp/zibanu-django-1.2.0a6.tar.gz` & `tmp/zibanu-django-1.2.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zibanu-django-1.2.0a6.tar", last modified: Sat May 13 14:29:57 2023, max compression
+gzip compressed data, was "zibanu-django-1.2.0a8.tar", last modified: Tue May 23 16:48:56 2023, max compression
```

## Comparing `zibanu-django-1.2.0a6.tar` & `zibanu-django-1.2.0a8.tar`

### file list

```diff
@@ -1,147 +1,162 @@
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.589411 zibanu-django-1.2.0a6/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-1.2.0a6/LICENSE
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      207 2023-03-31 15:51:33.000000 zibanu-django-1.2.0a6/MANIFEST.in
--rw-r--r--   0 macercha  (1000) macercha  (1000)    41365 2023-05-13 14:29:57.588411 zibanu-django-1.2.0a6/PKG-INFO
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      158 2023-01-18 12:15:22.000000 zibanu-django-1.2.0a6/README.md
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      849 2023-05-13 14:27:36.000000 zibanu-django-1.2.0a6/pyproject.toml
--rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-05-13 14:29:57.589411 zibanu-django-1.2.0a6/setup.cfg
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.557412 zibanu-django-1.2.0a6/zibanu/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      623 2022-12-10 15:21:05.000000 zibanu-django-1.2.0a6/zibanu/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.558412 zibanu-django-1.2.0a6/zibanu/django/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-11 23:08:20.000000 zibanu-django-1.2.0a6/zibanu/django/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      895 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a6/zibanu/django/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.558412 zibanu-django-1.2.0a6/zibanu/django/auth/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:20:31.000000 zibanu-django-1.2.0a6/zibanu/django/auth/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.559412 zibanu-django-1.2.0a6/zibanu/django/auth/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:25:30.000000 zibanu-django-1.2.0a6/zibanu/django/auth/api/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.559412 zibanu-django-1.2.0a6/zibanu/django/auth/api/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      648 2023-04-27 14:40:31.000000 zibanu-django-1.2.0a6/zibanu/django/auth/api/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      749 2023-04-27 12:00:18.000000 zibanu-django-1.2.0a6/zibanu/django/auth/api/serializers/profile.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3051 2023-04-27 12:17:39.000000 zibanu-django-1.2.0a6/zibanu/django/auth/api/serializers/token.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3944 2023-05-13 14:19:35.000000 zibanu-django-1.2.0a6/zibanu/django/auth/api/serializers/user.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.560412 zibanu-django-1.2.0a6/zibanu/django/auth/api/services/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      376 2023-04-27 14:42:35.000000 zibanu-django-1.2.0a6/zibanu/django/auth/api/services/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3165 2023-05-13 14:20:35.000000 zibanu-django-1.2.0a6/zibanu/django/auth/api/services/user.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      915 2023-04-10 18:51:33.000000 zibanu-django-1.2.0a6/zibanu/django/auth/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.560412 zibanu-django-1.2.0a6/zibanu/django/auth/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:32:01.000000 zibanu-django-1.2.0a6/zibanu/django/auth/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.560412 zibanu-django-1.2.0a6/zibanu/django/auth/lib/choices/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:48:01.000000 zibanu-django-1.2.0a6/zibanu/django/auth/lib/choices/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.560412 zibanu-django-1.2.0a6/zibanu/django/auth/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    24474 2023-04-11 22:39:55.000000 zibanu-django-1.2.0a6/zibanu/django/auth/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:31:28.000000 zibanu-django-1.2.0a6/zibanu/django/auth/migrations/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1605 2023-04-11 22:39:53.000000 zibanu-django-1.2.0a6/zibanu/django/auth/models.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      856 2023-04-28 00:32:16.000000 zibanu-django-1.2.0a6/zibanu/django/auth/urls.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.561412 zibanu-django-1.2.0a6/zibanu/django/db/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 18:13:01.000000 zibanu-django-1.2.0a6/zibanu/django/db/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.561412 zibanu-django-1.2.0a6/zibanu/django/db/backends/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0a6/zibanu/django/db/backends/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.561412 zibanu-django-1.2.0a6/zibanu/django/db/backends/oracle/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0a6/zibanu/django/db/backends/oracle/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1158 2023-02-07 01:58:51.000000 zibanu-django-1.2.0a6/zibanu/django/db/backends/oracle/base.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.562412 zibanu-django-1.2.0a6/zibanu/django/db/models/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      766 2023-01-17 11:51:34.000000 zibanu-django-1.2.0a6/zibanu/django/db/models/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      931 2023-03-01 18:58:00.000000 zibanu-django-1.2.0a6/zibanu/django/db/models/dated_model.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1458 2023-03-03 23:10:34.000000 zibanu-django-1.2.0a6/zibanu/django/db/models/manager.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      738 2022-12-20 14:58:49.000000 zibanu-django-1.2.0a6/zibanu/django/db/models/model.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.553412 zibanu-django-1.2.0a6/zibanu/django/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.553412 zibanu-django-1.2.0a6/zibanu/django/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.562412 zibanu-django-1.2.0a6/zibanu/django/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2274 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a6/zibanu/django/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3598 2023-04-27 15:33:39.000000 zibanu-django-1.2.0a6/zibanu/django/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.562412 zibanu-django-1.2.0a6/zibanu/django/logging/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-03-16 14:08:34.000000 zibanu-django-1.2.0a6/zibanu/django/logging/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      919 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a6/zibanu/django/logging/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.563412 zibanu-django-1.2.0a6/zibanu/django/logging/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 20:39:57.000000 zibanu-django-1.2.0a6/zibanu/django/logging/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.564412 zibanu-django-1.2.0a6/zibanu/django/logging/lib/events/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a6/zibanu/django/logging/lib/events/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1018 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a6/zibanu/django/logging/lib/events/on_change_password.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1243 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a6/zibanu/django/logging/lib/events/on_login.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      975 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a6/zibanu/django/logging/lib/events/on_send_mail.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.564412 zibanu-django-1.2.0a6/zibanu/django/logging/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:05:35.000000 zibanu-django-1.2.0a6/zibanu/django/logging/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      453 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a6/zibanu/django/logging/lib/signals.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.554412 zibanu-django-1.2.0a6/zibanu/django/logging/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.554412 zibanu-django-1.2.0a6/zibanu/django/logging/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.564412 zibanu-django-1.2.0a6/zibanu/django/logging/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a6/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1185 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a6/zibanu/django/logging/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.565412 zibanu-django-1.2.0a6/zibanu/django/logging/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1501 2023-03-15 21:32:53.000000 zibanu-django-1.2.0a6/zibanu/django/logging/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1143 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a6/zibanu/django/logging/migrations/0002_maillog.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:33:26.000000 zibanu-django-1.2.0a6/zibanu/django/logging/migrations/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1946 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a6/zibanu/django/logging/models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.565412 zibanu-django-1.2.0a6/zibanu/django/repository/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-03 02:16:47.000000 zibanu-django-1.2.0a6/zibanu/django/repository/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.565412 zibanu-django-1.2.0a6/zibanu/django/repository/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-04 20:42:37.000000 zibanu-django-1.2.0a6/zibanu/django/repository/api/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      958 2023-02-03 02:43:10.000000 zibanu-django-1.2.0a6/zibanu/django/repository/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.565412 zibanu-django-1.2.0a6/zibanu/django/repository/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-04 20:45:36.000000 zibanu-django-1.2.0a6/zibanu/django/repository/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.566412 zibanu-django-1.2.0a6/zibanu/django/repository/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      566 2023-02-04 20:47:18.000000 zibanu-django-1.2.0a6/zibanu/django/repository/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      740 2023-02-04 21:36:16.000000 zibanu-django-1.2.0a6/zibanu/django/repository/lib/managers/document.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.566412 zibanu-django-1.2.0a6/zibanu/django/repository/lib/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      593 2023-02-04 20:45:36.000000 zibanu-django-1.2.0a6/zibanu/django/repository/lib/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     6973 2023-04-11 22:50:39.000000 zibanu-django-1.2.0a6/zibanu/django/repository/lib/utils/document_generator.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.555412 zibanu-django-1.2.0a6/zibanu/django/repository/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.555412 zibanu-django-1.2.0a6/zibanu/django/repository/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.566412 zibanu-django-1.2.0a6/zibanu/django/repository/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1605 2023-02-09 14:40:51.000000 zibanu-django-1.2.0a6/zibanu/django/repository/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2664 2023-04-11 22:52:31.000000 zibanu-django-1.2.0a6/zibanu/django/repository/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.567412 zibanu-django-1.2.0a6/zibanu/django/repository/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1372 2023-02-03 02:43:34.000000 zibanu-django-1.2.0a6/zibanu/django/repository/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      427 2023-02-08 14:23:11.000000 zibanu-django-1.2.0a6/zibanu/django/repository/migrations/0002_document_description.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-02-03 02:23:41.000000 zibanu-django-1.2.0a6/zibanu/django/repository/migrations/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1575 2023-02-08 14:23:06.000000 zibanu-django-1.2.0a6/zibanu/django/repository/models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.567412 zibanu-django-1.2.0a6/zibanu/django/rest_framework/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 12:39:27.000000 zibanu-django-1.2.0a6/zibanu/django/rest_framework/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1650 2023-04-28 00:41:44.000000 zibanu-django-1.2.0a6/zibanu/django/rest_framework/decorators.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.567412 zibanu-django-1.2.0a6/zibanu/django/rest_framework/exceptions/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      973 2022-12-20 02:49:47.000000 zibanu-django-1.2.0a6/zibanu/django/rest_framework/exceptions/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2039 2023-04-27 15:30:28.000000 zibanu-django-1.2.0a6/zibanu/django/rest_framework/exceptions/api_exception.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.568412 zibanu-django-1.2.0a6/zibanu/django/rest_framework/fields/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a6/zibanu/django/rest_framework/fields/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1142 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a6/zibanu/django/rest_framework/fields/current_user_default.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.568412 zibanu-django-1.2.0a6/zibanu/django/rest_framework/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1560 2022-12-20 10:51:58.000000 zibanu-django-1.2.0a6/zibanu/django/rest_framework/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-02-27 20:11:57.000000 zibanu-django-1.2.0a6/zibanu/django/rest_framework/serializers/fields.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      867 2022-12-14 09:18:30.000000 zibanu-django-1.2.0a6/zibanu/django/rest_framework/serializers/model_serializer.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.569412 zibanu-django-1.2.0a6/zibanu/django/rest_framework/viewsets/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-02-13 14:05:54.000000 zibanu-django-1.2.0a6/zibanu/django/rest_framework/viewsets/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    10487 2023-04-28 00:47:56.000000 zibanu-django-1.2.0a6/zibanu/django/rest_framework/viewsets/model_viewset.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1332 2023-02-13 14:05:54.000000 zibanu-django-1.2.0a6/zibanu/django/rest_framework/viewsets/viewset.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.569412 zibanu-django-1.2.0a6/zibanu/django/template/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-01-28 17:50:45.000000 zibanu-django-1.2.0a6/zibanu/django/template/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      663 2023-01-28 20:32:11.000000 zibanu-django-1.2.0a6/zibanu/django/template/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.570412 zibanu-django-1.2.0a6/zibanu/django/template/context_processors/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      624 2023-01-29 02:00:01.000000 zibanu-django-1.2.0a6/zibanu/django/template/context_processors/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-01-29 02:00:01.000000 zibanu-django-1.2.0a6/zibanu/django/template/context_processors/full_static_uri.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2023-01-28 20:37:34.000000 zibanu-django-1.2.0a6/zibanu/django/template/context_processors/site.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.556412 zibanu-django-1.2.0a6/zibanu/django/template/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.556412 zibanu-django-1.2.0a6/zibanu/django/template/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.570412 zibanu-django-1.2.0a6/zibanu/django/template/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      519 2023-02-09 14:42:38.000000 zibanu-django-1.2.0a6/zibanu/django/template/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1022 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a6/zibanu/django/template/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.571412 zibanu-django-1.2.0a6/zibanu/django/template/templatetags/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-07 23:57:31.000000 zibanu-django-1.2.0a6/zibanu/django/template/templatetags/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1539 2023-01-29 02:38:53.000000 zibanu-django-1.2.0a6/zibanu/django/template/templatetags/static_uri.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      666 2023-02-08 00:00:29.000000 zibanu-django-1.2.0a6/zibanu/django/template/templatetags/string_concat.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2009 2023-02-16 14:53:50.000000 zibanu-django-1.2.0a6/zibanu/django/template/templatetags/subtotal_dict.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1216 2023-02-08 15:25:53.000000 zibanu-django-1.2.0a6/zibanu/django/template/templatetags/sum_dict.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.572412 zibanu-django-1.2.0a6/zibanu/django/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      863 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a6/zibanu/django/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3332 2023-04-28 21:35:15.000000 zibanu-django-1.2.0a6/zibanu/django/utils/code_generator.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1895 2023-02-26 20:02:32.000000 zibanu-django-1.2.0a6/zibanu/django/utils/date_time.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1163 2023-03-03 13:27:43.000000 zibanu-django-1.2.0a6/zibanu/django/utils/error_messages.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     4325 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a6/zibanu/django/utils/mail.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      562 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a6/zibanu/django/utils/request_utils.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1251 2022-12-14 09:24:38.000000 zibanu-django-1.2.0a6/zibanu/django/utils/user.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      699 2023-03-03 13:27:43.000000 zibanu-django-1.2.0a6/zibanu/django/utils/validate_cache_code.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-13 14:29:57.588411 zibanu-django-1.2.0a6/zibanu_django.egg-info/
--rw-r--r--   0 macercha  (1000) macercha  (1000)    41365 2023-05-13 14:29:57.000000 zibanu-django-1.2.0a6/zibanu_django.egg-info/PKG-INFO
--rw-r--r--   0 macercha  (1000) macercha  (1000)     4085 2023-05-13 14:29:57.000000 zibanu-django-1.2.0a6/zibanu_django.egg-info/SOURCES.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-05-13 14:29:57.000000 zibanu-django-1.2.0a6/zibanu_django.egg-info/dependency_links.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       32 2023-05-13 14:29:57.000000 zibanu-django-1.2.0a6/zibanu_django.egg-info/requires.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2023-05-13 14:29:57.000000 zibanu-django-1.2.0a6/zibanu_django.egg-info/top_level.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.031683 zibanu-django-1.2.0a8/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-1.2.0a8/LICENSE
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      304 2023-05-13 16:38:59.000000 zibanu-django-1.2.0a8/MANIFEST.in
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    41365 2023-05-23 16:48:56.030683 zibanu-django-1.2.0a8/PKG-INFO
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      158 2023-01-18 12:15:22.000000 zibanu-django-1.2.0a8/README.md
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      886 2023-05-23 16:44:19.000000 zibanu-django-1.2.0a8/pyproject.toml
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-05-23 16:48:56.031683 zibanu-django-1.2.0a8/setup.cfg
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.010684 zibanu-django-1.2.0a8/zibanu/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      623 2022-12-10 15:21:05.000000 zibanu-django-1.2.0a8/zibanu/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.011684 zibanu-django-1.2.0a8/zibanu/django/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-11 23:08:20.000000 zibanu-django-1.2.0a8/zibanu/django/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      895 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a8/zibanu/django/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.012683 zibanu-django-1.2.0a8/zibanu/django/auth/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:20:31.000000 zibanu-django-1.2.0a8/zibanu/django/auth/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.012683 zibanu-django-1.2.0a8/zibanu/django/auth/api/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:25:30.000000 zibanu-django-1.2.0a8/zibanu/django/auth/api/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.013684 zibanu-django-1.2.0a8/zibanu/django/auth/api/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      648 2023-04-27 14:40:31.000000 zibanu-django-1.2.0a8/zibanu/django/auth/api/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      749 2023-04-27 12:00:18.000000 zibanu-django-1.2.0a8/zibanu/django/auth/api/serializers/profile.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3051 2023-04-27 12:17:39.000000 zibanu-django-1.2.0a8/zibanu/django/auth/api/serializers/token.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3944 2023-05-13 14:19:35.000000 zibanu-django-1.2.0a8/zibanu/django/auth/api/serializers/user.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.013684 zibanu-django-1.2.0a8/zibanu/django/auth/api/services/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      376 2023-04-27 14:42:35.000000 zibanu-django-1.2.0a8/zibanu/django/auth/api/services/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     8259 2023-05-23 16:17:03.000000 zibanu-django-1.2.0a8/zibanu/django/auth/api/services/user.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1245 2023-05-17 01:05:01.000000 zibanu-django-1.2.0a8/zibanu/django/auth/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.014684 zibanu-django-1.2.0a8/zibanu/django/auth/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:32:01.000000 zibanu-django-1.2.0a8/zibanu/django/auth/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.014684 zibanu-django-1.2.0a8/zibanu/django/auth/lib/choices/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:48:01.000000 zibanu-django-1.2.0a8/zibanu/django/auth/lib/choices/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1396 2023-05-17 00:58:35.000000 zibanu-django-1.2.0a8/zibanu/django/auth/lib/signal_events.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      412 2023-05-13 17:53:49.000000 zibanu-django-1.2.0a8/zibanu/django/auth/lib/signals.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1086 2023-05-13 15:23:33.000000 zibanu-django-1.2.0a8/zibanu/django/auth/lib/utils.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.005684 zibanu-django-1.2.0a8/zibanu/django/auth/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.005684 zibanu-django-1.2.0a8/zibanu/django/auth/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.014684 zibanu-django-1.2.0a8/zibanu/django/auth/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      818 2023-04-27 15:20:42.000000 zibanu-django-1.2.0a8/zibanu/django/auth/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1166 2023-04-27 15:20:12.000000 zibanu-django-1.2.0a8/zibanu/django/auth/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.015684 zibanu-django-1.2.0a8/zibanu/django/auth/migrations/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    24474 2023-04-11 22:39:55.000000 zibanu-django-1.2.0a8/zibanu/django/auth/migrations/0001_initial.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:31:28.000000 zibanu-django-1.2.0a8/zibanu/django/auth/migrations/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1605 2023-04-11 22:39:53.000000 zibanu-django-1.2.0a8/zibanu/django/auth/models.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.016683 zibanu-django-1.2.0a8/zibanu/django/auth/templates/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      487 2023-05-23 16:11:28.000000 zibanu-django-1.2.0a8/zibanu/django/auth/templates/change_password.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      324 2023-05-22 17:32:26.000000 zibanu-django-1.2.0a8/zibanu/django/auth/templates/change_password.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-05-13 16:44:16.000000 zibanu-django-1.2.0a8/zibanu/django/auth/templates/request-code.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-05-13 16:41:48.000000 zibanu-django-1.2.0a8/zibanu/django/auth/templates/request-code.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      559 2023-05-22 17:30:07.000000 zibanu-django-1.2.0a8/zibanu/django/auth/templates/request_password.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      346 2023-05-13 16:55:01.000000 zibanu-django-1.2.0a8/zibanu/django/auth/templates/request_password.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1067 2023-05-23 00:53:34.000000 zibanu-django-1.2.0a8/zibanu/django/auth/urls.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.016683 zibanu-django-1.2.0a8/zibanu/django/db/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 18:13:01.000000 zibanu-django-1.2.0a8/zibanu/django/db/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.016683 zibanu-django-1.2.0a8/zibanu/django/db/backends/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0a8/zibanu/django/db/backends/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.016683 zibanu-django-1.2.0a8/zibanu/django/db/backends/oracle/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-07 01:34:17.000000 zibanu-django-1.2.0a8/zibanu/django/db/backends/oracle/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1158 2023-02-07 01:58:51.000000 zibanu-django-1.2.0a8/zibanu/django/db/backends/oracle/base.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.017683 zibanu-django-1.2.0a8/zibanu/django/db/models/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      766 2023-01-17 11:51:34.000000 zibanu-django-1.2.0a8/zibanu/django/db/models/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      931 2023-03-01 18:58:00.000000 zibanu-django-1.2.0a8/zibanu/django/db/models/dated_model.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1458 2023-03-03 23:10:34.000000 zibanu-django-1.2.0a8/zibanu/django/db/models/manager.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      738 2022-12-20 14:58:49.000000 zibanu-django-1.2.0a8/zibanu/django/db/models/model.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.006684 zibanu-django-1.2.0a8/zibanu/django/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.006684 zibanu-django-1.2.0a8/zibanu/django/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.017683 zibanu-django-1.2.0a8/zibanu/django/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2274 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a8/zibanu/django/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3598 2023-04-27 15:33:39.000000 zibanu-django-1.2.0a8/zibanu/django/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.018684 zibanu-django-1.2.0a8/zibanu/django/logging/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-03-16 14:08:34.000000 zibanu-django-1.2.0a8/zibanu/django/logging/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      919 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a8/zibanu/django/logging/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.018684 zibanu-django-1.2.0a8/zibanu/django/logging/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 20:39:57.000000 zibanu-django-1.2.0a8/zibanu/django/logging/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.019683 zibanu-django-1.2.0a8/zibanu/django/logging/lib/events/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a8/zibanu/django/logging/lib/events/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1016 2023-05-13 19:57:25.000000 zibanu-django-1.2.0a8/zibanu/django/logging/lib/events/on_change_password.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1243 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a8/zibanu/django/logging/lib/events/on_login.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      975 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a8/zibanu/django/logging/lib/events/on_send_mail.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.019683 zibanu-django-1.2.0a8/zibanu/django/logging/lib/managers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:05:35.000000 zibanu-django-1.2.0a8/zibanu/django/logging/lib/managers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      452 2023-05-13 17:50:17.000000 zibanu-django-1.2.0a8/zibanu/django/logging/lib/signals.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.007684 zibanu-django-1.2.0a8/zibanu/django/logging/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.007684 zibanu-django-1.2.0a8/zibanu/django/logging/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.020683 zibanu-django-1.2.0a8/zibanu/django/logging/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      702 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a8/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1185 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a8/zibanu/django/logging/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.020683 zibanu-django-1.2.0a8/zibanu/django/logging/migrations/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1501 2023-03-15 21:32:53.000000 zibanu-django-1.2.0a8/zibanu/django/logging/migrations/0001_initial.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1143 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a8/zibanu/django/logging/migrations/0002_maillog.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-15 21:33:26.000000 zibanu-django-1.2.0a8/zibanu/django/logging/migrations/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1946 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a8/zibanu/django/logging/models.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.021683 zibanu-django-1.2.0a8/zibanu/django/repository/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-03 02:16:47.000000 zibanu-django-1.2.0a8/zibanu/django/repository/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.021683 zibanu-django-1.2.0a8/zibanu/django/repository/api/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-04 20:42:37.000000 zibanu-django-1.2.0a8/zibanu/django/repository/api/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      958 2023-02-03 02:43:10.000000 zibanu-django-1.2.0a8/zibanu/django/repository/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.021683 zibanu-django-1.2.0a8/zibanu/django/repository/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-04 20:45:36.000000 zibanu-django-1.2.0a8/zibanu/django/repository/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.022683 zibanu-django-1.2.0a8/zibanu/django/repository/lib/managers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      566 2023-02-04 20:47:18.000000 zibanu-django-1.2.0a8/zibanu/django/repository/lib/managers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      740 2023-02-04 21:36:16.000000 zibanu-django-1.2.0a8/zibanu/django/repository/lib/managers/document.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.022683 zibanu-django-1.2.0a8/zibanu/django/repository/lib/utils/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      593 2023-02-04 20:45:36.000000 zibanu-django-1.2.0a8/zibanu/django/repository/lib/utils/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     6973 2023-04-11 22:50:39.000000 zibanu-django-1.2.0a8/zibanu/django/repository/lib/utils/document_generator.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.008684 zibanu-django-1.2.0a8/zibanu/django/repository/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.008684 zibanu-django-1.2.0a8/zibanu/django/repository/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.023683 zibanu-django-1.2.0a8/zibanu/django/repository/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1605 2023-02-09 14:40:51.000000 zibanu-django-1.2.0a8/zibanu/django/repository/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2664 2023-04-11 22:52:31.000000 zibanu-django-1.2.0a8/zibanu/django/repository/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.023683 zibanu-django-1.2.0a8/zibanu/django/repository/migrations/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1372 2023-02-03 02:43:34.000000 zibanu-django-1.2.0a8/zibanu/django/repository/migrations/0001_initial.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      427 2023-02-08 14:23:11.000000 zibanu-django-1.2.0a8/zibanu/django/repository/migrations/0002_document_description.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-02-03 02:23:41.000000 zibanu-django-1.2.0a8/zibanu/django/repository/migrations/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1575 2023-02-08 14:23:06.000000 zibanu-django-1.2.0a8/zibanu/django/repository/models.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.023683 zibanu-django-1.2.0a8/zibanu/django/rest_framework/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-13 12:39:27.000000 zibanu-django-1.2.0a8/zibanu/django/rest_framework/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1650 2023-04-28 00:41:44.000000 zibanu-django-1.2.0a8/zibanu/django/rest_framework/decorators.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.024683 zibanu-django-1.2.0a8/zibanu/django/rest_framework/exceptions/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      973 2022-12-20 02:49:47.000000 zibanu-django-1.2.0a8/zibanu/django/rest_framework/exceptions/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2039 2023-04-27 15:30:28.000000 zibanu-django-1.2.0a8/zibanu/django/rest_framework/exceptions/api_exception.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.024683 zibanu-django-1.2.0a8/zibanu/django/rest_framework/fields/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a8/zibanu/django/rest_framework/fields/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1142 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a8/zibanu/django/rest_framework/fields/current_user_default.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.025683 zibanu-django-1.2.0a8/zibanu/django/rest_framework/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1560 2022-12-20 10:51:58.000000 zibanu-django-1.2.0a8/zibanu/django/rest_framework/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      651 2023-02-27 20:11:57.000000 zibanu-django-1.2.0a8/zibanu/django/rest_framework/serializers/fields.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      867 2022-12-14 09:18:30.000000 zibanu-django-1.2.0a8/zibanu/django/rest_framework/serializers/model_serializer.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.025683 zibanu-django-1.2.0a8/zibanu/django/rest_framework/viewsets/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-02-13 14:05:54.000000 zibanu-django-1.2.0a8/zibanu/django/rest_framework/viewsets/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    10487 2023-04-28 00:47:56.000000 zibanu-django-1.2.0a8/zibanu/django/rest_framework/viewsets/model_viewset.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1332 2023-02-13 14:05:54.000000 zibanu-django-1.2.0a8/zibanu/django/rest_framework/viewsets/viewset.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.026683 zibanu-django-1.2.0a8/zibanu/django/template/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-01-28 17:50:45.000000 zibanu-django-1.2.0a8/zibanu/django/template/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      663 2023-01-28 20:32:11.000000 zibanu-django-1.2.0a8/zibanu/django/template/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.026683 zibanu-django-1.2.0a8/zibanu/django/template/context_processors/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      624 2023-01-29 02:00:01.000000 zibanu-django-1.2.0a8/zibanu/django/template/context_processors/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      784 2023-01-29 02:00:01.000000 zibanu-django-1.2.0a8/zibanu/django/template/context_processors/full_static_uri.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2023-01-28 20:37:34.000000 zibanu-django-1.2.0a8/zibanu/django/template/context_processors/site.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.009684 zibanu-django-1.2.0a8/zibanu/django/template/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.009684 zibanu-django-1.2.0a8/zibanu/django/template/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.026683 zibanu-django-1.2.0a8/zibanu/django/template/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      519 2023-02-09 14:42:38.000000 zibanu-django-1.2.0a8/zibanu/django/template/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1022 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a8/zibanu/django/template/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.027683 zibanu-django-1.2.0a8/zibanu/django/template/templatetags/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-07 23:57:31.000000 zibanu-django-1.2.0a8/zibanu/django/template/templatetags/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1539 2023-01-29 02:38:53.000000 zibanu-django-1.2.0a8/zibanu/django/template/templatetags/static_uri.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      666 2023-02-08 00:00:29.000000 zibanu-django-1.2.0a8/zibanu/django/template/templatetags/string_concat.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2009 2023-02-16 14:53:50.000000 zibanu-django-1.2.0a8/zibanu/django/template/templatetags/subtotal_dict.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1216 2023-02-08 15:25:53.000000 zibanu-django-1.2.0a8/zibanu/django/template/templatetags/sum_dict.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.029683 zibanu-django-1.2.0a8/zibanu/django/utils/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      863 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a8/zibanu/django/utils/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3332 2023-04-28 21:35:15.000000 zibanu-django-1.2.0a8/zibanu/django/utils/code_generator.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1895 2023-02-26 20:02:32.000000 zibanu-django-1.2.0a8/zibanu/django/utils/date_time.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1163 2023-03-03 13:27:43.000000 zibanu-django-1.2.0a8/zibanu/django/utils/error_messages.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     5768 2023-05-23 00:00:08.000000 zibanu-django-1.2.0a8/zibanu/django/utils/mail.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      562 2023-03-31 15:46:10.000000 zibanu-django-1.2.0a8/zibanu/django/utils/request_utils.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1080 2023-05-13 15:24:32.000000 zibanu-django-1.2.0a8/zibanu/django/utils/user.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      699 2023-03-03 13:27:43.000000 zibanu-django-1.2.0a8/zibanu/django/utils/validate_cache_code.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-23 16:48:56.030683 zibanu-django-1.2.0a8/zibanu_django.egg-info/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    41365 2023-05-23 16:48:55.000000 zibanu-django-1.2.0a8/zibanu_django.egg-info/PKG-INFO
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     4586 2023-05-23 16:48:56.000000 zibanu-django-1.2.0a8/zibanu_django.egg-info/SOURCES.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-05-23 16:48:55.000000 zibanu-django-1.2.0a8/zibanu_django.egg-info/dependency_links.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       62 2023-05-23 16:48:55.000000 zibanu-django-1.2.0a8/zibanu_django.egg-info/requires.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2023-05-23 16:48:55.000000 zibanu-django-1.2.0a8/zibanu_django.egg-info/top_level.txt
```

### Comparing `zibanu-django-1.2.0a6/LICENSE` & `zibanu-django-1.2.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/PKG-INFO` & `zibanu-django-1.2.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibanu-django
-Version: 1.2.0a6
+Version: 1.2.0a8
 Summary: Zibanu library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `zibanu-django-1.2.0a6/pyproject.toml` & `zibanu-django-1.2.0a8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "zibanu-django"
-version = "1.2.0-alpha.6"
+version = "1.2.0-alpha.8"
 authors = [
     {name="Mario Cerón", email="mario.ceron@cqinversiones.co"}
 ]
 description = "Zibanu library for django projects"
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
@@ -23,14 +23,15 @@
     "Framework :: Django :: 4.1",
     "Environment :: Web Environment",
     "Operating System :: OS Independent",
     "Topic :: Internet :: WWW/HTTP"
 ]
 dependencies = [
     "Django>=4.1",
-    "djangorestframework"
+    "djangorestframework",
+    "djangorestframework-simplejwt"
 ]
 keywords = [
     "django",
     "zibanu",
     "library"
 ]
```

### Comparing `zibanu-django-1.2.0a6/zibanu/__init__.py` & `zibanu-django-1.2.0a8/zibanu/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/apps.py` & `zibanu-django-1.2.0a8/zibanu/django/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/auth/api/serializers/__init__.py` & `zibanu-django-1.2.0a8/zibanu/django/auth/api/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/auth/api/serializers/profile.py` & `zibanu-django-1.2.0a8/zibanu/django/auth/api/serializers/profile.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/auth/api/serializers/token.py` & `zibanu-django-1.2.0a8/zibanu/django/auth/api/serializers/token.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/auth/api/serializers/user.py` & `zibanu-django-1.2.0a8/zibanu/django/auth/api/serializers/user.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/auth/migrations/0001_initial.py` & `zibanu-django-1.2.0a8/zibanu/django/auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/auth/models.py` & `zibanu-django-1.2.0a8/zibanu/django/auth/models.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/auth/urls.py` & `zibanu-django-1.2.0a8/zibanu/django/auth/urls.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,10 +12,12 @@
 from rest_framework_simplejwt.views import TokenObtainSlidingView
 from rest_framework_simplejwt.views import TokenRefreshSlidingView
 from zibanu.django.auth.api.services import UserService
 
 urlpatterns = [
     path("login/", TokenObtainSlidingView.as_view(), name="token_obtain"),
     path("refresh/", TokenRefreshSlidingView.as_view(), name="token_refresh"),
+    path("change-password/", UserService.as_view({"post": "change_password"}), name="change_password"),
+    path("request-password/", UserService.as_view({"post": "request_password"}), name="request_password"),
     path("user/list/", UserService.as_view({"post": "list"}), name="list_users"),
     path("user/add/", UserService.as_view({"post": "create"}), name="add_user")
 ]
```

### Comparing `zibanu-django-1.2.0a6/zibanu/django/db/backends/oracle/base.py` & `zibanu-django-1.2.0a8/zibanu/django/db/backends/oracle/base.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/db/models/__init__.py` & `zibanu-django-1.2.0a8/zibanu/django/db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/db/models/dated_model.py` & `zibanu-django-1.2.0a8/zibanu/django/db/models/dated_model.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/db/models/manager.py` & `zibanu-django-1.2.0a8/zibanu/django/db/models/manager.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/db/models/model.py` & `zibanu-django-1.2.0a8/zibanu/django/db/models/model.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.2.0a8/zibanu/django/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.2.0a8/zibanu/django/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/logging/apps.py` & `zibanu-django-1.2.0a8/zibanu/django/logging/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/logging/lib/events/__init__.py` & `zibanu-django-1.2.0a8/zibanu/django/logging/lib/events/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/logging/lib/events/on_change_password.py` & `zibanu-django-1.2.0a8/zibanu/django/logging/lib/events/on_change_password.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 # Project:      CFHL Transactional Backend
 # Module Name:  on_change_password
 # Description:
 # ****************************************************************
 from django.dispatch import receiver
 from typing import Any
 from zibanu.django.logging.lib.signals import change_password
-from zibanu.django.logging.lib.signals import retrieve_password
+from zibanu.django.logging.lib.signals import request_password
 from zibanu.django.logging.models import Log
 from zibanu.django.utils import get_ip_address
 
 
 @receiver(change_password)
-@receiver(retrieve_password)
+@receiver(request_password)
 def on_change_password(sender: Any, user: Any, **kwargs):
     """
     Evento manager for change_password signal
     """
     action = kwargs.get("action", None)
     class_name = sender.__name__
     ip_address = get_ip_address(kwargs.get("request", None))
```

### Comparing `zibanu-django-1.2.0a6/zibanu/django/logging/lib/events/on_login.py` & `zibanu-django-1.2.0a8/zibanu/django/logging/lib/events/on_login.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/logging/lib/events/on_send_mail.py` & `zibanu-django-1.2.0a8/zibanu/django/logging/lib/events/on_send_mail.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.2.0a8/zibanu/django/logging/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/logging/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.2.0a8/zibanu/django/logging/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/logging/migrations/0001_initial.py` & `zibanu-django-1.2.0a8/zibanu/django/logging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/logging/migrations/0002_maillog.py` & `zibanu-django-1.2.0a8/zibanu/django/logging/migrations/0002_maillog.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/logging/models.py` & `zibanu-django-1.2.0a8/zibanu/django/logging/models.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/repository/apps.py` & `zibanu-django-1.2.0a8/zibanu/django/repository/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/repository/lib/managers/__init__.py` & `zibanu-django-1.2.0a8/zibanu/django/repository/lib/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/repository/lib/managers/document.py` & `zibanu-django-1.2.0a8/zibanu/django/repository/lib/managers/document.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/repository/lib/utils/__init__.py` & `zibanu-django-1.2.0a8/zibanu/django/repository/lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/repository/lib/utils/document_generator.py` & `zibanu-django-1.2.0a8/zibanu/django/repository/lib/utils/document_generator.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/repository/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.2.0a8/zibanu/django/repository/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/repository/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.2.0a8/zibanu/django/repository/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/repository/migrations/0001_initial.py` & `zibanu-django-1.2.0a8/zibanu/django/repository/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/repository/models.py` & `zibanu-django-1.2.0a8/zibanu/django/repository/models.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/rest_framework/decorators.py` & `zibanu-django-1.2.0a8/zibanu/django/rest_framework/decorators.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/rest_framework/exceptions/__init__.py` & `zibanu-django-1.2.0a8/zibanu/django/rest_framework/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/rest_framework/exceptions/api_exception.py` & `zibanu-django-1.2.0a8/zibanu/django/rest_framework/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/rest_framework/fields/__init__.py` & `zibanu-django-1.2.0a8/zibanu/django/rest_framework/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/rest_framework/fields/current_user_default.py` & `zibanu-django-1.2.0a8/zibanu/django/rest_framework/fields/current_user_default.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/rest_framework/serializers/__init__.py` & `zibanu-django-1.2.0a8/zibanu/django/rest_framework/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/rest_framework/serializers/fields.py` & `zibanu-django-1.2.0a8/zibanu/django/rest_framework/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/rest_framework/serializers/model_serializer.py` & `zibanu-django-1.2.0a8/zibanu/django/rest_framework/serializers/model_serializer.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/rest_framework/viewsets/__init__.py` & `zibanu-django-1.2.0a8/zibanu/django/rest_framework/viewsets/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/rest_framework/viewsets/model_viewset.py` & `zibanu-django-1.2.0a8/zibanu/django/rest_framework/viewsets/model_viewset.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/rest_framework/viewsets/viewset.py` & `zibanu-django-1.2.0a8/zibanu/django/rest_framework/viewsets/viewset.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/template/apps.py` & `zibanu-django-1.2.0a8/zibanu/django/template/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/template/context_processors/__init__.py` & `zibanu-django-1.2.0a8/zibanu/django/template/context_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/template/context_processors/full_static_uri.py` & `zibanu-django-1.2.0a8/zibanu/django/template/context_processors/full_static_uri.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/template/context_processors/site.py` & `zibanu-django-1.2.0a8/zibanu/django/template/context_processors/site.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/template/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-1.2.0a8/zibanu/django/template/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/template/locale/es/LC_MESSAGES/django.po` & `zibanu-django-1.2.0a8/zibanu/django/template/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/template/templatetags/static_uri.py` & `zibanu-django-1.2.0a8/zibanu/django/template/templatetags/static_uri.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/template/templatetags/string_concat.py` & `zibanu-django-1.2.0a8/zibanu/django/template/templatetags/string_concat.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/template/templatetags/subtotal_dict.py` & `zibanu-django-1.2.0a8/zibanu/django/template/templatetags/subtotal_dict.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/template/templatetags/sum_dict.py` & `zibanu-django-1.2.0a8/zibanu/django/template/templatetags/sum_dict.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/utils/__init__.py` & `zibanu-django-1.2.0a8/zibanu/django/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/utils/code_generator.py` & `zibanu-django-1.2.0a8/zibanu/django/utils/code_generator.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/utils/date_time.py` & `zibanu-django-1.2.0a8/zibanu/django/utils/date_time.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/utils/error_messages.py` & `zibanu-django-1.2.0a8/zibanu/django/utils/error_messages.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/utils/request_utils.py` & `zibanu-django-1.2.0a8/zibanu/django/utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu/django/utils/user.py` & `zibanu-django-1.2.0a8/zibanu/django/utils/user.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,31 +7,24 @@
 # IDE:          PyCharm
 # Developed by: macercha
 # Date:         14/12/22 4:21 AM
 # Project:      CFHL Transactional Backend
 # Module Name:  user
 # Description:
 # ****************************************************************
-from django.contrib import auth
-from rest_framework_simplejwt.models import TokenUser
 from typing import Any
-
+from zibanu.django.auth.lib.utils import get_user as auth_get_user
 
 def get_user(user: Any) -> Any:
     """
     Function to get User objecto from TokenUser or another object.
     :param user: Any: User object to be converted
     :return: User: User object.
     """
-    local_user = user
-    user_model = auth.get_user_model()
-    if isinstance(user, TokenUser):
-        local_user = user_model.objects.get(pk=local_user.id)
-
-    return local_user
+    return auth_get_user(user)
 
 
 def get_user_object(user: Any) -> Any:
     """
     Legacy function. This function will be discontinued in future versions.
     :param user: Any: User object from request or auth to be returned
     :return: User: User object
```

### Comparing `zibanu-django-1.2.0a6/zibanu/django/utils/validate_cache_code.py` & `zibanu-django-1.2.0a8/zibanu/django/utils/validate_cache_code.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-1.2.0a6/zibanu_django.egg-info/PKG-INFO` & `zibanu-django-1.2.0a8/zibanu_django.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibanu-django
-Version: 1.2.0a6
+Version: 1.2.0a8
 Summary: Zibanu library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `zibanu-django-1.2.0a6/zibanu_django.egg-info/SOURCES.txt` & `zibanu-django-1.2.0a8/zibanu_django.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,28 @@
 zibanu/django/auth/api/serializers/__init__.py
 zibanu/django/auth/api/serializers/profile.py
 zibanu/django/auth/api/serializers/token.py
 zibanu/django/auth/api/serializers/user.py
 zibanu/django/auth/api/services/__init__.py
 zibanu/django/auth/api/services/user.py
 zibanu/django/auth/lib/__init__.py
+zibanu/django/auth/lib/signal_events.py
+zibanu/django/auth/lib/signals.py
+zibanu/django/auth/lib/utils.py
 zibanu/django/auth/lib/choices/__init__.py
+zibanu/django/auth/locale/es/LC_MESSAGES/django.mo
+zibanu/django/auth/locale/es/LC_MESSAGES/django.po
 zibanu/django/auth/migrations/0001_initial.py
 zibanu/django/auth/migrations/__init__.py
+zibanu/django/auth/templates/change_password.html
+zibanu/django/auth/templates/change_password.txt
+zibanu/django/auth/templates/request-code.html
+zibanu/django/auth/templates/request-code.txt
+zibanu/django/auth/templates/request_password.html
+zibanu/django/auth/templates/request_password.txt
 zibanu/django/db/__init__.py
 zibanu/django/db/backends/__init__.py
 zibanu/django/db/backends/oracle/__init__.py
 zibanu/django/db/backends/oracle/base.py
 zibanu/django/db/models/__init__.py
 zibanu/django/db/models/dated_model.py
 zibanu/django/db/models/manager.py
```

